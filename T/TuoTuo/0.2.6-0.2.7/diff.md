# Comparing `tmp/TuoTuo-0.2.6.tar.gz` & `tmp/TuoTuo-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TuoTuo-0.2.6.tar", last modified: Wed May  3 20:49:43 2023, max compression
+gzip compressed data, was "TuoTuo-0.2.7.tar", last modified: Tue May 16 22:34:22 2023, max compression
```

## Comparing `TuoTuo-0.2.6.tar` & `TuoTuo-0.2.7.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 20:49:43.075698 TuoTuo-0.2.6/
--rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.2.6/.DS_Store
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 20:49:43.063190 TuoTuo-0.2.6/.github/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 20:49:43.065901 TuoTuo-0.2.6/.github/workflows/
--rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.2.6/.github/workflows/python-package.yml
--rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.2.6/.github/workflows/python-publish.yml
--rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.2.6/.gitignore
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 20:49:43.066232 TuoTuo-0.2.6/.vscode/
--rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.2.6/.vscode/c_cpp_properties.json
--rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.2.6/LICENSE
--rw-r--r--   0 ericliu    (501) staff       (20)       41 2023-05-03 15:52:33.000000 TuoTuo-0.2.6/MANIFEST.in
--rw-r--r--   0 ericliu    (501) staff       (20)     1538 2023-05-03 20:49:43.075823 TuoTuo-0.2.6/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.2.6/README.md
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 20:49:43.067162 TuoTuo-0.2.6/TuoTuo.egg-info/
--rw-r--r--   0 ericliu    (501) staff       (20)     1538 2023-05-03 20:49:43.000000 TuoTuo-0.2.6/TuoTuo.egg-info/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      865 2023-05-03 20:49:43.000000 TuoTuo-0.2.6/TuoTuo.egg-info/SOURCES.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-03 20:49:43.000000 TuoTuo-0.2.6/TuoTuo.egg-info/dependency_links.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       66 2023-05-03 20:49:43.000000 TuoTuo-0.2.6/TuoTuo.egg-info/requires.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        7 2023-05-03 20:49:43.000000 TuoTuo-0.2.6/TuoTuo.egg-info/top_level.txt
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 20:49:43.068017 TuoTuo-0.2.6/notebook/
--rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.2.6/notebook/Our Model vs SKLearn.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.2.6/notebook/__init__.py
--rw-r--r--   0 ericliu    (501) staff       (20)      505 2023-05-03 17:21:30.000000 TuoTuo-0.2.6/pyproject.toml
--rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.2.6/requirements.txt
--rw-r--r--   0 ericliu    (501) staff       (20)      197 2023-05-03 20:49:43.076145 TuoTuo-0.2.6/setup.cfg
--rw-r--r--   0 ericliu    (501) staff       (20)     1996 2023-05-03 20:49:37.000000 TuoTuo-0.2.6/setup.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 20:49:43.071496 TuoTuo-0.2.6/tuotuo/
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.2.6/tuotuo/__init__.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 20:49:43.063702 TuoTuo-0.2.6/tuotuo/build/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 20:49:43.071900 TuoTuo-0.2.6/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.2.6/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 20:49:43.073113 TuoTuo-0.2.6/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
--rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.2.6/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
--rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.2.6/tuotuo/cutils.c
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.2.6/tuotuo/cutils.cpython-38-darwin.so
--rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.2.6/tuotuo/cutils.pyx
--rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.2.6/tuotuo/generator.py
--rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.2.6/tuotuo/lda_model.py
--rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.2.6/tuotuo/text_pre_processor.py
--rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.2.6/tuotuo/utils.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-16 22:34:22.944815 TuoTuo-0.2.7/
+-rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.2.7/.DS_Store
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-16 22:34:22.929121 TuoTuo-0.2.7/.github/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-16 22:34:22.931423 TuoTuo-0.2.7/.github/workflows/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.2.7/.github/workflows/python-package.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.2.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)       96 2023-05-16 22:24:56.000000 TuoTuo-0.2.7/.gitignore
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-16 22:34:22.931758 TuoTuo-0.2.7/.vscode/
+-rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.2.7/.vscode/c_cpp_properties.json
+-rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.2.7/LICENSE
+-rw-r--r--   0 ericliu    (501) staff       (20)       41 2023-05-03 15:52:33.000000 TuoTuo-0.2.7/MANIFEST.in
+-rw-r--r--   0 ericliu    (501) staff       (20)     4926 2023-05-16 22:34:22.944943 TuoTuo-0.2.7/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)     4085 2023-05-16 22:25:37.000000 TuoTuo-0.2.7/README.md
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-16 22:34:22.932535 TuoTuo-0.2.7/TuoTuo.egg-info/
+-rw-r--r--   0 ericliu    (501) staff       (20)     4926 2023-05-16 22:34:22.000000 TuoTuo-0.2.7/TuoTuo.egg-info/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      922 2023-05-16 22:34:22.000000 TuoTuo-0.2.7/TuoTuo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-16 22:34:22.000000 TuoTuo-0.2.7/TuoTuo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       66 2023-05-16 22:34:22.000000 TuoTuo-0.2.7/TuoTuo.egg-info/requires.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        7 2023-05-16 22:34:22.000000 TuoTuo-0.2.7/TuoTuo.egg-info/top_level.txt
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-16 22:34:22.932655 TuoTuo-0.2.7/images/
+-rw-r--r--   0 ericliu    (501) staff       (20)    13783 2023-05-16 21:17:31.000000 TuoTuo-0.2.7/images/generated_doc_perplexities.png
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-16 22:34:22.933714 TuoTuo-0.2.7/notebook/
+-rw-r--r--   0 ericliu    (501) staff       (20)    62686 2023-05-16 21:25:53.000000 TuoTuo-0.2.7/notebook/Our Model vs SKLearn.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.2.7/notebook/__init__.py
+-rw-r--r--   0 ericliu    (501) staff       (20)      505 2023-05-03 17:21:30.000000 TuoTuo-0.2.7/pyproject.toml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.2.7/requirements.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)      197 2023-05-16 22:34:22.945223 TuoTuo-0.2.7/setup.cfg
+-rw-r--r--   0 ericliu    (501) staff       (20)     1992 2023-05-16 22:30:53.000000 TuoTuo-0.2.7/setup.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-16 22:34:22.940962 TuoTuo-0.2.7/tuotuo/
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.2.7/tuotuo/__init__.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-16 22:34:22.929607 TuoTuo-0.2.7/tuotuo/build/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-16 22:34:22.941322 TuoTuo-0.2.7/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.2.7/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-16 22:34:22.942512 TuoTuo-0.2.7/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
+-rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.2.7/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
+-rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.2.7/tuotuo/cutils.c
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.2.7/tuotuo/cutils.cpython-38-darwin.so
+-rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.2.7/tuotuo/cutils.pyx
+-rw-r--r--   0 ericliu    (501) staff       (20)     1432 2023-05-16 20:38:49.000000 TuoTuo-0.2.7/tuotuo/document.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.2.7/tuotuo/generator.py
+-rw-r--r--   0 ericliu    (501) staff       (20)    15681 2023-05-16 20:35:53.000000 TuoTuo-0.2.7/tuotuo/lda_model.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     3377 2023-05-03 21:22:06.000000 TuoTuo-0.2.7/tuotuo/text_pre_processor.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     5557 2023-05-16 19:59:25.000000 TuoTuo-0.2.7/tuotuo/utils.py
```

### Comparing `TuoTuo-0.2.6/.DS_Store` & `TuoTuo-0.2.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.6/.github/workflows/python-package.yml` & `TuoTuo-0.2.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.6/.github/workflows/python-publish.yml` & `TuoTuo-0.2.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.6/.vscode/c_cpp_properties.json` & `TuoTuo-0.2.7/.vscode/c_cpp_properties.json`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.6/LICENSE` & `TuoTuo-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.6/TuoTuo.egg-info/SOURCES.txt` & `TuoTuo-0.2.7/TuoTuo.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 .github/workflows/python-publish.yml
 .vscode/c_cpp_properties.json
 TuoTuo.egg-info/PKG-INFO
 TuoTuo.egg-info/SOURCES.txt
 TuoTuo.egg-info/dependency_links.txt
 TuoTuo.egg-info/requires.txt
 TuoTuo.egg-info/top_level.txt
+images/generated_doc_perplexities.png
 notebook/Our Model vs SKLearn.ipynb
 notebook/__init__.py
 tuotuo/__init__.py
 tuotuo/cutils.c
 tuotuo/cutils.cpython-38-darwin.so
 tuotuo/cutils.pyx
+tuotuo/document.py
 tuotuo/generator.py
 tuotuo/lda_model.py
 tuotuo/text_pre_processor.py
 tuotuo/utils.py
 tuotuo.egg-info/PKG-INFO
 tuotuo.egg-info/SOURCES.txt
 tuotuo.egg-info/dependency_links.txt
```

### Comparing `TuoTuo-0.2.6/notebook/Our Model vs SKLearn.ipynb` & `TuoTuo-0.2.7/notebook/Our Model vs SKLearn.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9513275296152217%*

 * *Differences: {"'cells'": "{0: {'execution_count': 59, 'source': {insert: [(15, '\\n'), (16, 'from "*

 * *            "tuotuo.document import Document \\n'), (17, '\\n')]}}, 2: {'execution_count': 45}, 3: "*

 * *            "{'execution_count': 46, 'outputs': {0: {'execution_count': 46}}}, 4: "*

 * *            "{'execution_count': 47, 'outputs': {0: {'execution_count': 47}}}, 5: "*

 * *            "{'execution_count': 48}, 6: {'execution_count': 49}, 8: {'execution_count': 50}, 9: "*

 * *            "{'execution_count': 51}, 11: {'execution_cou […]*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 59,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "The autoreload extension is already loaded. To reload it, use:\n",
@@ -26,14 +26,17 @@
                 "from collections import defaultdict\n",
                 "from pprint import pprint\n",
                 "import matplotlib.pyplot as plt \n",
                 "\n",
                 "from sklearn.decomposition import LatentDirichletAllocation \n",
                 "from tuotuo.lda_model import LDASmoothed \n",
                 "from tuotuo.generator import doc_generator \n",
+                "\n",
+                "from tuotuo.document import Document \n",
+                "\n",
                 "from tuotuo.utils import (\n",
                 "    get_vocab_from_docs, \n",
                 "    get_np_wct, \n",
                 "    data_loader,\n",
                 "    text_pipeline, \n",
                 "    process_documents,\n",
                 "    compute_elbo,\n",
@@ -60,95 +63,112 @@
             "metadata": {},
             "source": [
                 "# Document Generation"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 45,
             "metadata": {},
             "outputs": [],
             "source": [
                 "gen = doc_generator(\n",
                 "    M = 100,\n",
                 "    L = 20, \n",
                 "    topic_prior = tr.tensor([1,1,1,1,1], dtype=tr.double)\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 46,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Dirichlet(concentration: torch.Size([5]))"
                         ]
                     },
-                    "execution_count": 30,
+                    "execution_count": 46,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "gen.alpha"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": 47,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "torch.Size([100, 5])"
                         ]
                     },
-                    "execution_count": 31,
+                    "execution_count": 47,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "gen.theta.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": 48,
             "metadata": {},
             "outputs": [],
             "source": [
                 "#gen.theta"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": 49,
             "metadata": {},
             "outputs": [],
             "source": [
                 "docs = gen.generate_doc()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 57,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "<class 'dict'>\n"
+                    ]
+                }
+            ],
+            "source": [
+                "print(type(docs)) "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 50,
             "metadata": {},
             "outputs": [],
             "source": [
                 "#docs_raw_dict, raw_word_2_idx, raw_idx_2_word = data_loader('ap')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": 51,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "There are 100 documents in the dataset after processing\n",
@@ -159,15 +179,15 @@
             ],
             "source": [
                 "result = process_documents(docs, sample=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": 58,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "dict_keys(['documents', 'vocab_doc_count_dict', 'vocab_doc_count_array', 'vocab_to_idx', 'idx_to_vocab'])\n"
@@ -176,15 +196,88 @@
             ],
             "source": [
                 "print(result.keys())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": 52,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "dict_keys(['documents', 'vocab_doc_count_dict', 'vocab_doc_count_array', 'vocab_to_idx', 'idx_to_vocab'])\n"
+                    ]
+                }
+            ],
+            "source": [
+                "print(result.keys())"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 71,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "['contract', 'divorce', 'infection', 'FIFA', 'court', 'concert', 'recreation', 'astrophysics', 'athletics', 'research', 'Symmetrical', 'energy', 'evidence', 'quantum', 'form', 'asymmetrical', 'content', 'Olympic', 'scientst', 'exercise', 'bruise', 'physical', 'Technique', 'contagious', 'copyright', 'appetite', 'genetics', 'game', 'football', 'picture', 'Craftsmanship', 'decongestant', 'electricity', 'immunology', 'injection', 'allergy', 'accuse', 'bankrupt', 'attorney', 'fever']\n"
+                    ]
+                }
+            ],
+            "source": [
+                "print(list(result['vocab_doc_count_dict'].keys()))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 73,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "list1 = list(result['vocab_doc_count_dict'].keys()) \n",
+                "list2 = list(result['vocab_to_idx'].keys())\n",
+                "\n",
+                "for l1, l2 in zip(list1, list2): \n",
+                "    assert l1 == l2 "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 63,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "array([[2., 0., 0., ..., 0., 0., 0.],\n",
+                            "       [1., 0., 0., ..., 0., 0., 0.],\n",
+                            "       [1., 0., 0., ..., 0., 0., 1.],\n",
+                            "       ...,\n",
+                            "       [0., 0., 0., ..., 0., 1., 1.],\n",
+                            "       [0., 0., 0., ..., 0., 1., 0.],\n",
+                            "       [0., 0., 0., ..., 1., 1., 0.]])"
+                        ]
+                    },
+                    "execution_count": 63,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "result['vocab_doc_count_array'].T"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 53,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "(100, 40)\n"
@@ -205,15 +298,87 @@
                 "        doc_vocab_count[doc_idx, vocab_idx] += 1 \n",
                 "\n",
                 "print(doc_vocab_count.shape)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 38,
+            "execution_count": 55,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "array([[2., 1., 1., ..., 0., 0., 0.],\n",
+                            "       [0., 0., 0., ..., 0., 0., 0.],\n",
+                            "       [0., 0., 0., ..., 0., 0., 0.],\n",
+                            "       ...,\n",
+                            "       [0., 0., 0., ..., 0., 0., 1.],\n",
+                            "       [0., 0., 0., ..., 1., 1., 1.],\n",
+                            "       [0., 0., 1., ..., 1., 0., 0.]])"
+                        ]
+                    },
+                    "execution_count": 55,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "doc_vocab_count "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 64,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "True"
+                        ]
+                    },
+                    "execution_count": 64,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "(result['vocab_doc_count_array'].T == doc_vocab_count).all()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 70,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "array([[2., 1., 1., ..., 0., 0., 0.],\n",
+                            "       [0., 0., 0., ..., 0., 0., 0.],\n",
+                            "       [0., 0., 0., ..., 0., 0., 0.],\n",
+                            "       ...,\n",
+                            "       [0., 0., 0., ..., 0., 0., 1.],\n",
+                            "       [0., 0., 0., ..., 1., 1., 1.],\n",
+                            "       [0., 0., 1., ..., 1., 0., 0.]])"
+                        ]
+                    },
+                    "execution_count": 70,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "doc_vocab_count"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 69,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -229,74 +394,74 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>accuse</th>\n",
-                            "      <th>evidence</th>\n",
-                            "      <th>bruise</th>\n",
+                            "      <th>contract</th>\n",
+                            "      <th>divorce</th>\n",
+                            "      <th>infection</th>\n",
                             "      <th>FIFA</th>\n",
-                            "      <th>Craftsmanship</th>\n",
-                            "      <th>picture</th>\n",
                             "      <th>court</th>\n",
-                            "      <th>Technique</th>\n",
+                            "      <th>concert</th>\n",
+                            "      <th>recreation</th>\n",
                             "      <th>astrophysics</th>\n",
-                            "      <th>immunology</th>\n",
+                            "      <th>athletics</th>\n",
+                            "      <th>research</th>\n",
                             "      <th>...</th>\n",
-                            "      <th>exercise</th>\n",
-                            "      <th>appetite</th>\n",
-                            "      <th>energy</th>\n",
-                            "      <th>football</th>\n",
+                            "      <th>Craftsmanship</th>\n",
+                            "      <th>decongestant</th>\n",
+                            "      <th>electricity</th>\n",
+                            "      <th>immunology</th>\n",
                             "      <th>injection</th>\n",
-                            "      <th>game</th>\n",
                             "      <th>allergy</th>\n",
-                            "      <th>Symmetrical</th>\n",
-                            "      <th>decongestant</th>\n",
-                            "      <th>athletics</th>\n",
+                            "      <th>accuse</th>\n",
+                            "      <th>bankrupt</th>\n",
+                            "      <th>attorney</th>\n",
+                            "      <th>fever</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
@@ -304,21 +469,21 @@
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>2.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
@@ -330,20 +495,20 @@
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
@@ -352,23 +517,23 @@
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
@@ -401,202 +566,234 @@
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>95</th>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>96</th>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>3.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>97</th>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>98</th>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>3.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>99</th>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "<p>100 rows \u00d7 40 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "    accuse  evidence  bruise  FIFA  Craftsmanship  picture  court  Technique  \\\n",
-                            "0      1.0       1.0     1.0   1.0            1.0      1.0    1.0        1.0   \n",
-                            "1      2.0       0.0     0.0   0.0            0.0      0.0    0.0        0.0   \n",
-                            "2      0.0       1.0     0.0   0.0            2.0      0.0    0.0        1.0   \n",
-                            "3      0.0       1.0     1.0   0.0            0.0      0.0    0.0        0.0   \n",
-                            "4      0.0       1.0     0.0   0.0            0.0      0.0    0.0        0.0   \n",
-                            "..     ...       ...     ...   ...            ...      ...    ...        ...   \n",
-                            "95     0.0       0.0     0.0   0.0            1.0      0.0    0.0        1.0   \n",
-                            "96     0.0       0.0     0.0   0.0            1.0      1.0    0.0        0.0   \n",
-                            "97     0.0       0.0     0.0   0.0            0.0      1.0    0.0        0.0   \n",
-                            "98     0.0       0.0     1.0   0.0            0.0      0.0    0.0        1.0   \n",
-                            "99     0.0       0.0     1.0   0.0            2.0      0.0    0.0        1.0   \n",
+                            "    contract  divorce  infection  FIFA  court  concert  recreation  \\\n",
+                            "0        2.0      1.0        1.0   1.0    2.0      1.0         1.0   \n",
+                            "1        0.0      0.0        0.0   0.0    0.0      0.0         1.0   \n",
+                            "2        0.0      0.0        0.0   0.0    0.0      0.0         0.0   \n",
+                            "3        0.0      1.0        1.0   1.0    0.0      0.0         1.0   \n",
+                            "4        0.0      0.0        0.0   0.0    0.0      1.0         0.0   \n",
+                            "..       ...      ...        ...   ...    ...      ...         ...   \n",
+                            "95       0.0      0.0        1.0   0.0    0.0      0.0         0.0   \n",
+                            "96       0.0      0.0        0.0   0.0    0.0      0.0         0.0   \n",
+                            "97       0.0      0.0        0.0   0.0    0.0      0.0         0.0   \n",
+                            "98       0.0      0.0        0.0   0.0    0.0      1.0         1.0   \n",
+                            "99       0.0      0.0        1.0   0.0    1.0      0.0         0.0   \n",
+                            "\n",
+                            "    astrophysics  athletics  research  ...  Craftsmanship  decongestant  \\\n",
+                            "0            1.0        0.0       0.0  ...            0.0           0.0   \n",
+                            "1            0.0        1.0       1.0  ...            0.0           0.0   \n",
+                            "2            2.0        0.0       0.0  ...            0.0           0.0   \n",
+                            "3            0.0        0.0       1.0  ...            0.0           0.0   \n",
+                            "4            0.0        0.0       0.0  ...            0.0           0.0   \n",
+                            "..           ...        ...       ...  ...            ...           ...   \n",
+                            "95           0.0        1.0       0.0  ...            0.0           0.0   \n",
+                            "96           0.0        0.0       0.0  ...            0.0           0.0   \n",
+                            "97           0.0        0.0       0.0  ...            0.0           1.0   \n",
+                            "98           0.0        1.0       1.0  ...            0.0           0.0   \n",
+                            "99           0.0        0.0       1.0  ...            1.0           0.0   \n",
                             "\n",
-                            "    astrophysics  immunology  ...  exercise  appetite  energy  football  \\\n",
-                            "0            1.0         1.0  ...       0.0       0.0     0.0       0.0   \n",
-                            "1            0.0         1.0  ...       0.0       0.0     0.0       0.0   \n",
-                            "2            0.0         0.0  ...       0.0       0.0     0.0       0.0   \n",
-                            "3            1.0         1.0  ...       0.0       0.0     0.0       0.0   \n",
-                            "4            1.0         1.0  ...       0.0       0.0     0.0       0.0   \n",
-                            "..           ...         ...  ...       ...       ...     ...       ...   \n",
-                            "95           0.0         1.0  ...       0.0       0.0     0.0       0.0   \n",
-                            "96           0.0         0.0  ...       0.0       1.0     0.0       0.0   \n",
-                            "97           1.0         0.0  ...       0.0       0.0     0.0       0.0   \n",
-                            "98           0.0         1.0  ...       0.0       0.0     0.0       0.0   \n",
-                            "99           0.0         0.0  ...       0.0       0.0     0.0       0.0   \n",
+                            "    electricity  immunology  injection  allergy  accuse  bankrupt  attorney  \\\n",
+                            "0           0.0         0.0        0.0      0.0     0.0       0.0       0.0   \n",
+                            "1           0.0         0.0        0.0      0.0     0.0       0.0       0.0   \n",
+                            "2           0.0         0.0        0.0      0.0     0.0       0.0       0.0   \n",
+                            "3           0.0         0.0        0.0      0.0     0.0       0.0       0.0   \n",
+                            "4           0.0         0.0        0.0      0.0     0.0       0.0       0.0   \n",
+                            "..          ...         ...        ...      ...     ...       ...       ...   \n",
+                            "95          0.0         1.0        0.0      0.0     0.0       1.0       0.0   \n",
+                            "96          0.0         0.0        0.0      0.0     2.0       3.0       0.0   \n",
+                            "97          0.0         0.0        1.0      0.0     0.0       0.0       0.0   \n",
+                            "98          0.0         0.0        0.0      0.0     0.0       1.0       1.0   \n",
+                            "99          0.0         2.0        1.0      0.0     0.0       1.0       0.0   \n",
                             "\n",
-                            "    injection  game  allergy  Symmetrical  decongestant  athletics  \n",
-                            "0         0.0   0.0      0.0          0.0           0.0        0.0  \n",
-                            "1         0.0   0.0      0.0          0.0           0.0        0.0  \n",
-                            "2         0.0   0.0      0.0          0.0           0.0        0.0  \n",
-                            "3         0.0   0.0      0.0          0.0           0.0        0.0  \n",
-                            "4         0.0   0.0      0.0          0.0           0.0        0.0  \n",
-                            "..        ...   ...      ...          ...           ...        ...  \n",
-                            "95        1.0   0.0      0.0          0.0           1.0        0.0  \n",
-                            "96        0.0   1.0      0.0          0.0           0.0        0.0  \n",
-                            "97        0.0   0.0      0.0          0.0           1.0        0.0  \n",
-                            "98        1.0   0.0      3.0          0.0           1.0        0.0  \n",
-                            "99        1.0   0.0      1.0          0.0           0.0        0.0  \n",
+                            "    fever  \n",
+                            "0     0.0  \n",
+                            "1     0.0  \n",
+                            "2     0.0  \n",
+                            "3     0.0  \n",
+                            "4     0.0  \n",
+                            "..    ...  \n",
+                            "95    0.0  \n",
+                            "96    0.0  \n",
+                            "97    1.0  \n",
+                            "98    1.0  \n",
+                            "99    0.0  \n",
                             "\n",
                             "[100 rows x 40 columns]"
                         ]
                     },
-                    "execution_count": 38,
+                    "execution_count": 69,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "doc_vocab_count_df = pd.DataFrame(\n",
                 "    data = doc_vocab_count,\n",
                 "    columns = list(result['vocab_to_idx'].keys())\n",
                 ")\n",
                 "doc_vocab_count_df"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": 74,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "There are 100 documents in the dataset after processing\n",
+                        "On average estimated document length is 20.0 words per document after processing\n",
+                        "There are 40 unique vocab in the corpus after processing\n"
+                    ]
+                }
+            ],
+            "source": [
+                "train_docs = Document(docs)\n"
+            ]
+        },
+        {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Our Model"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": 85,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Topic Dirichlet Prior, Alpha\n",
@@ -607,132 +804,66 @@
                         "\n",
                         "Var Inf - Word Dirichlet prior, Lambda\n",
                         "(5, 40)\n",
                         "\n",
                         "Var Inf - Topic Dirichlet prior, Gamma\n",
                         "(100, 5)\n",
                         "\n",
-                        "Size of the vocab is 40\n",
-                        "Init perplexity = 98.58226277506884\n",
-                        "End perplexity = 50.540589733975764\n"
+                        "Init perplexity = 84.99592157507153\n",
+                        "End perplexity = 45.96696541539976\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "[<matplotlib.lines.Line2D at 0x1100121f0>]"
+                            "[<matplotlib.lines.Line2D at 0x1115ae400>]"
                         ]
                     },
-                    "execution_count": 39,
+                    "execution_count": 85,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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GjBggLKysnT++edr1apV4f3GGN17773Kz89XVlaWSktLtXHjxvYopc3oQQEAwHrtElB+8IMfaOnSpfrd736nzz77TBdffLFKS0u1c+dOSdLcuXM1b948LViwQBUVFerevbvGjRunurq69iinTRyhgMItHgAALJPygHLkyBG9+uqrmjt3rv7jP/5DgwcP1v3336/Bgwdr/vz5Msbol7/8pX72s59p/PjxGjlypH77299q165dWrx4carLaTOXo3lIaJIFAMA6KQ8oTU1NCgQCyszMjNqelZWl5cuXa8uWLaqsrFRpaWl4n8fjUXFxscrLy1NdTpuFr6DQgwIAgGVSHlCys7NVUlKiBx98ULt27VIgENDzzz+v8vJy7d69W5WVlZIkr9cb9Tmv1xveF6u+vl5+vz/q1V6c3OIBAMBy7dKD8rvf/U7GGPXt21dut1vz5s3TpEmTZLef2I+bM2eOPB5P+NW/f/8UV9zK6WCpewAArNYuAWXQoEF69913dfDgQW3fvl0rV65UY2OjTj31VPl8PklSVVVV1GeqqqrC+2LNnDlTNTU14df27dvbo2xJLNQGAEBH0K7roHTv3l35+fk6cOCA3nrrLY0fP15FRUXy+XwqKysLH+f3+1VRUaGSkpK453G73crJyYl6tRd6UAAAsJ6zPU761ltvyRij008/XZs2bdJdd92loUOH6rrrrpPNZtP06dP10EMPaciQISoqKtKsWbNUUFCgK6+8sj3KaROXgx4UAACs1i4BpaamRjNnztSOHTuUl5enCRMmaPbs2XK5XJKku+++W4cOHdJNN92k6upqjR07VkuWLDlq5o8VQkvd04MCAIB1bMaYTveX2O/3y+PxqKamJuW3e95Zv0fXLVqlEX09euOWsSk9NwAAJ7O2/P3mWTwxQj0ojQF6UAAAsAoBJUbrwwI73YUlAAC6DAJKDKedpe4BALAaASVG+BYP04wBALAMASVGaJpxgGnGAABYhoASo3WhNgIKAABWIaDEcLIOCgAAliOgxHCGV5KlBwUAAKsQUGLwsEAAAKxHQInROouHgAIAgFUIKDFcDtZBAQDAagSUGI6IWzyd8DFFAAB0CQSUGKEeFImZPAAAWIWAEsPpaB0SbvMAAGANAkoMrqAAAGA9AkoMR2RAYS0UAAAsQUCJwRUUAACsR0CJYbPZombyAACA9COgxMED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AABpR0BJgKcZAwBgHQJKAq09KNziAQAg3VIeUAYOHCibzXbUa+rUqZKkuro6TZ06Vb169VKPHj00YcIEVVVVpbqMr83BFRQAACyT8oCyatUq7d69O/xaunSpJOk73/mOJOn222/XG2+8oVdeeUXvvvuudu3apauvvjrVZXxtzpYeFGOkICEFAIC0cqb6hL179476/pFHHtGgQYN0wQUXqKamRs8++6xefPFFffOb35QkLVy4UMOGDdOKFSt03nnnpbqcExa6xSNJjcGg3HaHhdUAAHByadcelIaGBj3//PO6/vrrZbPZtGbNGjU2Nqq0tDR8zNChQ1VYWKjy8vKE56mvr5ff7496tbdQk6zEYm0AAKRbuwaUxYsXq7q6Wtdee60kqbKyUhkZGcrNzY06zuv1qrKyMuF55syZI4/HE37179+/Hatu5ogIKPShAACQXu0aUJ599lldeumlKigo+FrnmTlzpmpqasKv7du3p6jCxFz21qFpYi0UAADSKuU9KCFbt27V22+/rddeey28zefzqaGhQdXV1VFXUaqqquTz+RKey+12y+12t1epcdntNtlszU2yTDUGACC92u0KysKFC9WnTx9dfvnl4W2jRo2Sy+VSWVlZeNuGDRu0bds2lZSUtFcpJ4wHBgIAYI12uYISDAa1cOFCTZkyRU5n64/weDy64YYbNGPGDOXl5SknJ0e33HKLSkpKOtQMnhCn3a7GQIBbPAAApFm7BJS3335b27Zt0/XXX3/Uvscff1x2u10TJkxQfX29xo0bp6effro9yvjaWO4eAABrtEtAufjii2VM/D/qmZmZeuqpp/TUU0+1x49OKYcjdIuHHhQAANKJZ/EkEVpNlisoAACkFwElifAtHnpQAABIKwJKEjwwEAAAaxBQknDRgwIAgCUIKEmErqA0cosHAIC0IqAkEWqSZaE2AADSi4CShNNBDwoAAFYgoCTROouHHhQAANKJgJIEs3gAALAGASUJp4MeFAAArEBAScIZnsXDLR4AANKJgJJE6BYPV1AAAEgvAkoSLgfP4gEAwAoElCQcPIsHAABLEFCScNpZ6h4AACsQUJJwcosHAABLEFCScHKLBwAASxBQkmChNgAArEFASYIeFAAArEFASSL0sMBGbvEAAJBWBJQknHaWugcAwAoElCToQQEAwBoElCRCt3iaeBYPAABpRUBJ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",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "lda = LDASmoothed(\n",
-                "    docs = result['documents'],\n",
                 "    num_topics = 5, \n",
-                "    word_ct_dict = result['vocab_doc_count_dict'], \n",
-                "    num_doc_population = 100,\n",
-                "    word_ct_array = result['vocab_doc_count_array'],\n",
                 ")\n",
-                "print(f'Size of the vocab is {lda.V}')\n",
-                "lambda_init = lda._lambda_ \n",
                 "\n",
-                "perplexes = lda.partial_fit(\n",
-                "    X = doc_vocab_count,\n",
+                "perplexes = lda.fit(\n",
+                "    train_doc= train_docs,\n",
                 "    sampling= False,\n",
                 "    verbose=True, \n",
                 "    return_perplexities=True,\n",
                 ")\n",
                 "\n",
                 "plt.plot(perplexes)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 40,
+            "execution_count": 80,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{0: 'accuse',\n",
-                            " 1: 'evidence',\n",
-                            " 2: 'bruise',\n",
-                            " 3: 'FIFA',\n",
-                            " 4: 'Craftsmanship',\n",
-                            " 5: 'picture',\n",
-                            " 6: 'court',\n",
-                            " 7: 'Technique',\n",
-                            " 8: 'astrophysics',\n",
-                            " 9: 'immunology',\n",
-                            " 10: 'divorce',\n",
-                            " 11: 'attorney',\n",
-                            " 12: 'contract',\n",
-                            " 13: 'bankrupt',\n",
-                            " 14: 'Olympic',\n",
-                            " 15: 'asymmetrical',\n",
-                            " 16: 'form',\n",
-                            " 17: 'recreation',\n",
-                            " 18: 'content',\n",
-                            " 19: 'genetics',\n",
-                            " 20: 'research',\n",
-                            " 21: 'concert',\n",
-                            " 22: 'quantum',\n",
-                            " 23: 'scientst',\n",
-                            " 24: 'electricity',\n",
-                            " 25: 'fever',\n",
-                            " 26: 'physical',\n",
-                            " 27: 'contagious',\n",
-                            " 28: 'infection',\n",
-                            " 29: 'copyright',\n",
-                            " 30: 'exercise',\n",
-                            " 31: 'appetite',\n",
-                            " 32: 'energy',\n",
-                            " 33: 'football',\n",
-                            " 34: 'injection',\n",
-                            " 35: 'game',\n",
-                            " 36: 'allergy',\n",
-                            " 37: 'Symmetrical',\n",
-                            " 38: 'decongestant',\n",
-                            " 39: 'athletics'}"
+                            "9.728987995308097"
                         ]
                     },
-                    "execution_count": 40,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "lda.idx_2_word"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 41,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "21.407206305103696"
-                        ]
-                    },
-                    "execution_count": 41,
+                    "execution_count": 80,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "lda._lambda_[0,30]"
             ]
@@ -745,107 +876,107 @@
                 "- As we can see, without update the hyper-parameter $\\alpha$ and $\\eta$, we extract keywords from topics almost correctly. \n",
                 "\n",
                 "Although we still can see that some are not perfect, i.e. electricity ranked higher than scientist "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 42,
+            "execution_count": 83,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Topic 0\n",
-                        "Top 1 -> Craftsmanship\n",
-                        "Top 2 -> Technique\n",
-                        "Top 3 -> exercise\n",
-                        "Top 4 -> FIFA\n",
-                        "Top 5 -> content\n",
+                        "Top 1 -> physical\n",
+                        "Top 2 -> quantum\n",
+                        "Top 3 -> research\n",
+                        "Top 4 -> scientst\n",
+                        "Top 5 -> astrophysics\n",
                         "\n",
                         "Topic 1\n",
-                        "Top 1 -> copyright\n",
-                        "Top 2 -> contract\n",
-                        "Top 3 -> attorney\n",
-                        "Top 4 -> accuse\n",
-                        "Top 5 -> divorce\n",
+                        "Top 1 -> divorce\n",
+                        "Top 2 -> attorney\n",
+                        "Top 3 -> court\n",
+                        "Top 4 -> bankrupt\n",
+                        "Top 5 -> contract\n",
                         "\n",
                         "Topic 2\n",
-                        "Top 1 -> immunology\n",
-                        "Top 2 -> genetics\n",
-                        "Top 3 -> quantum\n",
-                        "Top 4 -> astrophysics\n",
-                        "Top 5 -> infection\n",
-                        "\n",
-                        "Topic 3\n",
-                        "Top 1 -> electricity\n",
-                        "Top 2 -> Symmetrical\n",
+                        "Top 1 -> content\n",
+                        "Top 2 -> Craftsmanship\n",
                         "Top 3 -> concert\n",
                         "Top 4 -> asymmetrical\n",
-                        "Top 5 -> picture\n",
+                        "Top 5 -> Symmetrical\n",
+                        "\n",
+                        "Topic 3\n",
+                        "Top 1 -> recreation\n",
+                        "Top 2 -> FIFA\n",
+                        "Top 3 -> football\n",
+                        "Top 4 -> Olympic\n",
+                        "Top 5 -> athletics\n",
                         "\n",
                         "Topic 4\n",
-                        "Top 1 -> contagious\n",
+                        "Top 1 -> fever\n",
                         "Top 2 -> appetite\n",
-                        "Top 3 -> injection\n",
+                        "Top 3 -> contagious\n",
                         "Top 4 -> decongestant\n",
-                        "Top 5 -> allergy\n",
+                        "Top 5 -> injection\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "for topic_index in range(lda._lambda_.shape[0]):\n",
                 "\n",
                 "    top5 = np.argsort(lda._lambda_[topic_index,:],)[-5:]\n",
                 "    print(f\"Topic {topic_index}\")\n",
                 "    for i, idx in enumerate(top5):\n",
-                "        print(f\"Top {i+1} -> {lda.idx_2_word[idx]}\")\n",
+                "        print(f\"Top {i+1} -> {lda.train_doc.idx_to_vocab[idx]}\")\n",
                 "    print()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Target model"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 43,
+            "execution_count": 84,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "alpha -> 1\n",
                         "eta -> 1\n",
                         "lambda\n",
                         "(5, 40)\n",
-                        "Init perplexity = 96.88781201053929\n",
-                        "End perplexity = 50.53892348630458\n"
+                        "Init perplexity = 100.09491669750783\n",
+                        "End perplexity = 51.81904206040911\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "[<matplotlib.lines.Line2D at 0x110092820>]"
+                            "[<matplotlib.lines.Line2D at 0x111560dc0>]"
                         ]
                     },
-                    "execution_count": 43,
+                    "execution_count": 84,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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Kioq0qZNmyy2uOuJRqOaPXu2CgoKlJ6erqFDh+qOO+5ocT8Q+jl5f//733XBBRcoNzdXPp9Py5cvb3G+NX26b98+TZ06VRkZGcrMzNSVV16p/fv3d0yDjQOWLVtmUlJSzP/8z/+Yf/7zn+YnP/mJyczMNBUVFbab1mVNmDDBLFmyxKxfv96888475vvf/77Jz883+/fvT1xz1VVXmby8PFNcXGzefPNNc/rpp5szzjjDYqu7tjVr1pghQ4aYUaNGmeuvvz5xnH5uH/v27TODBw82l112mSktLTVbtmwxL7/8stm8eXPimvnz55twOGyWL19u3n33XfODH/zAFBQUmEOHDllsedcyd+5c069fP/OnP/3JbN261Tz99NOmV69e5ve//33iGvo5eX/5y1/Mrbfeap555hkjyTz77LMtzremT8877zzzrW99y6xevdr84x//MMcdd5yZMmVKh7TXifBx2mmnmRkzZiR+j0ajJjc318ybN89iq7qX3bt3G0lm5cqVxhhjKisrTSgUMk8//XTimg8//NBIMiUlJbaa2WVVV1ebYcOGmRUrVpizzjorET7o5/bzX//1X2b8+PFfeT4Wi5ns7Gzz61//OnGssrLSpKammieffNKLJnYL559/vrniiitaHLvooovM1KlTjTH0c3v4YvhoTZ9+8MEHRpJZu3Zt4poXX3zR+Hw+s2PHjnZvY7efdqmrq9O6detUVFSUOOb3+1VUVKSSkhKLLeteqqqqJEl9+/aVJK1bt0719fUt+n348OHKz8+n39tgxowZOv/881v0p0Q/t6fnn39eY8eO1cUXX6yBAwdq9OjRevDBBxPnt27dqvLy8hZ9HQ6HNW7cOPo6CWeccYaKi4u1ceNGSdK7776rVatWaeLEiZLo547Qmj4tKSlRZmamxo4dm7imqKhIfr9fpaWl7d6mTndjufa2Z88eRaNRZWVltTielZWljz76yFKrupdYLKaZM2fqzDPP1MknnyxJKi8vV0pKijIzM1tcm5WVpfLycgut7LqWLVumt956S2vXrj3iHP3cfrZs2aJFixbpxhtv1C9+8QutXbtWP/vZz5SSkqJp06Yl+vPL/ltCX7feLbfcokgkouHDhysQCCgajWru3LmaOnWqJNHPHaA1fVpeXq6BAwe2OB8MBtW3b98O6fduHz7Q8WbMmKH169dr1apVtpvS7ZSVlen666/XihUrlJaWZrs53VosFtPYsWN11113SZJGjx6t9evXa/HixZo2bZrl1nUfTz31lJ544gktXbpUJ510kt555x3NnDlTubm59LNDuv20S//+/RUIBI6o/q+oqFB2dralVnUf1157rf70pz/ptdde06BBgxLHs7OzVVdXp8rKyhbX0+/JWbdunXbv3q1TTjlFwWBQwWBQK1eu1MKFCxUMBpWVlUU/t5OcnBydeOKJLY6NGDFC27dvl6REf/LfkqNz00036ZZbbtEll1yikSNH6kc/+pFuuOEGzZs3TxL93BFa06fZ2dnavXt3i/MNDQ3at29fh/R7tw8fKSkpGjNmjIqLixPHYrGYiouLVVhYaLFlXZsxRtdee62effZZvfrqqyooKGhxfsyYMQqFQi36fcOGDdq+fTv9noRzzjlH77//vt55553EY+zYsZo6dWriOf3cPs4888wjlotv3LhRgwcPliQVFBQoOzu7RV9HIhGVlpbS10k4ePCg/P6WXz2BQECxWEwS/dwRWtOnhYWFqqys1Lp16xLXvPrqq4rFYho3blz7N6rdS1g7oWXLlpnU1FTz8MMPmw8++MBMnz7dZGZmmvLycttN67KuvvpqEw6Hzd/+9jeza9euxOPgwYOJa6666iqTn59vXn31VfPmm2+awsJCU1hYaLHV3cPhq12MoZ/by5o1a0wwGDRz5841mzZtMk888YTp0aOHefzxxxPXzJ8/32RmZprnnnvOvPfee2bSpEksAU3StGnTzDHHHJNYavvMM8+Y/v37m5tvvjlxDf2cvOrqavP222+bt99+20gy99xzj3n77bfNtm3bjDGt69PzzjvPjB492pSWlppVq1aZYcOGsdT2aN13330mPz/fpKSkmNNOO82sXr3adpO6NElf+liyZEnimkOHDplrrrnG9OnTx/To0cP8y7/8i9m1a5e9RncTXwwf9HP7eeGFF8zJJ59sUlNTzfDhw80DDzzQ4nwsFjOzZ882WVlZJjU11Zxzzjlmw4YNllrbNUUiEXP99deb/Px8k5aWZo499lhz6623mtra2sQ19HPyXnvttS/9b/K0adOMMa3r071795opU6aYXr16mYyMDHP55Zeb6urqDmmvz5jDtpUDAADoYN2+5gMAAHQuhA8AAOApwgcAAPAU4QMAAHiK8AEAADxF+AAAAJ4ifAAAAE8RPgAAgKcIHwAAwFOEDwAA4CnCBwAA8BThAwAAeOr/Ay4hLtMIuPerAAAAAElFTkSuQmCC",
+                        "image/png": "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7bXXqrW1NT0NNjDGGPPkk0+a3Nxc8+///u/m7bffNtddd50pKioyjY2NtpvWZ02cONGsWLHCvPXWW+a1114z3/jGN8zQoUNNa2tr+Jzrr7/elJWVmZqaGrN582ZzwQUXmHHjxllsdd+2ceNGM3z4cHPuueeam2++Obyffj5++/fvN8OGDTNXX321qaurMx988IFZs2aN2bFjR/icxYsXG6/Xa1atWmVef/11881vftOUl5ebQ4cOWWx537Nw4UIzaNAg88ILL5idO3eap59+2hQUFJhf/vKX4XPo6977wx/+YH74wx+aZ555xkgyzz77bNTxo+nTiy++2Jx33nlmw4YN5s9//rM5/fTTzbRp09LSXgJKt/PPP9/Mnj07/D4QCJjS0lKzaNEii606sezbt89IMuvWrTPGGNPU1GRycnLM008/HT7n3XffNZJMbW2trWb2WS0tLWbkyJFm7dq15sILLwwHFPo5NX7wgx+YCRMmJDweDAaNz+czP/nJT8L7mpqajMfjMb/97W8z0cQTxqWXXmpmzpwZte/yyy8306dPN8bQ16kQG1COpk/feecdI8ls2rQpfM4f//hH43A4zO7du1PeRr7ikXT48GFt2bJF1dXV4X1Op1PV1dWqra212LITS3NzsyRp4MCBkqQtW7aoo6Mjqt8rKio0dOhQ+v0YzJ49W5deemlUf0r0c6o899xzGjt2rK644goNGTJEo0eP1q9//evw8Z07d6qhoSGqn71eryorK+nnXho3bpxqamq0bds2SdLrr7+u9evX65JLLpFEX6fD0fRpbW2tioqKNHbs2PA51dXVcjqdqqurS3mbUv40477o448/ViAQUHFxcdT+4uJivffee5ZadWIJBoOaM2eOxo8fr7PPPluS1NDQoNzcXBUVFUWdW1xcrIaGBgut7LuefPJJ/fWvf9WmTZuOOEY/p8YHH3ygZcuWae7cufrXf/1Xbdq0Sd/97neVm5urGTNmhPsy3n9H6Ofeuf322+X3+1VRUSGXy6VAIKCFCxdq+vTpkkRfp8HR9GlDQ4OGDBkSddztdmvgwIFp6XcCCjJi9uzZeuutt7R+/XrbTTnh1NfX6+abb9batWuVl5dnuzknrGAwqLFjx+qee+6RJI0ePVpvvfWWli9frhkzZlhu3Ynlqaee0uOPP64nnnhCZ511ll577TXNmTNHpaWl9PXnCF/xSBo8eLBcLtcRsxoaGxvl8/ksterEceONN+qFF17Qyy+/rFNPPTW83+fz6fDhw2pqaoo6n37vnS1btmjfvn360pe+JLfbLbfbrXXr1mnp0qVyu90qLi6mn1OgpKREZ555ZtS+UaNGadeuXZIU7kv+O3L8br31Vt1+++2aOnWqzjnnHF111VW65ZZbtGjRIkn0dTocTZ/6fD7t27cv6nhnZ6f279+fln4noEjKzc3VmDFjVFNTE94XDAZVU1Ojqqoqiy3r24wxuvHGG/Xss8/qpZdeUnl5edTxMWPGKCcnJ6rft27dql27dtHvvXDRRRfpzTff1GuvvRbexo4dq+nTp4df08/Hb/z48UdMk9+2bZuGDRsmSSovL5fP54vqZ7/fr7q6Ovq5lw4ePCinM/rXk8vlUjAYlERfp8PR9GlVVZWampq0ZcuW8DkvvfSSgsGgKisrU9+olJfd9lFPPvmk8Xg8ZuXKleadd94xs2bNMkVFRaahocF20/qsG264wXi9XvOnP/3J7N27N7wdPHgwfM71119vhg4dal566SWzefNmU1VVZaqqqiy2+sQQOYvHGPo5FTZu3GjcbrdZuHCh2b59u3n88cdNv379zGOPPRY+Z/HixaaoqMj8/ve/N2+88YaZNGkSU1+PwYwZM8wpp5wSnmb8zDPPmMGDB5vbbrstfA593XstLS3m1VdfNa+++qqRZH7+85+bV1991Xz44YfGmKPr04svvtiMHj3a1NXVmfXr15uRI0cyzTgT7r//fjN06FCTm5trzj//fLNhwwbbTerTJMXdVqxYET7n0KFD5jvf+Y456aSTTL9+/cw//uM/mr1799pr9AkiNqDQz6nx/PPPm7PPPtt4PB5TUVFhHnrooajjwWDQzJ8/3xQXFxuPx2Muuugis3XrVkut7bv8fr+5+eabzdChQ01eXp457bTTzA9/+EPT3t4ePoe+7r2XX3457n+TZ8yYYYw5uj795JNPzLRp00xBQYEpLCw011xzjWlpaUlLex3GRCzNBwAAkAWoQQEAAFmHgAIAALIOAQUAAGQdAgoAAMg6BBQAAJB1CCgAACDrEFAAAEDWIaAAAICsQ0ABAABZh4ACAACyDgEFAABkHQIKAADIOv8f1N0l0SHzRHsAAAAASUVORK5CYII=",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -860,15 +991,15 @@
                 "sklearn_lda._init_latent_vars(n_features = lda.V)\n",
                 "\n",
                 "print(f\"alpha -> {sklearn_lda.doc_topic_prior}\")\n",
                 "print(f\"eta -> {sklearn_lda.topic_word_prior}\")\n",
                 "\n",
                 "print('lambda')\n",
                 "print(sklearn_lda.components_.shape)\n",
-                "assert (sklearn_lda.components_ == lambda_init).all()\n",
+                "#assert (sklearn_lda.components_ == lambda_init).all()\n",
                 "\n",
                 "perplxities_sklearn = []\n",
                 "init_perplexity = sklearn_lda._perplexity_precomp_distr(\n",
                 "    doc_vocab_count, \n",
                 "    doc_topic_distr = lda._gamma_,\n",
                 "    sub_sampling=False\n",
                 ")\n",
```

### Comparing `TuoTuo-0.2.6/requirements.txt` & `TuoTuo-0.2.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.6/setup.py` & `TuoTuo-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     return cythonize(
         extensions, 
     )
 
 setup(
     name = 'TuoTuo',
     packages = ['tuotuo'],
-    version = '0.2.6',  
+    version = '0.2.7',  
     license='MIT',
     description = 'LDA & Neura based topic modelling library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'tuotuo Superman',
     author_email = 'tuotuo@HanwellSquare.BigForce.com',
     url = 'https://github.com/RobbenRibery/TuoTuo',
-    download_url = 'https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-test-0.06.tar.gz',
+    download_url = 'https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-0.2.7.tar.gz',
     keywords = ['Generative Topic Modelling','Latent Dirichlet Allocation'],
     install_requires=[            
         'numpy',
         'torch',
         'scipy',
         'pyro-ppl',
         'pandas',
```

### Comparing `TuoTuo-0.2.6/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so` & `TuoTuo-0.2.7/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.6/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o` & `TuoTuo-0.2.7/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.6/tuotuo/cutils.c` & `TuoTuo-0.2.7/tuotuo/cutils.c`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.6/tuotuo/cutils.cpython-38-darwin.so` & `TuoTuo-0.2.7/tuotuo/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.6/tuotuo/cutils.pyx` & `TuoTuo-0.2.7/tuotuo/cutils.pyx`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.6/tuotuo/generator.py` & `TuoTuo-0.2.7/tuotuo/generator.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.6/tuotuo/lda_model.py` & `TuoTuo-0.2.7/tuotuo/lda_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import List, Dict
+from typing import List, Dict, Union 
 import warnings 
 
 import torch as np 
 import numpy as np 
 
 from scipy.special import psi, gammaln, logsumexp, polygamma
 
+from tuotuo.document import Document
 from tuotuo.utils import (
     get_vocab_from_docs, 
     get_np_wct, 
     np_clip_for_exp,
 )
-
 from tuotuo.cutils import _dirichlet_expectation_2d
 
 from pprint import pprint
 
 SEED = 42 
 DTYPE = float
 
@@ -49,95 +49,44 @@
     """
     Class implemented the Smoothed Version of Latent Dirichlet Allocation
 
     for smoothed version of Latent Dirichlet Allocation 
     """
 
     def __init__(
-            self, 
-            docs: List[List[str]],
+            self,
             num_topics: int,
-            word_ct_dict: dict,
-            num_doc_population: int, 
-            word_ct_array: np.ndarray = None,
-            word_to_idx: dict = None, 
-            idx_to_word: dict = None, 
+            exchangeable_prior: bool = True, 
             verbose: bool = True,
         ) -> None:
-
-        assert get_vocab_from_docs(docs) == word_ct_dict
         
-        self.D_population = num_doc_population
-        self.docs = docs 
-        
-        # number of documents 
-        self.M = len(docs)
-
-        # number of unique words in corpus 
-        if word_ct_array is not None:
-            assert word_ct_array.shape[0] == len(word_ct_dict)
-
-            val_word_ct_array, val_word2idx = get_np_wct(word_ct_dict, docs)
-            assert (word_ct_array == val_word_ct_array).all()
-
-            word_2_idx = val_word2idx 
-        else:
-            word_ct_array, word_2_idx = get_np_wct(word_ct_dict, docs)
-
-        self.word_ct_array = word_ct_array
-
-        self.word_2_idx = word_2_idx 
-        self.word_2_idx:dict 
-
-        self.idx_2_word = {v:k for k,v in self.word_2_idx.items()}
-        self.idx_2_word: dict
-
-        # number of unique words in the corpus 
-        self.V = word_ct_array.shape[0]  
-
+        ## ------ parameters init ------ ##
         # number of topics 
         self.K = num_topics
 
-        #parameters init
+        ## ------ parameters init ------ ##
         # define the DGM hyper-parameters
         # Dirichlet Prior 
         np.random.seed(SEED)
-        self._alpha_ = 1#np.random.gamma(shape = 100, scale = 0.01, size =self.K)
-
+        if exchangeable_prior:
+            self._alpha_ = 1
+        else:
+            self._alpha_ = np.random.gamma(shape = 100, scale = 0.01, size = self.K)
         if verbose:
             print(f"Topic Dirichlet Prior, Alpha")
             print(self._alpha_)
             print() 
+
         # Dirichlet Prior - Exchangeable Dirichlet
         self._eta_ = 1
-
         if verbose:
             print(f"Exchangeable Word Dirichlet Prior, Eta ")
             print(self._eta_)
             print()
 
-
-        # define the Convexity-based Varitional Inference hyper-parameters 
-        #Dirichlet Prior, Surrogate for _eta_ 
-        np.random.seed(SEED)
-        self._lambda_ = np.random.gamma(shape=100, scale=0.01, size=(self.K, self.V),).astype(DTYPE, copy = False)
-        if verbose: 
-            print(f"Var Inf - Word Dirichlet prior, Lambda")
-            print(self._lambda_.shape)
-            print()
-
-        #Dirichlet Prior, Surrogate for _alpha_ 
-        self._gamma_ = self._alpha_ + np.ones((self.M,self.K), dtype=DTYPE) * self.V / self.K  
-        self._gamma_ = self._gamma_.astype(DTYPE, copy=False)
-        self._gamma_ : np.ndarray
-        if verbose: 
-            print(f"Var Inf - Topic Dirichlet prior, Gamma")
-            print(self._gamma_.shape)
-            print()
-
     def approx_elbo(
             self,
             X:np.ndarray,
             sampling:bool = False, 
             expec_log_theta: np.ndarray = None, 
             expec_log_beta: np.ndarray = None,
         ) -> float:
@@ -216,15 +165,16 @@
             self, 
             X:np.ndarray, 
             sampling:bool = False,
             expec_log_theta: np.ndarray = None, 
             expec_log_beta: np.ndarray = None,
         ) -> float: 
 
-        """compute the perplexity (per document) based on the approximated ELBO
+        """
+        compute the perplexity (per document) based on the approximated ELBO
 
         """
         num_doc = 1 if X.ndim == 1 else X.shape[0]
         elbo, expec_logs = self.approx_elbo(
             X, 
             sampling,
             expec_log_theta,
@@ -358,32 +308,61 @@
                 self.m_step(
                 lambda_update,
                 verbose,
         )
 
         return expec_log_theta, expec_log_beta
     
-    def partial_fit(
+    def fit(
         self, 
-        X:np.ndarray,
+        train_doc:Document,
         sampling:bool = False,
         threshold:float = 1e-05,
         em_num_step: int = 100,
         e_num_step:int = 100,
         batch:bool = True,
         verbose = False,
         return_perplexities: bool = False,
     ) -> None:  
         
-        """Complete the EM step, without updateing the hypterparameter
+        """Complete the EM step, without updating the hypterparameter
 
         Returns:
             _type_: _description_
         """
+
+        ## --- hyper param collection --- ## 
+        # number of document in training corpus 
+        self.train_doc = train_doc
+        self.M = train_doc.M
+
+        # number of unique words in the corpus 
+        self.V = train_doc.V 
+
+        # doc vocab count array
+        X = train_doc.doc_vocab_count_array
         
+        ## --- paramerters initilisation --- ##
+        # define the Convexity-based Varitional Inference hyper-parameters 
+        # Dirichlet Prior, Surrogate for _eta_ 
+        np.random.seed(SEED)
+        self._lambda_ = np.random.gamma(shape=100, scale=0.01, size=(self.K, self.V),).astype(DTYPE, copy = False)
+        if verbose: 
+            print(f"Var Inf - Word Dirichlet prior, Lambda")
+            print(self._lambda_.shape)
+            print()
+
+        #Dirichlet Prior, Surrogate for _alpha_ 
+        self._gamma_ = self._alpha_ + np.ones((self.M, self.K), dtype=DTYPE) * self.V / self.K  
+        self._gamma_ : np.ndarray
+        self._gamma_ = self._gamma_.astype(DTYPE, copy=False)
+        if verbose: 
+            print(f"Var Inf - Topic Dirichlet prior, Gamma")
+            print(self._gamma_.shape)
+            print()
 
         perplexities = []
         perplexity, expec_logs = \
             self.approx_perplexity(
             X,
             sampling=sampling,
         )
```

