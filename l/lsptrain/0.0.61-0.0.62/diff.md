# Comparing `tmp/lsptrain-0.0.61.tar.gz` & `tmp/lsptrain-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.61.tar", last modified: Tue May 16 03:40:20 2023, max compression
+gzip compressed data, was "lsptrain-0.0.62.tar", last modified: Wed May 17 02:43:37 2023, max compression
```

## Comparing `lsptrain-0.0.61.tar` & `lsptrain-0.0.62.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.981503 lsptrain-0.0.61/
--rw-rw-rw-   0        0        0      510 2023-05-16 03:40:20.980504 lsptrain-0.0.61/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-04-27 08:11:39.000000 lsptrain-0.0.61/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.959502 lsptrain-0.0.61/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.61/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.970503 lsptrain-0.0.61/lsptrain/nlp_classification/
--rw-rw-rw-   0        0        0       36 2023-05-16 02:22:37.000000 lsptrain-0.0.61/lsptrain/nlp_classification/__init__.py
--rw-rw-rw-   0        0        0     1175 2023-05-16 03:24:21.000000 lsptrain-0.0.61/lsptrain/nlp_classification/model.py
--rw-rw-rw-   0        0        0     7874 2023-05-16 03:38:46.000000 lsptrain-0.0.61/lsptrain/nlp_classification/train_scripts.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.972502 lsptrain-0.0.61/lsptrain/nlp_classification_predictor/
--rw-rw-rw-   0        0        0       89 2023-04-24 01:36:49.000000 lsptrain-0.0.61/lsptrain/nlp_classification_predictor/__init__.py
--rw-rw-rw-   0        0        0     4744 2023-04-24 01:36:49.000000 lsptrain-0.0.61/lsptrain/nlp_classification_predictor/predictor.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.975504 lsptrain-0.0.61/lsptrain/nlp_similarity_predictor/
--rw-rw-rw-   0        0        0       48 2023-04-27 07:37:30.000000 lsptrain-0.0.61/lsptrain/nlp_similarity_predictor/__init__.py
--rw-rw-rw-   0        0        0     2164 2023-04-27 09:06:10.000000 lsptrain-0.0.61/lsptrain/nlp_similarity_predictor/predictor.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.979503 lsptrain-0.0.61/lsptrain/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.61/lsptrain/utils/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-23 08:30:14.000000 lsptrain-0.0.61/lsptrain/utils/init_args.py
--rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.61/lsptrain/utils/init_logger.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.966503 lsptrain-0.0.61/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      510 2023-05-16 03:40:20.000000 lsptrain-0.0.61/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      600 2023-05-16 03:40:20.000000 lsptrain-0.0.61/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 03:40:20.000000 lsptrain-0.0.61/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-16 03:40:20.000000 lsptrain-0.0.61/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 03:40:20.000000 lsptrain-0.0.61/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 03:40:20.981503 lsptrain-0.0.61/setup.cfg
--rw-rw-rw-   0        0        0      722 2023-05-16 03:40:18.000000 lsptrain-0.0.61/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 02:43:37.237288 lsptrain-0.0.62/
+-rw-rw-rw-   0        0        0      543 2023-05-17 02:43:37.237288 lsptrain-0.0.62/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-05-16 06:43:26.000000 lsptrain-0.0.62/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 02:43:37.210289 lsptrain-0.0.62/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.62/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 02:43:37.220288 lsptrain-0.0.62/lsptrain/nlp_classification/
+-rw-rw-rw-   0        0        0       36 2023-05-16 02:22:37.000000 lsptrain-0.0.62/lsptrain/nlp_classification/__init__.py
+-rw-rw-rw-   0        0        0     1175 2023-05-16 03:24:21.000000 lsptrain-0.0.62/lsptrain/nlp_classification/model.py
+-rw-rw-rw-   0        0        0     7874 2023-05-16 03:38:46.000000 lsptrain-0.0.62/lsptrain/nlp_classification/train_scripts.py
+drwxrwxrwx   0        0        0        0 2023-05-17 02:43:37.222288 lsptrain-0.0.62/lsptrain/nlp_classification_predictor/
+-rw-rw-rw-   0        0        0       89 2023-04-24 01:36:49.000000 lsptrain-0.0.62/lsptrain/nlp_classification_predictor/__init__.py
+-rw-rw-rw-   0        0        0     4744 2023-04-24 01:36:49.000000 lsptrain-0.0.62/lsptrain/nlp_classification_predictor/predictor.py
+drwxrwxrwx   0        0        0        0 2023-05-17 02:43:37.232288 lsptrain-0.0.62/lsptrain/nlp_info_extract/
+-rw-rw-rw-   0        0        0      117 2023-05-17 01:59:29.000000 lsptrain-0.0.62/lsptrain/nlp_info_extract/__init__.py
+-rw-rw-rw-   0        0        0    18892 2023-05-16 08:22:01.000000 lsptrain-0.0.62/lsptrain/nlp_info_extract/download_pretrained_model.py
+-rw-rw-rw-   0        0        0    49710 2023-05-16 08:19:19.000000 lsptrain-0.0.62/lsptrain/nlp_info_extract/ernie.py
+-rw-rw-rw-   0        0        0     2519 2023-05-16 09:32:22.000000 lsptrain-0.0.62/lsptrain/nlp_info_extract/evaluate.py
+-rw-rw-rw-   0        0        0    30236 2023-05-17 02:19:05.000000 lsptrain-0.0.62/lsptrain/nlp_info_extract/model.py
+-rw-rw-rw-   0        0        0     7696 2023-05-16 09:40:47.000000 lsptrain-0.0.62/lsptrain/nlp_info_extract/train_scripts.py
+-rw-rw-rw-   0        0        0    47707 2023-05-16 07:24:46.000000 lsptrain-0.0.62/lsptrain/nlp_info_extract/util.py
+drwxrwxrwx   0        0        0        0 2023-05-17 02:43:37.235289 lsptrain-0.0.62/lsptrain/nlp_similarity_predictor/
+-rw-rw-rw-   0        0        0       48 2023-04-27 07:37:30.000000 lsptrain-0.0.62/lsptrain/nlp_similarity_predictor/__init__.py
+-rw-rw-rw-   0        0        0     2164 2023-04-27 09:06:10.000000 lsptrain-0.0.62/lsptrain/nlp_similarity_predictor/predictor.py
+drwxrwxrwx   0        0        0        0 2023-05-17 02:43:37.216289 lsptrain-0.0.62/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      543 2023-05-17 02:43:37.000000 lsptrain-0.0.62/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2023-05-17 02:43:37.000000 lsptrain-0.0.62/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 02:43:37.000000 lsptrain-0.0.62/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-17 02:43:37.000000 lsptrain-0.0.62/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-17 02:43:37.000000 lsptrain-0.0.62/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 02:43:37.237288 lsptrain-0.0.62/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-05-17 02:42:49.000000 lsptrain-0.0.62/setup.py
```

### Comparing `lsptrain-0.0.61/lsptrain/nlp_classification/model.py` & `lsptrain-0.0.62/lsptrain/nlp_classification/model.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.61/lsptrain/nlp_classification/train_scripts.py` & `lsptrain-0.0.62/lsptrain/nlp_classification/train_scripts.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.61/lsptrain/nlp_classification_predictor/predictor.py` & `lsptrain-0.0.62/lsptrain/nlp_classification_predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.61/lsptrain/nlp_similarity_predictor/predictor.py` & `lsptrain-0.0.62/lsptrain/nlp_similarity_predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.61/lsptrain.egg-info/SOURCES.txt` & `lsptrain-0.0.62/lsptrain.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,12 +7,16 @@
 lsptrain.egg-info/requires.txt
 lsptrain.egg-info/top_level.txt
 lsptrain/nlp_classification/__init__.py
 lsptrain/nlp_classification/model.py
 lsptrain/nlp_classification/train_scripts.py
 lsptrain/nlp_classification_predictor/__init__.py
 lsptrain/nlp_classification_predictor/predictor.py
+lsptrain/nlp_info_extract/__init__.py
+lsptrain/nlp_info_extract/download_pretrained_model.py
+lsptrain/nlp_info_extract/ernie.py
+lsptrain/nlp_info_extract/evaluate.py
+lsptrain/nlp_info_extract/model.py
+lsptrain/nlp_info_extract/train_scripts.py
+lsptrain/nlp_info_extract/util.py
 lsptrain/nlp_similarity_predictor/__init__.py
-lsptrain/nlp_similarity_predictor/predictor.py
-lsptrain/utils/__init__.py
-lsptrain/utils/init_args.py
-lsptrain/utils/init_logger.py
+lsptrain/nlp_similarity_predictor/predictor.py
```

### Comparing `lsptrain-0.0.61/setup.py` & `lsptrain-0.0.62/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.61',
+      version='0.0.62',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='https://www.gitee.com/ykallan/lsptrain',
       install_requires=['torch',
                         'transformers',
```

