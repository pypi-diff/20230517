# Comparing `tmp/audioldm_eval-0.0.1.tar.gz` & `tmp/audioldm_eval-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioldm_eval-0.0.1.tar", last modified: Sat Apr 29 16:48:17 2023, max compression
+gzip compressed data, was "audioldm_eval-0.0.2.tar", last modified: Wed May 17 14:26:16 2023, max compression
```

## Comparing `audioldm_eval-0.0.1.tar` & `audioldm_eval-0.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 16:48:17.187435 audioldm_eval-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1071 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4078 2023-04-29 16:48:17.184902 audioldm_eval-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3403 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 16:48:16.944208 audioldm_eval-0.0.1/audioldm_eval/
--rw-r--r--   0 root         (0) root         (0)      189 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 16:48:16.989417 audioldm_eval-0.0.1/audioldm_eval/audio/
--rw-r--r--   0 root         (0) root         (0)      146 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/audio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/audio/audio_processing.py
--rw-r--r--   0 root         (0) root         (0)     6248 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/audio/stft.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/audio/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 16:48:17.003676 audioldm_eval-0.0.1/audioldm_eval/datasets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6454 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/datasets/load_mel.py
--rw-r--r--   0 root         (0) root         (0)     1246 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/datasets/transforms.py
--rw-r--r--   0 root         (0) root         (0)    14408 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/eval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 16:48:17.025036 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20706 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/inception3.py
--rw-r--r--   0 root         (0) root         (0)     4622 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/melception.py
--rw-r--r--   0 root         (0) root         (0)     5305 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/melception_audioset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 16:48:17.081937 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7940 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/config.py
--rw-r--r--   0 root         (0) root         (0)     1085 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/evaluate.py
--rw-r--r--   0 root         (0) root         (0)     4234 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/finetune_template.py
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/losses.py
--rw-r--r--   0 root         (0) root         (0)    14159 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/main.py
--rw-r--r--   0 root         (0) root         (0)   128914 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/models.py
--rw-r--r--   0 root         (0) root         (0)     8592 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/pytorch_utils.py
--rw-r--r--   0 root         (0) root         (0)     4982 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 16:48:17.124039 audioldm_eval-0.0.1/audioldm_eval/metrics/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9023 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/metrics/fad.py
--rw-r--r--   0 root         (0) root         (0)     2230 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/metrics/fid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 16:48:17.180358 audioldm_eval-0.0.1/audioldm_eval/metrics/gs/
--rw-r--r--   0 root         (0) root         (0)       72 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/metrics/gs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2087 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/metrics/gs/geom_score.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/metrics/gs/top_utils.py
--rw-r--r--   0 root         (0) root         (0)     4758 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/metrics/gs/utils.py
--rw-r--r--   0 root         (0) root         (0)     1101 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/metrics/isc.py
--rw-r--r--   0 root         (0) root         (0)     3094 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/metrics/kid.py
--rw-r--r--   0 root         (0) root         (0)     6224 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/metrics/kl.py
--rw-r--r--   0 root         (0) root         (0)    13472 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/metrics/ndb.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-04-29 15:38:50.000000 audioldm_eval-0.0.1/audioldm_eval/metrics/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 16:48:16.969149 audioldm_eval-0.0.1/audioldm_eval.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4078 2023-04-29 16:48:16.000000 audioldm_eval-0.0.1/audioldm_eval.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1542 2023-04-29 16:48:16.000000 audioldm_eval-0.0.1/audioldm_eval.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 16:48:16.000000 audioldm_eval-0.0.1/audioldm_eval.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-04-29 16:48:16.000000 audioldm_eval-0.0.1/audioldm_eval.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-29 16:48:16.000000 audioldm_eval-0.0.1/audioldm_eval.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 16:48:17.186902 audioldm_eval-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4286 2023-04-29 16:47:52.000000 audioldm_eval-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.749132 audioldm_eval-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4082 2023-05-17 14:26:16.746697 audioldm_eval-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3407 2023-05-17 14:25:05.000000 audioldm_eval-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.466554 audioldm_eval-0.0.2/audioldm_eval/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.522530 audioldm_eval-0.0.2/audioldm_eval/audio/
+-rw-r--r--   0 root         (0) root         (0)      146 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/audio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/audio/audio_processing.py
+-rw-r--r--   0 root         (0) root         (0)     6248 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/audio/stft.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/audio/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.539919 audioldm_eval-0.0.2/audioldm_eval/datasets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6454 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/datasets/load_mel.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/datasets/transforms.py
+-rw-r--r--   0 root         (0) root         (0)    14540 2023-05-17 14:23:15.000000 audioldm_eval-0.0.2/audioldm_eval/eval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.562019 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20706 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/inception3.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/melception.py
+-rw-r--r--   0 root         (0) root         (0)     5305 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/melception_audioset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.626678 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7940 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/config.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/evaluate.py
+-rw-r--r--   0 root         (0) root         (0)     4234 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/finetune_template.py
+-rw-r--r--   0 root         (0) root         (0)      300 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/losses.py
+-rw-r--r--   0 root         (0) root         (0)    14159 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/main.py
+-rw-r--r--   0 root         (0) root         (0)   128914 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/models.py
+-rw-r--r--   0 root         (0) root         (0)     8592 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/pytorch_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4982 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.672083 audioldm_eval-0.0.2/audioldm_eval/metrics/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9023 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/fad.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/fid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.742370 audioldm_eval-0.0.2/audioldm_eval/metrics/gs/
+-rw-r--r--   0 root         (0) root         (0)       72 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/gs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/gs/geom_score.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/gs/top_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/gs/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/isc.py
+-rw-r--r--   0 root         (0) root         (0)     3094 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/kid.py
+-rw-r--r--   0 root         (0) root         (0)     6224 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/kl.py
+-rw-r--r--   0 root         (0) root         (0)    13472 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/ndb.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.498973 audioldm_eval-0.0.2/audioldm_eval.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4082 2023-05-17 14:26:16.000000 audioldm_eval-0.0.2/audioldm_eval.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-17 14:26:16.000000 audioldm_eval-0.0.2/audioldm_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 14:26:16.000000 audioldm_eval-0.0.2/audioldm_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-05-17 14:26:16.000000 audioldm_eval-0.0.2/audioldm_eval.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 14:26:16.000000 audioldm_eval-0.0.2/audioldm_eval.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 14:26:16.748697 audioldm_eval-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-05-17 14:25:38.000000 audioldm_eval-0.0.2/setup.py
```

### Comparing `audioldm_eval-0.0.1/LICENSE` & `audioldm_eval-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/PKG-INFO` & `audioldm_eval-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioldm_eval
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package is written for the evaluation of audio generation model.
 Home-page: https://github.com/haoheliu/audioldm_eval
 Author: Haohe Liu
 Author-email: haoheliu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -21,15 +21,15 @@
 
 This toolbox aims to unify audio generation model evaluation for easier future comparison.
 
 ## Quick Start
 
 First, prepare the environment
 ```shell
-git clone git@github.com:haoheliu/audioldm_eval.git
+git clone https://github.com/haoheliu/audioldm_eval.git
 cd audioldm_eval
 pip install -e .
 ```
 
 Second, generate test dataset by
 ```shell
 python3 gen_test_file.py
```

### Comparing `audioldm_eval-0.0.1/README.md` & `audioldm_eval-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This toolbox aims to unify audio generation model evaluation for easier future comparison.
 
 ## Quick Start
 
 First, prepare the environment
 ```shell
-git clone git@github.com:haoheliu/audioldm_eval.git
+git clone https://github.com/haoheliu/audioldm_eval.git
 cd audioldm_eval
 pip install -e .
 ```
 
 Second, generate test dataset by
 ```shell
 python3 gen_test_file.py
```

### Comparing `audioldm_eval-0.0.1/audioldm_eval/audio/audio_processing.py` & `audioldm_eval-0.0.2/audioldm_eval/audio/audio_processing.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/audio/stft.py` & `audioldm_eval-0.0.2/audioldm_eval/audio/stft.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/audio/tools.py` & `audioldm_eval-0.0.2/audioldm_eval/audio/tools.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/datasets/load_mel.py` & `audioldm_eval-0.0.2/audioldm_eval/datasets/load_mel.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/datasets/transforms.py` & `audioldm_eval-0.0.2/audioldm_eval/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/eval.py` & `audioldm_eval-0.0.2/audioldm_eval/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,16 @@
             mel_gen = mel_gen.cpu().numpy()[0]
             mel_target = mel_target.cpu().numpy()[0]
             psnrval = psnr(mel_gen, mel_target)
             if np.isinf(psnrval):
                 print("Infinite value encountered in psnr %s " % filename)
                 continue
             psnr_avg.append(psnrval)
-            ssim_avg.append(ssim(mel_gen, mel_target))
+            data_range = max(np.max(mel_gen), np.max(mel_target)) - min(np.min(mel_gen), np.min(mel_target))
+            ssim_avg.append(ssim(mel_gen, mel_target, data_range=data_range))
         return {"psnr": np.mean(psnr_avg), "ssim": np.mean(ssim_avg)}
 
     def calculate_metrics(self, generate_files_path, groundtruth_path, same_name, limit_num=None):
         # Generation, target
         torch.manual_seed(0)
 
         num_workers = 0
```

### Comparing `audioldm_eval-0.0.1/audioldm_eval/feature_extractors/inception3.py` & `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/inception3.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/feature_extractors/melception.py` & `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/melception.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/feature_extractors/melception_audioset.py` & `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/melception_audioset.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/config.py` & `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/config.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/evaluate.py` & `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/evaluate.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/finetune_template.py` & `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/finetune_template.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/main.py` & `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/main.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/models.py` & `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/models.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/pytorch_utils.py` & `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/feature_extractors/panns/utilities.py` & `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/utilities.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/metrics/fad.py` & `audioldm_eval-0.0.2/audioldm_eval/metrics/fad.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/metrics/fid.py` & `audioldm_eval-0.0.2/audioldm_eval/metrics/fid.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/metrics/gs/geom_score.py` & `audioldm_eval-0.0.2/audioldm_eval/metrics/gs/geom_score.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/metrics/gs/top_utils.py` & `audioldm_eval-0.0.2/audioldm_eval/metrics/gs/top_utils.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/metrics/gs/utils.py` & `audioldm_eval-0.0.2/audioldm_eval/metrics/gs/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/metrics/isc.py` & `audioldm_eval-0.0.2/audioldm_eval/metrics/isc.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/metrics/kid.py` & `audioldm_eval-0.0.2/audioldm_eval/metrics/kid.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/metrics/kl.py` & `audioldm_eval-0.0.2/audioldm_eval/metrics/kl.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/metrics/ndb.py` & `audioldm_eval-0.0.2/audioldm_eval/metrics/ndb.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval/metrics/validate.py` & `audioldm_eval-0.0.2/audioldm_eval/metrics/validate.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/audioldm_eval.egg-info/PKG-INFO` & `audioldm_eval-0.0.2/audioldm_eval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioldm-eval
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package is written for the evaluation of audio generation model.
 Home-page: https://github.com/haoheliu/audioldm_eval
 Author: Haohe Liu
 Author-email: haoheliu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -21,15 +21,15 @@
 
 This toolbox aims to unify audio generation model evaluation for easier future comparison.
 
 ## Quick Start
 
 First, prepare the environment
 ```shell
-git clone git@github.com:haoheliu/audioldm_eval.git
+git clone https://github.com/haoheliu/audioldm_eval.git
 cd audioldm_eval
 pip install -e .
 ```
 
 Second, generate test dataset by
 ```shell
 python3 gen_test_file.py
```

### Comparing `audioldm_eval-0.0.1/audioldm_eval.egg-info/SOURCES.txt` & `audioldm_eval-0.0.2/audioldm_eval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.1/setup.py` & `audioldm_eval-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # Package meta-data.
 NAME = "audioldm_eval"
 DESCRIPTION = "This package is written for the evaluation of audio generation model."
 URL = "https://github.com/haoheliu/audioldm_eval"
 EMAIL = "haoheliu@gmail.com"
 AUTHOR = "Haohe Liu"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "torch>=1.11.0",
     "torchaudio",
     "scikit-image",
     "torchlibrosa",
```

