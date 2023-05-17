# Comparing `tmp/bytez-0.1.87.tar.gz` & `tmp/bytez-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytez-0.1.87.tar", last modified: Wed May 17 01:46:07 2023, max compression
+gzip compressed data, was "bytez-0.1.9.tar", last modified: Fri Apr 28 01:02:38 2023, max compression
```

## Comparing `bytez-0.1.87.tar` & `bytez-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,15 @@
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:07.078531 bytez-0.1.87/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-17 01:46:07.078531 bytez-0.1.87/PKG-INFO
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       73 2023-03-26 07:05:33.000000 bytez-0.1.87/README.md
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:07.074531 bytez-0.1.87/bytez/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-14 20:59:27.000000 bytez-0.1.87/bytez/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)   106124 2023-05-17 01:46:00.000000 bytez-0.1.87/bytez/exports.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      988 2023-05-14 20:58:15.000000 bytez-0.1.87/bytez/model.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:07.074531 bytez-0.1.87/bytez/tasks/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:00:59.000000 bytez-0.1.87/bytez/tasks/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:07.074531 bytez-0.1.87/bytez/tasks/language_modelling/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:06.000000 bytez-0.1.87/bytez/tasks/language_modelling/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:07.074531 bytez-0.1.87/bytez/tasks/language_modelling/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:06.000000 bytez-0.1.87/bytez/tasks/language_modelling/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1438 2023-05-17 01:46:00.000000 bytez-0.1.87/bytez/tasks/language_modelling/_models/hazyresearch_h3.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      218 2023-05-17 01:38:03.000000 bytez-0.1.87/bytez/tasks/language_modelling/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:07.074531 bytez-0.1.87/bytez/tasks/style_transfer/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:57.000000 bytez-0.1.87/bytez/tasks/style_transfer/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:07.074531 bytez-0.1.87/bytez/tasks/style_transfer/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:59.000000 bytez-0.1.87/bytez/tasks/style_transfer/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      761 2023-05-14 20:47:16.000000 bytez-0.1.87/bytez/tasks/style_transfer/_models/cmd_style_transfer.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      686 2023-05-14 20:47:16.000000 bytez-0.1.87/bytez/tasks/style_transfer/_models/fast_style_transfer.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      706 2023-05-14 20:47:16.000000 bytez-0.1.87/bytez/tasks/style_transfer/_models/tensorflow_fast_style.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      547 2023-05-14 20:47:16.000000 bytez-0.1.87/bytez/tasks/style_transfer/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:07.078531 bytez-0.1.87/bytez/tasks/super_resolution/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:01:49.000000 bytez-0.1.87/bytez/tasks/super_resolution/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:07.078531 bytez-0.1.87/bytez/tasks/super_resolution/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:22.000000 bytez-0.1.87/bytez/tasks/super_resolution/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     2478 2023-05-14 20:58:15.000000 bytez-0.1.87/bytez/tasks/super_resolution/_models/holmes_alan_dsrvae.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      224 2023-05-14 20:58:15.000000 bytez-0.1.87/bytez/tasks/super_resolution/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:07.078531 bytez-0.1.87/bytez/tasks/text_summarization/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-15 21:02:31.000000 bytez-0.1.87/bytez/tasks/text_summarization/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:07.078531 bytez-0.1.87/bytez/tasks/text_summarization/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-15 21:02:31.000000 bytez-0.1.87/bytez/tasks/text_summarization/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      803 2023-05-14 21:13:12.000000 bytez-0.1.87/bytez/tasks/text_summarization/_models/chriskhanhtran_bert_extractive_summarization.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1079 2023-05-15 21:02:31.000000 bytez-0.1.87/bytez/tasks/text_summarization/_models/dmmiller612_bert_extractive_summarizer.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      564 2023-05-15 20:49:27.000000 bytez-0.1.87/bytez/tasks/text_summarization/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-17 01:46:07.074531 bytez-0.1.87/bytez.egg-info/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-17 01:46:07.000000 bytez-0.1.87/bytez.egg-info/PKG-INFO
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1218 2023-05-17 01:46:07.000000 bytez-0.1.87/bytez.egg-info/SOURCES.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        1 2023-05-17 01:46:07.000000 bytez-0.1.87/bytez.egg-info/dependency_links.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       70 2023-05-17 01:46:07.000000 bytez-0.1.87/bytez.egg-info/requires.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        6 2023-05-17 01:46:07.000000 bytez-0.1.87/bytez.egg-info/top_level.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-17 01:46:07.078531 bytez-0.1.87/setup.cfg
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      663 2023-05-17 01:46:06.000000 bytez-0.1.87/setup.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-04-28 01:02:38.356341 bytez-0.1.9/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      408 2023-04-28 01:02:38.356341 bytez-0.1.9/PKG-INFO
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       73 2023-03-26 07:05:33.000000 bytez-0.1.9/README.md
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-04-28 01:02:38.356341 bytez-0.1.9/bytez/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       32 2023-03-26 06:56:40.000000 bytez-0.1.9/bytez/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)    79093 2023-03-28 20:09:16.000000 bytez-0.1.9/bytez/main.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1068 2023-04-28 01:01:45.000000 bytez-0.1.9/bytez/pipeline.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-04-28 01:02:38.356341 bytez-0.1.9/bytez.egg-info/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      408 2023-04-28 01:02:38.000000 bytez-0.1.9/bytez.egg-info/PKG-INFO
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      212 2023-04-28 01:02:38.000000 bytez-0.1.9/bytez.egg-info/SOURCES.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        1 2023-04-28 01:02:38.000000 bytez-0.1.9/bytez.egg-info/dependency_links.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       70 2023-04-28 01:02:38.000000 bytez-0.1.9/bytez.egg-info/requires.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        6 2023-04-28 01:02:38.000000 bytez-0.1.9/bytez.egg-info/top_level.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-04-28 01:02:38.356341 bytez-0.1.9/setup.cfg
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      662 2023-04-28 01:02:36.000000 bytez-0.1.9/setup.py
```

### Comparing `bytez-0.1.87/setup.py` & `bytez-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 packages = find_packages()
 
 
 setup(
     name='bytez',
-    version='0.1.87',
+    version='0.1.9',
     packages=packages,
     install_requires=[
         'charset-normalizer==3.1.0',
         'idna==3.4',
         'requests==2.28.2',
         'urllib3==1.26.15',
     ],
```

