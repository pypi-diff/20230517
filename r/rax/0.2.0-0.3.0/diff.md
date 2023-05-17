# Comparing `tmp/rax-0.2.0.tar.gz` & `tmp/rax-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rax-0.2.0.tar", last modified: Thu Aug 11 19:34:05 2022, max compression
+gzip compressed data, was "rax-0.3.0.tar", last modified: Wed May 17 19:24:42 2023, max compression
```

## Comparing `rax-0.2.0.tar` & `rax-0.3.0.tar`

### file list

```diff
@@ -1,50 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 19:34:05.215450 rax-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-11 19:29:48.000000 rax-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-11 19:29:48.000000 rax-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4027 2022-08-11 19:34:05.215450 rax-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3258 2022-08-11 19:29:48.000000 rax-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 19:34:05.211450 rax-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     3966 2022-08-11 19:29:48.000000 rax-0.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 19:34:05.211450 rax-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-08-11 19:29:48.000000 rax-0.2.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 19:34:05.211450 rax-0.2.0/examples/approx_metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-08-11 19:29:48.000000 rax-0.2.0/examples/approx_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6067 2022-08-11 19:29:48.000000 rax-0.2.0/examples/approx_metrics/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-08-11 19:29:48.000000 rax-0.2.0/examples/approx_metrics/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 19:34:05.211450 rax-0.2.0/examples/flax_integration/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-08-11 19:29:48.000000 rax-0.2.0/examples/flax_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5675 2022-08-11 19:29:48.000000 rax-0.2.0/examples/flax_integration/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-08-11 19:29:48.000000 rax-0.2.0/examples/flax_integration/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 19:34:05.215450 rax-0.2.0/examples/t5x/
--rw-r--r--   0 runner    (1001) docker     (121)    12615 2022-08-11 19:29:48.000000 rax-0.2.0/examples/t5x/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     6762 2022-08-11 19:29:48.000000 rax-0.2.0/examples/t5x/models_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3632 2022-08-11 19:29:48.000000 rax-0.2.0/examples/t5x/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3171 2022-08-11 19:29:48.000000 rax-0.2.0/examples/t5x/tasks_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 19:34:05.215450 rax-0.2.0/rax/
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-08-11 19:29:48.000000 rax-0.2.0/rax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 19:34:05.215450 rax-0.2.0/rax/_src/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-08-11 19:29:48.000000 rax-0.2.0/rax/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21791 2022-08-11 19:29:48.000000 rax-0.2.0/rax/_src/losses.py
--rw-r--r--   0 runner    (1001) docker     (121)    21807 2022-08-11 19:29:48.000000 rax-0.2.0/rax/_src/losses_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    21904 2022-08-11 19:29:48.000000 rax-0.2.0/rax/_src/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    12576 2022-08-11 19:29:48.000000 rax-0.2.0/rax/_src/metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8162 2022-08-11 19:29:48.000000 rax-0.2.0/rax/_src/t12n.py
--rw-r--r--   0 runner    (1001) docker     (121)     9546 2022-08-11 19:29:48.000000 rax-0.2.0/rax/_src/t12n_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-08-11 19:29:48.000000 rax-0.2.0/rax/_src/types.py
--rw-r--r--   0 runner    (1001) docker     (121)    15183 2022-08-11 19:29:48.000000 rax-0.2.0/rax/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10699 2022-08-11 19:29:48.000000 rax-0.2.0/rax/_src/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-08-11 19:29:48.000000 rax-0.2.0/rax/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-08-11 19:29:48.000000 rax-0.2.0/rax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 19:34:05.215450 rax-0.2.0/rax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4027 2022-08-11 19:34:05.000000 rax-0.2.0/rax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-08-11 19:34:05.000000 rax-0.2.0/rax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-11 19:34:05.000000 rax-0.2.0/rax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-08-11 19:34:05.000000 rax-0.2.0/rax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-08-11 19:34:05.000000 rax-0.2.0/rax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 19:34:05.215450 rax-0.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-11 19:29:48.000000 rax-0.2.0/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-11 19:29:48.000000 rax-0.2.0/requirements/requirements-examples.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-11 19:29:48.000000 rax-0.2.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-08-11 19:29:48.000000 rax-0.2.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-11 19:34:05.215450 rax-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-08-11 19:29:48.000000 rax-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:24:42.683075 rax-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 19:21:10.000000 rax-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 19:21:10.000000 rax-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-17 19:24:42.683075 rax-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-17 19:21:10.000000 rax-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:24:42.679075 rax-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-17 19:21:10.000000 rax-0.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:24:42.679075 rax-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-17 19:21:10.000000 rax-0.3.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:24:42.679075 rax-0.3.0/examples/approx_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-17 19:21:10.000000 rax-0.3.0/examples/approx_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-05-17 19:21:10.000000 rax-0.3.0/examples/approx_metrics/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-17 19:21:10.000000 rax-0.3.0/examples/approx_metrics/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:24:42.679075 rax-0.3.0/examples/flax_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-17 19:21:10.000000 rax-0.3.0/examples/flax_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-05-17 19:21:10.000000 rax-0.3.0/examples/flax_integration/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-17 19:21:10.000000 rax-0.3.0/examples/flax_integration/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:24:42.679075 rax-0.3.0/examples/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-17 19:21:10.000000 rax-0.3.0/examples/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-17 19:21:10.000000 rax-0.3.0/examples/segmentation/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-17 19:21:10.000000 rax-0.3.0/examples/segmentation/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:24:42.679075 rax-0.3.0/examples/t5x/
+-rw-r--r--   0 runner    (1001) docker     (123)    12697 2023-05-17 19:21:10.000000 rax-0.3.0/examples/t5x/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-17 19:21:10.000000 rax-0.3.0/examples/t5x/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-17 19:21:10.000000 rax-0.3.0/examples/t5x/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-17 19:21:10.000000 rax-0.3.0/examples/t5x/tasks_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:24:42.679075 rax-0.3.0/rax/
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-17 19:21:10.000000 rax-0.3.0/rax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:24:42.683075 rax-0.3.0/rax/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/lambdaweights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/lambdaweights_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32179 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31294 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/losses_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26385 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/segment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/segment_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/t12n.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19455 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/t12n_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22174 2023-05-17 19:21:10.000000 rax-0.3.0/rax/_src/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-17 19:21:10.000000 rax-0.3.0/rax/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-17 19:21:10.000000 rax-0.3.0/rax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:24:42.683075 rax-0.3.0/rax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-17 19:24:42.000000 rax-0.3.0/rax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 19:24:42.000000 rax-0.3.0/rax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:24:42.000000 rax-0.3.0/rax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 19:24:42.000000 rax-0.3.0/rax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 19:24:42.000000 rax-0.3.0/rax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:24:42.683075 rax-0.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 19:21:10.000000 rax-0.3.0/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-17 19:21:10.000000 rax-0.3.0/requirements/requirements-examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 19:21:10.000000 rax-0.3.0/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 19:21:10.000000 rax-0.3.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:24:42.683075 rax-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-17 19:21:10.000000 rax-0.3.0/setup.py
```

### Comparing `rax-0.2.0/LICENSE` & `rax-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rax-0.2.0/PKG-INFO` & `rax-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: rax
-Version: 0.2.0
-Summary: Composable Learning-to-Rank using JAX.
+Version: 0.3.0
+Summary: Learning-to-Rank using JAX.
 Home-page: https://github.com/google/rax
 Author: Google
 Author-email: rax-dev@google.com
 License: Apache 2.0
 Keywords: learning-to-rank jax ranking
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 🦖 **Rax**: Composable Learning to Rank using JAX
+# 🦖 **Rax**: Learning-to-Rank using JAX
 
 [![Docs](https://readthedocs.org/projects/rax/badge/?version=latest)](https://rax.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/rax?color=brightgreen)](https://pypi.org/project/rax/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-brightgreen.svg)](https://github.com/google/rax/blob/main/LICENSE)
 
 **Rax** is a Learning-to-Rank library written in JAX. Rax provides off-the-shelf
 implementations of ranking losses and metrics to be used with JAX. It provides
@@ -53,40 +53,48 @@
 In a nutshell, given the scores and labels for a list of items, Rax can compute
 various ranking losses and metrics:
 
 ```python
 import jax.numpy as jnp
 import rax
 
-scores = jnp.asarray([2.2, -1.3, 5.4])  # output of a model.
-labels = jnp.asarray([1., 0., 0.])      # indicates doc 1 is relevant.
+scores = jnp.array([2.2, -1.3, 5.4])  # output of a model.
+labels = jnp.array([1.0,  0.0, 0.0])  # indicates doc 1 is relevant.
 
-rax.ndcg_metric(scores, labels)         # computes a ranking metric.
-rax.pairwise_hinge_loss(scores, labels) # computes a ranking loss.
+rax.ndcg_metric(scores, labels)  # computes a ranking metric.
+# 0.63092977
+
+rax.pairwise_hinge_loss(scores, labels)  # computes a ranking loss.
+# 2.1
 ```
 
 All of the Rax losses and metrics are purely functional and compose well with
 standard JAX transformations. Additionally, Rax provides ranking-specific
 transformations so you can build new ranking losses. An example is
 `rax.approx_t12n`, which can be used to transform any (non-differentiable)
 ranking metric into a differentiable loss. For example:
 
 ```python
 loss_fn = rax.approx_t12n(rax.ndcg_metric)
-loss_fn(scores, labels)            # differentiable approx ndcg loss.
+loss_fn(scores, labels)  # differentiable approx ndcg loss.
+# -0.63282484
+
 jax.grad(loss_fn)(scores, labels)  # computes gradients w.r.t. scores.
+# [-0.01276882  0.00549765  0.00727116]
 ```
 
 ## Installation
 
 See https://github.com/google/jax#installation for instructions on installing JAX.
 
 We suggest installing the latest stable version of Rax by running:
 
-`$ pip install rax`
+```
+$ pip install rax
+```
 
 ## Examples
 
 See the `examples/` directory for complete examples on how to use Rax.
 
 ## Citing Rax
```

### Comparing `rax-0.2.0/README.md` & `rax-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 🦖 **Rax**: Composable Learning to Rank using JAX
+# 🦖 **Rax**: Learning-to-Rank using JAX
 
 [![Docs](https://readthedocs.org/projects/rax/badge/?version=latest)](https://rax.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/rax?color=brightgreen)](https://pypi.org/project/rax/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-brightgreen.svg)](https://github.com/google/rax/blob/main/LICENSE)
 
 **Rax** is a Learning-to-Rank library written in JAX. Rax provides off-the-shelf
 implementations of ranking losses and metrics to be used with JAX. It provides
@@ -32,40 +32,48 @@
 In a nutshell, given the scores and labels for a list of items, Rax can compute
 various ranking losses and metrics:
 
 ```python
 import jax.numpy as jnp
 import rax
 
-scores = jnp.asarray([2.2, -1.3, 5.4])  # output of a model.
-labels = jnp.asarray([1., 0., 0.])      # indicates doc 1 is relevant.
+scores = jnp.array([2.2, -1.3, 5.4])  # output of a model.
+labels = jnp.array([1.0,  0.0, 0.0])  # indicates doc 1 is relevant.
 
-rax.ndcg_metric(scores, labels)         # computes a ranking metric.
-rax.pairwise_hinge_loss(scores, labels) # computes a ranking loss.
+rax.ndcg_metric(scores, labels)  # computes a ranking metric.
+# 0.63092977
+
+rax.pairwise_hinge_loss(scores, labels)  # computes a ranking loss.
+# 2.1
 ```
 
 All of the Rax losses and metrics are purely functional and compose well with
 standard JAX transformations. Additionally, Rax provides ranking-specific
 transformations so you can build new ranking losses. An example is
 `rax.approx_t12n`, which can be used to transform any (non-differentiable)
 ranking metric into a differentiable loss. For example:
 
 ```python
 loss_fn = rax.approx_t12n(rax.ndcg_metric)
-loss_fn(scores, labels)            # differentiable approx ndcg loss.
+loss_fn(scores, labels)  # differentiable approx ndcg loss.
+# -0.63282484
+
 jax.grad(loss_fn)(scores, labels)  # computes gradients w.r.t. scores.
+# [-0.01276882  0.00549765  0.00727116]
 ```
 
 ## Installation
 
 See https://github.com/google/jax#installation for instructions on installing JAX.
 
 We suggest installing the latest stable version of Rax by running:
 
-`$ pip install rax`
+```
+$ pip install rax
+```
 
 ## Examples
 
 See the `examples/` directory for complete examples on how to use Rax.
 
 ## Citing Rax
```

### Comparing `rax-0.2.0/docs/conf.py` & `rax-0.3.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -108,14 +108,22 @@
 
 # -- Options for bibtex ------------------------------------------------------
 
 bibtex_bibfiles = ['references.bib']
 bibtex_default_style = 'alpha'
 bibtex_reference_style = 'author_year'
 
+# -- Options for katex -------------------------------------------------------
+
+katex_options = r'''{
+    macros: {
+        "\\II": "\\mathbb{I}\\left[#1\\right]",
+        "\\op": "\\operatorname{#1}",
+    }
+}'''
 
 # -- Intersphinx configuration -----------------------------------------------
 
 intersphinx_mapping = {
     'jax': ('https://jax.readthedocs.io/en/latest/', None),
     'python': ('https://docs.python.org/3', None)
 }
```

### Comparing `rax-0.2.0/examples/__init__.py` & `rax-0.3.0/examples/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rax-0.2.0/examples/approx_metrics/__init__.py` & `rax-0.3.0/examples/approx_metrics/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rax-0.2.0/examples/approx_metrics/main.py` & `rax-0.3.0/examples/approx_metrics/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,27 +15,27 @@
 """Example of training a linear model on MSLR-WEB10K with approximate metrics.
 
 Usage with example output:
 
 $ python examples/approx_metrics/main.py
 {
   "ApproxAP": {
-    "AP": 0.5947682857513428,
-    "NDCG": 0.6587949991226196,
-    "R@50": 0.5807018876075745
+    "AP": 0.5950086116790771,
+    "NDCG": 0.6588592529296875,
+    "R@50": 0.5810613036155701
   },
   "ApproxNDCG": {
-    "AP": 0.587692141532898,
-    "NDCG": 0.6700138449668884,
-    "R@50": 0.5744442939758301
+    "AP": 0.587402880191803,
+    "NDCG": 0.6703540086746216,
+    "R@50": 0.5748950839042664
   },
   "ApproxR@50": {
-    "AP": 0.5849018096923828,
-    "NDCG": 0.6449851989746094,
-    "R@50": 0.5746314525604248
+    "AP": 0.5854976177215576,
+    "NDCG": 0.6438423991203308,
+    "R@50": 0.5757840871810913
   }
 }
 """
 
 import functools
 import json
 from typing import Optional, Sequence
@@ -47,25 +47,33 @@
 import rax
 
 # Used for loading data and data-preprocessing.
 import tensorflow as tf
 import tensorflow_datasets as tfds
 
 
-def prepare_dataset(ds: tf.data.Dataset,
-                    batch_size: int = 128,
-                    list_size: Optional[int] = 200,
-                    shuffle_size: Optional[int] = 1000,
-                    rng_seed: int = 42):
+def prepare_dataset(
+    ds: tf.data.Dataset,
+    batch_size: int = 128,
+    list_size: Optional[int] = 200,
+    shuffle_size: Optional[int] = 1000,
+    rng_seed: int = 42,
+):
   """Prepares a training dataset by applying padding/truncating/etc."""
   tf.random.set_seed(rng_seed)
   ds = ds.cache()
+  features_to_keep = set(["label", "float_features"])
+  ds = ds.map(lambda e: {k: v for k, v in e.items() if k in features_to_keep})
   ds = ds.map(lambda e: {**e, "mask": tf.ones_like(e["label"], dtype=tf.bool)})
   if list_size is not None:
-    pad = lambda t: tf.concat([t, tf.zeros(list_size, dtype=t.dtype)], -1)
+
+    def pad(t):
+      shape = tf.concat([tf.constant([list_size]), tf.shape(t)[1:]], 0)
+      return tf.concat([t, tf.zeros(shape, dtype=t.dtype)], 0)
+
     truncate = lambda t: t[:list_size]
     ds = ds.map(lambda e: tf.nest.map_structure(pad, e))
     ds = ds.map(lambda e: tf.nest.map_structure(truncate, e))
   if shuffle_size is not None:
     ds = ds.shuffle(shuffle_size, seed=rng_seed)
   ds = ds.padded_batch(batch_size)
   ds = ds.map(lambda e: (e, e.pop("label"), e.pop("mask")))
@@ -81,17 +89,15 @@
     w: The weights of the model.
     features: The features as input to the model.
 
   Returns:
     The model scores.
   """
   log1p = lambda x: jnp.sign(x) * jnp.log1p(jnp.abs(x))
-  features = jnp.concatenate(
-      [jnp.expand_dims(f, axis=-1) for f in features.values()], axis=-1)
-  return jnp.dot(log1p(features), w)
+  return jnp.dot(log1p(features["float_features"]), w)
 
 
 def train(ds, approx_metric, epochs: int = 10, lr: float = 10.0, seed: int = 7):
   """Trains a model using the given `approx_metric`.
 
   Args:
     ds: The dataset to train on.
@@ -100,15 +106,15 @@
     lr: The learning rate to use.
     seed: Random seed to initialize the model weights.
 
   Returns:
     The learned weights.
   """
   # Initialize the model weights.
-  number_of_features = len(next(iter(ds))[0])
+  number_of_features = next(iter(ds))[0]["float_features"].shape[-1]
   w = jax.random.uniform(jax.random.PRNGKey(seed), (number_of_features,))
 
   # Define loss and gradient function.
   def loss_fn(w, batch):
     features, labels, mask = batch
     scores = model_fn(w, features)
     return approx_metric(scores, labels, where=mask)
@@ -132,25 +138,26 @@
     metrics: A dict of metric callables.
 
   Returns:
     A dict with the same keys as metrics but with the computed metric values.
   """
   # Define initial metric values.
   metric_values = {
-      metric_name: Average(jnp.float32(0.), jnp.int32(0))
+      metric_name: Average(jnp.float32(0.0), jnp.int32(0))
       for metric_name in metrics
   }
 
   @jax.jit
   def update_metric_values(batch, metric_values):
     features, labels, mask = batch
     scores = model_fn(w, features)
     for metric_name, metric in metrics.items():
       metric_values[metric_name] = metric_values[metric_name].merge(
-          Average(metric(scores, labels, where=mask), jnp.int32(1)))
+          Average(metric(scores, labels, where=mask), jnp.int32(1))
+      )
     return metric_values
 
   # Iterate over each batch and update the metric average values.
   for batch in ds:
     metric_values = update_metric_values(batch, metric_values)
 
   # Return final metric values.
@@ -169,31 +176,32 @@
   # Build approx metrics. This uses the approx transformation to get an
   # approximate and differentiable version of the ranking metric. You can use
   # any of the Rax ranking metrics here. For this example, we will optimize AP,
   # NDCG and Recall@50.
   approx_ap = rax.approx_t12n(rax.ap_metric)
   approx_ndcg = rax.approx_t12n(rax.ndcg_metric)
   approx_recall_at_50 = rax.approx_t12n(
-      functools.partial(rax.recall_metric, topn=50))
+      functools.partial(rax.recall_metric, topn=50)
+  )
 
   # Train model with each of the approx metrics.
   w_ndcg = train(ds_train, approx_ndcg, epochs=epochs)
   w_ap = train(ds_train, approx_ap, epochs=epochs)
   w_recall = train(ds_train, approx_recall_at_50, epochs=epochs)
 
   # Evaluate each model on exact metrics and print a table of results:
   metrics = {
       "AP": rax.ap_metric,
       "NDCG": rax.ndcg_metric,
-      "R@50": functools.partial(rax.recall_metric, topn=50)
+      "R@50": functools.partial(rax.recall_metric, topn=50),
   }
 
   output = {
       "ApproxAP": eval_metrics(ds_train, w_ap, metrics),
       "ApproxNDCG": eval_metrics(ds_train, w_ndcg, metrics),
-      "ApproxR@50": eval_metrics(ds_train, w_recall, metrics)
+      "ApproxR@50": eval_metrics(ds_train, w_recall, metrics),
   }
   print(json.dumps(output, sort_keys=True, indent=2))
 
 
 if __name__ == "__main__":
   app.run(main)
```

### Comparing `rax-0.2.0/examples/flax_integration/__init__.py` & `rax-0.3.0/examples/flax_integration/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rax-0.2.0/examples/flax_integration/main.py` & `rax-0.3.0/examples/flax_integration/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,32 +16,32 @@
 
 Usage with example output:
 
 $ python examples/flax_integration/web30k.py
 [
   {
     "epoch": 1,
-    "loss": 371.3304748535156,
-    "metric/mrr": 0.8062829971313477,
-    "metric/ndcg": 0.6677320003509521,
-    "metric/ndcg@10": 0.4055347740650177
+    "loss": 371.3760681152344,
+    "metric/mrr": 0.8013861179351807,
+    "metric/ndcg": 0.6640667915344238,
+    "metric/ndcg@10": 0.3997730612754822
   },
   {
     "epoch": 2,
-    "loss": 370.42974853515625,
-    "metric/mrr": 0.8242350220680237,
-    "metric/ndcg": 0.6812514662742615,
-    "metric/ndcg@10": 0.43049752712249756
+    "loss": 370.382568359375,
+    "metric/mrr": 0.8243892192840576,
+    "metric/ndcg": 0.6807379722595215,
+    "metric/ndcg@10": 0.4295048117637634
   },
   {
     "epoch": 3,
-    "loss": 370.25244140625,
-    "metric/mrr": 0.8261540532112122,
-    "metric/ndcg": 0.6834192276000977,
-    "metric/ndcg@10": 0.4342570900917053
+    "loss": 370.13616943359375,
+    "metric/mrr": 0.8290443420410156,
+    "metric/ndcg": 0.684340238571167,
+    "metric/ndcg@10": 0.4365743100643158
   }
 ]
 """
 
 import collections
 import functools
 import json
@@ -67,17 +67,15 @@
 
 
 class DNN(nn.Module):
   """Implements a basic deep neural network for ranking."""
 
   @nn.compact
   def __call__(self, inputs):
-    # Concatenate the features into a feature vector.
-    x = [jnp.expand_dims(x, -1) for x in inputs.values()]
-    x = jnp.concatenate(x, -1)
+    x = inputs["float_features"]
 
     # Perform log1p transformation on the features.
     x = jnp.sign(x) * jnp.log1p(jnp.abs(x))
 
     # Run inputs through several layers, finally producing a single score per
     # item.
     x = nn.Dense(64)(x)
@@ -87,25 +85,33 @@
     x = nn.Dense(1)(x)
 
     # Remove the feature axis since it is now a single score per item.
     x = jnp.squeeze(x, -1)
     return x
 
 
-def prepare_dataset(ds: tf.data.Dataset,
-                    batch_size: int = 128,
-                    list_size: Optional[int] = 200,
-                    shuffle_size: Optional[int] = 1000,
-                    rng_seed: int = 42):
+def prepare_dataset(
+    ds: tf.data.Dataset,
+    batch_size: int = 128,
+    list_size: Optional[int] = 200,
+    shuffle_size: Optional[int] = 1000,
+    rng_seed: int = 42,
+):
   """Prepares a training dataset by applying padding/truncating/etc."""
   tf.random.set_seed(rng_seed)
   ds = ds.cache()
+  features_to_keep = set(["label", "float_features"])
+  ds = ds.map(lambda e: {k: v for k, v in e.items() if k in features_to_keep})
   ds = ds.map(lambda e: {**e, "mask": tf.ones_like(e["label"], dtype=tf.bool)})
   if list_size is not None:
-    pad = lambda t: tf.concat([t, tf.zeros(list_size, dtype=t.dtype)], -1)
+
+    def pad(t):
+      shape = tf.concat([tf.constant([list_size]), tf.shape(t)[1:]], 0)
+      return tf.concat([t, tf.zeros(shape, dtype=t.dtype)], 0)
+
     truncate = lambda t: t[:list_size]
     ds = ds.map(lambda e: tf.nest.map_structure(pad, e))
     ds = ds.map(lambda e: tf.nest.map_structure(truncate, e))
   if shuffle_size is not None:
     ds = ds.shuffle(shuffle_size, seed=rng_seed)
   ds = ds.padded_batch(batch_size)
   ds = ds.map(lambda e: (e, e.pop("label"), e.pop("mask")))
@@ -115,31 +121,32 @@
 
 def main(argv: Sequence[str]):
   del argv  # unused.
 
   # Load datasets.
   ds_train = prepare_dataset(tfds.load("mslr_web/30k_fold1", split="train"))
 
-  # Create model and optimizer.
+  # Create model and optimizer. The learning rate is set to a small value to
+  # ensure convergence and stability during training.
   model = DNN()
-  optimizer = optax.adam(learning_rate=0.01)
+  optimizer = optax.adam(learning_rate=0.001)
 
   # Create Rax loss and metrics.
   loss_fn = rax.softmax_loss
   metric_fns = {
       "metric/mrr": rax.mrr_metric,
       "metric/ndcg": rax.ndcg_metric,
-      "metric/ndcg@10": functools.partial(rax.ndcg_metric, topn=10)
+      "metric/ndcg@10": functools.partial(rax.ndcg_metric, topn=10),
   }
 
   # Implement train and eval logic.
   @jax.jit
   def train_step(
-      batch, model_state: ModelState,
-      opt_state: OptState) -> Tuple[jnp.ndarray, ModelState, OptState]:
+      batch, model_state: ModelState, opt_state: OptState
+  ) -> Tuple[jnp.ndarray, ModelState, OptState]:
     # Unpack batch.
     inputs, labels, mask = batch
 
     # Compute gradients wrt model params
     def _loss_fn(params):
       scores = model.apply(model_state.copy({"params": params}), inputs)
       loss = loss_fn(scores, labels, where=mask, reduce_fn=jnp.mean)
```

### Comparing `rax-0.2.0/examples/flax_integration/main_test.py` & `rax-0.3.0/examples/flax_integration/main_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -28,15 +28,16 @@
 
 class Web30kTest(absltest.TestCase):
 
   def test_end_to_end(self):
     mock_stdout = io.StringIO()
     with mock.patch("sys.stdout", mock_stdout):
       with tfds.testing.mock_data(
-          num_examples=256, policy=tfds.testing.MockPolicy.USE_CODE):
+          num_examples=16, policy=tfds.testing.MockPolicy.USE_CODE
+      ):
         argv = ()
         main.main(argv)
 
     # Get stdout output and parse json.
     output = json.loads(mock_stdout.getvalue())
 
     # Epochs should increase.
@@ -51,13 +52,13 @@
     # Metrics should increase consistently.
     self.assertLess(output[0]["metric/ndcg"], output[1]["metric/ndcg"])
     self.assertLess(output[1]["metric/ndcg"], output[2]["metric/ndcg"])
     self.assertLess(output[0]["metric/ndcg@10"], output[1]["metric/ndcg@10"])
     self.assertLess(output[1]["metric/ndcg@10"], output[2]["metric/ndcg@10"])
 
     # Evaluate metric values after training.
-    np.testing.assert_allclose(output[2]["metric/ndcg"], 0.829664, atol=0.02)
-    np.testing.assert_allclose(output[2]["metric/ndcg@10"], 0.652389, atol=0.02)
+    np.testing.assert_allclose(output[2]["metric/ndcg"], 0.829134, atol=0.03)
+    np.testing.assert_allclose(output[2]["metric/ndcg@10"], 0.650672, atol=0.03)
 
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `rax-0.2.0/examples/t5x/models.py` & `rax-0.3.0/examples/t5x/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,28 +12,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Ranking-specific encoder-decoder model and feature converter."""
 
 import functools
 import types
-from typing import Mapping, Optional, Sequence, Tuple, Union
+from typing import Any, Mapping, Optional, Sequence, Tuple, Union
 
 import flax
 import gin
 import jax
 import jax.numpy as jnp
 import rax
 import seqio
 from t5x import metrics as metrics_lib
 from t5x import models
 from t5x import optimizers
 import tensorflow as tf
 
 FeatureSpec = seqio.FeatureConverter.FeatureSpec
+PyTree = Any
 
 # Set up default loss and metric functions. For this we will use the Rax softmax
 # loss and several of the Rax metric functions. You can update these in the gin
 # config file to different values.
 DEFAULT_LOSS_FN = rax.softmax_loss
 
 DEFAULT_METRIC_FNS = types.MappingProxyType({
@@ -51,30 +52,32 @@
   TASK_FEATURES = {
       "inputs": FeatureSpec(dtype=tf.int32, rank=2, sequence_dim=1),
       "targets": FeatureSpec(dtype=tf.int32, rank=2, sequence_dim=1),
       "label": FeatureSpec(dtype=tf.float32),
       "mask": FeatureSpec(dtype=tf.bool),
   }
   MODEL_FEATURES = {
-      "encoder_input_tokens":
-          FeatureSpec(dtype=tf.int32, rank=2, sequence_dim=1),
-      "decoder_input_tokens":
-          FeatureSpec(dtype=tf.int32, rank=2, sequence_dim=1),
-      "decoder_target_tokens":
-          FeatureSpec(dtype=tf.int32, rank=2, sequence_dim=1),
-      "label":
-          FeatureSpec(dtype=tf.float32),
-      "mask":
-          FeatureSpec(dtype=tf.bool),
+      "encoder_input_tokens": FeatureSpec(
+          dtype=tf.int32, rank=2, sequence_dim=1
+      ),
+      "decoder_input_tokens": FeatureSpec(
+          dtype=tf.int32, rank=2, sequence_dim=1
+      ),
+      "decoder_target_tokens": FeatureSpec(
+          dtype=tf.int32, rank=2, sequence_dim=1
+      ),
+      "label": FeatureSpec(dtype=tf.float32),
+      "mask": FeatureSpec(dtype=tf.bool),
   }
   PACKING_FEATURE_DTYPES = None
 
   def _convert_features(
-      self, ds: tf.data.Dataset,
-      task_feature_lengths: Mapping[str, Union[int, Sequence[int]]]
+      self,
+      ds: tf.data.Dataset,
+      task_feature_lengths: Mapping[str, Union[int, Sequence[int]]],
   ) -> tf.data.Dataset:
     """Convert the dataset to be fed to the encoder-decoder model.
 
     This method adds a mask to indicate valid items in a list and additionally
     pads and truncates the task features to (list_size, sequence_length), so
     that it can be fed to the ranking encoder-decoder model.
 
@@ -87,71 +90,78 @@
       The converted dataset.
     """
 
     # Convert ragged tensors to dense tensors. The seqio `trim_and_pad_dataset`
     # cannot handle ragged tensors, so we convert them to dense here.
     def to_dense(features):
       return {
-          key:
-          value.to_tensor(0) if isinstance(value, tf.RaggedTensor) else value
+          key: (
+              value.to_tensor(0)
+              if isinstance(value, tf.RaggedTensor)
+              else value
+          )
           for key, value in features.items()
       }
 
     ds = ds.map(to_dense, num_parallel_calls=tf.data.AUTOTUNE)
 
     # Trim and pad the list_size dimension.
     ds = seqio.utils.trim_and_pad_dataset(
-        ds, {
+        ds,
+        {
             "label": task_feature_lengths["label"][0],
             "mask": task_feature_lengths["label"][0],
             "targets": task_feature_lengths["targets"][0],
-            "inputs": task_feature_lengths["inputs"][0]
-        })
+            "inputs": task_feature_lengths["inputs"][0],
+        },
+    )
 
     # Function to swap leading axes for "inputs" and "targets" so we can trim
     # and pad the sequence length. The seqio `trim_and_pad_dataset` can only pad
     # and truncate the leading dimension so this is needed to trim the sequence
     # length, which is the second dimension.
     def transpose_inputs_and_targets(task_features):
       return {
-          **task_features, "inputs":
-              tf.transpose(task_features["inputs"], [1, 0]),
-          "targets":
-              tf.transpose(task_features["targets"], [1, 0])
+          **task_features,
+          "inputs": tf.transpose(task_features["inputs"], [1, 0]),
+          "targets": tf.transpose(task_features["targets"], [1, 0]),
       }
 
     # Trim and pad the sequence length dimension. This first swaps the sequence
     # length to the first dimension, then trims and pads it, then swaps the
     # sequence length back to the second dimension.
     ds = ds.map(transpose_inputs_and_targets)
     ds = seqio.utils.trim_and_pad_dataset(
-        ds, {
+        ds,
+        {
             "targets": task_feature_lengths["targets"][1],
-            "inputs": task_feature_lengths["inputs"][1]
-        })
+            "inputs": task_feature_lengths["inputs"][1],
+        },
+    )
     ds = ds.map(transpose_inputs_and_targets)
 
     # Finally, this adds the actual model features to the dataset and returns
     # the result. Note that the model is only predicting a single target, so
     # there is no need to construct autoregressive decoder inputs and we can
     # just use the default decoder input (0).
     def add_features(task_features):
       return {
           "encoder_input_tokens": task_features["inputs"],
           "decoder_input_tokens": tf.zeros_like(task_features["targets"]),
           "decoder_target_tokens": task_features["targets"],
           "label": task_features["label"],
-          "mask": task_features["mask"]
+          "mask": task_features["mask"],
       }
 
     ds = ds.map(add_features)
     return ds
 
   def get_model_feature_lengths(
-      self, task_feature_lengths: Mapping[str, int]) -> Mapping[str, int]:
+      self, task_feature_lengths: Mapping[str, int]
+  ) -> Mapping[str, int]:
     """Define the length relationship between input and output features.
 
     Args:
       task_feature_lengths: A mapping indicating the task feature lengths.
 
     Returns:
       A mapping indicating the model feature lengths.
@@ -173,34 +183,40 @@
   with leading dimensions (batch_size, list_size, ...). This allows it to handle
   listwise ranking data, which makes it possible to compute ranking losses and
   metrics.
   """
 
   FEATURE_CONVERTER_CLS = RankingEncDecFeatureConverter
 
-  def __init__(self,
-               module: flax.linen.Module,
-               input_vocabulary: seqio.Vocabulary,
-               output_vocabulary: seqio.Vocabulary,
-               optimizer_def: optimizers.OptimizerDefType,
-               rax_loss_fn: rax.types.LossFn = DEFAULT_LOSS_FN,
-               rax_metric_fns: Mapping[str,
-                                       rax.types.MetricFn] = DEFAULT_METRIC_FNS,
-               loss_normalizing_factor: Optional[float] = None):
+  def __init__(
+      self,
+      module: flax.linen.Module,
+      input_vocabulary: seqio.Vocabulary,
+      output_vocabulary: seqio.Vocabulary,
+      optimizer_def: optimizers.OptimizerDefType,
+      rax_loss_fn: rax.types.LossFn = DEFAULT_LOSS_FN,
+      rax_metric_fns: Mapping[str, rax.types.MetricFn] = DEFAULT_METRIC_FNS,
+      loss_normalizing_factor: Optional[float] = None,
+  ):
     super().__init__(
         module,
         input_vocabulary,
         output_vocabulary,
         optimizer_def,
-        loss_normalizing_factor=loss_normalizing_factor)
+        loss_normalizing_factor=loss_normalizing_factor,
+    )
     self._rax_loss_fn = rax_loss_fn
     self._rax_metric_fns = rax_metric_fns
 
-  def get_initial_variables(self, rng: jax.random.PRNGKeyArray, input_shapes,
-                            input_types):
+  def get_initial_variables(
+      self,
+      rng: jax.random.PRNGKeyArray,
+      input_shapes,  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
+      input_types,
+  ):
     """Initializes model variables for the given input shapes and types.
 
     This method supports computing variables for a batch of data of shape
     (batch_size, list_size, ...) by first flattening the leading batch
     dimensions.
 
     Args:
@@ -212,23 +228,26 @@
       The initialized model variables.
     """
     # Flatten (batch_size, list_size, ...) into (batch_size * list_size, ...)
     # for model inputs.
     batch_size, list_size, *_ = input_shapes["encoder_input_tokens"]
     input_shapes = {
         **input_shapes,
-        "encoder_input_tokens": (batch_size * list_size,) +
-                                input_shapes["encoder_input_tokens"][2:],
-        "decoder_input_tokens": (batch_size * list_size,) +
-                                input_shapes["decoder_input_tokens"][2:],
+        "encoder_input_tokens": (batch_size * list_size,) + input_shapes[
+            "encoder_input_tokens"
+        ][2:],
+        "decoder_input_tokens": (batch_size * list_size,) + input_shapes[
+            "decoder_input_tokens"
+        ][2:],
     }
     return super().get_initial_variables(rng, input_shapes, input_types)
 
-  def _compute_logits(self, params: models.PyTreeDef,
-                      batch: Mapping[str, jnp.ndarray], *args, **kwargs):
+  def _compute_logits(
+      self, params: PyTree, batch: Mapping[str, jnp.ndarray], *args, **kwargs
+  ):
     """Computes logits on a batch of data.
 
     This method supports computing logits for a batch of data of shape
     (batch_size, list_size, ...) by first flattening the leading batch
     dimensions and then feeding it to the model.
 
     Args:
@@ -240,44 +259,49 @@
     Returns:
       The logits computed on the given batch of data.
     """
     # Flatten (batch_size, list_size, ...) into (batch_size * list_size, ...)
     # for model inputs.
     batch_size, list_size, *_ = batch["encoder_input_tokens"].shape
     flattened_batch = {
-        **batch, "encoder_input_tokens":
-            jnp.reshape(batch["encoder_input_tokens"],
-                        (batch_size * list_size,) +
-                        batch["encoder_input_tokens"].shape[2:]),
-        "decoder_input_tokens":
-            jnp.reshape(batch["decoder_input_tokens"],
-                        (batch_size * list_size,) +
-                        batch["decoder_input_tokens"].shape[2:]),
-        "decoder_target_tokens":
-            jnp.reshape(batch["decoder_target_tokens"],
-                        (batch_size * list_size,) +
-                        batch["decoder_target_tokens"].shape[2:])
+        **batch,
+        "encoder_input_tokens": jnp.reshape(
+            batch["encoder_input_tokens"],
+            (batch_size * list_size,) + batch["encoder_input_tokens"].shape[2:],
+        ),
+        "decoder_input_tokens": jnp.reshape(
+            batch["decoder_input_tokens"],
+            (batch_size * list_size,) + batch["decoder_input_tokens"].shape[2:],
+        ),
+        "decoder_target_tokens": jnp.reshape(
+            batch["decoder_target_tokens"],
+            (batch_size * list_size,)
+            + batch["decoder_target_tokens"].shape[2:],
+        ),
     }
 
     # Compute logits on flattened inputs.
     output = super()._compute_logits(params, flattened_batch, *args, **kwargs)
 
     # Reshape output logits back to (batch_size, list_size, ...)
-    output = jnp.reshape(output, (batch_size, list_size) + output.shape[1:])
+    output = jnp.reshape(output, (batch_size, list_size) + output.shape[1:])  # pytype: disable=attribute-error  # jax-ndarray
 
     # Compute per-item scores. We do three vmaps here for each of the dimensions
     # (batch_size, list_size, sequence_length, ...)
     output = jax.vmap(jax.vmap(jax.vmap(jnp.take)))(
-        output, batch["decoder_target_tokens"])
+        output, batch["decoder_target_tokens"]
+    )
     output = jnp.squeeze(output, -1)
     return output
 
   def loss_fn(
-      self, params: models.PyTreeDef, batch: Mapping[str, jnp.ndarray],
-      dropout_rng: Optional[jnp.ndarray]
+      self,
+      params: PyTree,
+      batch: Mapping[str, jnp.ndarray],
+      dropout_rng: Optional[jnp.ndarray],
   ) -> Tuple[jnp.ndarray, metrics_lib.MetricsMap]:
     """Ranking loss function.
 
     Args:
       params: The parameters of the model.
       batch: The batch of data to compute the loss on.
       dropout_rng: An optional RNG key for dropout.
@@ -296,17 +320,21 @@
       loss = loss / self._loss_normalizing_factor
 
     # Compute ranking metrics.
     metrics = self._compute_metrics(loss, scores, labels, mask)
 
     return loss, metrics
 
-  def _compute_metrics(self, loss: jnp.ndarray, scores: jnp.ndarray,
-                       labels: jnp.ndarray,
-                       mask: Optional[jnp.ndarray]) -> metrics_lib.MetricsMap:
+  def _compute_metrics(
+      self,
+      loss: jnp.ndarray,
+      scores: jnp.ndarray,
+      labels: jnp.ndarray,
+      mask: Optional[jnp.ndarray],
+  ) -> metrics_lib.MetricsMap:
     """Computes ranking metrics.
 
     Args:
       loss: The loss for this batch.
       scores: The scores computed on this batch.
       labels: The relevance labels.
       mask: A mask indicating which items are valid.
@@ -321,13 +349,16 @@
         "loss": metrics_lib.AveragePerStep(total=loss),
         "debug/labels_mean": metrics_lib.AveragePerStep(total=labels_mean),
         "debug/scores_mean": metrics_lib.AveragePerStep(total=scores_mean),
         "debug/valid_items": metrics_lib.AveragePerStep(total=valid_items),
         "timing/steps_per_second": metrics_lib.StepsPerTime.from_model_output(),
         "timing/seconds": metrics_lib.Time(),
     }
-    metrics.update({
-        f"metrics/{key}":
-        metrics_lib.AveragePerStep(total=metric(scores, labels, where=mask))
-        for key, metric in self._rax_metric_fns.items()
-    })
+    metrics.update(
+        {
+            f"metrics/{key}": metrics_lib.AveragePerStep(
+                total=metric(scores, labels, where=mask)
+            )
+            for key, metric in self._rax_metric_fns.items()
+        }
+    )
     return metrics
```

### Comparing `rax-0.2.0/examples/t5x/models_test.py` & `rax-0.3.0/examples/t5x/models_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,79 +24,87 @@
 from examples.t5x import models
 import tensorflow as tf
 
 
 class RankingEncDecFeatureConverterTest(absltest.TestCase):
 
   def test_end_to_end(self):
-
     # Create sample dataset.
     ds = {
-        "inputs":
-            tf.ragged.constant([[5, 1024, 250, 1, 24, 205, 555],
-                                [5, 304, 200, 200], [1, 204, 333, 1024, 5]],
-                               dtype=tf.int32),
-        "targets":
-            tf.ragged.constant([[10], [10], [10]], dtype=tf.int32),
-        "label":
-            tf.constant([0., 1., 0.], dtype=tf.float32),
-        "mask":
-            tf.constant([True, True, True], dtype=tf.bool)
+        "inputs": tf.ragged.constant(
+            [
+                [5, 1024, 250, 1, 24, 205, 555],
+                [5, 304, 200, 200],
+                [1, 204, 333, 1024, 5],
+            ],
+            dtype=tf.int32,
+        ),
+        "targets": tf.ragged.constant([[10], [10], [10]], dtype=tf.int32),
+        "label": tf.constant([0.0, 1.0, 0.0], dtype=tf.float32),
+        "mask": tf.constant([True, True, True], dtype=tf.bool),
     }
     ds = tf.data.Dataset.from_tensors(ds)
 
     # Create feature converter.
     converter = models.RankingEncDecFeatureConverter(
-        pack=False, apply_length_check=False)
+        pack=False, apply_length_check=False
+    )
 
     # Convert the sample dataset using the feature converter.
     task_feature_lengths = {
         "inputs": (4, 5),
         "targets": (4, 1),
         "label": (4,),
-        "mask": (4,)
+        "mask": (4,),
     }
     ds_converted = converter(ds, task_feature_lengths)
 
     # Get an output sample and validate that it is correct.
     sample = next(iter(ds_converted))
     expected = {
-        "encoder_input_tokens":
-            tf.constant([[5, 1024, 250, 1, 24], [5, 304, 200, 200, 0],
-                         [1, 204, 333, 1024, 5], [0, 0, 0, 0, 0]],
-                        dtype=tf.int32),
-        "decoder_input_tokens":
-            tf.constant([[0], [0], [0], [0]], dtype=tf.int32),
-        "decoder_target_tokens":
-            tf.constant([[10], [10], [10], [0]], dtype=tf.int32),
-        "mask":
-            tf.constant([True, True, True, False], dtype=tf.bool),
-        "label":
-            tf.constant([0., 1., 0., 0.], dtype=tf.float32),
+        "encoder_input_tokens": tf.constant(
+            [
+                [5, 1024, 250, 1, 24],
+                [5, 304, 200, 200, 0],
+                [1, 204, 333, 1024, 5],
+                [0, 0, 0, 0, 0],
+            ],
+            dtype=tf.int32,
+        ),
+        "decoder_input_tokens": tf.constant(
+            [[0], [0], [0], [0]], dtype=tf.int32
+        ),
+        "decoder_target_tokens": tf.constant(
+            [[10], [10], [10], [0]], dtype=tf.int32
+        ),
+        "mask": tf.constant([True, True, True, False], dtype=tf.bool),
+        "label": tf.constant([0.0, 1.0, 0.0, 0.0], dtype=tf.float32),
     }
     self.assertCountEqual(sample, expected)
     for key in expected:
       np.testing.assert_equal(sample[key].numpy(), expected[key].numpy())
 
     # Validate that `get_model_feature_lengths` is correct as well.
     model_feature_lengths = converter.get_model_feature_lengths(
-        task_feature_lengths)
+        task_feature_lengths
+    )
     for key, expected_shape in model_feature_lengths.items():
       self.assertEqual(sample[key].shape, expected_shape)
 
 
 class RankingEncDecModelTest(absltest.TestCase):
 
   def test_get_initial_variables(self):
     # Create a RankingEncDecModel with mocked implementations.
     mocked_module = mock.Mock(spec=models.flax.linen.Module)
     mocked_vocab = mock.Mock(spec=models.seqio.Vocabulary)
     mocked_optimizer = mock.Mock(spec=models.optimizers.OptimizerDefType)
-    model = models.RankingEncDecModel(mocked_module, mocked_vocab, mocked_vocab,
-                                      mocked_optimizer)
+    model = models.RankingEncDecModel(
+        mocked_module, mocked_vocab, mocked_vocab, mocked_optimizer
+    )
 
     # Call method to initialize variables.
     rng = jax.random.PRNGKey(0)
     input_shapes = {
         "encoder_input_tokens": (16, 4, 5),
         "decoder_input_tokens": (16, 4, 1),
         "decoder_target_tokens": (16, 4, 1),
@@ -110,15 +118,15 @@
         ),
     }
     input_types = {
         "encoder_input_tokens": jax.numpy.int32,
         "decoder_input_tokens": jax.numpy.int32,
         "decoder_target_tokens": jax.numpy.int32,
         "mask": jax.numpy.bool_,
-        "label": jax.numpy.float32
+        "label": jax.numpy.float32,
     }
     model.get_initial_variables(rng, input_shapes, input_types)
 
     # Validate that the Flax module.init function is called with appropriate
     # initialization args where the leading (batch_size, list_size, ...)
     # dimensions are flattened to (batch_size * list_size, ...).
     mocked_module.init.assert_called()
@@ -129,37 +137,48 @@
     self.assertEqual(args[3].shape, (16 * 4, 1))  # decoder_target_tokens
 
   def test_loss_fn(self):
     # Create a RankingEncDecModel with mocked implementations.
     mocked_module = mock.Mock(spec=models.flax.linen.Module)
     mocked_vocab = mock.Mock(spec=models.seqio.Vocabulary)
     mocked_optimizer = mock.Mock(spec=models.optimizers.OptimizerDefType)
-    model = models.RankingEncDecModel(mocked_module, mocked_vocab, mocked_vocab,
-                                      mocked_optimizer)
+    model = models.RankingEncDecModel(
+        mocked_module, mocked_vocab, mocked_vocab, mocked_optimizer
+    )
 
     batch_key, return_key = jax.random.split(jax.random.PRNGKey(0))
     params = {}
     batch = {
         "encoder_input_tokens": jnp.ones((16, 4, 5), dtype=jnp.int32),
         "decoder_input_tokens": jnp.ones((16, 4, 1), dtype=jnp.int32),
         "decoder_target_tokens": jnp.ones((16, 4, 1), dtype=jnp.int32),
-        "mask": jnp.ones((
-            16,
-            4,
-        ), dtype=jnp.bool_),
-        "label": jnp.float32(jax.random.bernoulli(batch_key, 0.2, (
-            16,
-            4,
-        ))),
+        "mask": jnp.ones(
+            (
+                16,
+                4,
+            ),
+            dtype=jnp.bool_,
+        ),
+        "label": jnp.float32(
+            jax.random.bernoulli(
+                batch_key,
+                0.2,
+                (
+                    16,
+                    4,
+                ),
+            )
+        ),
     }
 
     # Set a random return value of the correct shape for the module apply
     # function.
     mocked_module.apply.return_value = jax.random.uniform(
-        return_key, (16 * 4, 1, 20))
+        return_key, (16 * 4, 1, 20)
+    )
 
     # Call the loss_fn on the model.
     loss, metrics = model.loss_fn(params, batch, None)
 
     # Check that the Flax module.apply function is called with appropriate call
     # args where the leading (batch_size, list_size, ...) dimensions are
     # flattened to (batch_size * list_size, ...).
```

### Comparing `rax-0.2.0/examples/t5x/tasks.py` & `rax-0.3.0/examples/t5x/tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,17 +17,19 @@
 from typing import Mapping
 
 import seqio
 import t5
 import tensorflow as tf
 
 
-def _msmarco_preprocessor(dataset: tf.data.Dataset,
-                          output_features: Mapping[str, t5.data.Feature],
-                          shuffle_lists: bool = True) -> tf.data.Dataset:
+def _msmarco_preprocessor(
+    dataset: tf.data.Dataset,
+    output_features: Mapping[str, t5.data.Feature],
+    shuffle_lists: bool = True,
+) -> tf.data.Dataset:
   """Preprocessor for MS-Marco listwise ranking task.
 
   Args:
     dataset: The ms_marco/v2.1 dataset.
     output_features: A mapping for each of the output features.
     shuffle_lists: If True, lists are shuffled which enforces uniformly random
       selection of documents when lists are truncated to a fixed list size.
@@ -36,16 +38,17 @@
     The processed dataset.
   """
 
   def extract_inputs(features):
     # Extract features from dataset and convert to model inputs.
     query = features["query"]
     passages = features["passages"]["passage_text"]
-    inputs = tf.strings.join(["Query:", query, "Document:", passages],
-                             separator=" ")
+    inputs = tf.strings.join(
+        ["Query:", query, "Document:", passages], separator=" "
+    )
     label = tf.cast(features["passages"]["is_selected"], dtype=tf.float32)
 
     # The target is an unused token to obtain a ranking score.
     targets = tf.fill(tf.shape(label), "<extra_id_10>")
 
     # Shuffle lists, this enforces uniformly random selection of documents when
     # lists are later truncated to a fixed list size.
@@ -54,60 +57,58 @@
       label = tf.gather(label, shuffle_idx)
       inputs = tf.gather(inputs, shuffle_idx)
 
     return {
         "inputs": inputs,
         "targets": targets,
         "label": label,
-        "mask": tf.ones_like(label, dtype=tf.bool)
+        "mask": tf.ones_like(label, dtype=tf.bool),
     }
 
   # Extract necessary inputs from MS-Marco dataset.
   dataset = dataset.map(extract_inputs, num_parallel_calls=tf.data.AUTOTUNE)
 
   # Tokenize only the text features, leave the others unchanged.
   tokenize_features = {
-      "inputs": output_features["inputs"], "targets": output_features["targets"]
+      "inputs": output_features["inputs"],
+      "targets": output_features["targets"],
   }
   dataset = seqio.preprocessors.tokenize(dataset, tokenize_features)
   return dataset
 
 
 _OUTPUT_FEATURES = {
-    "inputs":
-        t5.data.Feature(
-            vocabulary=t5.data.get_default_vocabulary(),
-            add_eos=False,
-            required=False,
-            rank=2),
-    "targets":
-        t5.data.Feature(
-            vocabulary=t5.data.get_default_vocabulary(),
-            add_eos=False,
-            rank=2),
-    "label":
-        t5.data.Feature(
-            vocabulary=seqio.PassThroughVocabulary(size=0),
-            add_eos=False,
-            required=False,
-            dtype=tf.float32,
-            rank=1),
-    "mask":
-        t5.data.Feature(
-            vocabulary=seqio.PassThroughVocabulary(size=0),
-            add_eos=False,
-            required=False,
-            dtype=tf.bool,
-            rank=1),
+    "inputs": t5.data.Feature(
+        vocabulary=t5.data.get_default_vocabulary(),
+        add_eos=False,
+        required=False,
+        rank=2,
+    ),
+    "targets": t5.data.Feature(
+        vocabulary=t5.data.get_default_vocabulary(), add_eos=False, rank=2
+    ),
+    "label": t5.data.Feature(
+        vocabulary=seqio.PassThroughVocabulary(size=0),
+        add_eos=False,
+        required=False,
+        dtype=tf.float32,
+        rank=1,
+    ),
+    "mask": t5.data.Feature(
+        vocabulary=seqio.PassThroughVocabulary(size=0),
+        add_eos=False,
+        required=False,
+        dtype=tf.bool,
+        rank=1,
+    ),
 }
 
 
 t5.data.TaskRegistry.add(
     "msmarco_qna21_ranking",
     seqio.Task,
     source=seqio.TfdsDataSource(
-        tfds_name="huggingface:ms_marco/v2.1", splits=["train", "validation"]),
-    preprocessors=[
-        _msmarco_preprocessor
-    ],
-    output_features=_OUTPUT_FEATURES)
-
+        tfds_name="huggingface:ms_marco/v2.1", splits=["train", "validation"]
+    ),
+    preprocessors=[_msmarco_preprocessor],
+    output_features=_OUTPUT_FEATURES,
+)
```

### Comparing `rax-0.2.0/examples/t5x/tasks_test.py` & `rax-0.3.0/examples/t5x/tasks_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,67 +25,76 @@
 class TasksTest(tf.test.TestCase):
 
   def test_msmarco_preprocessor(self):
     # Input sample data.
     ds = {
         "query": tf.constant(b"who founded google?"),
         "passages": {
-            "passage_text":
-                tf.constant([
-                    b"larry page and sergey brin",
-                    b"google is an American multinational technology company",
-                    b"google was founded in 1998",
-                ]),
-            "is_selected":
-                tf.constant([1, 0, 0])
-        }
+            "passage_text": tf.constant([
+                b"larry page and sergey brin",
+                b"google is an American multinational technology company",
+                b"google was founded in 1998",
+            ]),
+            "is_selected": tf.constant([1, 0, 0]),
+        },
     }
     ds = tf.data.Dataset.from_tensors(ds)
 
     # Perform preprocessing with mocked features.
     tf.random.set_seed(42)
     inputs_mock = mock.Mock()
     inputs_mock.vocabulary.encode_tf.return_value = tf.ragged.constant(
-        [[5, 1024, 250, 1, 24, 205, 555], [5, 304, 200, 200],
-         [1, 204, 333, 1024, 5]],
-        dtype=tf.int32)
+        [
+            [5, 1024, 250, 1, 24, 205, 555],
+            [5, 304, 200, 200],
+            [1, 204, 333, 1024, 5],
+        ],
+        dtype=tf.int32,
+    )
     targets_mock = mock.Mock()
     targets_mock.vocabulary.encode_tf.return_value = tf.ragged.constant(
-        [[10], [10], [10]], dtype=tf.int32)
+        [[10], [10], [10]], dtype=tf.int32
+    )
     label_mock = mock.Mock()
     mask_mock = mock.Mock()
     ds = tasks._msmarco_preprocessor(
-        ds, {
+        ds,
+        {
             "inputs": inputs_mock,
             "targets": targets_mock,
             "label": label_mock,
-            "mask": mask_mock
-        })
+            "mask": mask_mock,
+        },
+    )
 
     # Get a single batch of data and validate its contents.
     batch = next(iter(ds))
     expected = {
-        "inputs_pretokenized":
-            tf.constant([
-                b"Query: who founded google? Document: google was founded in 1998",
-                b"Query: who founded google? Document: larry page and sergey brin",
-                b"Query: who founded google? Document: google is an American multinational technology company"
-            ]),
-        "inputs":
-            tf.ragged.constant([[5, 1024, 250, 1, 24, 205, 555],
-                                [5, 304, 200, 200], [1, 204, 333, 1024, 5]],
-                               dtype=tf.int32),
-        "targets_pretokenized":
-            tf.constant([b"<extra_id_10>", b"<extra_id_10>", b"<extra_id_10>"]),
-        "targets":
-            tf.ragged.constant([[10], [10], [10]], dtype=tf.int32),
-        "label":
-            tf.constant([0., 1., 0.], dtype=tf.float32),
-        "mask":
-            tf.constant([True, True, True], dtype=tf.bool)
+        "inputs_pretokenized": tf.constant([
+            b"Query: who founded google? Document: google was founded in 1998",
+            b"Query: who founded google? Document: larry page and sergey brin",
+            (
+                b"Query: who founded google? Document: google is an"
+                b" American multinational technology company"
+            ),
+        ]),
+        "inputs": tf.ragged.constant(
+            [
+                [5, 1024, 250, 1, 24, 205, 555],
+                [5, 304, 200, 200],
+                [1, 204, 333, 1024, 5],
+            ],
+            dtype=tf.int32,
+        ),
+        "targets_pretokenized": tf.constant(
+            [b"<extra_id_10>", b"<extra_id_10>", b"<extra_id_10>"]
+        ),
+        "targets": tf.ragged.constant([[10], [10], [10]], dtype=tf.int32),
+        "label": tf.constant([0.0, 1.0, 0.0], dtype=tf.float32),
+        "mask": tf.constant([True, True, True], dtype=tf.bool),
     }
 
     for key in batch:
       self.assertAllEqual(batch[key], expected[key])
 
 
 if __name__ == "__main__":
```

### Comparing `rax-0.2.0/rax/__init__.py` & `rax-0.3.0/rax/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,57 +12,67 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Rax: Learning to Rank using JAX."""
 
 from rax import types
 from rax import utils
+from rax._src.lambdaweights import dcg2_lambdaweight
+from rax._src.lambdaweights import dcg_lambdaweight
+from rax._src.lambdaweights import labeldiff_lambdaweight
 from rax._src.losses import listmle_loss
 from rax._src.losses import pairwise_hinge_loss
 from rax._src.losses import pairwise_logistic_loss
 from rax._src.losses import pairwise_mse_loss
+from rax._src.losses import pairwise_qr_loss
+from rax._src.losses import pairwise_soft_zero_one_loss
 from rax._src.losses import pointwise_mse_loss
 from rax._src.losses import pointwise_sigmoid_loss
 from rax._src.losses import poly1_softmax_loss
 from rax._src.losses import softmax_loss
 from rax._src.losses import unique_softmax_loss
 from rax._src.metrics import ap_metric
 from rax._src.metrics import dcg_metric
 from rax._src.metrics import mrr_metric
 from rax._src.metrics import ndcg_metric
 from rax._src.metrics import precision_metric
 from rax._src.metrics import recall_metric
 from rax._src.t12n import approx_t12n
 from rax._src.t12n import bound_t12n
 from rax._src.t12n import gumbel_t12n
+from rax._src.t12n import segment_t12n
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
-# pyformat: disable
 __all__ = [
+    "dcg2_lambdaweight",
+    "dcg_lambdaweight",
+    "labeldiff_lambdaweight",
     "listmle_loss",
     "pairwise_hinge_loss",
     "pairwise_logistic_loss",
     "pairwise_mse_loss",
+    "pairwise_qr_loss",
+    "pairwise_soft_zero_one_loss",
     "pointwise_mse_loss",
     "pointwise_sigmoid_loss",
     "poly1_softmax_loss",
     "unique_softmax_loss",
     "softmax_loss",
     "ap_metric",
     "dcg_metric",
     "mrr_metric",
     "ndcg_metric",
     "precision_metric",
     "recall_metric",
     "approx_t12n",
     "bound_t12n",
     "gumbel_t12n",
+    "segment_t12n",
 ]
-# pyformat: enable
 
 # copybara: stripped(1)
 
 #  _________________________________________
 # / Please don't use symbols in `_src` they \
 # \ are not part of the Rax public API.     /
 #  -----------------------------------------
```

### Comparing `rax-0.2.0/rax/_src/__init__.py` & `rax-0.3.0/examples/segmentation/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `rax-0.2.0/rax/_src/losses.py` & `rax-0.3.0/rax/_src/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,580 +1,622 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Implementations of common ranking losses in JAX.
+"""Utility functions for Rax."""
 
-A ranking loss is a differentiable function that expresses the cost of a ranking
-induced by item scores compared to a ranking induced from relevance labels. Rax
-provides a number of ranking losses as JAX functions that are implemented
-according to the :class:`~rax.types.LossFn` interface.
-
-Loss functions are designed to operate on the last dimension of its inputs. The
-leading dimensions are considered batch dimensions. To compute per-list losses,
-for example to apply per-list weighting or for distributed computing of losses
-across devices, please use standard JAX transformations such as :func:`jax.vmap`
-or :func:`jax.pmap`.
-
-Standalone usage:
-
->>> scores = jnp.array([2., 1., 3.])
->>> labels = jnp.array([1., 0., 0.])
->>> rax.softmax_loss(scores, labels)
-DeviceArray(1.4076059, dtype=float32)
-
-Usage with a batch of data and a mask to indicate valid items.
-
->>> scores = jnp.array([[2., 1., 0.], [1., 0.5, 1.5]])
->>> labels = jnp.array([[1., 0., 0.], [0., 0., 1.]])
->>> where = jnp.array([[True, True, False], [True, True, True]])
->>> rax.pairwise_hinge_loss(
-...     scores, labels, where=where, reduce_fn=jnp.mean)
-DeviceArray(0.16666667, dtype=float32)
-
-To compute gradients of each loss function, please use standard JAX
-transformations such as :func:`jax.grad` or :func:`jax.value_and_grad`:
-
->>> scores = jnp.asarray([[0., 1., 3.], [1., 2., 0.]])
->>> labels = jnp.asarray([[0., 0., 1.], [1., 0., 0.]])
->>> jax.grad(rax.softmax_loss)(scores, labels, reduce_fn=jnp.mean)
-DeviceArray([[ 0.02100503,  0.0570976 , -0.07810265],
-             [-0.37763578,  0.33262047,  0.04501529]], dtype=float32)
+import functools
+import inspect
 
-"""
-
-import operator
-from typing import Callable, Optional
+from typing import Any, Callable, Optional, Sequence, TypeVar
 
 import jax
 import jax.numpy as jnp
 
-from rax._src import metrics
-from rax._src import utils
+from rax._src import segment_utils
 from rax._src.types import Array
-from rax._src.types import ReduceFn
+
+T = TypeVar("T")
 
 
-def softmax_loss(scores: Array,
-                 labels: Array,
-                 *,
-                 where: Optional[Array] = None,
-                 weights: Optional[Array] = None,
-                 label_fn: Callable[..., Array] = lambda a, where: a,
-                 reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
-  r"""Softmax loss.
-
-  Definition:
-
-  .. math::
-      \ell(s, y) =
-      - \sum_i y_i \log \frac{\exp(s_i)}{\sum_j \exp(s_j)}
+def safe_reduce(
+    a: Array,
+    where: Optional[Array] = None,
+    reduce_fn: Optional[Callable[..., Array]] = None,
+) -> Array:
+  """Reduces the values of given array while preventing NaN in the output.
+
+  For :func:`jax.numpy.mean` reduction, this additionally prevents ``NaN`` in
+  the output if all elements are masked. This can happen with pairwise losses
+  where there are no valid pairs because all labels are the same. In this
+  situation, 0 is returned instead.
+
+  When there is no ``reduce_fn``, this will set elements of ``a`` to 0 according
+  to the ``where`` mask.
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the loss. Items for which
-      this is False will be ignored when computing the loss.
-    weights: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating the weight for each item.
-    label_fn: A label function that maps labels to probabilities. Default keeps
-      labels as-is.
-    reduce_fn: An optional function that reduces the loss values. Can be
-      :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
-      is performed.
+    a: The :class:`jax.Array` to reduce.
+    where: An optional :class:`jax.Array` indicating which elements to include
+      in the reduction.
+    reduce_fn: The function used to reduce. If None, no reduction is performed.
 
   Returns:
-    The softmax loss.
+    The result of reducing the values of ``a`` using given ``reduce_fn``.
   """
-  # Applies mask so that masked elements do not count towards the loss.
-  if where is not None:
-    labels = jnp.where(where, labels, jnp.zeros_like(labels))
-    scores = jnp.where(where, scores, -jnp.ones_like(scores) * jnp.inf)
-
-  # Apply weights to labels.
-  if weights is not None:
-    labels *= weights
-
-  # Scales labels and scores to match the cross entropy loss.
-  labels_probabilities = label_fn(labels, where=where)
-  scores_log_softmax = jax.nn.log_softmax(scores, axis=-1)
-
-  # Computes per-element cross entropy.
-  softmax_cross_entropy = labels_probabilities * scores_log_softmax
-
-  # Reduces softmax cross-entropy loss.
-  loss = -jnp.sum(softmax_cross_entropy, axis=-1, where=where)
-  return utils.safe_reduce(loss, reduce_fn=reduce_fn)
+  # Reduce values if there is a reduce_fn, otherwise keep the values as-is.
+  output = reduce_fn(a, where=where) if reduce_fn is not None else a
 
+  if reduce_fn is jnp.mean:
+    # For mean reduction, we have to check whether the input contains any NaN
+    # values, to ensure that masked mean reduction does not hide them (see
+    # below).
+    is_input_valid = jnp.logical_not(jnp.any(jnp.isnan(a)))
+
+    # The standard jnp.mean implementation returns NaN if `where` is False
+    # everywhere. This can happen in our case, e.g. pairwise losses with no
+    # valid pairs. Instead, we prefer that the loss returns 0 in these cases.
+    # Note that this only hides those NaN values if the input did not contain
+    # any NaN values. Otherwise it just returns the output as-is.
+    output = jnp.where(jnp.isnan(output) & is_input_valid, 0.0, output)
+
+  if reduce_fn is None and where is not None:
+    # When there is no reduce_fn (i.e. we are returning an unreduced
+    # loss/metric), set the values of `a` to 0 for invalid (masked) items.
+    # This makes sure that manual sum reduction on an unreduced loss works as
+    # expected:
+    # `jnp.sum(loss_fn(reduce_fn=None)) == loss_fn(reduce_fn=jnp.sum)`
+    output = jnp.where(where, output, 0.0)
+
+  return output
+
+
+def normalize_probabilities(
+    unscaled_probabilities: Array,
+    *,
+    where: Optional[Array] = None,
+    segments: Optional[Array] = None,
+    axis: int = -1,
+) -> Array:
+  """Normalizes given unscaled probabilities so they sum to one in given axis.
+
+  This will scale the given unscaled probabilities such that its valid
+  (non-masked) elements will sum to one along the given axis. Note that the
+  array should have only non-negative elements.
 
-def poly1_softmax_loss(scores: Array,
-                       labels: Array,
-                       *,
-                       epsilon: float = 1.0,
-                       where: Optional[Array] = None,
-                       weights: Optional[Array] = None,
-                       reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
-  r"""Poly1 softmax loss.
+  For cases where all valid elements along the given axis are zero, this will
+  return a uniform distribution over those valid elements.
 
-  Definition :cite:p:`leng2022polyloss`:
-
-  .. math::
-      \ell(s, y) = softmax(s, y) + \epsilon * (1 - pt)
-
-  where :math:`softmax` is the standard softmax loss as implemented in
-  :func:`~rax.softmax_loss` and :math:`pt` is the target softmax probability
-  defined as:
-
-  .. math::
-      pt = \sum_i \frac{y_i}{\sum_j y_j} \frac{\exp(s_i)}{\sum_j \exp(s_j)}
+  For cases where all elements along the given axis are invalid (masked), this
+  will return a uniform distribution over those invalid elements.
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    epsilon: A float hyperparameter indicating the weight of the leading
-      polynomial coefficient in the poly loss.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the loss. Items for which
-      this is False will be ignored when computing the loss.
-    weights: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating the weight for each item.
-    reduce_fn: An optional function that reduces the loss values. Can be
-      :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
-      is performed.
+    unscaled_probabilities: The probabilities to normalize.
+    where: An optional :class:`jax.Array` indicating which elements to include
+      in the normalization.
+    segments: An optional :class:`jax.Array` to indicate segments of items that
+      should be grouped together. Like ``[0, 0, 1, 0, 2]``. The segments may or
+      may not be sorted.
+    axis: The axis to normalize on.
 
   Returns:
-    The poly1 softmax loss.
+    Given unscaled probabilities normalized so they sum to one for the valid
+    (non-masked) items in the given axis.
   """
-  # Compute softmax cross-entropy loss without batch reduction.
-  ce = softmax_loss(
-      scores, labels, where=where, weights=weights, reduce_fn=None)
-
-  # Applies mask so that masked elements do not count towards the loss.
-  if where is not None:
-    labels = jnp.where(where, labels, jnp.zeros_like(labels))
-    scores = jnp.where(where, scores, -jnp.ones_like(scores) * jnp.inf)
-
-  # Apply weights to labels.
-  if weights is not None:
-    labels *= weights
-
-  # Compute target probabilities.
-  scores_softmax = jax.nn.softmax(scores)
-  labels_normalized = utils.normalize_probabilities(labels, where=where)
-  pt = jnp.sum(labels_normalized * scores_softmax, where=where, axis=-1)
+  # Swap axes so the axis we want to normalize is always last.
+  unscaled_probabilities = jnp.swapaxes(unscaled_probabilities, axis, -1)
+  where = None if where is None else jnp.swapaxes(where, axis, -1)
+  segments = None if segments is None else jnp.swapaxes(segments, axis, -1)
 
-  # For lists where all items are masked, this sets pt to 1 so that the term
-  # (1 - pt) is set to 0 for the loss computation.
-  if where is not None:
-    pt = jnp.where(jnp.all(jnp.logical_not(where), axis=-1), 1., pt)
+  if where is None:
+    where = jnp.ones_like(unscaled_probabilities, dtype=jnp.bool_)
 
-  # Compute and return the poly1 loss.
-  loss = ce + epsilon * (1. - pt)
-  return utils.safe_reduce(loss, reduce_fn=reduce_fn)
-
-
-def unique_softmax_loss(scores: Array,
-                        labels: Array,
-                        *,
-                        where: Optional[Array] = None,
-                        weights: Optional[Array] = None,
-                        gain_fn: Optional[Callable[
-                            [Array], Array]] = metrics.default_gain_fn,
-                        reduce_fn: ReduceFn = jnp.mean) -> Array:
-  r"""Unique softmax loss.
-
-  Definition :cite:p:`zhu2020listwise`:
-
-  .. math::
-      \ell(s, y) =
-      - \sum_i \operatorname{gain}(y_i)
-      \log \frac{\exp(s_i)}{\exp(s_i) + \sum_{j : y_j < y_i} \exp(s_j)}
+  # Sum only the valid items across the given axis and sum mask to correctly
+  # normalize all-zero elements with mask.
+  if segments is None:
+    unscaled_probabilities_sum = jnp.sum(
+        unscaled_probabilities, axis=-1, keepdims=True, where=where
+    )
+    where_sum = jnp.sum(where, axis=-1, keepdims=True)
+    where_sum = jnp.where(
+        where_sum == 0.0,
+        jnp.sum(jnp.ones_like(where), axis=-1, keepdims=True),
+        where_sum,
+    )
+  else:
+    unscaled_probabilities_sum = segment_utils.segment_sum(
+        unscaled_probabilities, segments, where=where
+    )
+    where_sum = segment_utils.segment_sum(where, segments)
+    where_sum = jnp.where(
+        where_sum == 0.0,
+        segment_utils.segment_sum(jnp.ones_like(where), segments),
+        where_sum,
+    )
+
+  # Compute output
+  output = jnp.where(
+      unscaled_probabilities_sum != 0.0,
+      unscaled_probabilities / unscaled_probabilities_sum,
+      jnp.ones_like(where, dtype=unscaled_probabilities.dtype) / where_sum,
+  )
+
+  # Swap the axis back to its original position and return the result.
+  output = jnp.swapaxes(output, axis, -1)
+  return output
+
+
+def logcumsumexp(
+    x: Array,
+    *,
+    axis: int = -1,
+    where: Optional[Array] = None,
+    reverse: bool = False,
+):
+  """Computes the cumulative logsumexp.
 
-  where :math:`\operatorname{gain}(y_i)` is a user-specified gain function
-  applied to label :math:`y_i` to boost items with higher relevance.
+  This is a numerically safe and efficient implementation of a cumulative
+  logsumexp operation.
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the loss. Items for which
-      this is False will be ignored when computing the loss.
-    weights: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating the weight for each item.
-    gain_fn: An optional function that maps relevance labels to gain values. If
-      provided, the per-item losses are multiplied by ``gain_fn(label)`` to
-      boost the importance of relevant items.
-    reduce_fn: An optional function that reduces the loss values. Can be
-      :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
-      is performed.
+    x: The :class:`~jax.Array` to compute the cumulative logsumexp for.
+    axis: The axis over which the cumulative sum should take place.
+    where: An optional :class:`~jax.Array` of the same shape as ``x`` indicating
+      which items are valid for computing the cumulative logsumexp.
+    reverse: Whether to compute the cumulative sum in reverse.
 
   Returns:
-    The unique softmax loss.
+    A :class:`~jax.Array` of the same shape as ``x`` representing the cumulative
+    logsumexp of the values of ``x``.
   """
-  # Construct pairwise matrices for scores and labels. The labels matrix will
-  # indicate, for each item, which other items have a smaller label.
-  labels_lt = jnp.expand_dims(labels, -2) < jnp.expand_dims(labels, -1)
-  scores_repeated = jnp.repeat(
-      jnp.expand_dims(scores, -2), scores.shape[-1], axis=-2)
-
-  # Build an identity mask to select items during softmax computation.
-  identity_mask = jnp.identity(scores.shape[-1], dtype=jnp.bool_)
-
-  # Apply mask to ignore invalid items.
-  if where is not None:
-    labels_lt &= jnp.expand_dims(where, -2)
-    identity_mask &= jnp.expand_dims(where, -2)
+  if where is None:
+    where = jnp.ones_like(x, dtype=jnp.bool_)
 
-  # Compute log-softmax for each of the items' unique softmax distribution. This
-  # effectively computes the log_softmax for each item using only itself and
-  # items with a smaller relevance label in the denominator. The computed
-  # log_softmax distribution is reduced by selecting its diagonal elements.
-  log_softmax = jax.nn.log_softmax(
-      scores_repeated,
-      axis=-1,
-      where=(identity_mask | labels_lt),
-      initial=jnp.min(scores))
-  log_softmax = jnp.diagonal(log_softmax, axis1=-2, axis2=-1)
-
-  # Apply per-item weights.
-  if weights is not None:
-    log_softmax *= weights
-
-  # Apply per-item `gain_fn` boost.
-  if gain_fn is not None:
-    log_softmax *= gain_fn(labels)
-
-  # Compute per-list loss and return a reduced loss.
-  loss = -jnp.sum(log_softmax, axis=-1, where=where)
-  return utils.safe_reduce(loss, reduce_fn=reduce_fn)
-
-
-def listmle_loss(scores: Array,
-                 labels: Array,
-                 *,
-                 key: Optional[Array] = None,
-                 where: Optional[Array] = None,
-                 reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
-  r"""ListMLE Loss.
-
-  .. note::
-
-    This loss performs sorting using the given labels. If the labels contain
-    multiple identical values, you should provide a :func:`~jax.random.PRNGKey`
-    to the ``key`` argument to make sure ties are broken randomly during the
-    sorting operation.
-
-  Definition :cite:p:`xia2008listwise`:
-
-  .. math::
-      \ell(s, y) =
-      - \sum_i \log
-        \frac{\exp(s_i)}{\sum_j I[rank(y_j) \ge rank(y_i)] \exp(s_j)}
+  # Flip the inputs if the cumulative sum needs to be in reverse.
+  if reverse:
+    x = jnp.flip(x, axis=axis)
+    where = jnp.flip(where, axis=axis)
+
+  # Mask out invalid entries so they do not count in the summation.
+  x = jnp.where(where, x, -jnp.inf)
+
+  # Make the axis on which to perform the operation the leading axis which is
+  # necessary for `jax.lax.scan` used below.
+  x = jnp.swapaxes(x, axis, 0)
+  where = jnp.swapaxes(where, axis, 0)
+
+  # Compute cumulative maximum.
+  m = jax.lax.cummax(x, axis=0)
+
+  # Compute `exp(x_i - m_i)` for each i.
+  x_shifted = jnp.exp(x - m)
+  x_shifted = jnp.where(where, x_shifted, 0.0)
+
+  # Compute `exp(m_{i-1} - m_i)` for each i. This is used to perform an
+  # efficient version of the internal cumulative sumation (see below).
+  # Note that `m_{i-1} <= m_i` for all i because m_i is a cumulative maximum, so
+  # this is numerically safe.
+  m_diffs = jnp.exp(jnp.minimum(0.0, jnp.roll(m, 1, axis=0) - m))
+  m_diffs = jnp.where(where, m_diffs, 1.0)
+
+  # We wish to compute the following output values (for each i):
+  #
+  #   out[i] = sum_{j=1}^{i} exp(x_j - m_i)
+  #
+  # This can be implemented in a vectorized way using a pairwise broadcasted
+  # expansion of x and m and computing all pairs `exp(x_j - m_i)` with
+  # appropriating masking. This approach would have an O(n^2) complexity.
+  # The O(n^2) can be avoided by using a recursive definition of out[i]:
+  #
+  #   out[1] = exp(x_1 - m_1)
+  #   out[i] = exp(x_i - m_i) + exp(m_{i-1} - m_i) * out[i-1]
+  #
+  # This recursive formulation allows for an o(n) complexity implementation
+  # using `jax.lax.scan` and is used here.
+  def f(previous, x):
+    out_i = x[0] + previous * x[1]
+    return out_i, out_i
+
+  initial = jnp.zeros(x.shape[1:], dtype=x.dtype)
+  out = jax.lax.scan(f, initial, (x_shifted, m_diffs))[1]
+
+  # Compute the log of the cumulative sum and correct for the cumulative
+  # maximum shift.
+  tiny = jnp.finfo(x.dtype).tiny
+  out = jnp.log(out + tiny) + m
+
+  # Swap axes back and flip output if the cumulative sum needs to be in reverse.
+  out = jnp.swapaxes(out, 0, axis)
+  if reverse:
+    out = jnp.flip(out, axis=axis)
+
+  return out
+
+
+def sort_by(
+    scores: Array,
+    tensors_to_sort: Sequence[Array],
+    axis: int = -1,
+    where: Optional[Array] = None,
+    segments: Optional[Array] = None,
+    key: Optional[Array] = None,
+) -> Sequence[Array]:
+  """Sorts given list of tensors by given scores.
 
-  where :math:`\operatorname{rank}(y_i)` indicates the rank of item :math:`i`
-  after sorting all labels :math:`y`.
+  Each of the entries in the `tensors_to_sort` sequence must be a tensor that
+  matches the shape of the `scores`.
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    key: An optional :func:`~jax.random.PRNGKey` to perform random tie-breaking.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the loss. Items for which
-      this is False will be ignored when computing the loss.
-    reduce_fn: An optional function that reduces the loss values. Can be
-      :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
-      is performed.
+    scores: A ``[..., list_size]``-:class:`~jax.Array`, indicating the score for
+      each item.
+    tensors_to_sort: A sequence of tensors of the same shape as scores. These
+      are the tensors that will be sorted in the order of scores.
+    axis: The axis to sort on, by default this is the last axis.
+    where: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      which items are valid. Invalid entries are pushed to the end.
+    segments: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      which items in the list should be grouped together. Items will be sorted
+      within each segment, but not across segments.
+    key: An optional :func:`jax.random.PRNGKey`. If provided, ties will be
+      broken randomly using this key. If not provided, ties will retain the
+      order of their appearance in the `scores` array.
 
   Returns:
-    The listmle loss.
+    A tuple containing the tensors of ``tensors_to_sort`` sorted in the order of
+    ``scores``.
   """
-  # Sort scores and mask by labels.
-  if where is None:
-    where = jnp.ones_like(scores, dtype=jnp.bool_)
-
-  scores_sorted, where_sorted = utils.sort_by(
-      labels, [scores, where], where=where, key=key)
-
-  # Compute cumulative logsumexp.
-  lse = utils.logcumsumexp(
-      scores_sorted, axis=-1, where=where_sorted, reverse=True)
-
-  # Reduce list MLE loss.
-  loss = -jnp.sum(scores_sorted - lse, axis=-1, where=where_sorted)
-  return utils.safe_reduce(loss, reduce_fn=reduce_fn)
-
+  # Sets up the keys we want to sort on.
+  sort_operands = []
+  if segments is not None:
+    sort_operands.append(segments)
+  if where is not None:
+    sort_operands.append(jnp.logical_not(where))
+  sort_operands.append(-scores)
+  if key is not None:
+    sort_operands.append(jax.random.uniform(key, scores.shape))
+  num_keys = len(sort_operands)
+
+  # Adds the tensors that we want sort.
+  sort_operands.extend(tensors_to_sort)
+
+  # Performs sort and returns the sorted tensors.
+  sorted_values = jax.lax.sort(sort_operands, dimension=axis, num_keys=num_keys)
+  sorted_values = sorted_values[num_keys:]
+
+  # Revert segments to their original positions.
+  if segments is not None:
+    segment_indices = jnp.argsort(jnp.argsort(segments, axis), axis)
+    sorted_values = tuple(
+        jnp.take_along_axis(values, segment_indices, axis=axis)
+        for values in sorted_values
+    )
+
+  return sorted_values
+
+
+def ranks(
+    scores: Array,
+    *,
+    where: Optional[Array] = None,
+    segments: Optional[Array] = None,
+    axis: int = -1,
+    key: Optional[Array] = None,
+) -> Array:
+  """Computes the ranks for given scores.
 
-def compute_pairs(a: Array, op: Callable[[Array, Array], Array]) -> Array:
-  """Computes pairs based on values of `a` and the given pairwise `op`.
+  Note that the ranks returned by this function are not differentiable due to
+  the sort operation having no gradients.
 
   Args:
-    a: The array used to form pairs. The last axis is used to form pairs.
-    op: The binary op to map a pair of values to a single value.
+    scores: A ``[..., list_size]``-:class:`~jax.Array`, indicating the score for
+      each item.
+    where: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      which items are valid.
+    segments: A :class:`~jax.Array` to indicate segments of items that should be
+      grouped together. Like ``[0, 0, 1, 0, 2]``. The segments may or may not be
+      sorted.
+    axis: The axis to sort on, by default this is the last axis.
+    key: An optional :func:`jax.random.PRNGKey`. If provided, ties will be
+      broken randomly using this key. If not provided, ties will retain the
+      order of their appearance in the `scores` array.
 
   Returns:
-    A new array with the same leading dimensions as `a`, but with the last
-    dimension expanded so it includes all pairs `op(a[..., i], a[..., j])`
+    A :class:`~jax.Array` with the same shape as `scores` that indicates the
+    1-based rank of each item.
   """
-  a_i = jnp.expand_dims(a, -1)
-  a_j = jnp.expand_dims(a, -2)
-  result_shape = jnp.broadcast_shapes(a_i.shape, a_j.shape)
-  result = jnp.broadcast_to(op(a_i, a_j), result_shape)
-  out_shape = tuple(result.shape[:-2]) + (result.shape[-2] * result.shape[-1],)
-  return jnp.reshape(result, out_shape)
-
-
-def pairwise_hinge_loss(scores: Array,
-                        labels: Array,
-                        *,
-                        where: Optional[Array] = None,
-                        weights: Optional[Array] = None,
-                        reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
-  r"""Pairwise hinge loss.
-
-  Definition:
-
-  .. math::
-      \ell(s, y) =
-      \sum_i \sum_j I[y_i > y_j] \max(0, 1 - (s_i - s_j))
+  # Construct `arange` tensor and broadcast it to the shape of `scores`.
+  arange_broadcast_dims = list(range(len(scores.shape)))
+  del arange_broadcast_dims[axis]
+  arange = jnp.arange(scores.shape[axis])
+  arange = jnp.expand_dims(arange, axis=arange_broadcast_dims)
+  arange = jnp.broadcast_to(arange, scores.shape)
+
+  # Compute per segment ranks when segments are set.
+  if segments is not None:
+    # TODO(xuanhui): Support any axis as it works only for axis=-1 for now.
+    if axis != -1:
+      raise ValueError(
+          "only axis=-1 is supported when segments are set, but given"
+          f" axis={axis}."
+      )
+    sorted_segments, sorted_indices = sort_by(
+        scores,
+        [segments, arange],
+        where=where,
+        key=key,
+    )
+    sorted_ranks = segment_utils.in_segment_indices(sorted_segments) + 1
+    # Scatter the ranks back to their corresponding entries.
+    return sort_by(-sorted_indices, [sorted_ranks])[0]
+
+  # Perform an argsort on the scores along given axis. This returns the indices
+  # that would sort the scores. Note that we can not use the `jnp.argsort`
+  # method here as it does not support masked arrays or randomized tie-breaking.
+  indices = sort_by(scores, [arange], axis=axis, where=where, key=key)[0]
+
+  # Perform an argsort on the indices to get the 1-based ranks.
+  return jnp.argsort(indices, axis=axis) + 1
+
+
+def approx_ranks(
+    scores: Array,
+    *,
+    where: Optional[Array] = None,
+    segments: Optional[Array] = None,
+    key: Optional[Array] = None,
+    step_fn: Callable[[Array], Array] = jax.nn.sigmoid,
+) -> Array:
+  """Computes approximate ranks.
+
+  This can be used to construct differentiable approximations of metrics. For
+  example:
+
+  >>> import functools
+  >>> approx_ndcg = functools.partial(
+  ...     rax.ndcg_metric, rank_fn=rax.utils.approx_ranks)
+  >>> scores = jnp.asarray([-1., 1., 0.])
+  >>> labels = jnp.asarray([0., 0., 1.])
+  >>> print(approx_ndcg(scores, labels))
+  0.63092977
+  >>> print(jax.grad(approx_ndcg)(scores, labels))
+  [-0.03763788 -0.03763788  0.07527576]
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the loss. Items for which
-      this is False will be ignored when computing the loss.
-    weights: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating the weight for each item.
-    reduce_fn: An optional function that reduces the loss values. Can be
-      :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
-      is performed.
+    scores: A ``[..., list_size]``-:class:`~jax.Array`, indicating the score for
+      each item.
+    where: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      which items are valid.
+    segments: A :class:`~jax.Array` to indicate segments of items that should be
+      grouped together. Like ``[0, 0, 1, 0, 2]``. The segments may or may not be
+      sorted.
+    key: An optional :func:`jax.random.PRNGKey`. Unused by ``approx_ranks``.
+    step_fn: A callable that approximates the step function ``x >= 0``.
 
   Returns:
-    The pairwise hinge loss.
+    A :class:`~jax.Array` of the same shape as ``scores``, indicating
+    the 1-based approximate rank of each item.
   """
-  # Expand scores and labels into pairwise versions.
-  scores = compute_pairs(scores, operator.sub)
-  labels = compute_pairs(labels, operator.gt)
 
-  # Compute hinge function on scores.
-  scores = jax.nn.relu(1. - scores)
+  del key  # unused for approximate ranks.
+
+  score_i = jnp.expand_dims(scores, axis=-1)
+  score_j = jnp.expand_dims(scores, axis=-2)
+  score_pairs = step_fn(score_j - score_i)
 
-  # Apply mask to labels, so only valid items are considered.
+  # Build mask to prevent counting (i == j) pairs.
+  pair_mask = jnp.triu(jnp.tril(jnp.ones_like(score_pairs))) == 0.0
   if where is not None:
-    where = compute_pairs(where, operator.and_)
-    labels &= where
+    where = jnp.expand_dims(where, axis=-1) & jnp.expand_dims(where, axis=-2)
+    pair_mask &= where
+  # Mask out pairs that are not in the same segment.
+  if segments is not None:
+    pair_mask &= segment_utils.same_segment_mask(segments)
+
+  return jnp.sum(score_pairs, axis=-1, where=pair_mask, initial=1.0)
+
+
+def cutoff(
+    a: Array,
+    n: Optional[int] = None,
+    where: Optional[Array] = None,
+    segments: Optional[Array] = None,
+) -> Array:
+  """Computes a binary array to select the largest ``n`` values of ``a``.
 
-  # Apply weights to scores.
-  if weights is not None:
-    weights = compute_pairs(weights, lambda x, y: x)
-    scores *= weights
-
-  return utils.safe_reduce(scores, where=labels, reduce_fn=reduce_fn)
-
-
-def pairwise_logistic_loss(scores: Array,
-                           labels: Array,
-                           *,
-                           where: Optional[Array] = None,
-                           weights: Optional[Array] = None,
-                           reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
-  r"""Pairwise logistic loss.
-
-  Definition :cite:p:`burges2005learning`:
-
-  .. math::
-      \ell(s, y) =
-      \sum_i \sum_j I[y_i > y_j] \log(1 + \exp(-(s_i - s_j)))
+  This function computes a binary :class:`~jax.Array` that selects the ``n``
+  largest values of ``a`` across its last dimension.
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the loss. Items for which
-      this is False will be ignored when computing the loss.
-    weights: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating the weight for each item.
-    reduce_fn: An optional function that reduces the loss values. Can be
-      :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
-      is performed.
+    a: The :class:`~jax.Array` to select the topn from.
+    n: The cutoff value. If None, no cutoff is performed.
+    where: A mask to indicate which values to include in the topn calculation.
+    segments: A :class:`~jax.Array` to indicate segments of items that should be
+      grouped together. Like ``[0, 0, 1, 0, 2]``. The segments may or may not be
+      sorted.
 
   Returns:
-    The pairwise logistic loss.
+    A :class:`~jax.Array` of the same shape as ``a``, where the ``n`` largest
+    values are set to 1, and the smaller values are set to 0.
   """
-  # Expand scores and labels into pairwise versions.
-  scores = compute_pairs(scores, operator.sub)
-  labels = compute_pairs(labels, operator.gt)
+  if n is None:
+    return jnp.ones_like(a)
 
-  # Compute numerically stable version of logistic function on scores.
-  scores = jax.nn.relu(-scores) + jnp.log1p(jnp.exp(-jnp.abs(scores)))
-
-  # Apply mask to labels, so only valid items are considered.
+  results = ranks(a, where=where, segments=segments) <= n
   if where is not None:
-    where = compute_pairs(where, operator.and_)
-    labels &= where
-
-  # Apply weights to scores.
-  if weights is not None:
-    weights = compute_pairs(weights, lambda x, y: x)
-    scores *= weights
+    results &= where
+  return jnp.float32(results)
 
-  return utils.safe_reduce(scores, where=labels, reduce_fn=reduce_fn)
 
+def approx_cutoff(
+    a: Array,
+    n: Optional[int] = None,
+    *,
+    where: Optional[Array] = None,
+    segments: Optional[Array] = None,
+    step_fn: Callable[[Array], Array] = jax.nn.sigmoid,
+) -> Array:
+  """Approximately select the largest ``n`` values of ``a``.
 
-def pointwise_sigmoid_loss(scores: Array,
-                           labels: Array,
-                           *,
-                           where: Optional[Array] = None,
-                           weights: Optional[Array] = None,
-                           reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
-  r"""Sigmoid cross entropy loss.
-
-  Definition:
-
-  .. math::
-      \ell(s, y) =
-      \sum_i y_i * -log(sigmoid(s_i)) + (1 - y_i) * -log(1 - sigmoid(s_i))
-
-  This loss converts graded relevance to binary relevance by considering items
-  with ``label >= 1`` as relevant and items with ``label < 1`` as non-relevant.
+  This function computes a :class:`~jax.Array` that is the probability of an
+  item being in the ``n`` largest values of ``a`` across its last dimension.
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    where: An optional [..., list_size]-Array, indicating which items are valid
-      for computing the loss. Items for which this is False will be ignored when
-      computing the loss.
-    weights: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating the weight for each item.
-    reduce_fn: An optional function that reduces the loss values. Can be
-      :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
-      is performed.
+    a: The :class:`~jax.Array` to select the topn from.
+    n: The cutoff value. If None, no cutoff is performed.
+    where: A mask to indicate which values to include in the topn calculation.
+    segments: A :class:`~jax.Array` to indicate segments of items that should be
+      grouped together. Like ``[0, 0, 1, 0, 2]``. The segments may or may not be
+      sorted.
+    step_fn: A function that computes an approximation of ``x >= 0``.
 
   Returns:
-    The sigmoid cross entropy loss.
+    A :class:`~jax.Array` of the same shape as ``a``.
   """
+  if n is None:
+    return jnp.ones_like(a)
 
-  # Convert to binary relevance labels.
-  labels = jnp.where(labels >= 1, jnp.ones_like(labels), jnp.zeros_like(labels))
-
-  # A numerically stable version of sigmoid cross entropy.
-  loss = (
-      jax.nn.relu(scores) - scores * labels +
-      jnp.log(1. + jnp.exp(-jnp.abs(scores))))
-
-  if weights is not None:
-    loss *= weights
-
-  return utils.safe_reduce(loss, where=where, reduce_fn=reduce_fn)
+  # When `n` is 0, everything is cut off.
+  if n == 0:
+    return jnp.zeros_like(a)
+
+  a_ranks = ranks(a, where=where, segments=segments)
+  if segments is None:
+    # Place the cutoff point between a[n] and a[n+1]. For exact `step_fn`, this
+    # does not make a difference. But for approximate step functions (e.g.
+    # sigmoid), this ensures the cutoff value at `n` can be close to 1, and the
+    # cutoff value at `n+1` can be close to 0.
+    a_cutoff = (
+        jnp.sum(
+            jnp.where((a_ranks == n) | (a_ranks == n + 1), a, 0),
+            axis=-1,
+            keepdims=True,
+        )
+        / 2.0
+    )
+    num_valid = jnp.sum(
+        jnp.ones_like(a, dtype=jnp.int32), where=where, axis=-1, keepdims=True
+    )
+  else:
+    # Place the cutoff point between a[n] and a[n+1]. For exact `step_fn`, this
+    # does not make a difference. But for approximate step functions (e.g.
+    # sigmoid), this ensures the cutoff value at `n` can be close to 1, and the
+    # cutoff value at `n+1` can be close to 0.
+    a_cutoff = (
+        segment_utils.segment_sum(
+            jnp.where((a_ranks == n) | (a_ranks == n + 1), a, 0), segments
+        )
+        / 2.0
+    )
+    num_valid = segment_utils.segment_sum(
+        jnp.ones_like(a, dtype=jnp.int32), segments, where=where
+    )
+
+  # Compute the cutoffs but prevent gradients in the cutoff-point calculation so
+  # only gradients are computed on `a`.
+  a_cutoff = jax.lax.stop_gradient(a_cutoff)
+  cutoffs = step_fn(a - a_cutoff)
+
+  # A mask can indicate a different list size for each list in `a`, so this
+  # checks if a valid cutoff exists for each list.
+  cutoffs = jnp.where(num_valid > n, cutoffs, jnp.ones_like(cutoffs))
 
+  if where is not None:
+    # Mask out invalid entries.
+    cutoffs = jnp.where(where, cutoffs, jnp.zeros_like(cutoffs))
 
-def pointwise_mse_loss(scores: Array,
-                       labels: Array,
-                       *,
-                       where: Optional[Array] = None,
-                       weights: Optional[Array] = None,
-                       reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
-  r"""Mean squared error loss.
+  return cutoffs
 
-  Definition:
 
-  .. math::
-      \ell(s, y) = \sum_i (y_i - s_i)^2
+def compute_pairs(a: Array, op: Callable[[Array, Array], Array]) -> Array:
+  """Computes pairs based on values of `a` and the given pairwise `op`.
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the loss. Items for which
-      this is False will be ignored when computing the loss.
-    weights: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating the weight for each item.
-    reduce_fn: An optional function that reduces the loss values. Can be
-      :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
-      is performed.
+    a: The array used to form pairs. The last axis is used to form pairs.
+    op: The binary op to map a pair of values to a single value.
 
   Returns:
-    The mean squared error loss.
+    A :class:`jax.Array` with the same leading dimensions as `a`, but with the
+    last dimension expanded so it includes all pairs `op(a[..., i], a[..., j])`
   """
-  loss = jnp.square(scores - labels)
-
-  if weights is not None:
-    loss *= weights
-
-  return utils.safe_reduce(loss, where=where, reduce_fn=reduce_fn)
-
-
-def pairwise_mse_loss(scores: Array,
-                      labels: Array,
-                      *,
-                      where: Optional[Array] = None,
-                      weights: Optional[Array] = None,
-                      reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
-  r"""Pairwise mean squared error loss.
+  a_i = jnp.expand_dims(a, -1)
+  a_j = jnp.expand_dims(a, -2)
+  result_shape = jnp.broadcast_shapes(a_i.shape, a_j.shape)
+  result = jnp.broadcast_to(op(a_i, a_j), result_shape)
+  out_shape = tuple(result.shape[:-2]) + (result.shape[-2] * result.shape[-1],)
+  return jnp.reshape(result, out_shape)
 
-  Definition:
 
-  .. math::
-      \ell(s, y) =
-      \sum_i \sum_j ((y_i - y_j) - (s_i - s_j))^2
+def update_signature(
+    wrapped: Callable[..., Any],
+    *new_kwarg_names: str,
+) -> Callable[[T], T]:
+  """Function decorator to update a function signature by appending new kwargs.
+
+  This is useful for functions where standard :func:`functools.wraps` is not
+  sufficient because the wrapper has new kwargs that are not a part of the
+  signature of the wrapped function and :func:`inspect.signature` would fail to
+  expose those kwargs.
+
+  Example usage:
+
+  >>> def f(a, b):
+  ...   return a + b
+  >>> @utils.update_signature(f, "c")
+  ... def g(*args, c=42):
+  ...   return f(*args) + c
+  >>> import inspect
+  >>> inspect.signature(g)
+  <Signature (a, b, *, c=42)>
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the loss. Items for which
-      this is False will be ignored when computing the loss.
-    weights: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating the weight for each item.
-    reduce_fn: An optional function that reduces the loss values. Can be
-      :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
-      is performed.
+    wrapped: The function whose signature to apply to the decorated function.
+    *new_kwarg_names: Names of the new kwonly arguments to add to the signature
+      of the decorated function.
 
   Returns:
-    The pairwise mean squared error loss.
+    A wrapper that modifies the signature of the decorated function to be like
+    ``wrapped`` but with new keyword arguments added to it.
   """
-  # Expand scores and labels into pairwise versions.
-  scores = compute_pairs(scores, operator.sub)
-  labels = compute_pairs(labels, operator.sub)
-
-  # Compute pairwise mask.
-  if where is not None:
-    where = compute_pairs(where, operator.and_)
 
-  # Compute squared error between score pairs and label pairs.
-  loss = jnp.square(scores - labels)
+  def wrapper(fun: T) -> T:
+    # Get the signature of the wrapped function and the new function.
+    wrapped_signature = inspect.signature(wrapped)
+    fun_signature = inspect.signature(fun)
+
+    # Get the parameters of both the wrapped function and the new function. To
+    # prevent adding duplicate parameters, the `wrapped_parameters` will not
+    # contain any parameters from `new_kwarg_names`, as those will be provided
+    # by the new function `fun`.
+    wrapped_parameters = [
+        wrapped_signature.parameters[param]
+        for param in wrapped_signature.parameters
+        if param not in new_kwarg_names
+    ]
+    fun_parameters = [
+        fun_signature.parameters[param] for param in new_kwarg_names
+    ]
+
+    # Create a thin wrapper for the function. We will set the `__signature__`
+    # property on this wrapper and return it, leaving the original `fun`
+    # untouched.
+    @functools.wraps(fun)
+    def output_fun(*args, **kwargs):
+      return fun(*args, **kwargs)
+
+    # Construct a new signature by copying the `wrapped_signature`, but
+    # replacing its parameters.
+    output_fun.__signature__ = wrapped_signature.replace(
+        parameters=wrapped_parameters + fun_parameters
+    )
 
-  # Apply weights to scores.
-  if weights is not None:
-    weights = compute_pairs(weights, lambda x, y: x)
-    loss *= weights
+    return output_fun
 
-  return utils.safe_reduce(loss, where=where, reduce_fn=reduce_fn)
+  return wrapper
```

### Comparing `rax-0.2.0/rax/_src/metrics.py` & `rax-0.3.0/rax/_src/metrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -27,58 +27,67 @@
 
 Standalone usage of a metric:
 
 >>> import jax
 >>> import rax
 >>> scores = jnp.array([2., 1., 3.])
 >>> labels = jnp.array([2., 0., 1.])
->>> rax.ndcg_metric(scores, labels)
-DeviceArray(0.79670763, dtype=float32)
+>>> print(rax.ndcg_metric(scores, labels))
+0.79670763
 
 Usage with a batch of data and a mask to indicate valid items:
 
 >>> scores = jnp.array([[2., 1., 3.], [1., 0.5, 1.5]])
 >>> labels = jnp.array([[2., 0., 1.], [0., 0., 1.]])
 >>> where = jnp.array([[True, True, False], [True, True, True]])
->>> rax.ndcg_metric(scores, labels)
-DeviceArray(0.8983538, dtype=float32)
+>>> print(rax.ndcg_metric(scores, labels))
+0.8983538
 
 Usage with :func:`jax.vmap` batching and a mask to indicate valid items:
 
 >>> scores = jnp.array([[2., 1., 0.], [1., 0.5, 1.5]])
 >>> labels = jnp.array([[1., 0., 0.], [0., 0., 1.]])
 >>> where = jnp.array([[True, True, False], [True, True, True]])
->>> jax.vmap(rax.ndcg_metric)(scores, labels, where=where)
-DeviceArray([1., 1.], dtype=float32)
-
+>>> print(jax.vmap(rax.ndcg_metric)(scores, labels, where=where))
+[1. 1.]
 """
 
 from typing import Callable, Optional
 
 import jax.numpy as jnp
 
+from rax._src import segment_utils
 from rax._src import utils
 from rax._src.types import Array
 from rax._src.types import CutoffFn
 from rax._src.types import RankFn
 from rax._src.types import ReduceFn
 
 
-def _retrieved_items(scores: Array,
-                     ranks: Array,
-                     *,
-                     where: Optional[Array] = None,
-                     topn: Optional[int] = None,
-                     cutoff_fn: CutoffFn = utils.cutoff) -> Array:
+def _retrieved_items(
+    scores: Array,
+    ranks: Array,
+    *,
+    where: Optional[Array] = None,
+    segments: Optional[Array] = None,
+    topn: Optional[int] = None,
+    cutoff_fn: CutoffFn = utils.cutoff
+) -> Array:
   """Computes an array that indicates which items are retrieved.
 
   Args:
-    scores: A [..., list_size]-Array, indicating the score of each item.
-    ranks: A [..., list_size]-Array, indicating the 1-based rank of each item.
-    where: An optional [..., list_size]-Array, indicating which items are valid.
+    scores: A [..., list_size]-:class:`jax.Array`, indicating the score of each
+      item.
+    ranks: A [..., list_size]-:class:`jax.Array`, indicating the 1-based rank of
+      each item.
+    where: An optional [..., list_size]-:class:`jax.Array`, indicating which
+      items are valid.
+    segments: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      segments within each list. The retrieved items will only be computed on
+      items that share the same segment.
     topn: An optional integer value indicating at which rank items are cut off.
       If None, no cutoff is performed.
     cutoff_fn: A callable that computes a cutoff tensor indicating which
       elements to include and which ones to exclude based on a topn cutoff. The
       callable should accept a `ranks` Array and an `n` integer and return a
       cutoffs Array of the same shape as `ranks`.
 
@@ -90,86 +99,92 @@
   retrieved_items = jnp.float32(jnp.logical_not(jnp.isneginf(scores)))
 
   # Masked items should always be ignored and not retrieved.
   if where is not None:
     retrieved_items *= jnp.float32(where)
 
   # Only consider items in the topn as retrieved items.
-  retrieved_items *= cutoff_fn(-ranks, n=topn)
+  retrieved_items *= cutoff_fn(-ranks, segments=segments, n=topn)
 
   return retrieved_items
 
 
 def default_gain_fn(label: Array) -> Array:
   r"""Default gain function used for gain-based metrics.
 
   Definition:
 
   .. math::
-      \operatorname{gain}(y) = 2^{y} - 1
+      \op{gain}(y) = 2^{y} - 1
 
   Args:
     label: The label to compute the gain for.
 
   Returns:
     The gain value for given label.
   """
-  return jnp.power(2., label) - 1.
+  return jnp.power(2.0, label) - 1.0
 
 
 def default_discount_fn(rank: Array) -> Array:
   r"""Default discount function used for discount-based metrics.
 
   Definition:
 
   .. math::
-      \operatorname{discount}(r) = 1. / \log_2(r + 1)
+      \op{discount}(r) = 1. / \log_2(r + 1)
 
   Args:
     rank: The 1-based rank.
 
   Returns:
     The discount value for given rank.
   """
-  return 1. / jnp.log2(rank + 1)
+  return 1.0 / jnp.log2(rank + 1)
 
 
-def mrr_metric(scores: Array,
-               labels: Array,
-               *,
-               where: Optional[Array] = None,
-               topn: Optional[int] = None,
-               key: Optional[Array] = None,
-               rank_fn: RankFn = utils.ranks,
-               cutoff_fn: CutoffFn = utils.cutoff,
-               reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
+def mrr_metric(
+    scores: Array,
+    labels: Array,
+    *,
+    where: Optional[Array] = None,
+    segments: Optional[Array] = None,
+    topn: Optional[int] = None,
+    key: Optional[Array] = None,
+    rank_fn: RankFn = utils.ranks,
+    cutoff_fn: CutoffFn = utils.cutoff,
+    reduce_fn: Optional[ReduceFn] = jnp.mean
+) -> Array:
   r"""Mean Reciprocal Rank (MRR).
 
   .. note::
 
     This metric converts graded relevance to binary relevance by considering
     items with ``label >= 1`` as relevant and items with ``label < 1`` as
     non-relevant.
 
   Definition:
 
   .. math::
-      \operatorname{mrr}(s, y) = \max_i \frac{y_i}{\operatorname{rank}(s_i)}
+      \op{mrr}(s, y) = \max_i \frac{y_i}{\op{rank}(s_i)}
 
-  where :math:`\operatorname{rank}(s_i)` indicates the rank of item :math:`i`
+  where :math:`\op{rank}(s_i)` indicates the rank of item :math:`i`
   after sorting all scores :math:`s` using ``rank_fn``.
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item. Items for which the score is :math:`-\inf` are treated
-        as unranked items.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the metric.
+    scores: A ``[..., list_size]``-:class:`~jax.Array`, indicating the score of
+      each item. Items for which the score is :math:`-\inf` are treated as
+      unranked items.
+    labels: A ``[..., list_size]``-:class:`~jax.Array`, indicating the relevance
+      label for each item.
+    where: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      which items are valid for computing the metric.
+    segments: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      segments within each list. The metric will only be computed on items that
+      share the same segment.
     topn: An optional integer value indicating at which rank the metric cuts
       off. If ``None``, no cutoff is performed.
     key: An optional :func:`~jax.random.PRNGKey`. If provided, any random
       operations in this metric will be based on this key.
     rank_fn: A function that maps scores to 1-based ranks.
     cutoff_fn: A function that maps ranks and a cutoff integer to a binary array
       indicating which items are cutoff.
@@ -177,69 +192,100 @@
       :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
       is performed.
 
   Returns:
     The MRR metric.
   """
   # Get the relevant items.
-  relevant_items = jnp.where(labels >= 1, jnp.ones_like(labels),
-                             jnp.zeros_like(labels))
+  relevant_items = jnp.where(
+      labels >= 1, jnp.ones_like(labels), jnp.zeros_like(labels)
+  )
 
   # Get the retrieved items.
-  ranks = rank_fn(scores, where=where, key=key)
+  ranks = rank_fn(scores, where=where, segments=segments, key=key)
   retrieved_items = _retrieved_items(
-      scores, ranks, where=where, topn=topn, cutoff_fn=cutoff_fn)
+      scores,
+      ranks,
+      where=where,
+      segments=segments,
+      topn=topn,
+      cutoff_fn=cutoff_fn,
+  )
 
   # Compute reciprocal ranks.
-  reciprocal_ranks = jnp.reciprocal(jnp.where(ranks == 0., jnp.inf, ranks))
+  reciprocal_ranks = jnp.reciprocal(jnp.where(ranks == 0.0, jnp.inf, ranks))
 
   # Get the maximum reciprocal rank.
-  values = jnp.max(
-      relevant_items * retrieved_items * reciprocal_ranks,
-      axis=-1,
-      where=where,
-      initial=0.)
-  return utils.safe_reduce(values, reduce_fn=reduce_fn)
-
-
-def recall_metric(scores: Array,
-                  labels: Array,
-                  *,
-                  where: Optional[Array] = None,
-                  topn: Optional[int] = None,
-                  key: Optional[Array] = None,
-                  rank_fn: RankFn = utils.ranks,
-                  cutoff_fn: CutoffFn = utils.cutoff,
-                  reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
+  if segments is not None:
+    values = segment_utils.segment_max(
+        relevant_items * retrieved_items * reciprocal_ranks,
+        segments,
+        where=where,
+        initial=0.0,
+    )
+  else:
+    values = jnp.max(
+        relevant_items * retrieved_items * reciprocal_ranks,
+        axis=-1,
+        where=where,
+        initial=0.0,
+    )
+
+  # In the segmented case, values retain their list dimension. This constructs
+  # a mask so that only the first item per segment is used in reduce_fn.
+  if segments is not None:
+    where = segment_utils.first_item_segment_mask(segments, where=where)
+
+  # Setup mask to ignore lists with only invalid items in reduce_fn.
+  elif where is not None:
+    where = jnp.any(where, axis=-1)
+
+  return utils.safe_reduce(values, where=where, reduce_fn=reduce_fn)
+
+
+def recall_metric(
+    scores: Array,
+    labels: Array,
+    *,
+    where: Optional[Array] = None,
+    segments: Optional[Array] = None,
+    topn: Optional[int] = None,
+    key: Optional[Array] = None,
+    rank_fn: RankFn = utils.ranks,
+    cutoff_fn: CutoffFn = utils.cutoff,
+    reduce_fn: Optional[ReduceFn] = jnp.mean
+) -> Array:
   r"""Recall.
 
   .. note::
 
     This metric converts graded relevance to binary relevance by considering
     items with ``label >= 1`` as relevant and items with ``label < 1`` as
     non-relevant.
 
   Definition:
 
   .. math::
-      \operatorname{recall@n}(s, y) =
-      \frac{1}{\sum_i y_i}
-      \sum_i y_i \cdot \mathbb{I}\left[\operatorname{rank}(s_i) \leq n\right]
+      \op{recall@n}(s, y) = \frac{1}{\sum_i y_i}
+                            \sum_i y_i \cdot \II{\op{rank}(s_i) \leq n}
 
-  where :math:`\operatorname{rank}(s_i)` indicates the rank of item :math:`i`
+  where :math:`\op{rank}(s_i)` indicates the rank of item :math:`i`
   after sorting all scores :math:`s` using `rank_fn`.
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item. Items for which the score is :math:`-\inf` are treated
-        as unranked items.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the metric.
+    scores: A ``[..., list_size]``-:class:`~jax.Array`, indicating the score of
+      each item. Items for which the score is :math:`-\inf` are treated as
+      unranked items.
+    labels: A ``[..., list_size]``-:class:`~jax.Array`, indicating the relevance
+      label for each item.
+    where: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      which items are valid for computing the metric.
+    segments: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      segments within each list. The metric will only be computed on items that
+      share the same segment.
     topn: An optional integer value indicating at which rank the metric cuts
       off. If ``None``, no cutoff is performed.
     key: An optional :func:`~jax.random.PRNGKey`. If provided, any random
       operations in this metric will be based on this key.
     rank_fn: A function that maps scores to 1-based ranks.
     cutoff_fn: A function that maps ranks and a cutoff integer to a binary array
       indicating which items are cutoff.
@@ -247,68 +293,99 @@
       :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
       is performed.
 
   Returns:
     The recall metric.
   """
   # Get the relevant items.
-  relevant_items = jnp.where(labels >= 1, jnp.ones_like(labels),
-                             jnp.zeros_like(labels))
+  relevant_items = jnp.where(
+      labels >= 1, jnp.ones_like(labels), jnp.zeros_like(labels)
+  )
 
   # Get the retrieved items.
-  ranks = rank_fn(scores, where=where, key=key)
+  ranks = rank_fn(scores, where=where, segments=segments, key=key)
   retrieved_items = _retrieved_items(
-      scores, ranks, where=where, topn=topn, cutoff_fn=cutoff_fn)
+      scores,
+      ranks,
+      where=where,
+      segments=segments,
+      topn=topn,
+      cutoff_fn=cutoff_fn,
+  )
 
   # Compute number of retrieved+relevant items and relevant items.
-  n_retrieved_relevant = jnp.sum(
-      retrieved_items * relevant_items, where=where, axis=-1)
-  n_relevant = jnp.sum(relevant_items, where=where, axis=-1)
+  if segments is not None:
+    n_retrieved_relevant = segment_utils.segment_sum(
+        retrieved_items * relevant_items, segments, where=where
+    )
+    n_relevant = segment_utils.segment_sum(
+        relevant_items, segments, where=where
+    )
+  else:
+    n_retrieved_relevant = jnp.sum(
+        retrieved_items * relevant_items, where=where, axis=-1
+    )
+    n_relevant = jnp.sum(relevant_items, where=where, axis=-1)
 
   # Compute recall but prevent division by zero.
-  n_relevant = jnp.where(n_relevant == 0, 1., n_relevant)
+  n_relevant = jnp.where(n_relevant == 0, 1.0, n_relevant)
   values = n_retrieved_relevant / n_relevant
-  return utils.safe_reduce(values, reduce_fn=reduce_fn)
-
 
-def precision_metric(scores: Array,
-                     labels: Array,
-                     *,
-                     where: Optional[Array] = None,
-                     topn: Optional[int] = None,
-                     key: Optional[Array] = None,
-                     rank_fn: RankFn = utils.ranks,
-                     cutoff_fn: CutoffFn = utils.cutoff,
-                     reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
+  # In the segmented case, values retain their list dimension. This constructs
+  # a mask so that only the first item per segment is used in reduce_fn.
+  if segments is not None:
+    where = segment_utils.first_item_segment_mask(segments, where=where)
+
+  # Setup mask to ignore lists with only invalid items in reduce_fn.
+  elif where is not None:
+    where = jnp.any(where, axis=-1)
+
+  return utils.safe_reduce(values, where=where, reduce_fn=reduce_fn)
+
+
+def precision_metric(
+    scores: Array,
+    labels: Array,
+    *,
+    where: Optional[Array] = None,
+    segments: Optional[Array] = None,
+    topn: Optional[int] = None,
+    key: Optional[Array] = None,
+    rank_fn: RankFn = utils.ranks,
+    cutoff_fn: CutoffFn = utils.cutoff,
+    reduce_fn: Optional[ReduceFn] = jnp.mean
+) -> Array:
   r"""Precision.
 
   .. note::
 
     This metric converts graded relevance to binary relevance by considering
     items with ``label >= 1`` as relevant and items with ``label < 1`` as
     non-relevant.
 
   Definition:
 
   .. math::
-      \operatorname{precision@n}(s, y) =
-      \frac{1}{n}
-      \sum_i y_i \cdot \mathbb{I}\left[\operatorname{rank}(s_i) \leq n\right]
+      \op{precision@n}(s, y) = \frac{1}{n}
+                               \sum_i y_i \cdot \II{\op{rank}(s_i) \leq n}
 
-  where :math:`\operatorname{rank}(s_i)` indicates the rank of item :math:`i`
+  where :math:`\op{rank}(s_i)` indicates the rank of item :math:`i`
   after sorting all scores :math:`s` using ``rank_fn``.
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item. Items for which the score is :math:`-\inf` are treated
-        as unranked items.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the metric.
+    scores: A ``[..., list_size]``-:class:`~jax.Array`, indicating the score of
+      each item. Items for which the score is :math:`-\inf` are treated as
+      unranked items.
+    labels: A ``[..., list_size]``-:class:`~jax.Array`, indicating the relevance
+      label for each item.
+    where: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      which items are valid for computing the metric.
+    segments: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      segments within each list. The metric will only be computed on items that
+      share the same segment.
     topn: An optional integer value indicating at which rank the metric cuts
       off. If ``None``, no cutoff is performed.
     key: An optional :func:`~jax.random.PRNGKey`. If provided, any random
       operations in this metric will be based on this key.
     rank_fn: A function that maps scores to 1-based ranks.
     cutoff_fn: A function that maps ranks and a cutoff integer to a binary array
       indicating which items are cutoff.
@@ -316,68 +393,99 @@
       :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
       is performed.
 
   Returns:
     The precision metric.
   """
   # Get the relevant items.
-  relevant_items = jnp.where(labels >= 1, jnp.ones_like(labels),
-                             jnp.zeros_like(labels))
+  relevant_items = jnp.where(
+      labels >= 1, jnp.ones_like(labels), jnp.zeros_like(labels)
+  )
 
   # Get the retrieved items.
-  ranks = rank_fn(scores, where=where, key=key)
+  ranks = rank_fn(scores, where=where, segments=segments, key=key)
   retrieved_items = _retrieved_items(
-      scores, ranks, where=where, topn=topn, cutoff_fn=cutoff_fn)
+      scores,
+      ranks,
+      where=where,
+      segments=segments,
+      topn=topn,
+      cutoff_fn=cutoff_fn,
+  )
 
   # Compute number of retrieved+relevant items and retrieved items.
-  n_retrieved_relevant = jnp.sum(
-      retrieved_items * relevant_items, where=where, axis=-1)
-  n_retrieved = jnp.sum(retrieved_items, where=where, axis=-1)
+  if segments is not None:
+    n_retrieved_relevant = segment_utils.segment_sum(
+        retrieved_items * relevant_items, segments, where=where
+    )
+    n_retrieved = segment_utils.segment_sum(
+        retrieved_items, segments, where=where
+    )
+  else:
+    n_retrieved_relevant = jnp.sum(
+        retrieved_items * relevant_items, where=where, axis=-1
+    )
+    n_retrieved = jnp.sum(retrieved_items, where=where, axis=-1)
 
   # Compute precision but prevent division by zero.
-  n_retrieved = jnp.where(n_retrieved == 0, 1., n_retrieved)
+  n_retrieved = jnp.where(n_retrieved == 0, 1.0, n_retrieved)
   values = n_retrieved_relevant / n_retrieved
-  return utils.safe_reduce(values, reduce_fn=reduce_fn)
 
-
-def ap_metric(scores: Array,
-              labels: Array,
-              *,
-              where: Optional[Array] = None,
-              topn: Optional[int] = None,
-              key: Optional[Array] = None,
-              rank_fn: RankFn = utils.ranks,
-              cutoff_fn: CutoffFn = utils.cutoff,
-              reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
+  # In the segmented case, values retain their list dimension. This constructs
+  # a mask so that only the first item per segment is used in reduce_fn.
+  if segments is not None:
+    where = segment_utils.first_item_segment_mask(segments, where=where)
+
+  # Setup mask to ignore lists with only invalid items in reduce_fn.
+  elif where is not None:
+    where = jnp.any(where, axis=-1)
+
+  return utils.safe_reduce(values, where=where, reduce_fn=reduce_fn)
+
+
+def ap_metric(
+    scores: Array,
+    labels: Array,
+    *,
+    where: Optional[Array] = None,
+    segments: Optional[Array] = None,
+    topn: Optional[int] = None,
+    key: Optional[Array] = None,
+    rank_fn: RankFn = utils.ranks,
+    cutoff_fn: CutoffFn = utils.cutoff,
+    reduce_fn: Optional[ReduceFn] = jnp.mean
+) -> Array:
   r"""Average Precision.
 
   .. note::
 
     This metric converts graded relevance to binary relevance by considering
     items with ``label >= 1`` as relevant and items with ``label < 1`` as
     non-relevant.
 
   Definition:
 
   .. math::
-      \operatorname{ap}(s, y) =
-      \frac{1}{\sum_i y_i}
-      \sum_i y_i \operatorname{precision@rank}_{s_i}(s, y)
+      \op{ap}(s, y) =
+      \frac{1}{\sum_i y_i} \sum_i y_i \op{precision@rank}_{s_i}(s, y)
 
-  where :math:`\operatorname{precision@rank}_{s_i}(s, y)` indicates the
+  where :math:`\op{precision@rank}_{s_i}(s, y)` indicates the
   precision at the rank of item :math:`i`.
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item. Items for which the score is :math:`-\inf` are treated
-        as unranked items.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the metric.
+    scores: A ``[..., list_size]``-:class:`~jax.Array`, indicating the score of
+      each item. Items for which the score is :math:`-\inf` are treated as
+      unranked items.
+    labels: A ``[..., list_size]``-:class:`~jax.Array`, indicating the relevance
+      label for each item.
+    where: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      which items are valid for computing the metric.
+    segments: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      segments within each list. The metric will only be computed on items that
+      share the same segment.
     topn: An optional integer value indicating at which rank the metric cuts
       off. If ``None``, no cutoff is performed.
     key: An optional :func:`~jax.random.PRNGKey`. If provided, any random
       operations in this metric will be based on this key.
     rank_fn: A function that maps scores to 1-based ranks.
     cutoff_fn: A function that maps ranks and a cutoff integer to a binary array
       indicating which items are cutoff.
@@ -385,84 +493,113 @@
       :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
       is performed.
 
   Returns:
     The average precision metric.
   """
   # Get the relevant items.
-  relevant_items = jnp.where(labels >= 1, jnp.ones_like(labels),
-                             jnp.zeros_like(labels))
+  relevant_items = jnp.where(
+      labels >= 1, jnp.ones_like(labels), jnp.zeros_like(labels)
+  )
 
   # Get the retrieved items.
-  ranks = rank_fn(scores, where=where, key=key)
+  ranks = rank_fn(scores, where=where, segments=segments, key=key)
   retrieved_items = _retrieved_items(
-      scores, ranks, where=where, topn=topn, cutoff_fn=cutoff_fn)
-
-  # Compute ranks.
-  ranks = rank_fn(scores, where=where, key=key)
+      scores,
+      ranks,
+      where=where,
+      segments=segments,
+      topn=topn,
+      cutoff_fn=cutoff_fn,
+  )
 
   # Compute a matrix of all precision@k values
   relevant_i = jnp.expand_dims(relevant_items, axis=-1)
   relevant_j = jnp.expand_dims(relevant_items, axis=-2)
   ranks_i = jnp.expand_dims(ranks, axis=-1)
   ranks_j = jnp.expand_dims(ranks, axis=-2)
   prec_at_k = ((ranks_i >= ranks_j) * relevant_i * relevant_j) / ranks_i
 
   # Only include precision@k for retrieved items.
-  sum_prec_at_k = jnp.sum(
-      prec_at_k * jnp.expand_dims(retrieved_items, -1), axis=(-2, -1))
-
-  # Compute number of relevant items.
-  n_relevant = jnp.sum(relevant_items, where=where, axis=-1)
+  prec_mask = None
+  if segments is not None:
+    prec_mask = segment_utils.same_segment_mask(segments)
+  prec_at_k = jnp.sum(
+      prec_at_k * jnp.expand_dims(retrieved_items, -1), axis=-1, where=prec_mask
+  )
+
+  # Compute summed precision@k for each list and the number of relevant items.
+  if segments is not None:
+    sum_prec_at_k = segment_utils.segment_sum(prec_at_k, segments, where=where)
+    n_relevant = segment_utils.segment_sum(
+        relevant_items, segments, where=where
+    )
+  else:
+    sum_prec_at_k = jnp.sum(prec_at_k, axis=-1)
+    n_relevant = jnp.sum(relevant_items, where=where, axis=-1)
 
   # Compute average precision but prevent division by zero.
-  n_relevant = jnp.where(n_relevant == 0, 1., n_relevant)
+  n_relevant = jnp.where(n_relevant == 0, 1.0, n_relevant)
   values = sum_prec_at_k / n_relevant
-  return utils.safe_reduce(values, reduce_fn=reduce_fn)
-
 
-def dcg_metric(scores: Array,
-               labels: Array,
-               *,
-               where: Optional[Array] = None,
-               topn: Optional[int] = None,
-               weights: Optional[Array] = None,
-               key: Optional[Array] = None,
-               gain_fn: Callable[[Array], Array] = default_gain_fn,
-               discount_fn: Callable[[Array], Array] = default_discount_fn,
-               rank_fn: RankFn = utils.ranks,
-               cutoff_fn: CutoffFn = utils.cutoff,
-               reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
+  # In the segmented case, values retain their list dimension. This constructs
+  # a mask so that only the first item per segment is used in reduce_fn.
+  if segments is not None:
+    where = segment_utils.first_item_segment_mask(segments, where=where)
+
+  # Setup mask to ignore lists with only invalid items in reduce_fn.
+  elif where is not None:
+    where = jnp.any(where, axis=-1)
+
+  return utils.safe_reduce(values, where=where, reduce_fn=reduce_fn)
+
+
+def dcg_metric(
+    scores: Array,
+    labels: Array,
+    *,
+    where: Optional[Array] = None,
+    segments: Optional[Array] = None,
+    topn: Optional[int] = None,
+    weights: Optional[Array] = None,
+    key: Optional[Array] = None,
+    gain_fn: Callable[[Array], Array] = default_gain_fn,
+    discount_fn: Callable[[Array], Array] = default_discount_fn,
+    rank_fn: RankFn = utils.ranks,
+    cutoff_fn: CutoffFn = utils.cutoff,
+    reduce_fn: Optional[ReduceFn] = jnp.mean
+) -> Array:
   r"""Discounted cumulative gain (DCG).
 
   Definition :cite:p:`jarvelin2002cumulated`:
 
   .. math::
-      \operatorname{dcg}(s, y) =
-      \sum_i \operatorname{gain}(y_i)
-      \cdot \operatorname{discount}(\operatorname{rank}(s_i))
+      \op{dcg}(s, y) = \sum_i \op{gain}(y_i) \cdot \op{discount}(\op{rank}(s_i))
 
-  where :math:`\operatorname{rank}(s_i)` indicates the 1-based rank of item
-  :math:`i` as computed by ``rank_fn``, :math:`\operatorname{gain}(y)` indicates
+  where :math:`\op{rank}(s_i)` indicates the 1-based rank of item
+  :math:`i` as computed by ``rank_fn``, :math:`\op{gain}(y)` indicates
   the per-item gains as computed by ``gain_fn``, and,
-  :math:`\operatorname{discount}(r)` indicates the per-item rank discounts as
+  :math:`\op{discount}(r)` indicates the per-item rank discounts as
   computed by ``discount_fn``.
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item. Items for which the score is :math:`-\inf` are treated
-        as unranked items.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the metric.
+    scores: A ``[..., list_size]``-:class:`~jax.Array`, indicating the score of
+      each item. Items for which the score is :math:`-\inf` are treated as
+      unranked items.
+    labels: A ``[..., list_size]``-:class:`~jax.Array`, indicating the relevance
+      label for each item.
+    where: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      which items are valid for computing the metric.
+    segments: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      segments within each list. The metric will only be computed on items that
+      share the same segment.
     topn: An optional integer value indicating at which rank the metric cuts
       off. If ``None``, no cutoff is performed.
-    weights: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating the per-item weights.
+    weights: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      the per-item weights.
     key: An optional :func:`~jax.random.PRNGKey`. If provided, any random
       operations in this metric will be based on this key.
     gain_fn: A function that maps relevance label to gain values.
     discount_fn: A function that maps 1-based ranks to discount values.
     rank_fn: A function that maps scores to 1-based ranks.
     cutoff_fn: A function that maps ranks and a cutoff integer to a binary array
       indicating which items are cutoff.
@@ -470,65 +607,91 @@
       :func:`jax.numpy.sum` or :func:`jax.numpy.mean`. If ``None``, no reduction
       is performed.
 
   Returns:
     The DCG metric.
   """
   # Get the retrieved items.
-  ranks = rank_fn(scores, where=where, key=key)
+  ranks = rank_fn(scores, where=where, segments=segments, key=key)
   retrieved_items = _retrieved_items(
-      scores, ranks, where=where, topn=topn, cutoff_fn=cutoff_fn)
+      scores,
+      ranks,
+      segments=segments,
+      where=where,
+      topn=topn,
+      cutoff_fn=cutoff_fn,
+  )
 
   # Computes (weighted) gains.
   gains = gain_fn(labels)
   if weights is not None:
     gains *= weights
 
   # Computes rank discounts.
   discounts = discount_fn(ranks)
 
   # Compute DCG.
-  values = jnp.sum(retrieved_items * gains * discounts, axis=-1, where=where)
-  return utils.safe_reduce(values, reduce_fn=reduce_fn)
-
-
-def ndcg_metric(scores: Array,
-                labels: Array,
-                *,
-                where: Optional[Array] = None,
-                topn: Optional[int] = None,
-                weights: Optional[Array] = None,
-                key: Optional[Array] = None,
-                gain_fn: Callable[[Array], Array] = default_gain_fn,
-                discount_fn: Callable[[Array], Array] = default_discount_fn,
-                rank_fn: RankFn = utils.ranks,
-                cutoff_fn: CutoffFn = utils.cutoff,
-                reduce_fn: Optional[ReduceFn] = jnp.mean) -> Array:
+  if segments is not None:
+    values = segment_utils.segment_sum(
+        retrieved_items * gains * discounts, segments, where=where
+    )
+  else:
+    values = jnp.sum(retrieved_items * gains * discounts, axis=-1, where=where)
+
+  # In the segmented case, values retain their list dimension. This constructs
+  # a mask so that only the first item per segment is used in reduce_fn.
+  if segments is not None:
+    where = segment_utils.first_item_segment_mask(segments, where=where)
+
+  # Setup mask to ignore lists with only invalid items in reduce_fn.
+  elif where is not None:
+    where = jnp.any(where, axis=-1)
+
+  return utils.safe_reduce(values, where=where, reduce_fn=reduce_fn)
+
+
+def ndcg_metric(
+    scores: Array,
+    labels: Array,
+    *,
+    where: Optional[Array] = None,
+    segments: Optional[Array] = None,
+    topn: Optional[int] = None,
+    weights: Optional[Array] = None,
+    key: Optional[Array] = None,
+    gain_fn: Callable[[Array], Array] = default_gain_fn,
+    discount_fn: Callable[[Array], Array] = default_discount_fn,
+    rank_fn: RankFn = utils.ranks,
+    cutoff_fn: CutoffFn = utils.cutoff,
+    reduce_fn: Optional[ReduceFn] = jnp.mean
+) -> Array:
   r"""Normalized discounted cumulative gain (NDCG).
 
   Definition :cite:p:`jarvelin2002cumulated`:
 
   .. math::
-      \operatorname{ndcg}(s, y) =
-      \operatorname{dcg}(s, y) / \operatorname{dcg}(y, y)
+      \op{ndcg}(s, y) = \op{dcg}(s, y) / \op{dcg}(y, y)
 
-  where :math:`\operatorname{dcg}` is the discounted cumulative gain metric.
+  where :math:`\op{dcg}` is the discounted cumulative gain metric.
 
   Args:
-    scores: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      score of each item. Items for which the score is :math:`-\inf` are treated
-        as unranked items.
-    labels: A ``[..., list_size]``-:class:`~jax.numpy.ndarray`, indicating the
-      relevance label for each item.
-    where: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating which items are valid for computing the metric.
+    scores: A ``[..., list_size]``-:class:`~jax.Array`, indicating the score of
+      each item. Items for which the score is :math:`-\inf` are treated as
+      unranked items.
+    labels: A ``[..., list_size]``-:class:`~jax.Array`, indicating the relevance
+      label for each item.
+    where: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      which items are valid for computing the metric.
+    segments: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      segments within each list. The metric will only be computed on items that
+      share the same segment.
     topn: An optional integer value indicating at which rank the metric cuts
       off. If ``None``, no cutoff is performed.
-    weights: An optional ``[..., list_size]``-:class:`~jax.numpy.ndarray`,
-      indicating the per-item weights.
+    weights: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+      the per-item weights.
     key: An optional :func:`~jax.random.PRNGKey`. If provided, any random
       operations in this metric will be based on this key.
     gain_fn: A function that maps relevance label to gain values.
     discount_fn: A function that maps 1-based ranks to discount values.
     rank_fn: A function that maps scores to 1-based ranks.
     cutoff_fn: A function that maps ranks and a cutoff integer to a binary array
       indicating which items are cutoff.
@@ -540,37 +703,51 @@
     The NDCG metric.
   """
   # Compute regular dcg.
   regular_dcg = dcg_metric(
       scores,
       labels,
       where=where,
+      segments=segments,
       topn=topn,
       weights=weights,
       key=key,
       gain_fn=gain_fn,
       discount_fn=discount_fn,
       rank_fn=rank_fn,
       cutoff_fn=cutoff_fn,
-      reduce_fn=None)
+      reduce_fn=None,
+  )
 
   # The ideal dcg is computed by ordering items by their (weighted) gains.
   ideal_scores = gain_fn(labels)
   if weights is not None:
     ideal_scores *= weights
   ideal_dcg = dcg_metric(
       ideal_scores,
       labels,
       where=where,
+      segments=segments,
       topn=topn,
       weights=weights,
       key=None,
       gain_fn=gain_fn,
       discount_fn=discount_fn,
       rank_fn=utils.ranks,
       cutoff_fn=utils.cutoff,
-      reduce_fn=None)
+      reduce_fn=None,
+  )
 
   # Compute the result as `dcg / ideal_dcg` while preventing division by zero.
-  ideal_dcg = jnp.where(ideal_dcg == 0., 1., ideal_dcg)
+  ideal_dcg = jnp.where(ideal_dcg == 0.0, 1.0, ideal_dcg)
   values = regular_dcg / ideal_dcg
-  return utils.safe_reduce(values, reduce_fn=reduce_fn)
+
+  # In the segmented case, values retain their list dimension. This constructs
+  # a mask so that only the first item per segment is used in reduce_fn.
+  if segments is not None:
+    where = segment_utils.first_item_segment_mask(segments, where=where)
+
+  # Setup mask to ignore lists with only invalid items in reduce_fn.
+  elif where is not None:
+    where = jnp.any(where, axis=-1)
+
+  return utils.safe_reduce(values, where=where, reduce_fn=reduce_fn)
```

### Comparing `rax-0.2.0/rax/_src/types.py` & `rax-0.3.0/rax/_src/types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,124 +14,170 @@
 
 """Rax-specific types and protocols.
 
 .. note::
 
   Types and protocols are provided for **type-checking** convenience only. You
   do **not** need to instantiate, subclass or extend them.
-
 """
 
 from typing import Optional, Tuple, Union
 import jax
 
 # Protocol is a python 3.8+ feature. For older versions, we can use
 # typing_extensions, which provides the same functionality.
 try:
   from typing import Protocol  # pylint: disable=g-import-not-at-top
 except ImportError:
   from typing_extensions import Protocol  # pylint: disable=g-import-not-at-top
 
-
 # Type alias for a JAX array.
-Array = jax.numpy.ndarray
+Array = jax.Array
 
 
 class RankFn(Protocol):
   """:class:`typing.Protocol` for rank functions."""
 
-  def __call__(self, scores: Array, where: Optional[Array],
-               key: Optional[Array]) -> Array:
+  def __call__(
+      self,
+      scores: Array,
+      where: Optional[Array],
+      key: Optional[Array],
+      segments: Optional[Array] = None,
+  ) -> Array:
     """Computes 1-based ranks based on the given scores.
 
     Args:
       scores: The scores to compute the 1-based ranks for.
-      where: An optional :class:`jax.numpy.ndarray` of the same shape as ``a``
-        that indicates which elements to rank. Other elements will be ranked
-        last.
+      where: An optional :class:`~jax.Array` of the same shape as ``a`` that
+        indicates which elements to rank. Other elements will be ranked last.
       key: An optional :func:`~jax.random.PRNGKey` used for random operations.
+      segments: An optional :class:`~jax.Array` of the same shape as ``a`` that
+        indicates which elements to group together.
 
     Returns:
-      A :class:`jax.numpy.ndarray` of the same shape as ``scores`` that
+      A :class:`~jax.Array` of the same shape as ``scores`` that
       represents the 1-based ranks.
     """
     pass
 
 
 class CutoffFn(Protocol):
   """:class:`typing.Protocol` for cutoff functions."""
 
-  def __call__(self, a: Array, n: Optional[int]) -> Array:
+  def __call__(
+      self, a: Array, n: Optional[int], segments: Optional[Array] = None
+  ) -> Array:
     """Computes cutoffs based on the given array.
 
     Args:
       a: The array for which to compute the cutoffs.
       n: The position of the cutoff.
+      segments: An optional :class:`~jax.Array` of the same shape as ``a`` that
+        indicates which elements to group together.
 
     Returns:
-      A binary :class:`jax.numpy.ndarray` of the same shape as ``a`` that
+      A binary :class:`~jax.Array` of the same shape as ``a`` that
       represents which elements of ``a`` should be selected for the topn cutoff.
     """
     pass
 
 
 class ReduceFn(Protocol):
   """:class:`typing.Protocol` for reduce functions."""
 
-  def __call__(self, a: Array, where: Optional[Array],
-               axis: Optional[Union[int, Tuple[int, ...]]]) -> Array:
+  def __call__(
+      self,
+      a: Array,
+      where: Optional[Array],
+      axis: Optional[Union[int, Tuple[int, ...]]],
+  ) -> Array:
     """Reduces an array across one or more dimensions.
 
     Args:
       a: The array to reduce.
-      where: An optional :class:`jax.numpy.ndarray` of the same shape as ``a``
-        that indicates which elements to include in the reduction.
+      where: An optional :class:`~jax.Array` of the same shape as ``a`` that
+        indicates which elements to include in the reduction.
       axis: One or more axes to use for the reduction. If ``None`` this reduces
         across all available axes.
 
     Returns:
-      A :class:`jax.numpy.ndarray` that represents the reduced result of ``a``
+      A :class:`~jax.Array` that represents the reduced result of ``a``
       over given ``axis``.
     """
     pass
 
 
 class LossFn(Protocol):
   """:class:`typing.Protocol` for loss functions."""
 
-  def __call__(self, scores: Array, labels: Array, *,
-               where: Optional[Array], **kwargs) -> Array:
+  def __call__(
+      self, scores: Array, labels: Array, *, where: Optional[Array], **kwargs
+  ) -> Array:
     """Computes a loss.
 
     Args:
       scores: The score of each item.
       labels: The label of each item.
-      where: An optional :class:`jax.numpy.ndarray` of the same shape as
-        ``scores`` that indicates which elements to include in the loss.
+      where: An optional :class:`~jax.Array` of the same shape as ``scores``
+        that indicates which elements to include in the loss.
       **kwargs: Optional loss-specific keyword arguments.
 
     Returns:
-      A :class:`jax.numpy.ndarray` that represents the loss computed on the
+      A :class:`~jax.Array` that represents the loss computed on the
       given ``scores`` and ``labels``.
     """
     pass
 
 
 class MetricFn(Protocol):
   """:class:`typing.Protocol` for metric functions."""
 
-  def __call__(self, scores: Array, labels: Array, *,
-               where: Optional[Array], **kwargs) -> Array:
+  def __call__(
+      self, scores: Array, labels: Array, *, where: Optional[Array], **kwargs
+  ) -> Array:
     """Computes a metric.
 
     Args:
       scores: The score of each item.
       labels: The label of each item.
-      where: An optional :class:`jax.numpy.ndarray` of the same shape as
-        ``scores`` that indicates which elements to include in the metric.
+      where: An optional :class:`~jax.Array` of the same shape as ``scores``
+        that indicates which elements to include in the metric.
       **kwargs: Optional metric-specific keyword arguments.
 
     Returns:
-      A :class:`jax.numpy.ndarray` that represents the metric computed on the
+      A :class:`~jax.Array` that represents the metric computed on the
       given ``scores`` and ``labels``.
     """
     pass
+
+
+class LambdaweightFn(Protocol):
+  """:class:`typing.Protocol` for lambdaweight functions."""
+
+  def __call__(
+      self,
+      scores: Array,
+      labels: Array,
+      *,
+      where: Optional[Array],
+      weights: Optional[Array],
+      **kwargs
+  ) -> Array:
+    """Computes lambdaweights.
+
+    Args:
+      scores: A ``[..., list_size]``-:class:`~jax.Array`, indicating the score
+        of each item.
+      labels: A ``[..., list_size]``-:class:`~jax.Array`, indicating the
+        relevance label for each item.
+      where: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+        which items are valid for computing the lambdaweights. Items for which
+        this is False will be ignored when computing the lambdaweights.
+      weights: An optional ``[..., list_size]``-:class:`~jax.Array`, indicating
+        the weight for each item.
+      **kwargs: Optional lambdaweight-specific keyword arguments.
+
+    Returns:
+      A :class:`~jax.Array` that represents the lambda weights.
+    """
+    pass
```

### Comparing `rax-0.2.0/rax/types.py` & `rax-0.3.0/rax/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,22 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Rax-specific types."""
 
 from rax._src.types import CutoffFn
+from rax._src.types import LambdaweightFn
 from rax._src.types import LossFn
 from rax._src.types import MetricFn
 from rax._src.types import RankFn
 from rax._src.types import ReduceFn
 
-# pyformat: disable
 __all__ = [
     "CutoffFn",
+    "LambdaweightFn",
     "LossFn",
     "MetricFn",
     "RankFn",
     "ReduceFn",
 ]
-# pyformat: enable
-
```

### Comparing `rax-0.2.0/rax/utils.py` & `rax-0.3.0/rax/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,16 +15,13 @@
 """Rax-specific utilities."""
 
 from rax._src.utils import approx_cutoff
 from rax._src.utils import approx_ranks
 from rax._src.utils import cutoff
 from rax._src.utils import ranks
 
-# pyformat: disable
 __all__ = [
     "approx_cutoff",
     "approx_ranks",
     "cutoff",
     "ranks",
 ]
-# pyformat: enable
-
```

### Comparing `rax-0.2.0/rax.egg-info/PKG-INFO` & `rax-0.3.0/rax.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: rax
-Version: 0.2.0
-Summary: Composable Learning-to-Rank using JAX.
+Version: 0.3.0
+Summary: Learning-to-Rank using JAX.
 Home-page: https://github.com/google/rax
 Author: Google
 Author-email: rax-dev@google.com
 License: Apache 2.0
 Keywords: learning-to-rank jax ranking
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 🦖 **Rax**: Composable Learning to Rank using JAX
+# 🦖 **Rax**: Learning-to-Rank using JAX
 
 [![Docs](https://readthedocs.org/projects/rax/badge/?version=latest)](https://rax.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/rax?color=brightgreen)](https://pypi.org/project/rax/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-brightgreen.svg)](https://github.com/google/rax/blob/main/LICENSE)
 
 **Rax** is a Learning-to-Rank library written in JAX. Rax provides off-the-shelf
 implementations of ranking losses and metrics to be used with JAX. It provides
@@ -53,40 +53,48 @@
 In a nutshell, given the scores and labels for a list of items, Rax can compute
 various ranking losses and metrics:
 
 ```python
 import jax.numpy as jnp
 import rax
 
-scores = jnp.asarray([2.2, -1.3, 5.4])  # output of a model.
-labels = jnp.asarray([1., 0., 0.])      # indicates doc 1 is relevant.
+scores = jnp.array([2.2, -1.3, 5.4])  # output of a model.
+labels = jnp.array([1.0,  0.0, 0.0])  # indicates doc 1 is relevant.
 
-rax.ndcg_metric(scores, labels)         # computes a ranking metric.
-rax.pairwise_hinge_loss(scores, labels) # computes a ranking loss.
+rax.ndcg_metric(scores, labels)  # computes a ranking metric.
+# 0.63092977
+
+rax.pairwise_hinge_loss(scores, labels)  # computes a ranking loss.
+# 2.1
 ```
 
 All of the Rax losses and metrics are purely functional and compose well with
 standard JAX transformations. Additionally, Rax provides ranking-specific
 transformations so you can build new ranking losses. An example is
 `rax.approx_t12n`, which can be used to transform any (non-differentiable)
 ranking metric into a differentiable loss. For example:
 
 ```python
 loss_fn = rax.approx_t12n(rax.ndcg_metric)
-loss_fn(scores, labels)            # differentiable approx ndcg loss.
+loss_fn(scores, labels)  # differentiable approx ndcg loss.
+# -0.63282484
+
 jax.grad(loss_fn)(scores, labels)  # computes gradients w.r.t. scores.
+# [-0.01276882  0.00549765  0.00727116]
 ```
 
 ## Installation
 
 See https://github.com/google/jax#installation for instructions on installing JAX.
 
 We suggest installing the latest stable version of Rax by running:
 
-`$ pip install rax`
+```
+$ pip install rax
+```
 
 ## Examples
 
 See the `examples/` directory for complete examples on how to use Rax.
 
 ## Citing Rax
```

### Comparing `rax-0.2.0/rax.egg-info/SOURCES.txt` & `rax-0.3.0/rax.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,38 @@
 examples/__init__.py
 examples/approx_metrics/__init__.py
 examples/approx_metrics/main.py
 examples/approx_metrics/main_test.py
 examples/flax_integration/__init__.py
 examples/flax_integration/main.py
 examples/flax_integration/main_test.py
+examples/segmentation/__init__.py
+examples/segmentation/main.py
+examples/segmentation/main_test.py
 examples/t5x/models.py
 examples/t5x/models_test.py
 examples/t5x/tasks.py
 examples/t5x/tasks_test.py
 rax/__init__.py
 rax/types.py
 rax/utils.py
 rax.egg-info/PKG-INFO
 rax.egg-info/SOURCES.txt
 rax.egg-info/dependency_links.txt
 rax.egg-info/requires.txt
 rax.egg-info/top_level.txt
 rax/_src/__init__.py
+rax/_src/lambdaweights.py
+rax/_src/lambdaweights_test.py
 rax/_src/losses.py
 rax/_src/losses_test.py
 rax/_src/metrics.py
 rax/_src/metrics_test.py
+rax/_src/segment_utils.py
+rax/_src/segment_utils_test.py
 rax/_src/t12n.py
 rax/_src/t12n_test.py
 rax/_src/types.py
 rax/_src/utils.py
 rax/_src/utils_test.py
 requirements/requirements-docs.txt
 requirements/requirements-examples.txt
```

### Comparing `rax-0.2.0/setup.py` & `rax-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Google LLC.
+# Copyright 2023 Google LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -44,30 +44,31 @@
 
 setup(
     name='rax',
     version=_get_version(),
     url='https://github.com/google/rax',
     license='Apache 2.0',
     author='Google',
-    description=('Composable Learning-to-Rank using JAX.'),
+    description='Learning-to-Rank using JAX.',
     long_description=open(os.path.join(_CURRENT_DIR, 'README.md')).read(),
     long_description_content_type='text/markdown',
     author_email='rax-dev@google.com',
     keywords='learning-to-rank jax ranking',
     packages=find_namespace_packages(exclude=['*_test.py']),
     install_requires=_parse_requirements(
-        os.path.join(_CURRENT_DIR, 'requirements', 'requirements.txt')),
+        os.path.join(_CURRENT_DIR, 'requirements', 'requirements.txt')
+    ),
     tests_require=_parse_requirements(
-        os.path.join(_CURRENT_DIR, 'requirements', 'requirements-test.txt')),
-    python_requires='>=3.7',
+        os.path.join(_CURRENT_DIR, 'requirements', 'requirements-test.txt')
+    ),
+    python_requires='>=3.8',
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 )
-
```

