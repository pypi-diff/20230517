# Comparing `tmp/bnlearn-0.7.9.tar.gz` & `tmp/bnlearn-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnlearn-0.7.9.tar", last modified: Wed Nov 30 18:21:03 2022, max compression
+gzip compressed data, was "bnlearn-0.8.0.tar", last modified: Wed May 17 11:02:38 2023, max compression
```

## Comparing `bnlearn-0.7.9.tar` & `bnlearn-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,37 @@
-drwxrwxrwx   0        0        0        0 2022-11-30 18:21:03.121947 bnlearn-0.7.9/
--rw-rw-rw-   0        0        0     1231 2022-05-09 18:05:29.000000 bnlearn-0.7.9/LICENSE
--rw-rw-rw-   0        0        0      643 2022-05-09 18:05:29.000000 bnlearn-0.7.9/MANIFEST.in
--rw-rw-rw-   0        0        0    11694 2022-11-30 18:21:03.121947 bnlearn-0.7.9/PKG-INFO
--rw-rw-rw-   0        0        0    11047 2022-11-11 13:31:48.000000 bnlearn-0.7.9/README.md
-drwxrwxrwx   0        0        0        0 2022-11-30 18:21:03.022614 bnlearn-0.7.9/bnlearn/
--rw-rw-rw-   0        0        0     4300 2022-11-30 18:17:50.000000 bnlearn-0.7.9/bnlearn/__init__.py
--rw-rw-rw-   0        0        0    68464 2022-11-30 18:10:56.000000 bnlearn-0.7.9/bnlearn/bnlearn.py
--rw-rw-rw-   0        0        0     1745 2022-05-09 18:05:29.000000 bnlearn-0.7.9/bnlearn/confmatrix.py
-drwxrwxrwx   0        0        0        0 2022-11-30 18:21:03.097673 bnlearn-0.7.9/bnlearn/data/
--rw-rw-rw-   0        0        0        0 2022-05-09 18:05:29.000000 bnlearn-0.7.9/bnlearn/data/__init__.py
--rw-rw-rw-   0        0        0    40174 2022-11-30 18:11:34.000000 bnlearn-0.7.9/bnlearn/examples.py
--rw-rw-rw-   0        0        0     3556 2022-08-05 17:21:16.000000 bnlearn-0.7.9/bnlearn/inference.py
--rw-rw-rw-   0        0        0    16904 2022-05-09 18:05:29.000000 bnlearn-0.7.9/bnlearn/network.py
--rw-rw-rw-   0        0        0     7294 2022-10-22 11:52:54.000000 bnlearn-0.7.9/bnlearn/parameter_learning.py
--rw-rw-rw-   0        0        0    25097 2022-10-22 11:38:13.000000 bnlearn-0.7.9/bnlearn/structure_learning.py
-drwxrwxrwx   0        0        0        0 2022-11-30 18:21:03.119898 bnlearn-0.7.9/bnlearn/tests/
--rw-rw-rw-   0        0        0        0 2022-11-30 17:18:09.000000 bnlearn-0.7.9/bnlearn/tests/__init__.py
--rw-rw-rw-   0        0        0    13205 2022-11-30 17:18:09.000000 bnlearn-0.7.9/bnlearn/tests/test_bnlearn.py
--rw-rw-rw-   0        0        0     8222 2022-11-30 17:18:09.000000 bnlearn-0.7.9/bnlearn/tests/test_structure_learning.py
-drwxrwxrwx   0        0        0        0 2022-11-30 18:21:03.082540 bnlearn-0.7.9/bnlearn.egg-info/
--rw-rw-rw-   0        0        0    11694 2022-11-30 18:21:02.000000 bnlearn-0.7.9/bnlearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      495 2022-11-30 18:21:02.000000 bnlearn-0.7.9/bnlearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-30 18:21:02.000000 bnlearn-0.7.9/bnlearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2022-11-30 18:21:02.000000 bnlearn-0.7.9/bnlearn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-11-30 18:21:02.000000 bnlearn-0.7.9/bnlearn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-30 18:21:03.122929 bnlearn-0.7.9/setup.cfg
--rw-rw-rw-   0        0        0     2080 2022-11-30 17:18:09.000000 bnlearn-0.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:02:38.010879 bnlearn-0.8.0/
+-rw-rw-rw-   0        0        0     1231 2022-05-09 18:05:29.000000 bnlearn-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0      643 2022-05-09 18:05:29.000000 bnlearn-0.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12268 2023-05-17 11:02:37.996634 bnlearn-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11621 2023-03-27 17:45:39.000000 bnlearn-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 11:02:37.870445 bnlearn-0.8.0/bnlearn/
+-rw-rw-rw-   0        0        0     4477 2023-05-17 11:01:32.000000 bnlearn-0.8.0/bnlearn/__init__.py
+-rw-rw-rw-   0        0        0    69616 2023-05-17 11:00:22.000000 bnlearn-0.8.0/bnlearn/bnlearn.py
+-rw-rw-rw-   0        0        0     1745 2022-05-09 18:05:29.000000 bnlearn-0.8.0/bnlearn/confmatrix.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:02:37.928915 bnlearn-0.8.0/bnlearn/data/
+-rw-rw-rw-   0        0        0        0 2022-05-09 18:05:29.000000 bnlearn-0.8.0/bnlearn/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:02:37.948190 bnlearn-0.8.0/bnlearn/discretize/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:59:05.000000 bnlearn-0.8.0/bnlearn/discretize/__init__.py
+-rw-rw-rw-   0        0        0     3410 2023-05-16 18:28:43.000000 bnlearn-0.8.0/bnlearn/discretize/discretize.py
+-rw-rw-rw-   0        0        0    19168 2023-05-16 18:32:33.000000 bnlearn-0.8.0/bnlearn/discretize/learn_discrete_bayes_net.py
+-rw-rw-rw-   0        0        0    45280 2023-05-16 21:41:39.000000 bnlearn-0.8.0/bnlearn/examples.py
+-rw-rw-rw-   0        0        0     1330 2023-05-12 07:28:50.000000 bnlearn-0.8.0/bnlearn/examples_discretize.py
+-rw-rw-rw-   0        0        0     3555 2023-04-01 15:11:24.000000 bnlearn-0.8.0/bnlearn/inference.py
+-rw-rw-rw-   0        0        0    16904 2023-04-01 12:44:53.000000 bnlearn-0.8.0/bnlearn/network.py
+-rw-rw-rw-   0        0        0     7419 2023-04-29 10:55:11.000000 bnlearn-0.8.0/bnlearn/parameter_learning.py
+-rw-rw-rw-   0        0        0    25079 2023-05-09 15:43:00.000000 bnlearn-0.8.0/bnlearn/structure_learning.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:02:37.953589 bnlearn-0.8.0/bnlearn/tests/
+-rw-rw-rw-   0        0        0        0 2022-11-30 17:18:09.000000 bnlearn-0.8.0/bnlearn/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:02:37.995637 bnlearn-0.8.0/bnlearn/tests/discretize/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:59:05.000000 bnlearn-0.8.0/bnlearn/tests/discretize/__init__.py
+-rw-rw-rw-   0        0        0     2293 2023-04-29 10:59:05.000000 bnlearn-0.8.0/bnlearn/tests/discretize/test_discretize.py
+-rw-rw-rw-   0        0        0     9366 2023-05-12 07:28:13.000000 bnlearn-0.8.0/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py
+-rw-rw-rw-   0        0        0    13506 2023-05-14 19:03:35.000000 bnlearn-0.8.0/bnlearn/tests/test_bnlearn.py
+-rw-rw-rw-   0        0        0     8222 2022-11-30 17:18:09.000000 bnlearn-0.8.0/bnlearn/tests/test_structure_learning.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:02:37.926635 bnlearn-0.8.0/bnlearn.egg-info/
+-rw-rw-rw-   0        0        0    12268 2023-05-17 11:02:37.000000 bnlearn-0.8.0/bnlearn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2023-05-17 11:02:37.000000 bnlearn-0.8.0/bnlearn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 11:02:37.000000 bnlearn-0.8.0/bnlearn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      204 2023-05-17 11:02:37.000000 bnlearn-0.8.0/bnlearn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 11:02:37.000000 bnlearn-0.8.0/bnlearn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 11:02:38.011879 bnlearn-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     2071 2023-05-16 15:14:21.000000 bnlearn-0.8.0/setup.py
```

### Comparing `bnlearn-0.7.9/LICENSE` & `bnlearn-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bnlearn-0.7.9/MANIFEST.in` & `bnlearn-0.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bnlearn-0.7.9/PKG-INFO` & `bnlearn-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,80 +1,97 @@
 Metadata-Version: 2.1
 Name: bnlearn
-Version: 0.7.9
+Version: 0.8.0
 Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
 Home-page: https://erdogant.github.io/bnlearn
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.7.9.tar.gz
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.0.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
+![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
 [![Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/issues)
 [![Project Status](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://pepy.tech/project/bnlearn/)
 [![Downloads](https://pepy.tech/badge/bnlearn)](https://pepy.tech/project/bnlearn)
 [![DOI](https://zenodo.org/badge/231263493.svg)](https://zenodo.org/badge/latestdoi/231263493)
 [![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
-[![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
+[![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
+![GitHub repo size](https://img.shields.io/github/repo-size/erdogant/bnlearn)
 [![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#colab-notebook)
 <!---[![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)-->
 <!---[![Coffee](https://img.shields.io/badge/coffee-black-grey.svg)](https://erdogant.github.io/donate/?currency=USD&amount=5)-->
 
 
 ### 
 
-``bnlearn`` is Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods. This work is inspired by the R package (bnlearn.com) that has been very usefull to me for many years. Although there are very good Python packages for probabilistic graphical models, it still can remain difficult (and somethimes unnecessarily) to (re)build certain pipelines. Bnlearn for python (this package) is build on the <a href="https://github.com/pgmpy/pgmpy">pgmpy</a> package and contains the most-wanted pipelines. Navigate to [API documentations](https://erdogant.github.io/bnlearn/) for more detailed information.
+``bnlearn`` is Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
+Because probabilistic graphical models can be difficult in usage, Bnlearn for python (this package) is build on the <a href="https://github.com/pgmpy/pgmpy">pgmpy</a> package and contains the most-wanted pipelines. Navigate to [API documentations](https://erdogant.github.io/bnlearn/) for more detailed information.
 
 # 
 **⭐️ Star this repo if you like it ⭐️**
 # 
 
-### Blogs
+### Read the Medium blog for more details.
 
-Read the blogs to get a structured overview of bayesian methods and detailed usage of ``bnlearn``.
+<p align="left">
+  <a href="https://towardsdatascience.com/a-step-by-step-guide-in-detecting-causal-relationships-using-bayesian-structure-learning-in-python-c20c6b31cee5" target="_blank">
+    <img src="https://github.com/erdogant/bnlearn/blob/master/docs/figs/medium_blog2.png?raw=true" width="150" />
+  </a>
+
+  <a href="https://towardsdatascience.com/a-step-by-step-guide-in-designing-knowledge-driven-models-using-bayesian-theorem-7433f6fd64be" target="_blank">
+  <img src="https://github.com/erdogant/bnlearn/blob/master/docs/figs/medium_blog1.png?raw=true" width="150" />
+  </a>
 
-* [Step-by-step guide for structure learning.](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
-* [Step-by-step guide for knowledge-driven models.](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
+</p>
+
+
+---
 
 # 
 
 
 ### [Documentation pages](https://erdogant.github.io/bnlearn/)
 
 On the [documentation pages](https://erdogant.github.io/bnlearn/) you can find detailed information about the working of the ``bnlearn`` with many examples. 
 
 # 
 
 ### Installation
 
 ##### It is advisable to create a new environment (e.g. with Conda). 
 ```bash
-conda create -n env_bnlearn python=3.8
+conda create -n env_bnlearn python=3.10
 conda activate env_bnlearn
 ```
 
 ##### Install bnlearn from PyPI
 ```bash
 pip install bnlearn
 ```
 
+##### Install bnlearn from github source
+```bash
+pip install git+https://github.com/erdogant/bnlearn
+```
+
 ##### The following functions are available after installation:
 
 ```python
 # Import library
 import bnlearn as bn
 
 # Structure learning
@@ -290,16 +307,24 @@
 
 ### References
 * https://erdogant.github.io/bnlearn/
 * http://pgmpy.org
 * https://programtalk.com/python-examples/pgmpy.factors.discrete.TabularCPD/
 * http://www.bnlearn.com/bnrepository/
 
-### Contribute
-* All kinds of contributions are welcome!
+
+### Contributors
+Setting up and maintaining bnlearn has been possible thanks to users and contributors. Thanks to:
+
+<p align="left">
+  <a href="https://github.com/erdogant/bnlearn/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=erdogant/bnlearn" />
+  </a>
+</p>
+
 
 ### Citation
 Please cite ``bnlearn`` in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
```

#### html2text {}

```diff
@@ -1,60 +1,60 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.7.9 Summary: Python package for
+Metadata-Version: 2.1 Name: bnlearn Version: 0.8.0 Summary: Python package for
 learning the graphical structure of Bayesian networks, parameter learning,
 inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
 Author: Erdogan Taskesen Author-email: erdogant@gmail.com License: UNKNOWN
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.7.9.tar.gz
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.0.tar.gz
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE # bnlearn - Library for Bayesian network learning and
 inference [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://
 img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version](https://
-img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) [![License]
+img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) ![GitHub
+Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn) [![License]
 (https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/
 erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/
 forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [!
 [Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)]
 (https://github.com/erdogant/bnlearn/issues) [![Project Status](http://
 www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
 #active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
 pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
 (https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
 231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
 img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
-[![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://
-erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) [!
-[Donate](https://img.shields.io/badge/Support%20this%20project-
+[![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
+erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) ![GitHub
+repo size](https://img.shields.io/github/repo-size/erdogant/bnlearn) [![Donate]
+(https://img.shields.io/badge/Support%20this%20project-
 grey.svg?logo=github%20sponsors)](https://erdogant.github.io/bnlearn/pages/
 html/Documentation.html#) [![Colab](https://colab.research.google.com/assets/
 colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/
 Documentation.html#colab-notebook)   ### ``bnlearn`` is Python package for
 learning the graphical structure of Bayesian networks, parameter learning,
-inference and sampling methods. This work is inspired by the R package
-(bnlearn.com) that has been very usefull to me for many years. Although there
-are very good Python packages for probabilistic graphical models, it still can
-remain difficult (and somethimes unnecessarily) to (re)build certain pipelines.
-Bnlearn for python (this package) is build on the pgmpy package and contains
-the most-wanted pipelines. Navigate to [API documentations](https://
-erdogant.github.io/bnlearn/) for more detailed information. # **â­ï¸ Star
-this repo if you like it â­ï¸** # ### Blogs Read the blogs to get a
-structured overview of bayesian methods and detailed usage of ``bnlearn``. *
-[Step-by-step guide for structure learning.](https://erdogant.github.io/
-bnlearn/pages/html/Documentation.html#medium-blog) * [Step-by-step guide for
-knowledge-driven models.](https://erdogant.github.io/bnlearn/pages/html/
-Documentation.html#medium-blog) # ### [Documentation pages](https://
-erdogant.github.io/bnlearn/) On the [documentation pages](https://
-erdogant.github.io/bnlearn/) you can find detailed information about the
-working of the ``bnlearn`` with many examples. # ### Installation ##### It is
-advisable to create a new environment (e.g. with Conda). ```bash conda create -
-n env_bnlearn python=3.8 conda activate env_bnlearn ``` ##### Install bnlearn
-from PyPI ```bash pip install bnlearn ``` ##### The following functions are
-available after installation: ```python # Import library import bnlearn as bn #
-Structure learning bn.structure_learning.fit() # Compute edge strength with the
-test statistic bn.independence_test(model, df, test='chi_square', prune=True) #
+inference and sampling methods. Because probabilistic graphical models can be
+difficult in usage, Bnlearn for python (this package) is build on the pgmpy
+package and contains the most-wanted pipelines. Navigate to [API
+documentations](https://erdogant.github.io/bnlearn/) for more detailed
+information. # **â­ï¸ Star this repo if you like it â­ï¸** # ### Read the
+Medium blog for more details.
+[https://github.com/erdogant/bnlearn/blob/master/docs/figs/
+medium_blog2.png?raw=true] [https://github.com/erdogant/bnlearn/blob/master/
+docs/figs/medium_blog1.png?raw=true]
+--- # ### [Documentation pages](https://erdogant.github.io/bnlearn/) On the
+[documentation pages](https://erdogant.github.io/bnlearn/) you can find
+detailed information about the working of the ``bnlearn`` with many examples. #
+### Installation ##### It is advisable to create a new environment (e.g. with
+Conda). ```bash conda create -n env_bnlearn python=3.10 conda activate
+env_bnlearn ``` ##### Install bnlearn from PyPI ```bash pip install bnlearn ```
+##### Install bnlearn from github source ```bash pip install git+https://
+github.com/erdogant/bnlearn ``` ##### The following functions are available
+after installation: ```python # Import library import bnlearn as bn # Structure
+learning bn.structure_learning.fit() # Compute edge strength with the test
+statistic bn.independence_test(model, df, test='chi_square', prune=True) #
 Parameter learning bn.parameter_learning.fit() # Inference bn.inference.fit() #
 Make predictions bn.predict() # Based on a DAG, you can sample the number of
 samples you want. bn.sampling() # Load well known examples to play arround with
 or load your own .bif file. bn.import_DAG() # Load simple dataframe of
 sprinkler dataset. bn.import_example() # Compare 2 graphs bn.compare_networks()
 # Plot graph bn.plot() # To make the directed grapyh undirected
 bn.to_undirected() # Convert to one-hot datamatrix bn.df2onehot() # Derive the
@@ -129,13 +129,16 @@
 ('sprinkler') query = bn.inference.fit(model, variables=['Rain'], evidence=
 {'Cloudy':1,'Sprinkler':0, 'Wet_Grass':1}) print(query) print(query.df) # Lets
 try another inference query = bn.inference.fit(model, variables=['Rain'],
 evidence={'Cloudy':1}) print(query) print(query.df) ```
 ===============================================================================
 ### References * https://erdogant.github.io/bnlearn/ * http://pgmpy.org *
 https://programtalk.com/python-examples/pgmpy.factors.discrete.TabularCPD/ *
-http://www.bnlearn.com/bnrepository/ ### Contribute * All kinds of
-contributions are welcome! ### Citation Please cite ``bnlearn`` in your
-publications if this is useful for your research. See column right for citation
-information. ### Maintainer * Erdogan Taskesen, github: [erdogant](https://
-github.com/erdogant) * Contributions are welcome. * If you wish to buy me a
-Coffee for this work, it is very appreciated :)
+http://www.bnlearn.com/bnrepository/ ### Contributors Setting up and
+maintaining bnlearn has been possible thanks to users and contributors. Thanks
+to:
+[https://contrib.rocks/image?repo=erdogant/bnlearn]
+### Citation Please cite ``bnlearn`` in your publications if this is useful for
+your research. See column right for citation information. ### Maintainer *
+Erdogan Taskesen, github: [erdogant](https://github.com/erdogant) *
+Contributions are welcome. * If you wish to buy me a Coffee for this work, it
+is very appreciated :)
```

### Comparing `bnlearn-0.7.9/README.md` & `bnlearn-0.8.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,80 @@
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
+![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
 [![Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/issues)
 [![Project Status](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://pepy.tech/project/bnlearn/)
 [![Downloads](https://pepy.tech/badge/bnlearn)](https://pepy.tech/project/bnlearn)
 [![DOI](https://zenodo.org/badge/231263493.svg)](https://zenodo.org/badge/latestdoi/231263493)
 [![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
-[![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
+[![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
+![GitHub repo size](https://img.shields.io/github/repo-size/erdogant/bnlearn)
 [![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#colab-notebook)
 <!---[![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)-->
 <!---[![Coffee](https://img.shields.io/badge/coffee-black-grey.svg)](https://erdogant.github.io/donate/?currency=USD&amount=5)-->
 
 
 ### 
 
-``bnlearn`` is Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods. This work is inspired by the R package (bnlearn.com) that has been very usefull to me for many years. Although there are very good Python packages for probabilistic graphical models, it still can remain difficult (and somethimes unnecessarily) to (re)build certain pipelines. Bnlearn for python (this package) is build on the <a href="https://github.com/pgmpy/pgmpy">pgmpy</a> package and contains the most-wanted pipelines. Navigate to [API documentations](https://erdogant.github.io/bnlearn/) for more detailed information.
+``bnlearn`` is Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
+Because probabilistic graphical models can be difficult in usage, Bnlearn for python (this package) is build on the <a href="https://github.com/pgmpy/pgmpy">pgmpy</a> package and contains the most-wanted pipelines. Navigate to [API documentations](https://erdogant.github.io/bnlearn/) for more detailed information.
 
 # 
 **⭐️ Star this repo if you like it ⭐️**
 # 
 
-### Blogs
+### Read the Medium blog for more details.
 
-Read the blogs to get a structured overview of bayesian methods and detailed usage of ``bnlearn``.
+<p align="left">
+  <a href="https://towardsdatascience.com/a-step-by-step-guide-in-detecting-causal-relationships-using-bayesian-structure-learning-in-python-c20c6b31cee5" target="_blank">
+    <img src="https://github.com/erdogant/bnlearn/blob/master/docs/figs/medium_blog2.png?raw=true" width="150" />
+  </a>
+
+  <a href="https://towardsdatascience.com/a-step-by-step-guide-in-designing-knowledge-driven-models-using-bayesian-theorem-7433f6fd64be" target="_blank">
+  <img src="https://github.com/erdogant/bnlearn/blob/master/docs/figs/medium_blog1.png?raw=true" width="150" />
+  </a>
 
-* [Step-by-step guide for structure learning.](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
-* [Step-by-step guide for knowledge-driven models.](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
+</p>
+
+
+---
 
 # 
 
 
 ### [Documentation pages](https://erdogant.github.io/bnlearn/)
 
 On the [documentation pages](https://erdogant.github.io/bnlearn/) you can find detailed information about the working of the ``bnlearn`` with many examples. 
 
 # 
 
 ### Installation
 
 ##### It is advisable to create a new environment (e.g. with Conda). 
 ```bash
-conda create -n env_bnlearn python=3.8
+conda create -n env_bnlearn python=3.10
 conda activate env_bnlearn
 ```
 
 ##### Install bnlearn from PyPI
 ```bash
 pip install bnlearn
 ```
 
+##### Install bnlearn from github source
+```bash
+pip install git+https://github.com/erdogant/bnlearn
+```
+
 ##### The following functions are available after installation:
 
 ```python
 # Import library
 import bnlearn as bn
 
 # Structure learning
@@ -273,16 +290,24 @@
 
 ### References
 * https://erdogant.github.io/bnlearn/
 * http://pgmpy.org
 * https://programtalk.com/python-examples/pgmpy.factors.discrete.TabularCPD/
 * http://www.bnlearn.com/bnrepository/
 
-### Contribute
-* All kinds of contributions are welcome!
+
+### Contributors
+Setting up and maintaining bnlearn has been possible thanks to users and contributors. Thanks to:
+
+<p align="left">
+  <a href="https://github.com/erdogant/bnlearn/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=erdogant/bnlearn" />
+  </a>
+</p>
+
 
 ### Citation
 Please cite ``bnlearn`` in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
```

#### html2text {}

```diff
@@ -1,51 +1,52 @@
 # bnlearn - Library for Bayesian network learning and inference [![Python]
 (https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
 pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
-(https://pypi.org/project/bnlearn/) [![License](https://img.shields.io/badge/
-license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/
-LICENSE) [![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)]
-(https://github.com/erdogant/bnlearn/network) [![Open Issues](https://
-img.shields.io/github/issues/erdogant/bnlearn.svg)](https://github.com/
-erdogant/bnlearn/issues) [![Project Status](http://www.repostatus.org/badges/
-latest/active.svg)](http://www.repostatus.org/#active) [![Downloads](https://
-pepy.tech/badge/bnlearn/month)](https://pepy.tech/project/bnlearn/) [!
-[Downloads](https://pepy.tech/badge/bnlearn)](https://pepy.tech/project/
-bnlearn) [![DOI](https://zenodo.org/badge/231263493.svg)](https://zenodo.org/
-badge/latestdoi/231263493) [![Docs](https://img.shields.io/badge/Sphinx-Docs-
-Green)](https://erdogant.github.io/bnlearn/) [![Medium](https://img.shields.io/
-badge/Medium-Blog-green)](https://erdogant.github.io/bnlearn/pages/html/
-Documentation.html#medium-blog) [![Donate](https://img.shields.io/badge/
-Support%20this%20project-grey.svg?logo=github%20sponsors)](https://
-erdogant.github.io/bnlearn/pages/html/Documentation.html#) [![Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/
-bnlearn/pages/html/Documentation.html#colab-notebook)   ### ``bnlearn`` is
-Python package for learning the graphical structure of Bayesian networks,
-parameter learning, inference and sampling methods. This work is inspired by
-the R package (bnlearn.com) that has been very usefull to me for many years.
-Although there are very good Python packages for probabilistic graphical
-models, it still can remain difficult (and somethimes unnecessarily) to
-(re)build certain pipelines. Bnlearn for python (this package) is build on the
-pgmpy package and contains the most-wanted pipelines. Navigate to [API
+(https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
+img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
+img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
+bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
+erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
+Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
+github.com/erdogant/bnlearn/issues) [![Project Status](http://
+www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
+#active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
+pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
+(https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
+231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
+img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
+[![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
+erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) ![GitHub
+repo size](https://img.shields.io/github/repo-size/erdogant/bnlearn) [![Donate]
+(https://img.shields.io/badge/Support%20this%20project-
+grey.svg?logo=github%20sponsors)](https://erdogant.github.io/bnlearn/pages/
+html/Documentation.html#) [![Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/
+Documentation.html#colab-notebook)   ### ``bnlearn`` is Python package for
+learning the graphical structure of Bayesian networks, parameter learning,
+inference and sampling methods. Because probabilistic graphical models can be
+difficult in usage, Bnlearn for python (this package) is build on the pgmpy
+package and contains the most-wanted pipelines. Navigate to [API
 documentations](https://erdogant.github.io/bnlearn/) for more detailed
-information. # **â­ï¸ Star this repo if you like it â­ï¸** # ### Blogs Read
-the blogs to get a structured overview of bayesian methods and detailed usage
-of ``bnlearn``. * [Step-by-step guide for structure learning.](https://
-erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) * [Step-
-by-step guide for knowledge-driven models.](https://erdogant.github.io/bnlearn/
-pages/html/Documentation.html#medium-blog) # ### [Documentation pages](https://
-erdogant.github.io/bnlearn/) On the [documentation pages](https://
-erdogant.github.io/bnlearn/) you can find detailed information about the
-working of the ``bnlearn`` with many examples. # ### Installation ##### It is
-advisable to create a new environment (e.g. with Conda). ```bash conda create -
-n env_bnlearn python=3.8 conda activate env_bnlearn ``` ##### Install bnlearn
-from PyPI ```bash pip install bnlearn ``` ##### The following functions are
-available after installation: ```python # Import library import bnlearn as bn #
-Structure learning bn.structure_learning.fit() # Compute edge strength with the
-test statistic bn.independence_test(model, df, test='chi_square', prune=True) #
+information. # **â­ï¸ Star this repo if you like it â­ï¸** # ### Read the
+Medium blog for more details.
+[https://github.com/erdogant/bnlearn/blob/master/docs/figs/
+medium_blog2.png?raw=true] [https://github.com/erdogant/bnlearn/blob/master/
+docs/figs/medium_blog1.png?raw=true]
+--- # ### [Documentation pages](https://erdogant.github.io/bnlearn/) On the
+[documentation pages](https://erdogant.github.io/bnlearn/) you can find
+detailed information about the working of the ``bnlearn`` with many examples. #
+### Installation ##### It is advisable to create a new environment (e.g. with
+Conda). ```bash conda create -n env_bnlearn python=3.10 conda activate
+env_bnlearn ``` ##### Install bnlearn from PyPI ```bash pip install bnlearn ```
+##### Install bnlearn from github source ```bash pip install git+https://
+github.com/erdogant/bnlearn ``` ##### The following functions are available
+after installation: ```python # Import library import bnlearn as bn # Structure
+learning bn.structure_learning.fit() # Compute edge strength with the test
+statistic bn.independence_test(model, df, test='chi_square', prune=True) #
 Parameter learning bn.parameter_learning.fit() # Inference bn.inference.fit() #
 Make predictions bn.predict() # Based on a DAG, you can sample the number of
 samples you want. bn.sampling() # Load well known examples to play arround with
 or load your own .bif file. bn.import_DAG() # Load simple dataframe of
 sprinkler dataset. bn.import_example() # Compare 2 graphs bn.compare_networks()
 # Plot graph bn.plot() # To make the directed grapyh undirected
 bn.to_undirected() # Convert to one-hot datamatrix bn.df2onehot() # Derive the
@@ -120,13 +121,16 @@
 ('sprinkler') query = bn.inference.fit(model, variables=['Rain'], evidence=
 {'Cloudy':1,'Sprinkler':0, 'Wet_Grass':1}) print(query) print(query.df) # Lets
 try another inference query = bn.inference.fit(model, variables=['Rain'],
 evidence={'Cloudy':1}) print(query) print(query.df) ```
 ===============================================================================
 ### References * https://erdogant.github.io/bnlearn/ * http://pgmpy.org *
 https://programtalk.com/python-examples/pgmpy.factors.discrete.TabularCPD/ *
-http://www.bnlearn.com/bnrepository/ ### Contribute * All kinds of
-contributions are welcome! ### Citation Please cite ``bnlearn`` in your
-publications if this is useful for your research. See column right for citation
-information. ### Maintainer * Erdogan Taskesen, github: [erdogant](https://
-github.com/erdogant) * Contributions are welcome. * If you wish to buy me a
-Coffee for this work, it is very appreciated :)
+http://www.bnlearn.com/bnrepository/ ### Contributors Setting up and
+maintaining bnlearn has been possible thanks to users and contributors. Thanks
+to:
+[https://contrib.rocks/image?repo=erdogant/bnlearn]
+### Citation Please cite ``bnlearn`` in your publications if this is useful for
+your research. See column right for citation information. ### Maintainer *
+Erdogan Taskesen, github: [erdogant](https://github.com/erdogant) *
+Contributions are welcome. * If you wish to buy me a Coffee for this work, it
+is very appreciated :)
```

### Comparing `bnlearn-0.7.9/bnlearn/__init__.py` & `bnlearn-0.8.0/bnlearn/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,56 +29,59 @@
 
 # Import function in new level
 import bnlearn.structure_learning as structure_learning
 import bnlearn.parameter_learning as parameter_learning
 import bnlearn.inference as inference
 import bnlearn.network as network
 import bnlearn.confmatrix as confmatrix
+from bnlearn.discretize.discretize import discretize, discretize_value
 from packaging import version
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.7.9'
-
-try:
-    import pgmpy
-except:
-    raise ImportError('[bnlearn] >Error: pgmpy version "0.1.13" or higher must be installed manually. Try to: <conda install -c ankurankan pgmpy> or <pip install -U pgmpy>=0.1.13>')
+__version__ = '0.8.0'
 
+import pgmpy
 # Check version pgmpy
-if version.parse(pgmpy.__version__) < version.parse("0.1.13"):
-    raise ImportError('[bnlearn] >Error: This release requires pgmpy to be version >= 0.1.13. Try to: <conda install -c ankurankan pgmpy> or <pip install -U pgmpy>=0.1.13>')
+if version.parse(pgmpy.__version__) < version.parse("0.1.18"):
+    raise ImportError('[bnlearn] >Error: This release requires pgmpy to be version >= 0.1.18. Try to: <pip install -U pgmpy>=0.1.18>')
 
 # Version check
 import matplotlib
 if not version.parse(matplotlib.__version__) >= version.parse("3.3.4"):
     raise ImportError('[bnlearn] >Error: Matplotlib version should be >= v3.3.4.\nTry to: pip install -U matplotlib')
 
 import networkx as nx
 if not version.parse(nx.__version__) >= version.parse("2.7.1"):
     raise ImportError('[bnlearn] >Error: networkx version should be > 2.7.1.\nTry to: pip install -U networkx')
 
+import numpy as np
+if not version.parse(np.__version__) >= version.parse("1.24.1"):
+    raise ImportError('[bnlearn] >Error: numpy version should be > 1.24.1.\nTry to: pip install -U numpy')
+
+import pandas as pd
+if not version.parse(pd.__version__) <= version.parse("1.5.3"):
+    raise ImportError('[bnlearn] >Error: pands version should be <= 1.5.3.')
 
 # module level doc-string
 __doc__ = """
-BNLEARN - bnlearn is an Python package for learning the graphical structure of Bayesian networks, estimate their parameters, perform inference, sampling and comparing networks.
+bnlearn - bnlearn is an Python package for learning the graphical structure of Bayesian networks, estimate their parameters, perform inference, sampling and comparing networks.
 ================================================================================================================================================================================
 
 Description
 -----------
-* Learning a Bayesian network can be split into two problems:
+* Learning a Bayesian network can be split into:
     * Structure learning: Given a set of data samples, estimate a DAG that captures the dependencies between the variables.
     * Parameter learning: Given a set of data samples and a DAG that captures the dependencies between the variables.
     * Making inferences.
     * Parameter and structure learning is for *discrete* nodes
         * Score-based structure estimation (BIC/BDeu/K2 score; exhaustive search, hill climb/tabu search)
         * Constraint-based structure estimation (PC)
         * Hybrid structure estimation (MMHC)
 
-
 Example
 -------
 >>> # Import library
 >>> import bnlearn as bn
 >>> model = bn.import_DAG('sprinkler')
 >>> # Print CPDs
 >>> bn.print_CPD(model)
@@ -107,13 +110,13 @@
 >>> bn.plot(model_pl)
 >>>
 >>> # Compare networks
 >>> scores, adjmat = bn.compare_networks(model_sl, model)
 
 References
 ----------
-* Blog1: https://towardsdatascience.com/a-step-by-step-guide-in-detecting-causal-relationships-using-bayesian-structure-learning-in-python-c20c6b31cee5
-* Blog2: https://towardsdatascience.com/a-step-by-step-guide-in-designing-knowledge-driven-models-using-bayesian-theorem-7433f6fd64be
+* Blog: https://towardsdatascience.com/a-step-by-step-guide-in-detecting-causal-relationships-using-bayesian-structure-learning-in-python-c20c6b31cee5
+* Blog: https://towardsdatascience.com/a-step-by-step-guide-in-designing-knowledge-driven-models-using-bayesian-theorem-7433f6fd64be
 * Github: https://github.com/erdogant/bnlearn
-* Documentation: https://bnlearn.readthedocs.io
+* Documentation: https://erdogant.github.io/bnlearn/
 
 """
```

### Comparing `bnlearn-0.7.9/bnlearn/bnlearn.py` & `bnlearn-0.8.0/bnlearn/bnlearn.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,43 +6,50 @@
 # Licence     : See LICENSE
 # ------------------------------------
 
 
 # %% Libraries
 import os
 import copy
-import wget
-import zipfile
 import itertools
 import pandas as pd
 import numpy as np
 import networkx as nx
 import matplotlib.pyplot as plt
+# import logging
+
 from pathlib import Path
 from tqdm import tqdm
 from tabulate import tabulate
 from decimal import Decimal
 
 from pgmpy.models import BayesianNetwork, NaiveBayes
 from pgmpy.factors.discrete import TabularCPD
 from pgmpy.sampling import BayesianModelSampling, GibbsSampling
-from pgmpy import readwrite
 from pgmpy.metrics import structure_score
 
 from ismember import ismember
+import datazets as dz
 import pypickle
 import bnlearn
 
+# logger = logging.getLogger('')
+# for handler in logger.handlers[:]: #get rid of existing old handlers
+#     logger.removeHandler(handler)
+# console = logging.StreamHandler()
+# formatter = logging.Formatter('[bnlearn] >%(levelname)s> %(message)s')
+# console.setFormatter(formatter)
+# logger.addHandler(console)
+# logger = logging.getLogger(__name__)
+
 
 # %%  Convert adjmat to bayesian model
 def to_bayesiannetwork(model, verbose=3):
     """Convert adjacency matrix to BayesianNetwork.
 
-    Description
-    -----------
     Convert a adjacency to a Bayesian model. This is required as some of the
     functionalities, such as ``structure_learning`` output a DAGmodel.
     If the output of ``structure_learning`` is provided, the adjmat is extracted and processed.
 
     Parameters
     ----------
     model : pd.DataFrame()
@@ -121,15 +128,15 @@
 
     if (not isinstance(DAG, list)) and ('pgmpy' not in str(type(DAG))):
         raise Exception("[bnlearn] >Error: Input DAG should be a list. in the form [('A','B'), ('B','C')] or a <pgmpy.models.BayesianNetwork>")
     elif ('pgmpy' in str(type(DAG))):
         # Extract methodtype from existing model.
         if ('bayesianmodel' in str(type(DAG)).lower()):
             methodtype='bayes'
-        elif('naivebayes' in str(type(DAG)).lower()):
+        elif ('naivebayes' in str(type(DAG)).lower()):
             methodtype='naivebayes'
         if verbose>=3: print('[bnlearn] >No changes made to existing %s DAG.' %(methodtype))
     elif isinstance(DAG, list) and methodtype=='naivebayes':
         if verbose>=3: print('[bnlearn] >%s DAG created.' %(methodtype))
         edges=DAG
         DAG = NaiveBayes()
         DAG.add_edges_from(edges)
@@ -310,15 +317,15 @@
         # Run over the edges
         for edge in edges:
             adjmat.loc[edge[0], edge[1]]=True
         adjmat.index.name='source'
         adjmat.columns.name='target'
     else:
         if verbose>=1: print('[bnlearn] >Could not convert to adjmat because nodes and/or edges were missing.')
-    return(adjmat)
+    return adjmat
 
 
 # %%  Convert vector into sparse dataframe
 def vec2df(source, target, weights=None):
     """Convert source-target edges into sparse dataframe.
 
     Description
@@ -430,15 +437,15 @@
 
         # Sort to make ordering of columns and rows similar
         [IA, IB] = ismember(adjmat.columns.values, adjmat.index.values)
         adjmat = adjmat.iloc[IB, :]
         adjmat.index.name='source'
         adjmat.columns.name='target'
 
-    return(adjmat)
+    return adjmat
 
 
 # %%  Convert adjacency matrix to vector
 def adjmat2vec(adjmat, min_weight=1):
     """Convert adjacency matrix into vector with source and target.
 
     Parameters
@@ -470,15 +477,15 @@
     # Remove self loops and no-connected edges
     Iloc1 = adjmat['source']!=adjmat['target']
     Iloc2 = adjmat['weight']>=min_weight
     Iloc = Iloc1 & Iloc2
     # Take only connected nodes
     adjmat = adjmat.loc[Iloc, :]
     adjmat.reset_index(drop=True, inplace=True)
-    return(adjmat)
+    return adjmat
 
 
 # %%
 def adjmat2dict(adjmat):
     """Convert adjacency matrix to dict.
 
     Parameters
@@ -566,31 +573,32 @@
     elif methodtype=='gibbs':
         if verbose>=3: print('[bnlearn] >Gibbs sampling for %.0d samples..' %(n))
         # Gibbs sampling
         gibbs = GibbsSampling(DAG['model'])
         df = gibbs.sample(size=n, seed=None)
     else:
         if verbose>=3: print('[bnlearn] >Methodtype [%s] unknown' %(methodtype))
-    return(df)
+    return df
 
 
 # %% Convert BIF model to bayesian model
 def _bif2bayesian(pathname, verbose=3):
     """Return the fitted bayesian model.
 
     Example
     -------
     >>> from pgmpy.readwrite import BIFReader
     >>> reader = BIFReader("bif_test.bif")
     >>> reader.get_model()
     <pgmpy.models.BayesianNetwork object at 0x7f20af154320>
     """
+    from pgmpy.readwrite import BIFReader
     if verbose>=3: print('[bnlearn] >Loading bif file <%s>' %(pathname))
 
-    bifmodel=readwrite.BIF.BIFReader(path=pathname)
+    bifmodel = BIFReader(path=pathname)
 
     try:
         model = BayesianNetwork(bifmodel.variable_edges)
         model.name = bifmodel.network_name
         model.add_nodes_from(bifmodel.variable_names)
 
         tabular_cpds = []
@@ -610,41 +618,14 @@
 
         return model
 
     except AttributeError:
         raise AttributeError('[bnlearn] >First get states of variables, edges, parents and network names')
 
 
-# %%
-# def query2df(query, variables=None):
-#     """Convert query from inference model to a dataframe.
-
-#     Parameters
-#     ----------
-#     query : Object from the inference model.
-#         Convert query object to a dataframe.
-#     variables : list
-#         Order or select variables.
-
-#     Returns
-#     -------
-#     df : pd.DataFrame()
-#         Dataframe with inferences.
-
-#     """
-#     df = pd.DataFrame(data=list(itertools.product(np.arange(0, len(query.values)), repeat=len(query.variables))), columns=query.variables)
-#     df['p'] = query.values.flatten()
-#     # Order or filter on input variables
-#     if variables is not None:
-#         # Add Pvalue column
-#         variables = variables + ['p']
-#         df = df[variables]
-#     return df
-
-
 def query2df(query, variables=None, verbose=3):
     """Convert query from inference model to a dataframe.
 
     Parameters
     ----------
     query : Object from the inference model.
         Convert query object to a dataframe.
@@ -661,14 +642,19 @@
     getP = []
     for value_index, prob in enumerate(itertools.product(*[range(card) for card in query.cardinality])):
         states.append(prob)
         getP.append(query.values.ravel()[value_index])
 
     df = pd.DataFrame(data=states, columns=query.scope())
     df['p'] = getP
+
+    # Convert the numbers into variable names
+    for col in query.scope():
+        df[col] = np.array(query.state_names[col])[df[col].values.astype(int)]
+
     # Order or filter on input variables
     if variables is not None:
         # Add Pvalue column
         variables = variables + ['p']
         df = df[variables]
 
     # Print table to screen
@@ -805,22 +791,22 @@
     --------
     >>> import bnlearn as bn
     >>> edges = [('A', 'B'), ('A', 'C'), ('A', 'D')]
     >>> # Create DAG and store in model
     >>> model = bn.make_DAG(edges)
     >>> node_properties = bn.get_node_properties(model)
     >>> # Adjust the properties
-    >>> node_properties['A']['node_size']=2000
+    >>> node_properties['A']['node_size']=100
     >>> node_properties['A']['node_color']='#000000'
     >>> # Make plot
     >>> fig = bn.plot(model, interactive=False, node_properties=node_properties)
     >>>
     >>> # Example: Specify all nodes
-    >>> node_properties = bn.get_node_properties(model, node_size=1000, node_color='#000000')
-    >>> fig = bn.plot(model, interactive=False, node_properties=node_properties)
+    >>> node_properties = bn.get_node_properties(model, node_size=10, node_color='#000000')
+    >>> bn.plot(model, interactive=True, node_properties=node_properties)
 
     """
     # https://networkx.org/documentation/networkx-1.7/reference/generated/networkx.drawing.nx_pylab.draw_networkx_nodes.html
     nodes = {}
     defaults={'node_color': node_color, 'node_size': node_size}
     adjmat = model.get('adjmat', None)
 
@@ -893,16 +879,21 @@
     edges = {}
     defaults = {'color': color, 'weight': weight}
     adjmat = model.get('independence_test', None)
     # Use edge weights from test statistic
     if adjmat is not None:
         if verbose>=3: print('[bnlearn]> Set edge weights based on the [%s] test statistic.' %(model['independence_test'].columns[-2]))
         logp = -np.log10(model['independence_test']['p_value'])
-        logp[np.isinf(logp)] = logp[np.isfinite(logp)].max()
+        Iloc = np.isinf(logp)
+        max_logp = np.max(logp[~Iloc]) * 1.5  # For visualization purposes, set the max higher then what is present to mark the difference.
+        if np.isnan(max_logp): max_logp = 1
+        logp.loc[Iloc] = max_logp
+        # Rescale the weights
         weights = _normalize_weights(logp.values, minscale=minscale, maxscale=maxscale)
+        # Add to adjmat
         adjmat = vec2adjmat(model['independence_test']['source'], model['independence_test']['target'], weights=weights)
     else:
         adjmat = model.get('adjmat', None)
 
     # Get model edges
     model_edges = adjmat2vec(adjmat)[['source', 'target']].values
     # model_edges = model['model'].edges() if (model.get('model_edges', None) is None) else model['model_edges']
@@ -929,15 +920,15 @@
          scale=1,
          interactive=False,
          title='bnlearn_causal_network',
          node_color=None,
          node_size=None,
          node_properties=None,
          edge_properties=None,
-         params_interactive={'width': '70%', 'height': '800px', 'notebook': False, 'layout': None, 'font_color': False, 'bgcolor': '#ffffff'},
+         params_interactive={'minmax_distance': [100, 250], 'figsize': (1500, 800), 'notebook': False, 'font_color': 'node_color', 'bgcolor': '#ffffff', 'show_slider': True, 'filepath': None},
          params_static={'minscale': 1, 'maxscale': 10, 'figsize': (15, 10), 'width': None, 'height': None, 'font_size': 14, 'font_family': 'sans-serif', 'alpha': 0.8, 'node_shape': 'o', 'layout': 'spring_layout', 'font_color': '#000000', 'facecolor': 'white', 'edge_alpha': 0.8, 'arrowstyle': '-|>', 'arrowsize': 30, 'visible': True},
          verbose=3):
     """Plot the learned stucture.
 
     Parameters
     ----------
     model : dict
@@ -995,43 +986,42 @@
     >>> # plot static
     >>> fig = bn.plot(model)
     >>>
     >>> # plot interactive
     >>> fig = bn.plot(model, interactive=True)
     >>>
     >>> # plot interactive with various settings
-    >>> fig = bn.plot(model, interactive=True, node_color='#8A0707', node_size=35, params_interactive = {'height':'800px', 'width':'70%', 'bgcolor':'#0f0f0f0f'})
+    >>> fig = bn.plot(model, interactive=True, node_color='#8A0707', node_size=35, params_interactive = {'figsize':(800, 600), 'bgcolor':'#0f0f0f0f'})
     >>>
     >>> # plot with node properties
     >>> node_properties = bn.get_node_properties(model)
     >>> # Make some changes
     >>> node_properties['xray']['node_color']='#8A0707'
     >>> node_properties['xray']['node_size']=50
     >>> # Plot
     >>> fig = bn.plot(model, interactive=True, node_properties=node_properties)
     >>>
 
     """
-    ax = None
+    fig = None
     # Check whether edges are available
     if model['adjmat'].sum().sum()==0:
         if verbose>=3: print('[bnlearn]> Nothing to plot because no edges are present between nodes. ')
         return None
 
     # Plot properties
-    defaults = {'height': '800px', 'width': '70%', 'notebook': False, 'layout': None, 'font_color': False, 'bgcolor': '#ffffff', 'directed': True}
+    defaults = {'minmax_distance': [100, 250], 'figsize': (1500, 800), 'notebook': False, 'font_color': 'node_color', 'bgcolor': '#ffffff', 'directed': True, 'show_slider': True, 'filepath': None}
     params_interactive = {**defaults, **params_interactive}
     defaults = {'minscale': 1, 'maxscale': 10, 'figsize': (15, 10), 'height': None, 'width': None, 'font_size': 14, 'font_family': 'sans-serif', 'alpha': 0.8, 'layout': 'spring_layout', 'font_color': 'k', 'facecolor': '#ffffff', 'node_shape': 'o', 'edge_alpha': 0.8, 'arrowstyle': '-|>', 'arrowsize': 30, 'visible': True}
     params_static = {**defaults, **params_static}
 
     # DEPRECATED IN LATER VERSION
     if (params_static.get('width') is not None) or (params_static.get('height') is not None):
         # if verbose>=2: print('[bnlearn]> Warning: [height] and [width] will be removed in further version. Please use: params_static={"figsize": (15, 10)}.')
         params_static['figsize'] = (15 if params_static['width'] is None else params_static['width'], 10 if params_static['height'] is None else params_static['height'])
-    # END BLOCK
 
     out = {}
     G = nx.DiGraph()  # Directed graph
     node_size_default = 10 if interactive else 800
     if (node_properties is not None) and (node_size is not None):
         if verbose>=2: print('[bnlearn]> Warning: if both "node_size" and "node_properties" are used, "node_size" will be used.')
 
@@ -1050,102 +1040,126 @@
     if 'dict' in str(type(model)):
         bnmodel = model.get('model', None)
     else:
         bnmodel = model.copy()
 
     # get node properties
     nodelist, node_colors, node_sizes, edgelist, edge_colors, edge_weights = _plot_properties(G, node_properties, edge_properties, node_color, node_size)
-
-    # Bayesian model
-    if ('bayes' in str(type(bnmodel)).lower()) or ('pgmpy' in str(type(bnmodel)).lower()):
-        if verbose>=3: print('[bnlearn] >Plot based on Bayesian model')
-        # positions for all nodes
-        G = nx.DiGraph(model['adjmat'])
-        pos = bnlearn.network.graphlayout(G, pos=pos, scale=scale, layout=params_static['layout'], verbose=verbose)
-    elif 'networkx' in str(type(bnmodel)):
-        if verbose>=3: print('[bnlearn] >Plot based on networkx model')
-        G = bnmodel
-        pos = bnlearn.network.graphlayout(G, pos=pos, scale=scale, layout=params_static['layout'], verbose=verbose)
-    else:
-        if verbose>=3: print('[bnlearn] >Plot based on adjacency matrix')
-        G = bnlearn.network.adjmat2graph(model['adjmat'])
-        # Get positions
-        pos = bnlearn.network.graphlayout(G, pos=pos, scale=scale, layout=params_static['layout'], verbose=verbose)
+    tooltip = nodelist
 
     # Plot
     if interactive:
+        if hasattr(model["model"], 'get_cpds'):
+            tooltip = []
+            for node in nodelist:
+                tip = model["model"].get_cpds(node)
+                if tip is None: tip = node
+                tooltip.append(tip)
+
         # Make interactive plot
-        ax = _plot_interactive(model, params_interactive, nodelist, node_colors, node_sizes, edgelist, edge_colors, edge_weights, title, verbose=verbose)
+        fig = _plot_interactive(params_interactive, nodelist, node_colors, node_sizes, edgelist, edge_colors, edge_weights, title, tooltip, verbose=verbose)
     else:
+
+        # Bayesian model
+        if ('bayes' in str(type(bnmodel)).lower()) or ('pgmpy' in str(type(bnmodel)).lower()):
+            if verbose>=3: print('[bnlearn] >Plot based on Bayesian model')
+            # positions for all nodes
+            G = nx.DiGraph(model['adjmat'])
+            pos = bnlearn.network.graphlayout(G, pos=pos, scale=scale, layout=params_static['layout'], verbose=verbose)
+        elif 'networkx' in str(type(bnmodel)):
+            if verbose>=3: print('[bnlearn] >Plot based on networkx model')
+            G = bnmodel
+            pos = bnlearn.network.graphlayout(G, pos=pos, scale=scale, layout=params_static['layout'], verbose=verbose)
+        else:
+            if verbose>=3: print('[bnlearn] >Plot based on adjacency matrix')
+            G = bnlearn.network.adjmat2graph(model['adjmat'])
+            # Get positions
+            pos = bnlearn.network.graphlayout(G, pos=pos, scale=scale, layout=params_static['layout'], verbose=verbose)
+
         # Make static plot
-        ax = _plot_static(model, params_static, nodelist, node_colors, node_sizes, G, pos, edge_colors, edge_weights, visible=params_static['visible'])
+        fig = _plot_static(model, params_static, nodelist, node_colors, node_sizes, G, pos, edge_colors, edge_weights, visible=params_static['visible'])
 
     # Store
-    out['ax']=ax
+    out['fig']=fig
+    out['ax']=fig  # Should be removed in later releases
     out['pos']=pos
     out['G']=G
     out['node_properties']=node_properties
     out['edge_properties']=edge_properties
     return out
 
 
 # %% Plot interactive
 # def _plot_static(model, params_static, nodelist, node_colors, node_sizes, title, verbose=3):
 def _plot_static(model, params_static, nodelist, node_colors, node_sizes, G, pos, edge_colors, edge_weights, visible=True):
     # Bootup figure
-    ax = plt.figure(figsize=params_static['figsize'], facecolor=params_static['facecolor'])
+    fig = plt.figure(figsize=params_static['figsize'], facecolor=params_static['facecolor'], dpi=100)
+    fig.set_visible(visible)
     # nodes
     nx.draw_networkx_nodes(G, pos, nodelist=nodelist, node_size=node_sizes, alpha=params_static['alpha'], node_color=node_colors, node_shape=params_static['node_shape'])
     # edges
     # nx.draw_networkx_edges(G, pos, arrowstyle='-|>', arrowsize=30, edge_color=edge_color, width=edge_weights)
     nx.draw_networkx_edges(G, pos, arrowstyle=params_static['arrowstyle'], arrowsize=params_static['arrowsize'], edge_color=edge_colors, width=edge_weights, alpha=params_static['edge_alpha'])
     # Labels
     nx.draw_networkx_labels(G, pos, font_size=params_static['font_size'], font_family=params_static['font_family'], font_color=params_static['font_color'])
     # Plot text of the weights
     # nx.draw_networkx_edge_labels(G, pos, edge_labels=nx.get_edge_attributes(G, 'weight'), font_color=params_static['font_color'])
     # Making figure nice
-    # ax = plt.gca()
-    # ax.set_axis_off()
-    ax.set_visible(visible)
-    return ax
+    # fig = plt.gca()
+    # fig.set_axis_off()
+    if visible:
+        plt.show()
+    # Return
+    return fig
 
 
 # %% Plot interactive
-def _plot_interactive(model, params_interactive, nodelist, node_colors, node_sizes, edgelist, edge_colors, edge_weights, title, verbose=3):
+def _plot_interactive(params_interactive, nodelist, node_colors, node_sizes, edgelist, edge_colors, edge_weights, title, tooltip, verbose=3):
+    # Try to import d3blocks
     try:
-        from pyvis.network import Network
-        from IPython.core.display import display, HTML
+        # Load library
+        from d3blocks import D3Blocks
     except ModuleNotFoundError:
-        if verbose>=1: raise Exception('[bnlearn] >"pyvis" module is not installed. Please pip install first: "pip install pyvis"')
-    # Convert adjacency matrix into Networkx Graph
-    G = bnlearn.network.adjmat2graph(model['adjmat'])
-    # Setup of the interactive network figure
-    g = Network(**params_interactive)
-    # Convert from graph G
-    g.from_nx(G)
-    # Nodes
-    for i, _ in enumerate(g.nodes):
-        g.nodes[i]['color']=node_colors[np.where(nodelist==g.nodes[i].get('label'))[0][0]]
-        g.nodes[i]['size']=node_sizes[np.where(nodelist==g.nodes[i].get('label'))[0][0]]
-
-    # Edges
-    g_edges = list(map(lambda x: (x.get('from'), x.get('to')), g.edges))
-    for i, _ in enumerate(g.edges):
-        idx = np.where(list(map(lambda x: g_edges[i]==x, edgelist)))[0][0]
-        g.edges[i]['color']=edge_colors[idx]
-        g.edges[i]['weight']=edge_weights[idx]
-
-    # Create advanced buttons
-    g.show_buttons(filter_=['physics'])
-    # Display
-    filename = title.strip().replace(' ', '_') + '.html'
-    g.show(filename)
-    display(HTML(filename))
-    # webbrowser.open('bnlearn.html')
-    return os.path.abspath(filename)
+        if verbose>=1: raise Exception('[bnlearn] >"d3blocks" library is not installed. Please pip install first: "pip install d3blocks"')
+
+    if params_interactive['filepath'] is None: params_interactive['filepath'] = title.strip().replace(' ', '_') + '.html'
+
+    # Initialize
+    d3 = D3Blocks()
+
+    # Set the min_weight
+    X = pd.DataFrame(data=edgelist, columns=['source', 'target'])
+    X['weight'] = edge_weights
+    
+    # Create network using default
+    d3.d3graph(X,
+               showfig=False,
+               title=title,
+               notebook=params_interactive['notebook'])
+
+    # Change node properties
+    d3.D3graph.set_node_properties(label=nodelist,
+                                   tooltip=tooltip,
+                                   size=node_sizes,
+                                   color=node_colors,
+                                   fontcolor=params_interactive['font_color'],
+                                   )
+
+    # Change edge properties
+    d3.D3graph.set_edge_properties(directed=params_interactive['directed'],
+                                   minmax_distance=params_interactive['minmax_distance'],
+                                   marker_color=edge_colors)
+
+    # Show the interactive plot
+    d3.D3graph.show(show_slider=params_interactive['show_slider'],
+                    filepath=params_interactive['filepath'],
+                    figsize=params_interactive['figsize'])
+
+    # Return
+    return os.path.abspath(d3.D3graph.config['filepath'])
 
 
 # %% Plot properties
 def _plot_properties(G, node_properties, edge_properties, node_color, node_size):
     # Set edge properties in Graph G
     # edges=[*bnmodel.edges()]
     edges = list(edge_properties.keys())
@@ -1239,75 +1253,53 @@
                 order.append(stack.pop())
             stack.append(v)
 
     return stack + order[::-1]
 
 
 # %% Example data
-def import_example(data='sprinkler', n=10000, verbose=3):
+def import_example(data='sprinkler', url=None, sep=',', n=10000, verbose=3):
     """Load example dataset.
 
     Parameters
     ----------
     data: str, (default: sprinkler)
         Pre-defined examples.
-        'titanic', 'sprinkler', 'alarm', 'andes', 'asia', 'sachs', 'water', 'random', 'stormofswords'
+            * 'sprinkler'
+            * 'alarm'
+            * 'andes'
+            * 'asia'
+            * 'sachs'
+            * 'water'
+        Continous data sets:
+            * 'auto_mpg'
     n: int, optional
-        Number of samples to generate. The default is 1000.
+        Number of samples to generate. The default is 10000.
     verbose: int, (default: 3)
         Print progress to screen.
         0: None, 1: Error, 2: Warning, 3: Info, 4: Debug, 5: Trace
 
     Returns
     -------
     df: pd.DataFrame()
 
     """
-    if data=='random':
-        return pd.DataFrame(np.random.randint(low=0, high=2, size=(n, 5)), columns=['A', 'B', 'C', 'D', 'E'])
-
-    # Change name for downloading
-    if data=='titanic': data = 'titanic_train'
 
-    # Download example dataset from github source
-    PATH_TO_DATA = _download_example(data, verbose=verbose)
-
-    # Import dataset
-    if (data=='sprinkler') or (data=='titanic_train') or (data=='stormofswords'):
-        if verbose>=3: print('[bnlearn] >Import dataset..')
-        df = pd.read_csv(PATH_TO_DATA, delimiter=',')
-    else:
+    if (data=='alarm') or (data=='andes') or (data=='asia') or (data=='sachs') or (data=='water'):
         try:
-            _ = _unzip(PATH_TO_DATA, verbose=verbose)
             DAG = import_DAG(data, verbose=2)
             df = sampling(DAG, n=n, verbose=2)
         except:
             print('[bnlearn] >Error: Loading data not possible!')
             df = None
 
-    return df
-
-
-# %% Download data from github source
-def _download_example(data, verbose=3):
-    # Set url location
-    url = 'https://erdogant.github.io/datasets/'
-    url=url + data + '.zip'
-
-    curpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
-    PATH_TO_DATA = os.path.join(curpath, wget.filename_from_url(url))
-    if not os.path.isdir(curpath):
-        os.mkdir(curpath)
-
-    # Check file exists.
-    if not os.path.isfile(PATH_TO_DATA):
-        if verbose>=3: print('[bnlearn] >Downloading example [%s] dataset..' %(data))
-        wget.download(url, curpath)
+    else:
+        df = dz.get(data, url, sep, n=n, verbose=0)
 
-    return PATH_TO_DATA
+    return df
 
 
 # %% Make DAG
 def import_DAG(filepath='sprinkler', CPD=True, checkmodel=True, verbose=3):
     """Import Directed Acyclic Graph.
 
     Parameters
@@ -1332,35 +1324,40 @@
     Examples
     --------
     >>> import bnlearn as bn
     >>> model = bn.import_DAG('sprinkler')
     >>> fig = bn.plot(model)
 
     """
-    PATH_TO_DATA = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
-    out={}
-    model=None
-    filepath=filepath.lower()
+    out = {}
+    model = None
+    filepath= filepath.lower()
     if verbose>=3: print('[bnlearn] >Import <%s>' %(filepath))
+    # Get the data properties
+    dataproperties = dz.get_dataproperties(filepath)
+    # Get path to data
+    # PATH_TO_DATA = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
+    PATH_TO_DATA = dataproperties['curpath']
 
     # Load data
     if filepath=='sprinkler':
         model = _DAG_sprinkler(CPD=CPD)
     elif (filepath=='asia') or (filepath=='alarm') or (filepath=='andes') or (filepath=='sachs') or (filepath=='water'):
         getfile = os.path.join(PATH_TO_DATA, filepath +'.bif')
         if not os.path.isfile(getfile):
-            PATH_TO_DATA = _download_example(filepath, verbose=3)
-            _ = _unzip(PATH_TO_DATA, verbose=verbose)
+            PATH_TO_DATA = dz.download_from_url(dataproperties['filename'], url=dataproperties['url'])
+            _ = dz.unzip(PATH_TO_DATA)
+
         model = _bif2bayesian(getfile, verbose=verbose)
     else:
         if os.path.isfile(filepath):
             model = _bif2bayesian(filepath, verbose=verbose)
         else:
             if verbose>=3: print('[bnlearn] >filepath does not exist! <%s>' %(filepath))
-            return(out)
+            return out
 
     # Setup adjacency matrix
     adjmat = dag2adjmat(model)
 
     # Store
     out['model']=model
     out['adjmat']=adjmat
@@ -1370,30 +1367,14 @@
         check_model(out['model'], verbose=verbose)
         if verbose>=4:
             print_CPD(out)
 
     return(out)
 
 
-# %% unzip
-def _unzip(getZip, ext='.bif', verbose=3):
-    if not os.path.isdir(getZip):
-        if verbose>=3: print('[bnlearn] >Extracting files..')
-        [pathname, _] = os.path.split(getZip)
-        # Unzip
-        zip_ref = zipfile.ZipFile(getZip, 'r')
-        zip_ref.extractall(pathname)
-        zip_ref.close()
-        getPath = getZip.replace('.zip', ext)
-        if not os.path.isfile(getPath):
-            getPath = None
-
-    return getPath
-
-
 # %% Pre-processing of input raw dataset
 def df2onehot(df, y_min=10, perc_min_num=0.8, dtypes='pandas', excl_background=None, verbose=3):
     """Convert dataframe to one-hot matrix.
 
     Parameters
     ----------
     df : pd.DataFrame()
@@ -1785,25 +1766,75 @@
     show_message = True
     scores = {}
     # Get models and method
     if isinstance(model, dict):
         method = model.get('config')['method']
         model = model.get('model', None)
     if isinstance(scoring_method, str): scoring_method = [scoring_method]
-    if verbose>=3: print('[bnlearn] >Compute structure scores %s for model comparison (higher is better).' %(scoring_method))
+    if verbose>=3: print('[bnlearn] >Compute structure scores for model comparison (higher is better).' %(scoring_method))
 
     # Return if method not supported
     if np.any(np.isin(method, ['cs', 'constraintsearch'])):
         if verbose>=2: print('[bnlearn] >Warning: Structure scoring could not be computed. Method [%s] not supported.' %(method))
         return scores
 
     # Compute structure scores
     if model is not None:
         for s in scoring_method:
             try:
                 scores[s] = structure_score(model, df, scoring_method=s)
             except:
                 if verbose>=2 and show_message:
-                    print('[bnlearn] >Warning: Structure scoring could not be computed. DataFrame issues (?)')
+                    print('[bnlearn] >Skipping computing structure score for [%s].' %(s))
                     show_message=False
     # Return
     return scores
+
+
+# %%
+# def set_logger(verbose: [str, int] = 'info'):
+#     """Set the logger for verbosity messages.
+
+#     Parameters
+#     ----------
+#     verbose : [str, int], default is 'info' or 20
+#         Set the verbose messages using string or integer values.
+#         * [0, 60, None, 'silent', 'off', 'no']: No message.
+#         * [10, 'debug']: Messages from debug level and higher.
+#         * [20, 'info']: Messages from info level and higher.
+#         * [30, 'warning']: Messages from warning level and higher.
+#         * [50, 'critical']: Messages from critical level and higher.
+
+#     Returns
+#     -------
+#     None.
+
+#     > # Set the logger to warning
+#     > set_logger(verbose='warning')
+#     > # Test with different messages
+#     > logger.debug("Hello debug")
+#     > logger.info("Hello info")
+#     > logger.warning("Hello warning")
+#     > logger.critical("Hello critical")
+
+#     """
+#     # Set 0 and None as no messages.
+#     if (verbose==0) or (verbose is None):
+#         verbose=60
+#     # Convert str to levels
+#     if isinstance(verbose, str):
+#         levels = {'silent': 60,
+#                   'off': 60,
+#                   'no': 60,
+#                   'debug': 10,
+#                   'info': 20,
+#                   'warning': 30,
+#                   'critical': 50}
+#         verbose = levels[verbose]
+
+#     # Show examples
+#     logger.setLevel(verbose)
+
+# # %%
+# def disable_tqdm():
+#     """Set the logger for verbosity messages."""
+#     return (True if (logger.getEffectiveLevel()>=30) else False)
```

### Comparing `bnlearn-0.7.9/bnlearn/confmatrix.py` & `bnlearn-0.8.0/bnlearn/confmatrix.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.7.9/bnlearn/examples.py` & `bnlearn-0.8.0/bnlearn/examples.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,180 @@
 import pandas as pd
 import numpy as np
 from pgmpy.inference import VariableElimination
 from pgmpy.models import BayesianNetwork, NaiveBayes
 from pgmpy.estimators import ExhaustiveSearch, HillClimbSearch, TreeSearch
 from pgmpy.factors.discrete import TabularCPD
 
+# %%
+import bnlearn as bn
+
+# Load example dataset
+df = bn.import_example('sprinkler')
+
+edges = [('Cloudy', 'Sprinkler'),
+         ('Cloudy', 'Rain'),
+         ('Sprinkler', 'Wet_Grass'),
+         ('Rain', 'Wet_Grass')]
+
+# Make the actual Bayesian DAG
+DAG = bn.make_DAG(edges)
+model = bn.parameter_learning.fit(DAG, df)
+# Print CPDs
+CPD = bn.print_CPD(model)
+
+bn.check_model(CPD) # Input should be model
+bn.check_model(model)
+
+bn.plot(model, interactive=True, params_interactive={'filepath': r'c:/temp/bnlearn.html'})
+
+# %%
+import bnlearn as bn
+
+# Example dataset
+source=['Cloudy','Cloudy','Sprinkler','Rain']
+target=['Sprinkler','Rain','Wet_Grass','Wet_Grass']
+repeats=[1,2,1,3]
+
+adjmat = bn.vec2adjmat(source, target, weights=repeats)
+
+# Convert into sparse datamatrix
+df = bn.vec2df(source, target, weights=repeats)
+df = bn.adjmat2vec(adjmat)
+# Make DAG
+DAG = bn.make_DAG(list(zip(source, target)), verbose=0)
+# Make plot
+bn.plot(DAG, interactive=True, params_interactive={'filepath': r'c:/temp/bnlearn.html'})
+# bn.plot(DAG, interactive=True)
+# bn.plot(DAG, interactive=False)
+
+
+# %% Import examples
+import bnlearn as bn
+df = bn.import_example(data='sprinkler', n=1000)
+
+DAG = bn.import_DAG('Sprinkler')
+
+# %% Working with continues data
+import bnlearn as bn
+df = bn.import_example(data='auto_mpg')
+
+edges = [
+    ("cylinders", "displacement"),
+    ("displacement", "model_year"),
+    ("displacement", "weight"),
+    ("displacement", "horsepower"),
+    ("weight", "model_year"),
+    ("weight", "mpg"),
+    ("horsepower", "acceleration"),
+    ("mpg", "model_year"),
+]
+
+# Create DAG based on edges
+DAG = bn.make_DAG(edges)
+
+# df_num = df.select_dtypes(include='float64').columns.values
+continuous_columns = ["mpg", "displacement", "horsepower", "weight", "acceleration"]
+# Discretize the continous columns
+df_disc = bn.discretize(df, edges, continuous_columns, max_iterations=1)
+
+# Fit model based on DAG and discretize the continous columns
+model_mle = bn.parameter_learning.fit(DAG, df_disc)
+# model_mle = bn.parameter_learning.fit(DAG, data_disc, methodtype="maximumlikelihood")
+
+# Make plot
+bn.plot(model_mle)
+bn.plot(model_mle, interactive=True)
+# bn.independence_test(model, df)
+
+print(model_mle["model"].get_cpds("mpg"))
+
+
+print("Weight categories: ", df_disc["weight"].dtype.categories)
+evidence = {"weight": bn.discretize_value(df_disc["weight"], 3000.0)}
+print(evidence)
+print(bn.inference.fit(model_mle, variables=["mpg"], evidence=evidence, verbose=0))
+
+
+
+# %%
+import bnlearn as bn
+shapes = [(10000, 37), (10000, 223), (10000, 8), (10000, 11), (10000, 32), (352, 3)]
+for i, data in enumerate(['alarm', 'andes', 'asia', 'sachs', 'water', 'stormofswords']):
+    print(data)
+    df = bn.import_example(data=data)
+    assert df.shape==shapes[i]
+
+
+# %% Notebook example
+# Example dataframe sprinkler_data.csv can be loaded with: 
+import bnlearn as bn
+df = bn.import_example()
+# df = pd.read_csv('sprinkler_data.csv')
+model = bn.structure_learning.fit(df, verbose=0)
+
+# Set some colors to the edges and nodes
+node_properties = bn.get_node_properties(model)
+node_properties['Sprinkler']['node_color']='#FF0000'
+
+edge_properties = bn.get_edge_properties(model)
+edge_properties[('Cloudy', 'Rain')]['color']='#FF0000'
+edge_properties[('Cloudy', 'Rain')]['weight']=5
+
+G = bn.plot(model,
+            node_properties=node_properties,
+            edge_properties=edge_properties,
+            interactive=True,
+            params_interactive={'notebook': False},
+            )
+
+# G = bn.plot(model, interactive=True, params_interactive={'notebook': True}, node_properties=node_properties, edge_properties=edge_properties)
+
+# %%
+import bnlearn as bn
+model = bn.import_DAG('asia')
+
+# Make single inference
+query = bn.inference.fit(model, variables=['lung', 'bronc', 'xray'], evidence={'smoke':1})
+print(query)
+print(bn.query2df(query))
+
+# Lets create an example dataset with 100 samples and make inferences on the entire dataset.
+df = bn.sampling(model, n=10000)
+
+# Each sample will be assesed and the states with highest probability are returned.
+Pout = bn.predict(model, df, variables=['lung'])
+
+print(Pout)
+#     Cloudy  Rain         p
+# 0        0     0  0.647249
+# 1        0     0  0.604230
+# ..     ...   ...       ...
+# 998      0     0  0.604230
+# 999      1     1  0.878049
+
+# %%
+import bnlearn as bn
+model = bn.import_DAG('asia', CPD=True)
+CPDs = bn.print_CPD(model)
+CPDs.keys()
+# dict_keys(['asia', 'bronc', 'dysp', 'either', 'lung', 'smoke', 'tub', 'xray'])
+print(CPDs['smoke'])
+#    smoke    p
+# 0      0  0.5
+# 1      1  0.5
+
+print(model["model"].get_cpds('asia'))
+print(model["model"].get_cpds(np.array(list(CPDs.keys()))[1]))
+
 # %% Issue 65: return (fig, ax)
 import bnlearn as bn
 model = bn.import_DAG('sprinkler', CPD=True)
 df = bn.sampling(model, n=1000, methodtype='bayes')
 fig = bn.plot(model, params_static={'visible': True})
-
 fig2 = bn.plot(model, interactive=True)
 
 
 # %% Issue Mail:
 # from pgmpy.models import BayesianNetwork
 
 # # create instance
@@ -50,28 +210,31 @@
 model = bn.parameter_learning.fit(DAG, df)
 # Print CPDs
 CPD = bn.print_CPD(model)
 
 bn.check_model(CPD) # Input should be model
 bn.check_model(model)
 
+bn.plot(model, interactive=True)
+
 # %%
 import bnlearn as bn
 # print(bn.__version__)
 # print(dir(bn.structure_learning))
 # print(dir(bn.parameter_learning))
 # print(dir(bn.inference))
 
 # %%
 # Load asia DAG
 df = bn.import_example(data='asia')
 # Structure learning of sampled dataset
 model = bn.structure_learning.fit(df)
 # Make plot
 G = bn.plot(model)
+G = bn.plot(model, interactive=True)
 
 # %% Issue MAIL: Store CPDs after printing.
 import bnlearn as bn
 
 # Load example dataset
 df = bn.import_example('sprinkler')
 
@@ -137,21 +300,20 @@
 bn.plot(model)
 
 
 # %%
 import bnlearn as bn
 model = bn.import_DAG('water', verbose=0)
 # Sampling
-df = bn.sampling(model, n=1000, methodtype='markov', verbose=3)
-# Parameter learning
-model = bn.parameter_learning.fit(DAG, df, scoretype='bdeu', smooth=None)
+df = bn.sampling(model, n=1000, methodtype='bayes', verbose=3)
 
 
 # %% Naive Bayesian model
-df = bn.import_example('random')
+import bnlearn as bn
+df = bn.import_example('random_discrete')
 # Structure learning
 model = bn.structure_learning.fit(df, methodtype='nb', root_node="B", verbose=4, n_jobs=1)
 model = bn.structure_learning.fit(df, methodtype='hc', verbose=4, n_jobs=1)
 model = bn.structure_learning.fit(df, methodtype='cs', verbose=4, n_jobs=1)
 model = bn.structure_learning.fit(df, methodtype='cl', verbose=4, n_jobs=1)
 model = bn.structure_learning.fit(df, methodtype='tan', class_node="A", verbose=4, n_jobs=1)
 model = bn.structure_learning.fit(df, methodtype='ex', verbose=4, n_jobs=1)
@@ -228,15 +390,16 @@
 
 
 # %%
 import bnlearn as bn
 
 raw = bn.import_example('stormofswords')
 # Convert raw data into sparse datamatrix
-df = bn.vec2df(raw['source'], raw['target'], raw['weight'])
+df = bn.vec2adjmat(raw['source'], raw['target'], raw['weight'])
+# df = bn.vec2df(raw['source'], raw['target'], raw['weight'])
 # Make the actual Bayesian DAG
 DAG = bn.make_DAG(list(zip(raw['source'], raw['target'])), verbose=0)
 # Make plot
 bn.plot(DAG, interactive=True)
 bn.plot(DAG, interactive=False)
 
 # Parameter learning
@@ -338,27 +501,28 @@
 assert model['model_edges']==model1['model_edges']
 assert len(model1['model_edges'])==model1['independence_test'].shape[0]
 assert len(model2['model_edges'])==model2['independence_test'].shape[0]
 assert len(model2['model_edges'])<len(model1['model_edges'])
 assert len(model2['model_edges'])<len(model['model_edges'])
 
 # Plot
-# G = bn.plot(model1, interactive=True)
-# G = bn.plot(model2, interactive=True)
+G = bn.plot(model1, interactive=True)
+G = bn.plot(model2, interactive=False)
 
 
 # %% Adjust some edge properties
 # Load asia DAG
 df = bn.import_example(data='sprinkler')
 # Structure learning of sampled dataset
 model = bn.structure_learning.fit(df)
 # Compute edge strength with the chi_square test statistic
 model = bn.independence_test(model, df, test='chi_square', prune=True)
 # Make plot
 bn.plot(model)
+bn.plot(model, interactive=True, params_interactive={'filepath': r'c:/temp/output.html'})
 
 # %% Adjust some edge properties
 # Load asia DAG
 df = bn.import_example(data='asia')
 # Structure learning of sampled dataset
 model = bn.structure_learning.fit(df)
 # Make plot
@@ -462,22 +626,23 @@
 #     out['nr_succes_pop_n']=n
 #     out['samplesize_N']=N
 #     out['dtype']='categorical'
 #     return(out)
 
 
 # %% Naive Bayesian model
-df = bn.import_example('random')
+df = bn.import_example('random_discrete')
 # Structure learning
 model = bn.structure_learning.fit(df, methodtype='naivebayes', root_node="B")
 model = bn.independence_test(model, df, prune=True)
 # Plot
 bn.plot(model)
 
 # %% Naive Bayesian model
+from pgmpy.factors.discrete import TabularCPD
 
 edges = [('A', 'B'), ('A', 'C'), ('A', 'D')]
 DAG = bn.make_DAG(edges, methodtype='naivebayes')
 bn.plot(DAG)
 
 cpd_A = TabularCPD(variable='A', variable_card=3, values=[[0.3], [0.5], [0.2]])
 print(cpd_A)
@@ -1053,14 +1218,15 @@
 
 dfnum.loc[0:50, 'Survived'] = 2
 # Structure learning
 # DAG = bn.structure_learning.fit(dfnum, methodtype='cl', black_list=['Embarked','Parch','Name'], root_node='Survived', bw_list_method='nodes')
 DAG = bn.structure_learning.fit(dfnum, methodtype='hc', black_list=['Embarked', 'Parch', 'Name'], bw_list_method='edges')
 # Plot
 G = bn.plot(DAG)
+G = bn.plot(DAG, interactive=True)
 # Parameter learning
 model = bn.parameter_learning.fit(DAG, dfnum)
 # Make inference
 q1 = bn.inference.fit(model, variables=['Survived'], evidence={'Sex': True, 'Pclass': True}, verbose=0)
 q2 = bn.inference.fit(model, variables=['Survived'], evidence={'Sex': 0}, verbose=0)
 
 print(q1)
@@ -1081,14 +1247,15 @@
 
 df = bn.sampling(DAG, n=1000)
 vector = bn.adjmat2vec(DAG['adjmat'])
 adjmat = bn.vec2adjmat(vector['source'], vector['target'])
 
 # %%
 import bnlearn as bn
+from pgmpy.factors.discrete import TabularCPD
 
 edges = [('A', 'E'),
          ('S', 'E'),
          ('E', 'O'),
          ('E', 'R'),
          ('O', 'T'),
          ('R', 'T')]
@@ -1248,8 +1415,10 @@
 # Make inference
 q1 = bn.inference.fit(DAGmle, variables=['Wet_Grass', 'Cloudy', 'Sprinkler'], evidence={'Rain': 1})
 q1 = bn.inference.fit(DAGmle, variables=['Cloudy', 'Wet_Grass', 'Sprinkler'], evidence={'Rain': 1})
 q1 = bn.inference.fit(DAGbay, variables=['Wet_Grass'], evidence={'Rain': 1, 'Sprinkler': 0, 'Cloudy': 1})
 
 print(q1.values)
 
+
 # %%
+
```

### Comparing `bnlearn-0.7.9/bnlearn/inference.py` & `bnlearn-0.8.0/bnlearn/inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,8 +90,8 @@
         raise Exception('[bnlearn] >Error: Input model does not contain learned CPDs. hint: did you run parameter_learning.fit?')
 
     # Computing the probability P(class | evidence)
     query = model_infer.query(variables=variables, evidence=evidence, show_progress=(verbose>0))
     # Store also in dataframe
     query.df = bnlearn.query2df(query, variables=variables, verbose=verbose) if to_df else None
     # Return
-    return(query)
+    return query
```

### Comparing `bnlearn-0.7.9/bnlearn/network.py` & `bnlearn-0.8.0/bnlearn/network.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.7.9/bnlearn/parameter_learning.py` & `bnlearn-0.8.0/bnlearn/parameter_learning.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # %% Libraries
 from pgmpy.estimators import BayesianEstimator
 import bnlearn
 import warnings
 warnings.filterwarnings("ignore")
 
 
-# %% Sampling from model
+# %% Parameter learning
 def fit(model, df, methodtype='bayes', scoretype='bdeu', smooth=None, n_jobs=-1, verbose=3):
     """Learn the parameters given the DAG and data.
 
     Description
     -----------
     Maximum Likelihood Estimation
         A natural estimate for the CPDs is to simply use the *relative frequencies*,
@@ -107,14 +107,15 @@
 
     """
     config = {}
     config['verbose'] = verbose
     config['method'] = methodtype
     config['n_jobs'] = n_jobs
     adjmat = model['adjmat']
+    independence_test = model.get('independence_test', None)
 
     if (scoretype=='dirichlet') and (smooth is None):
         raise Exception('[bnlearn] >dirichlet requires "smooth" to be not None')
 
     # Check whether all labels in the adjacency matrix are included from the dataframe
     # adjmat, model = _check_adjmat(model, df)
     df = bnlearn._filter_df(adjmat, df, verbose=config['verbose'])
@@ -148,10 +149,10 @@
         return None
 
     out = {}
     out['model'] = model
     out['adjmat'] = adjmat
     out['config'] = config
     out['model_edges'] = list(model.edges())
-    out['structure_scores'] = bnlearn.structure_scores(out, df)
-
-    return(out)
+    out['structure_scores'] = bnlearn.structure_scores(out, df, verbose=verbose)
+    out['independence_test'] = independence_test
+    return out
```

### Comparing `bnlearn-0.7.9/bnlearn/structure_learning.py` & `bnlearn-0.8.0/bnlearn/structure_learning.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 import bnlearn
 
 
 # %% Structure Learning
 def fit(df, methodtype='hc', scoretype='bic', black_list=None, white_list=None, bw_list_method=None, max_indegree=None, tabu_length=100, epsilon=1e-4, max_iter=1e6, root_node=None, class_node=None, fixed_edges=None, return_all_dags=False, n_jobs=-1, verbose=3):
     """Structure learning fit model.
 
-    Description
-    -----------
     Search strategies for structure learning
     The search space of DAGs is super-exponential in the number of variables and the above scoring functions allow for local maxima.
 
     To learn model structure (a DAG) from a data set, there are three broad techniques:
         1. Score-based structure learning (BIC/BDeu/K2 score; exhaustive search, hill climb/tabu search)
             * exhaustivesearch
             * hillclimbsearch
@@ -187,18 +185,18 @@
         """TreeSearch based Structure Learning."""
         out = _treesearch(df, config['method'], config['root_node'], class_node=config['class_node'], n_jobs=config['n_jobs'], verbose=config['verbose'])
 
     # Store
     out['model_edges'] = list(out['model'].edges())
     out['adjmat'] = bnlearn.dag2adjmat(out['model'])
     out['config'] = config
-    out['structure_scores'] = bnlearn.structure_scores(out, df)
+    out['structure_scores'] = bnlearn.structure_scores(out, df, verbose=verbose)
 
     # return
-    return(out)
+    return out
 
 
 # %% Make Checks
 def _make_checks(df, config, verbose=3):
     assert isinstance(pd.DataFrame(), type(df)), 'df must be of type pd.DataFrame()'
     if not np.isin(config['scoring'], ['bic', 'k2', 'bdeu']): raise Exception('"scoretype=%s" is invalid.' %(config['scoring']))
     if not np.isin(config['method'], ['naivebayes', 'nb', 'tan', 'cl', 'chow-liu', 'hc', 'ex', 'cs', 'exhaustivesearch', 'hillclimbsearch', 'constraintsearch']): raise Exception('"methodtype=%s" is invalid.' %(config['method']))
```

### Comparing `bnlearn-0.7.9/bnlearn/tests/test_bnlearn.py` & `bnlearn-0.8.0/bnlearn/tests/test_bnlearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 
 import bnlearn as bn
 from pgmpy.factors.discrete import TabularCPD
 import numpy as np
 import pandas as pd
 
 
+def test_load_examples():
+    shapes = [(10000, 37), (10000, 223), (10000, 8), (10000, 11), (10000, 32), (352, 3)]
+    for i, data in enumerate(['alarm', 'andes', 'asia', 'sachs', 'water', 'stormofswords']):
+        print(data)
+        df = bn.import_example(data=data)
+        assert df.shape==shapes[i]
+
+
 def test_QUERY():
     # Load example DataFrame
     df = bn.import_example('titanic')
     dfhot, dfnum = bn.df2onehot(df)
     # Train model
     model_as = bn.structure_learning.fit(dfnum, methodtype='hc', scoretype='bic')
     model_as_p = bn.parameter_learning.fit(model_as, dfnum, methodtype='bayes')
@@ -24,16 +32,15 @@
     for variables in variables_list:
         for evidences in evidences_list:
             query = bn.inference.fit(model_as_p, variables=variables, evidence=evidences, to_df=True, verbose=0)
             assert query.df.shape == sizes[i]
             assert list(query.df.columns) == variables + ['p']
             i = i + 1
 
-    query = bn.inference.fit(model_as_p, variables=['Sex', 'Parch', 'SibSp'], evidence={'Survived': 0, 'Pclass': 1},
-                             to_df=True, verbose=0)
+    query = bn.inference.fit(model_as_p, variables=['Sex', 'Parch', 'SibSp'], evidence={'Survived': 0, 'Pclass': 1}, to_df=True, verbose=0)
     q = bn.query2df(query, variables=['SibSp', 'Sex'])
     assert q.shape == (48, 3)
     assert list(q.columns) == ['SibSp', 'Sex', 'p']
 
 
 def test_import_DAG():
     DAG = bn.import_DAG('Sprinkler')
@@ -116,15 +123,15 @@
     assert bn.vec2adjmat(out['source'], out['target']).shape == DAG['adjmat'].shape
 
 
 def test_parameter_learning():
     df = bn.import_example()
     model = bn.import_DAG('sprinkler', CPD=False)
     model_update = bn.parameter_learning.fit(model, df)
-    assert [*model_update.keys()] == ['model', 'adjmat', 'config', 'model_edges', 'structure_scores']
+    assert [*model_update.keys()] == ['model', 'adjmat', 'config', 'model_edges', 'structure_scores', 'independence_test']
 
 
 def test_inference():
     DAG = bn.import_DAG('sprinkler')
     q1 = bn.inference.fit(DAG, variables=['Wet_Grass'], evidence={'Rain': 1, 'Sprinkler': 0, 'Cloudy': 1}, to_df=False,
                           verbose=0)
     assert 'pgmpy.factors.discrete.DiscreteFactor.DiscreteFactor' in str(type(q1))
@@ -244,27 +251,26 @@
 
 
 def test_independence_test():
     df = bn.import_example(data='asia')
     # Structure learning of sampled dataset
     model = bn.structure_learning.fit(df)
     # Compute edge weights based on chi_square test statistic
-    tests = ['chi_square', 'g_sq', 'log_likelihood', 'freeman_tuckey', 'modified_log_likelihood', 'neyman',
-             'cressie_read']
+    tests = ['chi_square', 'g_sq', 'log_likelihood', 'freeman_tuckey', 'modified_log_likelihood', 'neyman', 'cressie_read']
     for test in tests:
         model = bn.independence_test(model, df, test=test)
         assert model.get('independence_test', None) is not None
         assert set(model['independence_test'].columns) == {test, 'dof', 'p_value', 'source', 'stat_test', 'target'}
         assert model['independence_test'].columns[-2] == test
         assert np.any(model['independence_test']['stat_test'])
         assert model['independence_test'].shape[0] > 1
 
     # Run 10 times with random data
     for i in np.arange(0, 10):
-        df = bn.import_example(data='random')
+        df = bn.import_example(data='random_discrete')
         # Parameter learning
         model = bn.structure_learning.fit(df)
         # Test for independence
         assert bn.independence_test(model, df, prune=False)
         # Test for independence
         assert bn.independence_test(model, df, prune=True)
```

### Comparing `bnlearn-0.7.9/bnlearn/tests/test_structure_learning.py` & `bnlearn-0.8.0/bnlearn/tests/test_structure_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.7.9/bnlearn.egg-info/PKG-INFO` & `bnlearn-0.8.0/bnlearn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,80 +1,97 @@
 Metadata-Version: 2.1
 Name: bnlearn
-Version: 0.7.9
+Version: 0.8.0
 Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
 Home-page: https://erdogant.github.io/bnlearn
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.7.9.tar.gz
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.0.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
+![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
 [![Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/issues)
 [![Project Status](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://pepy.tech/project/bnlearn/)
 [![Downloads](https://pepy.tech/badge/bnlearn)](https://pepy.tech/project/bnlearn)
 [![DOI](https://zenodo.org/badge/231263493.svg)](https://zenodo.org/badge/latestdoi/231263493)
 [![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
-[![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
+[![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
+![GitHub repo size](https://img.shields.io/github/repo-size/erdogant/bnlearn)
 [![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#colab-notebook)
 <!---[![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)-->
 <!---[![Coffee](https://img.shields.io/badge/coffee-black-grey.svg)](https://erdogant.github.io/donate/?currency=USD&amount=5)-->
 
 
 ### 
 
-``bnlearn`` is Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods. This work is inspired by the R package (bnlearn.com) that has been very usefull to me for many years. Although there are very good Python packages for probabilistic graphical models, it still can remain difficult (and somethimes unnecessarily) to (re)build certain pipelines. Bnlearn for python (this package) is build on the <a href="https://github.com/pgmpy/pgmpy">pgmpy</a> package and contains the most-wanted pipelines. Navigate to [API documentations](https://erdogant.github.io/bnlearn/) for more detailed information.
+``bnlearn`` is Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
+Because probabilistic graphical models can be difficult in usage, Bnlearn for python (this package) is build on the <a href="https://github.com/pgmpy/pgmpy">pgmpy</a> package and contains the most-wanted pipelines. Navigate to [API documentations](https://erdogant.github.io/bnlearn/) for more detailed information.
 
 # 
 **⭐️ Star this repo if you like it ⭐️**
 # 
 
-### Blogs
+### Read the Medium blog for more details.
 
-Read the blogs to get a structured overview of bayesian methods and detailed usage of ``bnlearn``.
+<p align="left">
+  <a href="https://towardsdatascience.com/a-step-by-step-guide-in-detecting-causal-relationships-using-bayesian-structure-learning-in-python-c20c6b31cee5" target="_blank">
+    <img src="https://github.com/erdogant/bnlearn/blob/master/docs/figs/medium_blog2.png?raw=true" width="150" />
+  </a>
+
+  <a href="https://towardsdatascience.com/a-step-by-step-guide-in-designing-knowledge-driven-models-using-bayesian-theorem-7433f6fd64be" target="_blank">
+  <img src="https://github.com/erdogant/bnlearn/blob/master/docs/figs/medium_blog1.png?raw=true" width="150" />
+  </a>
 
-* [Step-by-step guide for structure learning.](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
-* [Step-by-step guide for knowledge-driven models.](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
+</p>
+
+
+---
 
 # 
 
 
 ### [Documentation pages](https://erdogant.github.io/bnlearn/)
 
 On the [documentation pages](https://erdogant.github.io/bnlearn/) you can find detailed information about the working of the ``bnlearn`` with many examples. 
 
 # 
 
 ### Installation
 
 ##### It is advisable to create a new environment (e.g. with Conda). 
 ```bash
-conda create -n env_bnlearn python=3.8
+conda create -n env_bnlearn python=3.10
 conda activate env_bnlearn
 ```
 
 ##### Install bnlearn from PyPI
 ```bash
 pip install bnlearn
 ```
 
+##### Install bnlearn from github source
+```bash
+pip install git+https://github.com/erdogant/bnlearn
+```
+
 ##### The following functions are available after installation:
 
 ```python
 # Import library
 import bnlearn as bn
 
 # Structure learning
@@ -290,16 +307,24 @@
 
 ### References
 * https://erdogant.github.io/bnlearn/
 * http://pgmpy.org
 * https://programtalk.com/python-examples/pgmpy.factors.discrete.TabularCPD/
 * http://www.bnlearn.com/bnrepository/
 
-### Contribute
-* All kinds of contributions are welcome!
+
+### Contributors
+Setting up and maintaining bnlearn has been possible thanks to users and contributors. Thanks to:
+
+<p align="left">
+  <a href="https://github.com/erdogant/bnlearn/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=erdogant/bnlearn" />
+  </a>
+</p>
+
 
 ### Citation
 Please cite ``bnlearn`` in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
```

#### html2text {}

```diff
@@ -1,60 +1,60 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.7.9 Summary: Python package for
+Metadata-Version: 2.1 Name: bnlearn Version: 0.8.0 Summary: Python package for
 learning the graphical structure of Bayesian networks, parameter learning,
 inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
 Author: Erdogan Taskesen Author-email: erdogant@gmail.com License: UNKNOWN
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.7.9.tar.gz
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.0.tar.gz
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE # bnlearn - Library for Bayesian network learning and
 inference [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://
 img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version](https://
-img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) [![License]
+img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) ![GitHub
+Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn) [![License]
 (https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/
 erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/
 forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [!
 [Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)]
 (https://github.com/erdogant/bnlearn/issues) [![Project Status](http://
 www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
 #active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
 pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
 (https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
 231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
 img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
-[![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://
-erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) [!
-[Donate](https://img.shields.io/badge/Support%20this%20project-
+[![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
+erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) ![GitHub
+repo size](https://img.shields.io/github/repo-size/erdogant/bnlearn) [![Donate]
+(https://img.shields.io/badge/Support%20this%20project-
 grey.svg?logo=github%20sponsors)](https://erdogant.github.io/bnlearn/pages/
 html/Documentation.html#) [![Colab](https://colab.research.google.com/assets/
 colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/
 Documentation.html#colab-notebook)   ### ``bnlearn`` is Python package for
 learning the graphical structure of Bayesian networks, parameter learning,
-inference and sampling methods. This work is inspired by the R package
-(bnlearn.com) that has been very usefull to me for many years. Although there
-are very good Python packages for probabilistic graphical models, it still can
-remain difficult (and somethimes unnecessarily) to (re)build certain pipelines.
-Bnlearn for python (this package) is build on the pgmpy package and contains
-the most-wanted pipelines. Navigate to [API documentations](https://
-erdogant.github.io/bnlearn/) for more detailed information. # **â­ï¸ Star
-this repo if you like it â­ï¸** # ### Blogs Read the blogs to get a
-structured overview of bayesian methods and detailed usage of ``bnlearn``. *
-[Step-by-step guide for structure learning.](https://erdogant.github.io/
-bnlearn/pages/html/Documentation.html#medium-blog) * [Step-by-step guide for
-knowledge-driven models.](https://erdogant.github.io/bnlearn/pages/html/
-Documentation.html#medium-blog) # ### [Documentation pages](https://
-erdogant.github.io/bnlearn/) On the [documentation pages](https://
-erdogant.github.io/bnlearn/) you can find detailed information about the
-working of the ``bnlearn`` with many examples. # ### Installation ##### It is
-advisable to create a new environment (e.g. with Conda). ```bash conda create -
-n env_bnlearn python=3.8 conda activate env_bnlearn ``` ##### Install bnlearn
-from PyPI ```bash pip install bnlearn ``` ##### The following functions are
-available after installation: ```python # Import library import bnlearn as bn #
-Structure learning bn.structure_learning.fit() # Compute edge strength with the
-test statistic bn.independence_test(model, df, test='chi_square', prune=True) #
+inference and sampling methods. Because probabilistic graphical models can be
+difficult in usage, Bnlearn for python (this package) is build on the pgmpy
+package and contains the most-wanted pipelines. Navigate to [API
+documentations](https://erdogant.github.io/bnlearn/) for more detailed
+information. # **â­ï¸ Star this repo if you like it â­ï¸** # ### Read the
+Medium blog for more details.
+[https://github.com/erdogant/bnlearn/blob/master/docs/figs/
+medium_blog2.png?raw=true] [https://github.com/erdogant/bnlearn/blob/master/
+docs/figs/medium_blog1.png?raw=true]
+--- # ### [Documentation pages](https://erdogant.github.io/bnlearn/) On the
+[documentation pages](https://erdogant.github.io/bnlearn/) you can find
+detailed information about the working of the ``bnlearn`` with many examples. #
+### Installation ##### It is advisable to create a new environment (e.g. with
+Conda). ```bash conda create -n env_bnlearn python=3.10 conda activate
+env_bnlearn ``` ##### Install bnlearn from PyPI ```bash pip install bnlearn ```
+##### Install bnlearn from github source ```bash pip install git+https://
+github.com/erdogant/bnlearn ``` ##### The following functions are available
+after installation: ```python # Import library import bnlearn as bn # Structure
+learning bn.structure_learning.fit() # Compute edge strength with the test
+statistic bn.independence_test(model, df, test='chi_square', prune=True) #
 Parameter learning bn.parameter_learning.fit() # Inference bn.inference.fit() #
 Make predictions bn.predict() # Based on a DAG, you can sample the number of
 samples you want. bn.sampling() # Load well known examples to play arround with
 or load your own .bif file. bn.import_DAG() # Load simple dataframe of
 sprinkler dataset. bn.import_example() # Compare 2 graphs bn.compare_networks()
 # Plot graph bn.plot() # To make the directed grapyh undirected
 bn.to_undirected() # Convert to one-hot datamatrix bn.df2onehot() # Derive the
@@ -129,13 +129,16 @@
 ('sprinkler') query = bn.inference.fit(model, variables=['Rain'], evidence=
 {'Cloudy':1,'Sprinkler':0, 'Wet_Grass':1}) print(query) print(query.df) # Lets
 try another inference query = bn.inference.fit(model, variables=['Rain'],
 evidence={'Cloudy':1}) print(query) print(query.df) ```
 ===============================================================================
 ### References * https://erdogant.github.io/bnlearn/ * http://pgmpy.org *
 https://programtalk.com/python-examples/pgmpy.factors.discrete.TabularCPD/ *
-http://www.bnlearn.com/bnrepository/ ### Contribute * All kinds of
-contributions are welcome! ### Citation Please cite ``bnlearn`` in your
-publications if this is useful for your research. See column right for citation
-information. ### Maintainer * Erdogan Taskesen, github: [erdogant](https://
-github.com/erdogant) * Contributions are welcome. * If you wish to buy me a
-Coffee for this work, it is very appreciated :)
+http://www.bnlearn.com/bnrepository/ ### Contributors Setting up and
+maintaining bnlearn has been possible thanks to users and contributors. Thanks
+to:
+[https://contrib.rocks/image?repo=erdogant/bnlearn]
+### Citation Please cite ``bnlearn`` in your publications if this is useful for
+your research. See column right for citation information. ### Maintainer *
+Erdogan Taskesen, github: [erdogant](https://github.com/erdogant) *
+Contributions are welcome. * If you wish to buy me a Coffee for this work, it
+is very appreciated :)
```

### Comparing `bnlearn-0.7.9/setup.py` & `bnlearn-0.8.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,30 +12,29 @@
 # Setup ------------
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      install_requires=["pgmpy>=0.1.18",
                        "networkx>=2.7.1",
                        "matplotlib>=3.3.4",
-                       'numpy',
-                       'pandas',
+                       "numpy>=1.24.1",
+                       'pandas==1.5.3',
                        'tqdm',
                        'ismember',
-                       'sklearn',
+                       'scikit-learn',
                        'funcsigs',
                        'statsmodels',
                        'python-louvain',
                        'packaging',
-                       'wget',
                        'df2onehot',
                        'fsspec',
                        'pypickle',
                        'tabulate',
                        'ipywidgets',
-                       'pyvis'],
+                       'datazets'],
      python_requires='>=3',
      name='bnlearn',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.",
      long_description=long_description,
```

