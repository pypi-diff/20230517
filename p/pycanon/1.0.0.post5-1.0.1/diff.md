# Comparing `tmp/pycanon-1.0.0.post5.tar.gz` & `tmp/pycanon-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycanon-1.0.0.post5.tar", last modified: Wed Aug 10 10:47:22 2022, max compression
+gzip compressed data, was "pycanon-1.0.1.tar", last modified: Wed May 17 14:10:43 2023, max compression
```

## Comparing `pycanon-1.0.0.post5.tar` & `pycanon-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2022-08-10 10:47:22.016244 pycanon-1.0.0.post5/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)    11355 2022-05-12 20:28:02.000000 pycanon-1.0.0.post5/LICENSE
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)       25 2022-08-10 10:46:56.000000 pycanon-1.0.0.post5/MANIFEST.in
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     6195 2022-08-10 10:47:22.016244 pycanon-1.0.0.post5/PKG-INFO
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     5114 2022-08-01 09:22:00.000000 pycanon-1.0.0.post5/README.rst
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2022-08-10 10:47:22.016244 pycanon-1.0.0.post5/pycanon/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      659 2022-08-10 10:47:04.000000 pycanon-1.0.0.post5/pycanon/__init__.py
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2022-08-10 10:47:22.016244 pycanon-1.0.0.post5/pycanon/anonymity/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     1506 2022-06-28 08:43:12.000000 pycanon-1.0.0.post5/pycanon/anonymity/__init__.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     4638 2022-06-28 08:43:12.000000 pycanon-1.0.0.post5/pycanon/anonymity/_beta_likeness.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     2557 2022-06-28 08:43:12.000000 pycanon-1.0.0.post5/pycanon/anonymity/_delta_disclosure.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     3822 2022-06-28 08:43:12.000000 pycanon-1.0.0.post5/pycanon/anonymity/_k_anonymity.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     9571 2022-07-12 09:04:25.000000 pycanon-1.0.0.post5/pycanon/anonymity/_l_diversity.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     3096 2022-06-28 08:43:12.000000 pycanon-1.0.0.post5/pycanon/anonymity/_t_closeness.py
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2022-08-10 10:47:22.016244 pycanon-1.0.0.post5/pycanon/anonymity/utils/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      687 2022-06-28 08:43:12.000000 pycanon-1.0.0.post5/pycanon/anonymity/utils/__init__.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     7359 2022-06-28 08:43:12.000000 pycanon-1.0.0.post5/pycanon/anonymity/utils/aux_anonymity.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     3807 2022-07-12 09:04:25.000000 pycanon-1.0.0.post5/pycanon/anonymity/utils/aux_functions.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)    13015 2022-07-15 10:03:34.000000 pycanon-1.0.0.post5/pycanon/cli.py
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2022-08-10 10:47:22.016244 pycanon-1.0.0.post5/pycanon/report/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     2453 2022-07-12 09:04:25.000000 pycanon-1.0.0.post5/pycanon/report/__init__.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     2939 2022-06-28 08:43:12.000000 pycanon-1.0.0.post5/pycanon/report/base.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     2789 2022-06-28 08:43:12.000000 pycanon-1.0.0.post5/pycanon/report/json.py
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     5300 2022-06-28 08:43:12.000000 pycanon-1.0.0.post5/pycanon/report/pdf.py
-drwxr-xr-x   0 alvaro    (1000) alvaro    (1000)        0 2022-08-10 10:47:22.016244 pycanon-1.0.0.post5/pycanon.egg-info/
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     6195 2022-08-10 10:47:22.000000 pycanon-1.0.0.post5/pycanon.egg-info/PKG-INFO
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      709 2022-08-10 10:47:22.000000 pycanon-1.0.0.post5/pycanon.egg-info/SOURCES.txt
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)        1 2022-08-10 10:47:22.000000 pycanon-1.0.0.post5/pycanon.egg-info/dependency_links.txt
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)       45 2022-08-10 10:47:22.000000 pycanon-1.0.0.post5/pycanon.egg-info/entry_points.txt
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)       75 2022-08-10 10:47:22.000000 pycanon-1.0.0.post5/pycanon.egg-info/requires.txt
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)        8 2022-08-10 10:47:22.000000 pycanon-1.0.0.post5/pycanon.egg-info/top_level.txt
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)       77 2022-08-10 10:46:37.000000 pycanon-1.0.0.post5/requirements.txt
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)     1258 2022-08-10 10:47:22.016244 pycanon-1.0.0.post5/setup.cfg
--rw-r--r--   0 alvaro    (1000) alvaro    (1000)      216 2022-08-10 10:46:37.000000 pycanon-1.0.0.post5/setup.py
+drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/
+-rw-rw-r--   0 judith    (1000) judith    (1000)    11355 2023-05-12 12:04:19.000000 pycanon-1.0.1/LICENSE
+-rw-rw-r--   0 judith    (1000) judith    (1000)       25 2023-05-12 12:04:19.000000 pycanon-1.0.1/MANIFEST.in
+-rw-rw-r--   0 judith    (1000) judith    (1000)     6828 2023-05-17 14:10:43.209757 pycanon-1.0.1/PKG-INFO
+-rw-rw-r--   0 judith    (1000) judith    (1000)     5773 2023-05-12 12:04:19.000000 pycanon-1.0.1/README.rst
+drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/pycanon/
+-rw-rw-r--   0 judith    (1000) judith    (1000)      741 2023-05-15 06:37:16.000000 pycanon-1.0.1/pycanon/__init__.py
+drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/pycanon/anonymity/
+-rw-rw-r--   0 judith    (1000) judith    (1000)     1501 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/__init__.py
+-rw-rw-r--   0 judith    (1000) judith    (1000)     4143 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/_beta_likeness.py
+-rw-rw-r--   0 judith    (1000) judith    (1000)     2430 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/_delta_disclosure.py
+-rw-rw-r--   0 judith    (1000) judith    (1000)     3788 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/_k_anonymity.py
+-rw-rw-r--   0 judith    (1000) judith    (1000)     9319 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/_l_diversity.py
+-rw-rw-r--   0 judith    (1000) judith    (1000)     3135 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/_t_closeness.py
+drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/pycanon/anonymity/utils/
+-rw-rw-r--   0 judith    (1000) judith    (1000)      762 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/utils/__init__.py
+-rw-rw-r--   0 judith    (1000) judith    (1000)     6889 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/utils/aux_anonymity.py
+-rw-rw-r--   0 judith    (1000) judith    (1000)     4023 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/anonymity/utils/aux_functions.py
+-rw-rw-r--   0 judith    (1000) judith    (1000)    11958 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/cli.py
+drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/pycanon/report/
+-rw-rw-r--   0 judith    (1000) judith    (1000)     2634 2023-05-15 06:36:57.000000 pycanon-1.0.1/pycanon/report/__init__.py
+-rw-rw-r--   0 judith    (1000) judith    (1000)     2547 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/report/base.py
+-rw-rw-r--   0 judith    (1000) judith    (1000)     2772 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/report/json.py
+-rw-rw-r--   0 judith    (1000) judith    (1000)     5324 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/report/pdf.py
+-rw-rw-r--   0 judith    (1000) judith    (1000)     8350 2023-05-12 12:04:19.000000 pycanon-1.0.1/pycanon/report/pdf_utility_report.py
+drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/pycanon.egg-info/
+-rw-rw-r--   0 judith    (1000) judith    (1000)     6828 2023-05-17 14:10:43.000000 pycanon-1.0.1/pycanon.egg-info/PKG-INFO
+-rw-rw-r--   0 judith    (1000) judith    (1000)      790 2023-05-17 14:10:43.000000 pycanon-1.0.1/pycanon.egg-info/SOURCES.txt
+-rw-rw-r--   0 judith    (1000) judith    (1000)        1 2023-05-17 14:10:43.000000 pycanon-1.0.1/pycanon.egg-info/dependency_links.txt
+-rw-rw-r--   0 judith    (1000) judith    (1000)       44 2023-05-17 14:10:43.000000 pycanon-1.0.1/pycanon.egg-info/entry_points.txt
+-rw-rw-r--   0 judith    (1000) judith    (1000)       82 2023-05-17 14:10:43.000000 pycanon-1.0.1/pycanon.egg-info/requires.txt
+-rw-rw-r--   0 judith    (1000) judith    (1000)        8 2023-05-17 14:10:43.000000 pycanon-1.0.1/pycanon.egg-info/top_level.txt
+-rw-rw-r--   0 judith    (1000) judith    (1000)       85 2023-05-15 06:36:57.000000 pycanon-1.0.1/requirements.txt
+-rw-rw-r--   0 judith    (1000) judith    (1000)     1258 2023-05-17 14:10:43.209757 pycanon-1.0.1/setup.cfg
+-rw-rw-r--   0 judith    (1000) judith    (1000)      216 2023-05-12 12:04:19.000000 pycanon-1.0.1/setup.py
+drwxrwxr-x   0 judith    (1000) judith    (1000)        0 2023-05-17 14:10:43.209757 pycanon-1.0.1/tests/
+-rw-rw-r--   0 judith    (1000) judith    (1000)     1514 2023-05-12 12:04:19.000000 pycanon-1.0.1/tests/test_metrics.py
+-rw-rw-r--   0 judith    (1000) judith    (1000)     2760 2023-05-12 12:04:19.000000 pycanon-1.0.1/tests/test_reports.py
```

### Comparing `pycanon-1.0.0.post5/LICENSE` & `pycanon-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycanon-1.0.0.post5/PKG-INFO` & `pycanon-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pycanon
-Version: 1.0.0.post5
+Version: 1.0.1
 Summary: pyCANON, A Python library to check the level of anonymity of a dataset
 Home-page: https://gitlab.ifca.es/privacy-security/pycanon
 Author: Judith Sáinz-Pardo Díaz, Álvaro López García (IFCA (CSIC-UC))
 Author-email: sainzpardo@ifca.unican.es, aloga@ifca.unican.es
 License: Apache License 2.0
 Keywords: data,privacy,anonymity
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -22,18 +21,18 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Security
 License-File: LICENSE
 
 pyCANON
 =======
 
-|made-with-python| |License| |Documentation Status|
+|License| |Documentation Status| |Pipeline Status|
 
-pyCANON is a library and CLI to assess the values of the paramenters
-associated with the most common privacy-preserving techniques.
+pyCANON is a Python library and CLI to assess the values of the parameters
+associated with the most common privacy-preserving techniques via anonymization.
 
 **Authors:** Judith Sáinz-Pardo Díaz and Álvaro López García (IFCA - CSIC).
 
 Installation
 ------------
 
 We recommend to use Python3 with
@@ -61,32 +60,34 @@
 ---------------
 
 Example using the `adult
 dataset <https://archive.ics.uci.edu/ml/datasets/adult>`__:
 
 .. code:: python
 
+   import pandas as pd
    from pycanon import anonymity, report
 
    FILE_NAME = "adult.csv"
    QI = ["age", "education", "occupation", "relationship", "sex", "native-country"]
    SA = ["salary-class"]
+   DATA = pd.read_csv(FILE_NAME)
 
    # Calculate k for k-anonymity:
-   k = anonymity.k_anonymity(FILE_NAME, QI)
+   k = anonymity.k_anonymity(DATA, QI)
 
    # Print the anonymity report:
-   report.print_report(FILE_NAME, QI, SA)
+   report.print_report(DATA, QI, SA)
 
 Description
 -----------
 
 pyCANON allows to check if the following privacy-preserving techniques
 are verified and the value of the parameters associated with each of
-them:
+them.
 
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 | Technique                 | pyCANON function            | Parameters | Notes                                               |
 +===========================+=============================+============+=====================================================+
 | k-anonymity               | ``k_anonymity``             | *k*: int   |                                                     |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 | (α, k)-anonymity          | ``alpha_k_anonymity``       | *α*: float |                                                     |
@@ -107,16 +108,30 @@
 |                           |                             |            | (one-dimensional Earth Mover’s Distance) is used.   |
 |                           |                             |            | For categorical attributes, the metric "Equal       |
 |                           |                             |            | Distance" is used.                                  |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 | δ-disclosure privacy      | ``delta_disclosure``        | *δ*: float |                                                     |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 
+More information can be found in this `paper <https://www.nature.com/articles/s41597-022-01894-2>`__.
+
+
+Citation
+-----------
+If you are using pyCANON you can cite it as follows:: 
+
+   @article{sainzpardo2022pycanon,
+      title={A Python library to check the level of anonymity of a dataset},
+      author={S{\'a}inz-Pardo D{\'\i}az, Judith and L{\'o}pez Garc{\'\i}a, {\'A}lvaro},
+      journal={Scientific Data},
+      volume={9},
+      number={1},
+      pages={785},
+      year={2022},
+      publisher={Nature Publishing Group UK London}}
 
-.. |made-with-python| image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg
-   :target: https://www.python.org/
 .. |License| image:: https://img.shields.io/badge/License-Apache_2.0-blue.svg
    :target: https://gitlab.ifca.es/sainzj/check-anonymity/-/blob/main/LICENSE
 .. |Documentation Status| image:: https://readthedocs.org/projects/pycanon/badge/?version=latest
    :target: https://pycanon.readthedocs.io/en/latest/?badge=latest
-
-
+.. |Pipeline Status| image:: https://gitlab.ifca.es/privacy-security/pycanon/badges/main/pipeline.svg
+   :target: https://gitlab.ifca.es/privacy-security/pycanon/-/pipelines
```

### Comparing `pycanon-1.0.0.post5/README.rst` & `pycanon-1.0.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pyCANON
 =======
 
-|made-with-python| |License| |Documentation Status|
+|License| |Documentation Status| |Pipeline Status|
 
-pyCANON is a library and CLI to assess the values of the paramenters
-associated with the most common privacy-preserving techniques.
+pyCANON is a Python library and CLI to assess the values of the parameters
+associated with the most common privacy-preserving techniques via anonymization.
 
 **Authors:** Judith Sáinz-Pardo Díaz and Álvaro López García (IFCA - CSIC).
 
 Installation
 ------------
 
 We recommend to use Python3 with
@@ -36,32 +36,34 @@
 ---------------
 
 Example using the `adult
 dataset <https://archive.ics.uci.edu/ml/datasets/adult>`__:
 
 .. code:: python
 
+   import pandas as pd
    from pycanon import anonymity, report
 
    FILE_NAME = "adult.csv"
    QI = ["age", "education", "occupation", "relationship", "sex", "native-country"]
    SA = ["salary-class"]
+   DATA = pd.read_csv(FILE_NAME)
 
    # Calculate k for k-anonymity:
-   k = anonymity.k_anonymity(FILE_NAME, QI)
+   k = anonymity.k_anonymity(DATA, QI)
 
    # Print the anonymity report:
-   report.print_report(FILE_NAME, QI, SA)
+   report.print_report(DATA, QI, SA)
 
 Description
 -----------
 
 pyCANON allows to check if the following privacy-preserving techniques
 are verified and the value of the parameters associated with each of
-them:
+them.
 
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 | Technique                 | pyCANON function            | Parameters | Notes                                               |
 +===========================+=============================+============+=====================================================+
 | k-anonymity               | ``k_anonymity``             | *k*: int   |                                                     |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 | (α, k)-anonymity          | ``alpha_k_anonymity``       | *α*: float |                                                     |
@@ -82,14 +84,30 @@
 |                           |                             |            | (one-dimensional Earth Mover’s Distance) is used.   |
 |                           |                             |            | For categorical attributes, the metric "Equal       |
 |                           |                             |            | Distance" is used.                                  |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 | δ-disclosure privacy      | ``delta_disclosure``        | *δ*: float |                                                     |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 
+More information can be found in this `paper <https://www.nature.com/articles/s41597-022-01894-2>`__.
+
+
+Citation
+-----------
+If you are using pyCANON you can cite it as follows:: 
+
+   @article{sainzpardo2022pycanon,
+      title={A Python library to check the level of anonymity of a dataset},
+      author={S{\'a}inz-Pardo D{\'\i}az, Judith and L{\'o}pez Garc{\'\i}a, {\'A}lvaro},
+      journal={Scientific Data},
+      volume={9},
+      number={1},
+      pages={785},
+      year={2022},
+      publisher={Nature Publishing Group UK London}}
 
-.. |made-with-python| image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg
-   :target: https://www.python.org/
 .. |License| image:: https://img.shields.io/badge/License-Apache_2.0-blue.svg
    :target: https://gitlab.ifca.es/sainzj/check-anonymity/-/blob/main/LICENSE
 .. |Documentation Status| image:: https://readthedocs.org/projects/pycanon/badge/?version=latest
    :target: https://pycanon.readthedocs.io/en/latest/?badge=latest
+.. |Pipeline Status| image:: https://gitlab.ifca.es/privacy-security/pycanon/badges/main/pipeline.svg
+   :target: https://gitlab.ifca.es/privacy-security/pycanon/-/pipelines
```

### Comparing `pycanon-1.0.0.post5/pycanon/__init__.py` & `pycanon-1.0.1/pycanon/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,8 +10,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-__version__ = '1.0.0.post5'
+"""pyCANON is a library to check the values of the most common data privacy models."""
+
+__version__ = "1.0.1"
```

### Comparing `pycanon-1.0.0.post5/pycanon/anonymity/__init__.py` & `pycanon-1.0.1/pycanon/anonymity/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Copyright 2022 Spanish National Research Council (CSIC)
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may
 # not use this file except in compliance with the License. You may obtain
 # a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
@@ -30,19 +29,15 @@
 from ._l_diversity import entropy_l_diversity
 from ._l_diversity import recursive_c_l_diversity
 from ._t_closeness import t_closeness
 
 __all__ = [
     "basic_beta_likeness",
     "enhanced_beta_likeness",
-
     "delta_disclosure",
-
     "k_anonymity",
     "alpha_k_anonymity",
-
     "l_diversity",
     "entropy_l_diversity",
     "recursive_c_l_diversity",
-
     "t_closeness",
 ]
```

### Comparing `pycanon-1.0.0.post5/pycanon/anonymity/_beta_likeness.py` & `pycanon-1.0.1/pycanon/anonymity/_beta_likeness.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 import numpy as np
 import pandas as pd
 
 from pycanon.anonymity.utils import aux_anonymity
 from pycanon.anonymity.utils import aux_functions
 
 
-def basic_beta_likeness(data: pd.DataFrame,
-                        quasi_ident: typing.Union[typing.List, np.ndarray],
-                        sens_att: typing.Union[typing.List, np.ndarray],
-                        gen=True) -> float:
+def basic_beta_likeness(
+    data: pd.DataFrame,
+    quasi_ident: typing.Union[typing.List, np.ndarray],
+    sens_att: typing.Union[typing.List, np.ndarray],
+    gen=True,
+) -> float:
     """Calculate beta for basic beta-likeness.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
@@ -50,33 +52,33 @@
     quasi_ident = np.array(quasi_ident)
     sens_att = np.array(sens_att)
     aux_functions.check_qi(data, quasi_ident)
     aux_functions.check_sa(data, sens_att)
     beta_sens_att = []
     if gen:
         for sens_att_value in sens_att:
-            _, dist = aux_anonymity.aux_calculate_beta(data,
-                                                       quasi_ident,
-                                                       sens_att_value)
+            _, dist = aux_anonymity.aux_calculate_beta(
+                data, quasi_ident, sens_att_value
+            )
             beta_sens_att.append(max(dist))
     else:
         for i, sens_att_value in enumerate(sens_att):
             tmp_qi = np.concatenate([quasi_ident, np.delete(sens_att, i)])
-            _, dist = aux_anonymity.aux_calculate_beta(data,
-                                                       tmp_qi,
-                                                       sens_att_value)
+            _, dist = aux_anonymity.aux_calculate_beta(data, tmp_qi, sens_att_value)
             beta_sens_att.append(max(dist))
     beta = max(beta_sens_att)
     return beta
 
 
-def enhanced_beta_likeness(data: pd.DataFrame,
-                           quasi_ident: typing.Union[typing.List, np.ndarray],
-                           sens_att: typing.Union[typing.List, np.ndarray],
-                           gen=True) -> float:
+def enhanced_beta_likeness(
+    data: pd.DataFrame,
+    quasi_ident: typing.Union[typing.List, np.ndarray],
+    sens_att: typing.Union[typing.List, np.ndarray],
+    gen=True,
+) -> float:
     """Calculate beta for enhanced beta-likeness.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
@@ -96,22 +98,20 @@
     quasi_ident = np.array(quasi_ident)
     sens_att = np.array(sens_att)
     aux_functions.check_qi(data, quasi_ident)
     aux_functions.check_sa(data, sens_att)
     beta_sens_att = []
     if gen:
         for sens_att_value in sens_att:
-            p, dist = aux_anonymity.aux_calculate_beta(data,
-                                                       quasi_ident,
-                                                       sens_att_value)
+            p, dist = aux_anonymity.aux_calculate_beta(
+                data, quasi_ident, sens_att_value
+            )
             min_beta_lnp = [min(max(dist), -np.log(p_i)) for p_i in p]
             beta_sens_att.append(max(min_beta_lnp))
     else:
         for i, sens_att_value in enumerate(sens_att):
             tmp_qi = np.concatenate([quasi_ident, np.delete(sens_att, i)])
-            p, dist = aux_anonymity.aux_calculate_beta(data,
-                                                       tmp_qi,
-                                                       sens_att_value)
+            p, dist = aux_anonymity.aux_calculate_beta(data, tmp_qi, sens_att_value)
             min_beta_lnp = [min(max(dist), -np.log(p_i)) for p_i in p]
             beta_sens_att.append(max(min_beta_lnp))
     beta = max(beta_sens_att)
     return beta
```

### Comparing `pycanon-1.0.0.post5/pycanon/anonymity/_delta_disclosure.py` & `pycanon-1.0.1/pycanon/anonymity/_delta_disclosure.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 import numpy as np
 import pandas as pd
 
 from pycanon.anonymity.utils import aux_anonymity
 from pycanon.anonymity.utils import aux_functions
 
 
-def delta_disclosure(data: pd.DataFrame,
-                     quasi_ident: typing.Union[typing.List, np.ndarray],
-                     sens_att: typing.Union[typing.List, np.ndarray],
-                     gen=True) -> float:
+def delta_disclosure(
+    data: pd.DataFrame,
+    quasi_ident: typing.Union[typing.List, np.ndarray],
+    sens_att: typing.Union[typing.List, np.ndarray],
+    gen=True,
+) -> float:
     """Calculate delta for delta-disclousure privacy.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
@@ -51,18 +53,19 @@
     sens_att = np.array(sens_att)
     aux_functions.check_qi(data, quasi_ident)
     aux_functions.check_sa(data, sens_att)
     delta_sens_att = []
     if gen:
         for sens_att_value in sens_att:
             aux = aux_anonymity.aux_calculate_delta_disclosure(
-                data, quasi_ident, sens_att_value)
+                data, quasi_ident, sens_att_value
+            )
             delta_sens_att.append(aux)
     else:
         for i, sens_att_value in enumerate(sens_att):
             tmp_qi = np.concatenate([quasi_ident, np.delete(sens_att, i)])
-            aux = aux_anonymity.aux_calculate_delta_disclosure(data,
-                                                               tmp_qi,
-                                                               sens_att_value)
+            aux = aux_anonymity.aux_calculate_delta_disclosure(
+                data, tmp_qi, sens_att_value
+            )
             delta_sens_att.append(aux)
     delta = max(delta_sens_att)
     return delta
```

### Comparing `pycanon-1.0.0.post5/pycanon/anonymity/_k_anonymity.py` & `pycanon-1.0.1/pycanon/anonymity/_k_anonymity.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,40 +19,42 @@
 import numpy as np
 import pandas as pd
 
 from pycanon.anonymity.utils import aux_anonymity
 from pycanon.anonymity.utils import aux_functions
 
 
-def k_anonymity(data: pd.DataFrame,
-                quasi_ident: typing.Union[typing.List, np.ndarray]) -> int:
+def k_anonymity(
+    data: pd.DataFrame, quasi_ident: typing.Union[typing.List, np.ndarray]
+) -> int:
     """Calculate k for k-anonymity.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
     :type quasi_ident: list of strings
 
     :return: k value for k-anonymity.
     :rtype: int.
     """
-
     aux_functions.check_qi(data, quasi_ident)
 
     equiv_class = aux_anonymity.get_equiv_class(data, quasi_ident)
     k_anon = min([len(x) for x in equiv_class])
     return k_anon
 
 
-def alpha_k_anonymity(data: pd.DataFrame,
-                      quasi_ident: typing.Union[typing.List, np.ndarray],
-                      sens_att: typing.Union[typing.List, np.ndarray],
-                      gen=True) -> typing.Tuple[float, int]:
+def alpha_k_anonymity(
+    data: pd.DataFrame,
+    quasi_ident: typing.Union[typing.List, np.ndarray],
+    sens_att: typing.Union[typing.List, np.ndarray],
+    gen=True,
+) -> typing.Tuple[float, int]:
     """Calculate alpha and k for (alpha,k)-anonymity.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
@@ -78,27 +80,29 @@
     if gen:
         alpha_ec = []
         for ec in equiv_class:
             data_temp = data.iloc[aux_functions.convert(ec)]
             alpha_sa = []
             for sa in sens_att:
                 values = np.unique(data_temp[sa].values)
-                _alpha = [len(data_temp[data_temp[sa] == s]) /
-                          len(data_temp) for s in values]
+                _alpha = [
+                    len(data_temp[data_temp[sa] == s]) / len(data_temp) for s in values
+                ]
                 alpha_sa.append(max(_alpha))
             alpha_ec.append(max(alpha_sa))
         alpha = max(alpha_ec)
     else:
         alpha_sa = []
         for i, sa in enumerate(sens_att):
             tmp_qi = np.concatenate([quasi_ident, np.delete(sens_att, i)])
             equiv_class = aux_anonymity.get_equiv_class(data, tmp_qi)
             alpha_ec = []
             for ec in equiv_class:
                 data_temp = data.iloc[aux_functions.convert(ec)]
                 values = np.unique(data_temp[sa].values)
-                _alpha = [len(data_temp[data_temp[sa] == s]) /
-                          len(data_temp) for s in values]
+                _alpha = [
+                    len(data_temp[data_temp[sa] == s]) / len(data_temp) for s in values
+                ]
                 alpha_ec.append(max(_alpha))
             alpha_sa.append(max(alpha_ec))
         alpha = max(alpha_sa)
     return alpha, k_anon
```

### Comparing `pycanon-1.0.0.post5/pycanon/anonymity/_l_diversity.py` & `pycanon-1.0.1/pycanon/anonymity/_l_diversity.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 import numpy as np
 import pandas as pd
 
 from pycanon.anonymity.utils import aux_anonymity
 from pycanon.anonymity.utils import aux_functions
 
 
-def l_diversity(data: pd.DataFrame,
-                quasi_ident: typing.Union[typing.List, np.ndarray],
-                sens_att: typing.Union[typing.List, np.ndarray],
-                gen=True) -> int:
+def l_diversity(
+    data: pd.DataFrame,
+    quasi_ident: typing.Union[typing.List, np.ndarray],
+    sens_att: typing.Union[typing.List, np.ndarray],
+    gen=True,
+) -> int:
     """Calculate l for l-diversity.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
@@ -67,18 +69,20 @@
             for ec in equiv_class:
                 data_temp = data.iloc[aux_functions.convert(ec)]
                 l_ec.append(len(np.unique(data_temp[sa].values)))
             l_div.append(min(l_ec))
     return min(l_div)
 
 
-def entropy_l_diversity(data: pd.DataFrame,
-                        quasi_ident: typing.Union[typing.List, np.ndarray],
-                        sens_att: typing.Union[typing.List, np.ndarray],
-                        gen=True) -> float:
+def entropy_l_diversity(
+    data: pd.DataFrame,
+    quasi_ident: typing.Union[typing.List, np.ndarray],
+    sens_att: typing.Union[typing.List, np.ndarray],
+    gen=True,
+) -> float:
     """Calculate l for entropy l-diversity.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
@@ -104,44 +108,48 @@
         equiv_class = aux_anonymity.get_equiv_class(data, quasi_ident)
         entropy_ec = []
         for ec in equiv_class:
             data_temp = data.iloc[aux_functions.convert(ec)]
             entropy_sa = []
             for sa in sens_att:
                 values = np.unique(data_temp[sa].values)
-                p = [len(data_temp[data_temp[sa] == s])/len(data_temp)
-                     for s in values]
+                p = [
+                    len(data_temp[data_temp[sa] == s]) / len(data_temp) for s in values
+                ]
                 entropy = np.sum(p * np.log(p))
                 entropy_sa.append(-entropy)
             entropy_ec.append(min(entropy_sa))
-        ent_l = int(min(np.exp(1)**entropy_ec))
+        ent_l = int(min(np.exp(1) ** entropy_ec))
     else:
         entropy_sa = []
         for i, sa in enumerate(sens_att):
             tmp_qi = np.concatenate([quasi_ident, np.delete(sens_att, i)])
             equiv_class = aux_anonymity.get_equiv_class(data, tmp_qi)
             entropy_ec = []
             for ec in equiv_class:
                 data_temp = data.iloc[aux_functions.convert(ec)]
                 entropy = 0
                 values = np.unique(data_temp[sa].values)
-                p = [len(data_temp[data_temp[sa] == s])/len(data_temp)
-                     for s in values]
-                entropy = np.sum(p*np.log(p))
+                p = [
+                    len(data_temp[data_temp[sa] == s]) / len(data_temp) for s in values
+                ]
+                entropy = np.sum(p * np.log(p))
                 entropy_ec.append(-entropy)
             entropy_sa.append(min(entropy_ec))
-        ent_l = int(min(np.exp(1)**entropy_sa))
+        ent_l = int(min(np.exp(1) ** entropy_sa))
     return ent_l
 
 
-def recursive_c_l_diversity(data: pd.DataFrame,
-                            quasi_ident: typing.Union[typing.List, np.ndarray],
-                            sens_att: typing.Union[typing.List, np.ndarray],
-                            imp=False,
-                            gen=True) -> typing.Tuple[float, int]:
+def recursive_c_l_diversity(
+    data: pd.DataFrame,
+    quasi_ident: typing.Union[typing.List, np.ndarray],
+    sens_att: typing.Union[typing.List, np.ndarray],
+    imp=False,
+    gen=True,
+) -> typing.Tuple[float, int]:
     """Calculate c and l for recursive (c,l)-diversity.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
@@ -169,47 +177,48 @@
             equiv_class = aux_anonymity.get_equiv_class(data, quasi_ident)
             for sens_att_value in sens_att:
                 c_sa = []
                 for ec in equiv_class:
                     data_temp = data.iloc[aux_functions.convert(ec)]
                     values = np.unique(data_temp[sens_att_value].values)
                     r_ec = np.sort(
-                        [
-                            len(data_temp[data_temp[sens_att_value] == s])
-                            for s in values
-                        ]
+                        [len(data_temp[data_temp[sens_att_value] == s]) for s in values]
+                    )
+                    c_sa.append(
+                        np.floor(r_ec[0] / sum(r_ec[l_div - 1 :]) + 1)  # noqa: E203
                     )
-                    c_sa.append(np.floor(r_ec[0]/sum(r_ec[l_div - 1:]) + 1))
                 c_div_aux.append(int(max(c_sa)))
         else:
             for i, sa in enumerate(sens_att):
                 tmp_qi = np.concatenate([quasi_ident, np.delete(sens_att, i)])
                 equiv_class = aux_anonymity.get_equiv_class(data, tmp_qi)
                 c_sa = []
                 for ec in equiv_class:
                     data_temp = data.iloc[aux_functions.convert(ec)]
                     values = np.unique(data_temp[sa].values)
-                    r_ec = np.sort([len(data_temp[data_temp[sa] == s])
-                                   for s in values])
-                    c_sa.append(np.floor(r_ec[0]/sum(r_ec[l_div - 1:]) + 1))
+                    r_ec = np.sort([len(data_temp[data_temp[sa] == s]) for s in values])
+                    c_sa.append(
+                        np.floor(r_ec[0] / sum(r_ec[l_div - 1 :]) + 1)  # noqa: E203
+                    )
                 c_div_aux.append(int(max(c_sa)))
         c_div = np.max(c_div_aux)
     else:
         if imp:
-            print(f'c for (c,l)-diversity cannot be calculated as l={l_div}')
+            print(f"c for (c,l)-diversity cannot be calculated as l={l_div}")
         c_div = np.nan
     return c_div, l_div
 
 
-def _achieve_l_diversity(data: pd.DataFrame,
-                         quasi_ident: typing.Union[typing.List, np.ndarray],
-                         sens_att: typing.Union[typing.List, np.ndarray],
-                         l_new: int) -> pd.DataFrame:
-    """Given l, transform the dataset into a new one checking l-diversity for
-    the new l, only using suppression.
+def _achieve_l_diversity(
+    data: pd.DataFrame,
+    quasi_ident: typing.Union[typing.List, np.ndarray],
+    sens_att: typing.Union[typing.List, np.ndarray],
+    l_new: int,
+) -> pd.DataFrame:
+    """Transform dataset checking l-diversity for l, using suppression.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
     :type quasi_ident: list of strings
@@ -230,14 +239,15 @@
     aux_functions.check_sa(data, sens_att)
     equiv_class = aux_anonymity.get_equiv_class(data, quasi_ident)
     l_ec = []
     for ec in equiv_class:
         data_temp = data.iloc[aux_functions.convert(ec)]
         l_sa = [len(np.unique(data_temp[sa].values)) for sa in sens_att]
         l_ec.append(min(l_sa))
-    data_ec_l = pd.DataFrame({'equiv_class': equiv_class, 'l_ec': l_ec})
-    data_ec_l = data_ec_l[data_ec_l.l_ec < l_new]
-    ec_elim = np.concatenate([aux_functions.convert(x)
-                             for x in data_ec_l.equiv_class.values])
+    aux = pd.DataFrame({"equiv_class": equiv_class, "l_ec": l_ec})
+    data_ec_l = aux[aux.l_ec < l_new]
+    ec_elim = np.concatenate(
+        [aux_functions.convert(x) for x in data_ec_l.equiv_class.values]
+    )
     data_new = data.drop(ec_elim).reset_index()
-    data_new.drop('index', inplace=True, axis=1)
+    data_new.drop("index", inplace=True, axis=1)
     return data_new
```

### Comparing `pycanon-1.0.0.post5/pycanon/anonymity/_t_closeness.py` & `pycanon-1.0.1/pycanon/anonymity/_t_closeness.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 import numpy as np
 import pandas as pd
 
 from pycanon.anonymity.utils import aux_anonymity
 from pycanon.anonymity.utils import aux_functions
 
 
-def t_closeness(data: pd.DataFrame,
-                quasi_ident: typing.Union[typing.List, np.ndarray],
-                sens_att: typing.Union[typing.List, np.ndarray],
-                gen=True) -> float:
+def t_closeness(
+    data: pd.DataFrame,
+    quasi_ident: typing.Union[typing.List, np.ndarray],
+    sens_att: typing.Union[typing.List, np.ndarray],
+    gen=True,
+) -> float:
     """Calculate t for t-closeness.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
@@ -51,27 +53,31 @@
     sens_att = np.array(sens_att)
     aux_functions.check_qi(data, quasi_ident)
     aux_functions.check_sa(data, sens_att)
     t_sens_att = []
     if gen:
         for sens_att_value in sens_att:
             if pd.api.types.is_numeric_dtype(data[sens_att_value]):
-                t_sens_att.append(aux_anonymity.aux_t_closeness_num(
-                    data, quasi_ident, sens_att_value))
+                t_sens_att.append(
+                    aux_anonymity.aux_t_closeness_num(data, quasi_ident, sens_att_value)
+                )
             elif pd.api.types.is_string_dtype(data[sens_att_value]):
-                t_sens_att.append(aux_anonymity.aux_t_closeness_str(
-                    data, quasi_ident, sens_att_value))
+                t_sens_att.append(
+                    aux_anonymity.aux_t_closeness_str(data, quasi_ident, sens_att_value)
+                )
             else:
-                raise ValueError('Error, invalid sens_att value type')
+                raise ValueError("Error, invalid sens_att value type")
     else:
         for i, sens_att_value in enumerate(sens_att):
             if pd.api.types.is_numeric_dtype(data[sens_att_value]):
                 tmp_qi = np.concatenate([quasi_ident, np.delete(sens_att, i)])
-                t_sens_att.append(aux_anonymity.aux_t_closeness_num(
-                    data, tmp_qi, sens_att_value))
+                t_sens_att.append(
+                    aux_anonymity.aux_t_closeness_num(data, tmp_qi, sens_att_value)
+                )
             elif pd.api.types.is_string_dtype(data[sens_att_value]):
                 tmp_qi = np.concatenate([quasi_ident, np.delete(sens_att, i)])
-                t_sens_att.append(aux_anonymity.aux_t_closeness_str(
-                    data, tmp_qi, sens_att_value))
+                t_sens_att.append(
+                    aux_anonymity.aux_t_closeness_str(data, tmp_qi, sens_att_value)
+                )
             else:
-                raise ValueError('Error, invalid sens_att value type')
+                raise ValueError("Error, invalid sens_att value type")
     return max(t_sens_att)
```

### Comparing `pycanon-1.0.0.post5/pycanon/anonymity/utils/__init__.py` & `pycanon-1.0.1/pycanon/anonymity/utils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,11 +10,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""Package containing auxiliary functions related with privacy models."""
+
 __all__ = [
     "aux_anonymity",
     "aux_functions",
 ]
```

### Comparing `pycanon-1.0.0.post5/pycanon/anonymity/utils/aux_anonymity.py` & `pycanon-1.0.1/pycanon/anonymity/utils/aux_anonymity.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 import numpy as np
 import pandas as pd
 from pycanon.anonymity.utils import aux_functions
 
 from typing import Tuple, Union
 
 
-def get_equiv_class(data: pd.DataFrame,
-                    quasi_ident: Union[list, np.ndarray]) -> list:
+def get_equiv_class(data: pd.DataFrame, quasi_ident: Union[list, np.ndarray]) -> list:
     """Find the equivalence classes present in the dataset.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are the quasi-identifiers.
@@ -53,17 +52,17 @@
     while len(equiv_class) > 1:
         equiv_class = aux_functions.intersect(equiv_class)
         equiv_class = sorted(equiv_class, key=lambda x: len(x))
     equiv_class = [x for x in equiv_class[0] if len(x) > 0]
     return equiv_class
 
 
-def aux_calculate_beta(data: pd.DataFrame,
-                       quasi_ident: Union[list, np.ndarray],
-                       sens_att_value: str) -> Tuple[np.ndarray, list]:
+def aux_calculate_beta(
+    data: pd.DataFrame, quasi_ident: Union[list, np.ndarray], sens_att_value: str
+) -> Tuple[np.ndarray, list]:
     """Beta calculation for basic and enhanced beta-likeness.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
@@ -74,33 +73,29 @@
 
     :return: proportion of each value of the sensitive attribute in the entire
         database and distance from the proportion in each equivalence class.
     :rtype: np.array and list.
     """
     equiv_class = get_equiv_class(data, quasi_ident)
     values = np.unique(data[sens_att_value].values)
-    p = np.array([len(data[data[sens_att_value] == s]) / len(data)
-                  for s in values])
+    p = np.array([len(data[data[sens_att_value] == s]) / len(data) for s in values])
     q = []
     for ec in equiv_class:
         data_temp = data.iloc[aux_functions.convert(ec)]
         qi = np.array(
-            [
-                len(data_temp[data_temp[sens_att_value] == s]) / len(ec)
-                for s in values
-            ]
+            [len(data_temp[data_temp[sens_att_value] == s]) / len(ec) for s in values]
         )
         q.append(qi)
     dist = [max((q[i] - p) / p) for i in range(len(equiv_class))]
     return p, dist
 
 
-def aux_calculate_delta_disclosure(data: pd.DataFrame,
-                                   quasi_ident: Union[list, np.ndarray],
-                                   sens_att_value: str) -> float:
+def aux_calculate_delta_disclosure(
+    data: pd.DataFrame, quasi_ident: Union[list, np.ndarray], sens_att_value: str
+) -> float:
     """Delta calculation for delta-disclosure privacy.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
@@ -110,34 +105,30 @@
     :type sens_att_value: string
 
     :return: delta for the introduced SA.
     :rtype: float.
     """
     equiv_class = get_equiv_class(data, quasi_ident)
     values = np.unique(data[sens_att_value].values)
-    p = np.array([len(data[data[sens_att_value] == s]) / len(data)
-                  for s in values])
+    p = np.array([len(data[data[sens_att_value] == s]) / len(data) for s in values])
     q = []
     for ec in equiv_class:
         data_temp = data.iloc[aux_functions.convert(ec)]
         qi = np.array(
-            [
-                len(data_temp[data_temp[sens_att_value] == s]) / len(ec)
-                for s in values
-            ]
+            [len(data_temp[data_temp[sens_att_value] == s]) / len(ec) for s in values]
         )
         q.append(qi)
     aux = [max([np.abs(np.log(x)) for x in qi / p if x > 0]) for qi in q]
     return max(aux)
 
 
-def aux_t_closeness_num(data: pd.DataFrame,
-                        quasi_ident: Union[list, np.ndarray],
-                        sens_att_value: str) -> float:
-    """t calculation for t-closeness.
+def aux_t_closeness_num(
+    data: pd.DataFrame, quasi_ident: Union[list, np.ndarray], sens_att_value: str
+) -> float:
+    """Obtain t for t-closeness.
 
     Function used for numerical attributes: the definition of the EMD is used.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
@@ -149,39 +140,35 @@
 
     :return: t for the introduced SA (numerical).
     :rtype: float.
     """
     equiv_class = get_equiv_class(data, quasi_ident)
     values = np.unique(data[sens_att_value].values)
     m = len(values)
-    p = np.array([len(data[data[sens_att_value] == s]) / len(data)
-                  for s in values])
+    p = np.array([len(data[data[sens_att_value] == s]) / len(data) for s in values])
     emd = []
     for ec in equiv_class:
         data_temp = data.iloc[aux_functions.convert(ec)]
         qi = np.array(
-            [
-                len(data_temp[data_temp[sens_att_value] == s]) / len(ec)
-                for s in values
-            ]
+            [len(data_temp[data_temp[sens_att_value] == s]) / len(ec) for s in values]
         )
         r = qi - p
         abs_r, emd_ec = 0.0, 0.0
         for i in range(m):
             abs_r += r[i]
             emd_ec += np.abs(abs_r)
         emd_ec = 1 / (m - 1) * emd_ec
         emd.append(emd_ec)
     return max(emd)
 
 
-def aux_t_closeness_str(data: pd.DataFrame,
-                        quasi_ident: Union[list, np.ndarray],
-                        sens_att_value: list) -> float:
-    """t calculation for t-closeness.
+def aux_t_closeness_str(
+    data: pd.DataFrame, quasi_ident: Union[list, np.ndarray], sens_att_value: list
+) -> float:
+    """Obtain t for for t-closeness.
 
     Function used for categorical attributes: the metric "Equal Distance" is
     used.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
@@ -194,24 +181,20 @@
 
     :return: t for the introduced SA (categorical).
     :rtype: float.
     """
     equiv_class = get_equiv_class(data, quasi_ident)
     values = np.unique(data[sens_att_value].values)
     m = len(values)
-    p = np.array([len(data[data[sens_att_value] == s]) / len(data)
-                  for s in values])
+    p = np.array([len(data[data[sens_att_value] == s]) / len(data) for s in values])
     emd = []
     for ec in equiv_class:
         data_temp = data.iloc[aux_functions.convert(ec)]
         qi = np.array(
-            [
-                len(data_temp[data_temp[sens_att_value] == s]) / len(ec)
-                for s in values
-            ]
+            [len(data_temp[data_temp[sens_att_value] == s]) / len(ec) for s in values]
         )
         r = qi - p
         emd_ec = 0.0
         for i in range(m):
             emd_ec += np.abs(r[i])
         emd_ec = 0.5 * emd_ec
         emd.append(emd_ec)
```

### Comparing `pycanon-1.0.0.post5/pycanon/anonymity/utils/aux_functions.py` & `pycanon-1.0.1/pycanon/anonymity/utils/aux_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,118 +10,130 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-"""
-Module with different auxiliary functions.
-"""
+"""Module with different auxiliary functions."""
 
 import os
 import pathlib
 import typing
 
 import numpy as np
 import pandas as pd
 
 
-def read_file(file_name: typing.Union[str, pathlib.Path]) -> pd.DataFrame:
+def read_file(
+    file_name: typing.Union[str, pathlib.Path], sep: str = ","
+) -> pd.DataFrame:
     """Read the given file. Returns a pandas dataframe.
 
     :param file_name: file with the data under study.
     :type file_name: string or pathlib.Path
 
+    :param sep: delimiter to use for a csv file.
+    :type sep: string
+
     :return: dataframe with the data.
     :rtype: pandas dataframe.
     """
     if isinstance(file_name, str):
         file_name = pathlib.Path(file_name)
 
     _, file_extension = os.path.splitext(file_name)
-    if file_extension in ['.csv', '.xlsx', '.sav', '.txt']:
-        if file_extension in ['.csv', '.txt']:
+    if file_extension in [".csv", ".xlsx", ".sav", ".txt"]:
+        if file_extension in [".csv", ".txt"]:
             data = pd.read_csv(file_name)
-        elif file_extension == '.xlsx':
+        elif file_extension == ".xlsx":
             data = pd.read_excel(file_name)
         else:
             data = pd.read_spss(file_name)
     else:
-        raise ValueError('Invalid file extension.')
+        raise ValueError("Invalid file extension.")
     return data
 
 
-def check_qi(data: pd.DataFrame,
-             quasi_ident: typing.Union[typing.List, np.ndarray]) -> None:
-    """Checks if the entered quasi-identifiers are valid.
+def check_qi(
+    data: pd.DataFrame, quasi_ident: typing.Union[typing.List, np.ndarray]
+) -> None:
+    """Check if the entered quasi-identifiers are valid.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
     :type quasi_ident: list of strings
     """
     cols = data.columns
-    err_val = [i for i, v in enumerate(
-        [qi in cols for qi in quasi_ident]) if v is False]
+    err_val = [
+        i for i, v in enumerate([qi in cols for qi in quasi_ident]) if v is False
+    ]
     if len(err_val) > 0:
         raise ValueError(
-            f'Values not defined: {[quasi_ident[i] for i in err_val]}. '
-            'Cannot be quasi-identifiers'
+            f"Values not defined: {[quasi_ident[i] for i in err_val]}. "
+            "Cannot be quasi-identifiers"
         )
 
 
-def check_sa(data: pd.DataFrame,
-             sens_att: typing.Union[typing.List, np.ndarray]) -> None:
-    """Checks if the entered sensitive attributes are valid.
+def check_sa(
+    data: pd.DataFrame, sens_att: typing.Union[typing.List, np.ndarray]
+) -> None:
+    """Check if the entered sensitive attributes are valid.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param sens_att: list with the name of the columns of the dataframe
         that are the sensitive attributes.
     :type sens_att: is a list of strings
     """
     cols = data.columns
-    err_val = [i for i, v in enumerate(
-        [sa in cols for sa in sens_att]) if v is False]
+    err_val = [i for i, v in enumerate([sa in cols for sa in sens_att]) if v is False]
     if len(err_val) > 0:
         raise ValueError(
-            f'Values not defined: {[sens_att[i] for i in err_val]}. '
-            'Cannot be sensitive attributes')
+            f"Values not defined: {[sens_att[i] for i in err_val]}. "
+            "Cannot be sensitive attributes"
+        )
 
 
 def intersect(tmp: list) -> list:
     """Intersect two sets: the first and the second of the given list.
 
     :param tmp: list of sets sorted in decreasing order of
         cardinality
     :type tmp: list of numpy arrays
+
+    :return: list obtained when intersecting the first and the second sets
+        of the given list.
+    :rtype: list.
     """
     i, j = 0, 0
     tmp_new = []
     while i < len(tmp[0]):
         tmp1 = tmp[0][i]
         tmp2 = tmp[1][j]
         tmp_new.append(np.intersect1d(tmp1, tmp2))
-        if j < len(tmp[1])-1:
+        if j < len(tmp[1]) - 1:
             j += 1
         else:
             j = 0
             i += 1
     tmp[1] = tmp_new
     tmp = tmp[1:]
     return tmp
 
 
 def convert(ec_set: set) -> list:
-    """Converts a set with an equivalence class to a list.
+    """Convert a set with an equivalence class to a list.
 
     :param ec_set: set which will be convert into a list.
     :type ec_set: set
 
     :return: equivalence class into a list.
     :rtype: list.
     """
-    return [*ec_set, ]
+    return [
+        *ec_set,
+    ]
```

### Comparing `pycanon-1.0.0.post5/pycanon/cli.py` & `pycanon-1.0.1/pycanon/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""Module providing command line tools for pyCANON."""
+
 import pathlib
 import typing
 
 import tabulate
 import typer
 
 import pycanon
@@ -25,337 +27,338 @@
 from pycanon.anonymity.utils import aux_functions
 
 app = typer.Typer()
 
 
 @app.command()
 def k_anonymity(
-        filename: pathlib.Path = typer.Argument(
-            ...,
-            exists=True,
-            file_okay=True,
-            dir_okay=False,
-            writable=False,
-            readable=True,
-            resolve_path=True,
-        ),
-        qi: typing.List[str] = typer.Option(
-            ...,
-            help="Quasi-identifier, pass it multiple times to define multiple "
-                 "quasi-identifiers (QI)."
-        )
+    filename: pathlib.Path = typer.Argument(
+        ...,
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        writable=False,
+        readable=True,
+        resolve_path=True,
+    ),
+    qi: typing.List[str] = typer.Option(
+        ...,
+        help="Quasi-identifier, pass it multiple times to define multiple "
+        "quasi-identifiers (QI).",
+    ),
 ):
     """Calculate k-anonymity."""
     dataset = aux_functions.read_file(filename)
     typer.echo(anonymity.k_anonymity(dataset, qi))
 
 
 @app.command()
 def alpha_k_anonymity(
-        filename: pathlib.Path = typer.Argument(
-            ...,
-            exists=True,
-            file_okay=True,
-            dir_okay=False,
-            writable=False,
-            readable=True,
-            resolve_path=True,
-        ),
-        qi: typing.List[str] = typer.Option(
-            ...,
-            help="Quasi-identifier, pass it multiple times to define multiple "
-                 "quasi-identifiers (QI)."
-        ),
-        sa: typing.List[str] = typer.Option(
-            ...,
-            help="Sensitive attribute, pass it multiple times to define "
-                 "multiple sensitive attributes (SA)."
-        ),
-        gen: bool = typer.Option(
-            True,
-            help="Whether to generalize for the case of "
-                 "multiple SA: If true, generalization approach is applied, "
-                 "if False, the set of QI is updated for each SA."
-        )
+    filename: pathlib.Path = typer.Argument(
+        ...,
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        writable=False,
+        readable=True,
+        resolve_path=True,
+    ),
+    qi: typing.List[str] = typer.Option(
+        ...,
+        help="Quasi-identifier, pass it multiple times to define multiple "
+        "quasi-identifiers (QI).",
+    ),
+    sa: typing.List[str] = typer.Option(
+        ...,
+        help="Sensitive attribute, pass it multiple times to define "
+        "multiple sensitive attributes (SA).",
+    ),
+    gen: bool = typer.Option(
+        True,
+        help="Whether to generalize for the case of "
+        "multiple SA: If true, generalization approach is applied, "
+        "if False, the set of QI is updated for each SA.",
+    ),
 ):
     """Calculate (alpha,k)-anonymity."""
     dataset = aux_functions.read_file(filename)
     typer.echo(anonymity.alpha_k_anonymity(dataset, qi, sa, gen))
 
 
 @app.command()
 def l_diversity(
-        filename: pathlib.Path = typer.Argument(
-            ...,
-            exists=True,
-            file_okay=True,
-            dir_okay=False,
-            writable=False,
-            readable=True,
-            resolve_path=True,
-        ),
-        qi: typing.List[str] = typer.Option(
-            ...,
-            help="Quasi-identifier, pass it multiple times to define multiple "
-                 "quasi-identifiers (QI)."
-        ),
-        sa: typing.List[str] = typer.Option(
-            ...,
-            help="Sensitive attribute, pass it multiple times to define "
-                 "multiple sensitive attributes (SA)."
-        ),
-        gen: bool = typer.Option(
-            True,
-            help="Whether to generalize for the case of "
-                 "multiple SA: If true, generalization approach is applied, "
-                 "if False, the set of QI is updated for each SA."
-        )
+    filename: pathlib.Path = typer.Argument(
+        ...,
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        writable=False,
+        readable=True,
+        resolve_path=True,
+    ),
+    qi: typing.List[str] = typer.Option(
+        ...,
+        help="Quasi-identifier, pass it multiple times to define multiple "
+        "quasi-identifiers (QI).",
+    ),
+    sa: typing.List[str] = typer.Option(
+        ...,
+        help="Sensitive attribute, pass it multiple times to define "
+        "multiple sensitive attributes (SA).",
+    ),
+    gen: bool = typer.Option(
+        True,
+        help="Whether to generalize for the case of "
+        "multiple SA: If true, generalization approach is applied, "
+        "if False, the set of QI is updated for each SA.",
+    ),
 ):
     """Calculate l-diversity."""
     dataset = aux_functions.read_file(filename)
     typer.echo(anonymity.l_diversity(dataset, qi, sa, gen))
 
 
 @app.command()
 def entropy_l_diversity(
-        filename: pathlib.Path = typer.Argument(
-            ...,
-            exists=True,
-            file_okay=True,
-            dir_okay=False,
-            writable=False,
-            readable=True,
-            resolve_path=True,
-        ),
-        qi: typing.List[str] = typer.Option(
-            ...,
-            help="Quasi-identifier, pass it multiple times to define multiple "
-                 "quasi-identifiers (QI)."
-        ),
-        sa: typing.List[str] = typer.Option(
-            ...,
-            help="Sensitive attribute, pass it multiple times to define "
-                 "multiple sensitive attributes (SA)."
-        ),
-        gen: bool = typer.Option(
-            True,
-            help="Whether to generalize for the case of "
-                 "multiple SA: If true, generalization approach is applied, "
-                 "if False, the set of QI is updated for each SA."
-        )
+    filename: pathlib.Path = typer.Argument(
+        ...,
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        writable=False,
+        readable=True,
+        resolve_path=True,
+    ),
+    qi: typing.List[str] = typer.Option(
+        ...,
+        help="Quasi-identifier, pass it multiple times to define multiple "
+        "quasi-identifiers (QI).",
+    ),
+    sa: typing.List[str] = typer.Option(
+        ...,
+        help="Sensitive attribute, pass it multiple times to define "
+        "multiple sensitive attributes (SA).",
+    ),
+    gen: bool = typer.Option(
+        True,
+        help="Whether to generalize for the case of "
+        "multiple SA: If true, generalization approach is applied, "
+        "if False, the set of QI is updated for each SA.",
+    ),
 ):
     """Calculate entropy l-diversity."""
     dataset = aux_functions.read_file(filename)
     typer.echo(anonymity.entropy_l_diversity(dataset, qi, sa, gen))
 
 
 @app.command()
 def recursive_c_l_diversity(
-        filename: pathlib.Path = typer.Argument(
-            ...,
-            exists=True,
-            file_okay=True,
-            dir_okay=False,
-            writable=False,
-            readable=True,
-            resolve_path=True,
-        ),
-        qi: typing.List[str] = typer.Option(
-            ...,
-            help="Quasi-identifier, pass it multiple times to define multiple "
-                 "quasi-identifiers (QI)."
-        ),
-        sa: typing.List[str] = typer.Option(
-            ...,
-            help="Sensitive attribute, pass it multiple times to define "
-                 "multiple sensitive attributes (SA)."
-        ),
-        gen: bool = typer.Option(
-            True,
-            help="Whether to generalize for the case of "
-                 "multiple SA: If true, generalization approach is applied, "
-                 "if False, the set of QI is updated for each SA."
-        )
+    filename: pathlib.Path = typer.Argument(
+        ...,
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        writable=False,
+        readable=True,
+        resolve_path=True,
+    ),
+    qi: typing.List[str] = typer.Option(
+        ...,
+        help="Quasi-identifier, pass it multiple times to define multiple "
+        "quasi-identifiers (QI).",
+    ),
+    sa: typing.List[str] = typer.Option(
+        ...,
+        help="Sensitive attribute, pass it multiple times to define "
+        "multiple sensitive attributes (SA).",
+    ),
+    gen: bool = typer.Option(
+        True,
+        help="Whether to generalize for the case of "
+        "multiple SA: If true, generalization approach is applied, "
+        "if False, the set of QI is updated for each SA.",
+    ),
 ):
     """Calculate recursive (c,l)-diversity."""
     dataset = aux_functions.read_file(filename)
     typer.echo(anonymity.recursive_c_l_diversity(dataset, qi, sa, gen))
 
 
 @app.command()
 def basic_beta_likeness(
-        filename: pathlib.Path = typer.Argument(
-            ...,
-            exists=True,
-            file_okay=True,
-            dir_okay=False,
-            writable=False,
-            readable=True,
-            resolve_path=True,
-        ),
-        qi: typing.List[str] = typer.Option(
-            ...,
-            help="Quasi-identifier, pass it multiple times to define multiple "
-                 "quasi-identifiers (QI)."
-        ),
-        sa: typing.List[str] = typer.Option(
-            ...,
-            help="Sensitive attribute, pass it multiple times to define "
-                 "multiple sensitive attributes (SA)."
-        ),
-        gen: bool = typer.Option(
-            True,
-            help="Whether to generalize for the case of "
-                 "multiple SA: If true, generalization approach is applied, "
-                 "if False, the set of QI is updated for each SA."
-        )
+    filename: pathlib.Path = typer.Argument(
+        ...,
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        writable=False,
+        readable=True,
+        resolve_path=True,
+    ),
+    qi: typing.List[str] = typer.Option(
+        ...,
+        help="Quasi-identifier, pass it multiple times to define multiple "
+        "quasi-identifiers (QI).",
+    ),
+    sa: typing.List[str] = typer.Option(
+        ...,
+        help="Sensitive attribute, pass it multiple times to define "
+        "multiple sensitive attributes (SA).",
+    ),
+    gen: bool = typer.Option(
+        True,
+        help="Whether to generalize for the case of "
+        "multiple SA: If true, generalization approach is applied, "
+        "if False, the set of QI is updated for each SA.",
+    ),
 ):
     """Calculate basic beta-likeness."""
     dataset = aux_functions.read_file(filename)
     typer.echo(anonymity.basic_beta_likeness(dataset, qi, sa, gen))
 
 
 @app.command()
 def enhanced_beta_likeness(
-        filename: pathlib.Path = typer.Argument(
-            ...,
-            exists=True,
-            file_okay=True,
-            dir_okay=False,
-            writable=False,
-            readable=True,
-            resolve_path=True,
-        ),
-        qi: typing.List[str] = typer.Option(
-            ...,
-            help="Quasi-identifier, pass it multiple times to define multiple "
-                 "quasi-identifiers (QI)."
-        ),
-        sa: typing.List[str] = typer.Option(
-            ...,
-            help="Sensitive attribute, pass it multiple times to define "
-                 "multiple sensitive attributes (SA)."
-        ),
-        gen: bool = typer.Option(
-            True,
-            help="Whether to generalize for the case of "
-                 "multiple SA: If true, generalization approach is applied, "
-                 "if False, the set of QI is updated for each SA."
-        )
+    filename: pathlib.Path = typer.Argument(
+        ...,
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        writable=False,
+        readable=True,
+        resolve_path=True,
+    ),
+    qi: typing.List[str] = typer.Option(
+        ...,
+        help="Quasi-identifier, pass it multiple times to define multiple "
+        "quasi-identifiers (QI).",
+    ),
+    sa: typing.List[str] = typer.Option(
+        ...,
+        help="Sensitive attribute, pass it multiple times to define "
+        "multiple sensitive attributes (SA).",
+    ),
+    gen: bool = typer.Option(
+        True,
+        help="Whether to generalize for the case of "
+        "multiple SA: If true, generalization approach is applied, "
+        "if False, the set of QI is updated for each SA.",
+    ),
 ):
     """Calculate enhanced beta-likeness."""
     dataset = aux_functions.read_file(filename)
     typer.echo(anonymity.enhanced_beta_likeness(dataset, qi, sa, gen))
 
 
 @app.command()
 def t_closeness(
-        filename: pathlib.Path = typer.Argument(
-            ...,
-            exists=True,
-            file_okay=True,
-            dir_okay=False,
-            writable=False,
-            readable=True,
-            resolve_path=True,
-        ),
-        qi: typing.List[str] = typer.Option(
-            ...,
-            help="Quasi-identifier, pass it multiple times to define multiple "
-                 "quasi-identifiers (QI)."
-        ),
-        sa: typing.List[str] = typer.Option(
-            ...,
-            help="Sensitive attribute, pass it multiple times to define "
-                 "multiple sensitive attributes (SA)."
-        ),
-        gen: bool = typer.Option(
-            True,
-            help="Whether to generalize for the case of "
-                 "multiple SA: If true, generalization approach is applied, "
-                 "if False, the set of QI is updated for each SA."
-        )
+    filename: pathlib.Path = typer.Argument(
+        ...,
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        writable=False,
+        readable=True,
+        resolve_path=True,
+    ),
+    qi: typing.List[str] = typer.Option(
+        ...,
+        help="Quasi-identifier, pass it multiple times to define multiple "
+        "quasi-identifiers (QI).",
+    ),
+    sa: typing.List[str] = typer.Option(
+        ...,
+        help="Sensitive attribute, pass it multiple times to define "
+        "multiple sensitive attributes (SA).",
+    ),
+    gen: bool = typer.Option(
+        True,
+        help="Whether to generalize for the case of "
+        "multiple SA: If true, generalization approach is applied, "
+        "if False, the set of QI is updated for each SA.",
+    ),
 ):
     """Calculate t-closeness."""
     dataset = aux_functions.read_file(filename)
     typer.echo(anonymity.t_closeness(dataset, qi, sa, gen))
 
 
 @app.command()
 def delta_disclosure(
-        filename: pathlib.Path = typer.Argument(
-            ...,
-            exists=True,
-            file_okay=True,
-            dir_okay=False,
-            writable=False,
-            readable=True,
-            resolve_path=True,
-        ),
-        qi: typing.List[str] = typer.Option(
-            ...,
-            help="Quasi-identifier, pass it multiple times to define multiple "
-                 "quasi-identifiers (QI)."
-        ),
-        sa: typing.List[str] = typer.Option(
-            ...,
-            help="Sensitive attribute, pass it multiple times to define "
-                 "multiple sensitive attributes (SA)."
-        ),
-        gen: bool = typer.Option(
-            True,
-            help="Whether to generalize for the case of "
-                 "multiple SA: If true, generalization approach is applied, "
-                 "if False, the set of QI is updated for each SA."
-        )
+    filename: pathlib.Path = typer.Argument(
+        ...,
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        writable=False,
+        readable=True,
+        resolve_path=True,
+    ),
+    qi: typing.List[str] = typer.Option(
+        ...,
+        help="Quasi-identifier, pass it multiple times to define multiple "
+        "quasi-identifiers (QI).",
+    ),
+    sa: typing.List[str] = typer.Option(
+        ...,
+        help="Sensitive attribute, pass it multiple times to define "
+        "multiple sensitive attributes (SA).",
+    ),
+    gen: bool = typer.Option(
+        True,
+        help="Whether to generalize for the case of "
+        "multiple SA: If true, generalization approach is applied, "
+        "if False, the set of QI is updated for each SA.",
+    ),
 ):
     """Calculate delta-disclosure."""
     dataset = aux_functions.read_file(filename)
     typer.echo(anonymity.delta_disclosure(dataset, qi, sa, gen))
 
 
 @app.command()
 def report(
-        filename: pathlib.Path = typer.Argument(
-            ...,
-            exists=True,
-            file_okay=True,
-            dir_okay=False,
-            writable=False,
-            readable=True,
-            resolve_path=True,
-        ),
-        qi: typing.List[str] = typer.Option(
-            ...,
-            help="Quasi-identifier, pass it multiple times to define multiple "
-                 "quasi-identifiers (QI)."
-        ),
-        sa: typing.List[str] = typer.Option(
-            ...,
-            help="Sensible attribute, pass it multiple times to define "
-                 "multiple sensible attributes (SA)."
-        ),
-        gen: bool = typer.Option(
-            True,
-            help="Whether to generalize for the case of "
-                 "multiple SA: If true, generalization approach is applied, "
-                 "if False, the set of QI is updated for each SA."
-        )
+    filename: pathlib.Path = typer.Argument(
+        ...,
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        writable=False,
+        readable=True,
+        resolve_path=True,
+    ),
+    qi: typing.List[str] = typer.Option(
+        ...,
+        help="Quasi-identifier, pass it multiple times to define multiple "
+        "quasi-identifiers (QI).",
+    ),
+    sa: typing.List[str] = typer.Option(
+        ...,
+        help="Sensible attribute, pass it multiple times to define "
+        "multiple sensible attributes (SA).",
+    ),
+    gen: bool = typer.Option(
+        True,
+        help="Whether to generalize for the case of "
+        "multiple SA: If true, generalization approach is applied, "
+        "if False, the set of QI is updated for each SA.",
+    ),
 ):
     """Generate a complete privacy report."""
     dataset = aux_functions.read_file(filename)
 
     headers = ["Technique", "Values"]
 
     k_anon = anonymity.k_anonymity(dataset, qi)
     alpha, alpha_k = anonymity.alpha_k_anonymity(dataset, qi, sa, gen=gen)
     l_div = anonymity.l_diversity(dataset, qi, sa, gen=gen)
     entropy_l = anonymity.entropy_l_diversity(dataset, qi, sa, gen=gen)
-    c_div, l_c_div = anonymity.recursive_c_l_diversity(dataset, qi, sa,
-                                                       imp=False, gen=gen)
+    c_div, l_c_div = anonymity.recursive_c_l_diversity(
+        dataset, qi, sa, imp=False, gen=gen
+    )
     basic_beta = anonymity.basic_beta_likeness(dataset, qi, sa, gen=gen)
     enhanced_beta = anonymity.enhanced_beta_likeness(dataset, qi, sa, gen=gen)
     delta_disc = anonymity.delta_disclosure(dataset, qi, sa, gen=gen)
     t_clos = anonymity.t_closeness(dataset, qi, sa, gen=gen)
 
     vals = [
         ["k-anonymity", f"k = {k_anon}"],
@@ -369,29 +372,29 @@
         ["delta-disclosure", f"delta = {delta_disc}"],
     ]
 
     typer.echo(tabulate.tabulate(vals, headers=headers))
 
 
 def version_callback(version: bool):
+    """Return version info."""
     if version:
         typer.echo(pycanon.__version__)
         raise typer.Exit()
 
 
 @app.callback()
 def main(
     version: typing.Optional[bool] = typer.Option(
         False,
         "--version",
         help="Print version and exit",
         callback=version_callback,
-        is_eager=True
+        is_eager=True,
     )
 ):
     """Check the level of anonymity of a dataset."""
-
     pass
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pycanon-1.0.0.post5/pycanon/report/__init__.py` & `pycanon-1.0.1/pycanon/report/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""Generate reports with all privacy model's scores."""
+
 import pandas as pd
 
 from pycanon.report.base import get_report_values
 from pycanon.report.json import get_json_report
 from pycanon.report.pdf import get_pdf_report
+from pycanon.report.pdf_utility_report import get_pdf_utility_report
 
 
-def print_report(data: pd.DataFrame,
-                 quasi_ident: list,
-                 sens_att: list,
-                 gen=True) -> None:
+def print_report(
+    data: pd.DataFrame, quasi_ident: list, sens_att: list, gen=True
+) -> None:
     """Generate a report with the parameters obtained for each anonymity check.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
@@ -38,31 +40,40 @@
         that are the sensitive attributes.
     :type sens_att: is a list of strings
 
     :param gen: default to true. If true it is generalized for the case of
         multiple SA, if False, the set of QI is updated for each SA.
     :type gen: boolean
     """
-
     (
-        k_anon, (alpha, alpha_k), l_div, entropy_l, (c_div, l_c_div),
-        basic_beta, enhanced_beta, delta_disc, t_clos
+        k_anon,
+        (alpha, alpha_k),
+        l_div,
+        entropy_l,
+        (c_div, l_c_div),
+        basic_beta,
+        enhanced_beta,
+        delta_disc,
+        t_clos,
     ) = get_report_values(data, quasi_ident, sens_att, gen=gen)
 
-    print(f'''The dataset verifies:
+    print(
+        f"""The dataset verifies:
           \t - k-anonymity with k = {k_anon}
           \t - (alpha,k)-anonymity with alpha = {alpha} and k = {k_anon}
           \t - l-diversity with l = {l_div}
           \t - entropy l-diversity with l = {entropy_l}
           \t - (c,l)-diversity with c = {c_div} and l = {l_div}
           \t - basic beta-likeness with beta = {basic_beta}
           \t - enhanced beta-likeness with beta = {enhanced_beta}
           \t - t-closeness with t = {t_clos}
-          \t - delta-disclosure privacy with delta = {delta_disc}''')
+          \t - delta-disclosure privacy with delta = {delta_disc}"""
+    )
 
 
 __all__ = [
     "print_report",
     "get_json_report",
     "get_pdf_report",
     "get_report_values",
+    "get_pdf_utility_report",
 ]
```

### Comparing `pycanon-1.0.0.post5/pycanon/report/base.py` & `pycanon-1.0.1/pycanon/report/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,33 +9,29 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
+
+"""Get report values for all privacy models."""
+
 from typing import Tuple, Any
 
 import pandas as pd
 
 from pycanon import anonymity
 
 
-def get_report_values(data: pd.DataFrame,
-                      quasi_ident: list,
-                      sens_att: list,
-                      gen=True) -> Tuple[int,
-                                         Tuple[float, int],
-                                         int,
-                                         float,
-                                         Tuple[Any, int],
-                                         float,
-                                         float,
-                                         float,
-                                         float]:
+def get_report_values(
+    data: pd.DataFrame, quasi_ident: list, sens_att: list, gen=True
+) -> Tuple[
+    int, Tuple[float, int], int, float, Tuple[Any, int], float, float, float, float
+]:
     """Generate a report with the parameters obtained for each anonymity check.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
@@ -45,39 +41,29 @@
         that are the sensitive attributes.
     :type sens_att: is a list of strings
 
     :param gen: default to true. If true it is generalized for the case of
         multiple SA, if False, the set of QI is updated for each SA.
     :type gen: boolean
     """
-
-    k_anon = anonymity.k_anonymity(
-        data, quasi_ident
-    )
-    alpha, alpha_k = anonymity.alpha_k_anonymity(
-        data, quasi_ident, sens_att, gen
-    )
-    l_div = anonymity.l_diversity(
-        data, quasi_ident, sens_att, gen
-    )
-    entropy_l = anonymity.entropy_l_diversity(
-        data, quasi_ident, sens_att, gen
-    )
-    c_div, l_c_div = anonymity.recursive_c_l_diversity(
-        data, quasi_ident, sens_att, gen
-    )
-    basic_beta = anonymity.basic_beta_likeness(
-        data, quasi_ident, sens_att, gen
-    )
-    enhanced_beta = anonymity.enhanced_beta_likeness(
-        data, quasi_ident, sens_att, gen
-    )
-    delta_disc = anonymity.delta_disclosure(
-        data, quasi_ident, sens_att, gen
-    )
-    t_clos = anonymity.t_closeness(
-        data, quasi_ident, sens_att, gen
-    )
+    k_anon = anonymity.k_anonymity(data, quasi_ident)
+    alpha, alpha_k = anonymity.alpha_k_anonymity(data, quasi_ident, sens_att, gen)
+    l_div = anonymity.l_diversity(data, quasi_ident, sens_att, gen)
+    entropy_l = anonymity.entropy_l_diversity(data, quasi_ident, sens_att, gen)
+    c_div, l_c_div = anonymity.recursive_c_l_diversity(data, quasi_ident, sens_att, gen)
+    basic_beta = anonymity.basic_beta_likeness(data, quasi_ident, sens_att, gen)
+    enhanced_beta = anonymity.enhanced_beta_likeness(data, quasi_ident, sens_att, gen)
+    delta_disc = anonymity.delta_disclosure(data, quasi_ident, sens_att, gen)
+    t_clos = anonymity.t_closeness(data, quasi_ident, sens_att, gen)
 
     # TODO(aloga): Move to a better data type here
-    return (k_anon, (alpha, alpha_k), l_div, entropy_l, (c_div, l_c_div),
-            basic_beta, enhanced_beta, delta_disc, t_clos)
+    return (
+        k_anon,
+        (alpha, alpha_k),
+        l_div,
+        entropy_l,
+        (c_div, l_c_div),
+        basic_beta,
+        enhanced_beta,
+        delta_disc,
+        t_clos,
+    )
```

### Comparing `pycanon-1.0.0.post5/pycanon/report/json.py` & `pycanon-1.0.1/pycanon/report/json.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,39 +10,40 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""Get report values as JSON for all privacy models."""
+
 import json
 import typing
 
 import numpy as np
 import pandas as pd
 
 from pycanon.report import base
 
 
-class NpEncoder(json.JSONEncoder):
+class _NpEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.floating):
             return float(obj)
         if isinstance(obj, np.ndarray):
             return obj.tolist()
-        return super(NpEncoder, self).default(obj)
+        return super(_NpEncoder, self).default(obj)
 
 
-def get_json_report(data: pd.DataFrame,
-                    quasi_ident: list,
-                    sens_att: list,
-                    gen=True) -> str:
-    """Generate a report with the parameters obtained for each anonymity check.
+def get_json_report(
+    data: pd.DataFrame, quasi_ident: list, sens_att: list, gen=True
+) -> str:
+    """Generate a report (JSON) with the parameters obtained for each anonymity check.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
     :type quasi_ident: list of strings
@@ -52,27 +53,32 @@
     :type sens_att: is a list of strings
 
     :param gen: default to true. If true it is generalized for the case of
         multiple SA, if False, the set of QI is updated for each SA.
     :type gen: boolean
     """
     (
-        k_anon, (alpha, alpha_k), l_div, entropy_l, (c_div, l_c_div),
-        basic_beta, enhanced_beta, delta_disc, t_clos
+        k_anon,
+        (alpha, alpha_k),
+        l_div,
+        entropy_l,
+        (c_div, l_c_div),
+        basic_beta,
+        enhanced_beta,
+        delta_disc,
+        t_clos,
     ) = base.get_report_values(data, quasi_ident, sens_att, gen=gen)
 
-    json_data: typing.Dict[str, typing.Any] = {}
-    json_data['data'] = {
-        'quasi-identifiers': quasi_ident,
-        'sensitive attributes': sens_att
+    json_data: typing.Dict[str, typing.Any] = {
+        "data": {"quasi-identifiers": quasi_ident, "sensitive attributes": sens_att},
+        "k_anonymity": {"k": k_anon},
+        "alpha_k_anonymity": {"alpha": alpha, "k": alpha_k},
+        "l_diversity": {"l": l_div},
+        "entropy_l_diversity": {"l": entropy_l},
+        "recursive_c_l_diversity": {"c": c_div, "l": l_c_div},
+        "basic_beta_likeness": {"beta": basic_beta},
+        "enhanced_beta_likeness": {"beta": enhanced_beta},
+        "t_closeness": {"t": t_clos},
+        "delta_disclosure": {"delta": delta_disc},
     }
-    json_data['k_anonymity'] = {'k': k_anon}
-    json_data['alpha_k_anonymity'] = {'alpha': alpha, 'k': alpha_k}
-    json_data['l_diversity'] = {'l': l_div}
-    json_data['entropy_l_diversity'] = {'l': entropy_l}
-    json_data['recursive_c_l_diversity'] = {'c': c_div, 'l': l_c_div}
-    json_data['basic_beta_likeness'] = {'beta': basic_beta}
-    json_data['enhanced_beta_likeness'] = {'beta': enhanced_beta}
-    json_data['t_closeness'] = {'t': t_clos}
-    json_data['delta_disclosure'] = {'delta': delta_disc}
 
-    return json.dumps(json_data, cls=NpEncoder)
+    return json.dumps(json_data, cls=_NpEncoder)
```

### Comparing `pycanon-1.0.0.post5/pycanon/report/pdf.py` & `pycanon-1.0.1/pycanon/report/pdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,33 +10,39 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+"""Get report values as PDF file for all privacy models."""
+
 from datetime import datetime
 import os
+import typing
 
+import numpy as np
 import pandas as pd
 from reportlab.lib.pagesizes import A4
 from reportlab.platypus import SimpleDocTemplate, Paragraph, Spacer
 from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle
 from reportlab.platypus.tables import Table
 from reportlab.lib import colors
 
 from pycanon.report import base
 
 
-def get_pdf_report(data: pd.DataFrame,
-                   quasi_ident: list,
-                   sens_att: list,
-                   gen=True,
-                   file_pdf='report.pdf') -> None:
-    """Generate a report with the parameters obtained for each anonymity check.
+def get_pdf_report(
+    data: pd.DataFrame,
+    quasi_ident: typing.Union[typing.List, np.ndarray],
+    sens_att: typing.Union[typing.List, np.ndarray],
+    gen=True,
+    file_pdf="report.pdf",
+) -> None:
+    """Generate the PDF report with the parameters obtained for each anonymity check.
 
     :param data: dataframe with the data under study.
     :type data: pandas dataframe
 
     :param quasi_ident: list with the name of the columns of the dataframe
         that are quasi-identifiers.
     :type quasi_ident: list of strings
@@ -50,81 +56,117 @@
     :type gen: boolean
 
     :param file_pdf: name of the pdf file with the report. Default to
         'report.pdf'
     :type file_pdf: string with extension .pdf
     """
     (
-        k_anon, (alpha, alpha_k), l_div, entropy_l, (c_div, l_c_div),
-        basic_beta, enhanced_beta, delta_disc, t_clos
+        k_anon,
+        (alpha, alpha_k),
+        l_div,
+        entropy_l,
+        (c_div, l_c_div),
+        basic_beta,
+        enhanced_beta,
+        delta_disc,
+        t_clos,
     ) = base.get_report_values(data, quasi_ident, sens_att, gen=True)
 
     _, file_extension = os.path.splitext(file_pdf)
-    if file_extension != '.pdf':
-        raise ValueError(
-            'Invalid file extension. Expected .pdf extension for file_pdf')
-    doc = SimpleDocTemplate(file_pdf, pagesize=A4,
-                            rightMargin=50, leftMargin=50,
-                            topMargin=50, bottomMargin=50)
+    if file_extension != ".pdf":
+        raise ValueError("Invalid file extension. Expected .pdf extension for file_pdf")
+    doc = SimpleDocTemplate(
+        file_pdf,
+        pagesize=A4,
+        rightMargin=50,
+        leftMargin=50,
+        topMargin=50,
+        bottomMargin=50,
+    )
     story = []
     today = datetime.now()
     date = today.strftime("%b %d %Y %H:%M:%S")
 
     styles = getSampleStyleSheet()
-    styles.add(ParagraphStyle('JustifyRight11',
-                              fontName="Helvetica",
-                              fontSize=11,
-                              alignment=0,
-                              spaceAfter=5))
-    styles.add(ParagraphStyle('JustifyRight11Bold',
-                              fontName="Helvetica-Bold",
-                              fontSize=11,
-                              alignment=0,
-                              spaceAfter=10))
-    styles.add(ParagraphStyle('JustifyRight12BoldSpace',
-                              fontName="Helvetica-Bold",
-                              fontSize=12,
-                              alignment=0,
-                              spaceAfter=10))
-    styles.add(ParagraphStyle('main_title',
-                              fontName="Helvetica-Bold",
-                              fontSize=18,
-                              parent=styles['Heading2'],
-                              alignment=1,
-                              spaceAfter=20))
-
-    story.append(
-        Paragraph('PyCANON: Check ANONymity properties', styles["main_title"])
+    styles.add(
+        ParagraphStyle(
+            "JustifyRight11",
+            fontName="Helvetica",
+            fontSize=11,
+            alignment=0,
+            spaceAfter=5,
+        )
+    )
+    styles.add(
+        ParagraphStyle(
+            "JustifyRight11Bold",
+            fontName="Helvetica-Bold",
+            fontSize=11,
+            alignment=0,
+            spaceAfter=10,
+        )
+    )
+    styles.add(
+        ParagraphStyle(
+            "JustifyRight12BoldSpace",
+            fontName="Helvetica-Bold",
+            fontSize=12,
+            alignment=0,
+            spaceAfter=10,
+        )
     )
-    story.append(Paragraph('Report', styles["main_title"]))
+    styles.add(
+        ParagraphStyle(
+            "main_title",
+            fontName="Helvetica-Bold",
+            fontSize=18,
+            parent=styles["Heading2"],
+            alignment=1,
+            spaceAfter=20,
+        )
+    )
+
+    story.append(Paragraph("pyCANON: Check anonymity properties", styles["main_title"]))
+    story.append(Paragraph("Anonymity report", styles["main_title"]))
     story.append(Paragraph(date, styles["JustifyRight12BoldSpace"]))
 
-#    story.append(Paragraph(
-#        f'File (or pandas dataframe) name: {str(file_name)}',
-#        styles["JustifyRight11"])
-#    )
-    story.append(Paragraph(f'Quasi-identifiers: {quasi_ident}',
-                           styles["JustifyRight11"]))
-    story.append(Paragraph(f'Sensitive attribute(s): {sens_att}',
-                           styles["JustifyRight11"]))
+    #    story.append(Paragraph(
+    #        f'File (or pandas dataframe) name: {str(file_name)}',
+    #        styles["JustifyRight11"])
+    #    )
+    story.append(
+        Paragraph(f"Quasi-identifiers: {quasi_ident}", styles["JustifyRight11"])
+    )
+    story.append(
+        Paragraph(f"Sensitive attribute(s): {sens_att}", styles["JustifyRight11"])
+    )
     if len(sens_att) > 1:
-        story.append(Paragraph(f'Approach for more than one SA: {gen}',
-                               styles["JustifyRight11"]))
+        story.append(
+            Paragraph(f"Approach for more than one SA: {gen}", styles["JustifyRight11"])
+        )
     story.append(Spacer(1, 20))
-    prop = [(Paragraph('Anonymity property', styles["JustifyRight11Bold"]),
-             Paragraph('Value(s)', styles["JustifyRight11Bold"])),
-            ('k-anonymity', f'k = {k_anon}'),
-            ('(α,k)-anonymity', f'α = {alpha} and k = {k_anon}'),
-            ('l-diversity', f'l = {l_div}'),
-            ('Entropy l-diversity', f'l = {entropy_l}'),
-            ('(c,l)-diversity', f'c = {c_div} and l = {l_div}'),
-            ('Basic β-likeness', f'β = {basic_beta}'),
-            ('Enhanced β-likeness', f'β = {enhanced_beta}'),
-            ('t-closeness', f't = {t_clos}'),
-            ('δ-disclosure privacy', f'δ = {delta_disc}')]
+    prop = [
+        (
+            Paragraph("Anonymity technique", styles["JustifyRight11Bold"]),
+            Paragraph("Value(s)", styles["JustifyRight11Bold"]),
+        ),
+        ("k-anonymity", f"k = {k_anon}"),
+        ("(α,k)-anonymity", f"α = {alpha} and k = {k_anon}"),
+        ("l-diversity", f"l = {l_div}"),
+        ("Entropy l-diversity", f"l = {entropy_l}"),
+        ("(c,l)-diversity", f"c = {c_div} and l = {l_div}"),
+        ("Basic β-likeness", f"β = {basic_beta}"),
+        ("Enhanced β-likeness", f"β = {enhanced_beta}"),
+        ("t-closeness", f"t = {t_clos}"),
+        ("δ-disclosure privacy", f"δ = {delta_disc}"),
+    ]
 
     story.append(
-        Table(prop,
-              style=[('GRID', (0, 0), (-1, -1), 1, colors.grey),
-                     ('BACKGROUND', (0, 0), (1, 0), colors.aliceblue)])
+        Table(
+            prop,
+            style=[
+                ("GRID", (0, 0), (-1, -1), 1, colors.grey),
+                ("BACKGROUND", (0, 0), (1, 0), colors.aliceblue),
+            ],
+        )
     )
     doc.build(story)
```

### Comparing `pycanon-1.0.0.post5/pycanon.egg-info/PKG-INFO` & `pycanon-1.0.1/pycanon.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pycanon
-Version: 1.0.0.post5
+Version: 1.0.1
 Summary: pyCANON, A Python library to check the level of anonymity of a dataset
 Home-page: https://gitlab.ifca.es/privacy-security/pycanon
 Author: Judith Sáinz-Pardo Díaz, Álvaro López García (IFCA (CSIC-UC))
 Author-email: sainzpardo@ifca.unican.es, aloga@ifca.unican.es
 License: Apache License 2.0
 Keywords: data,privacy,anonymity
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -22,18 +21,18 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Security
 License-File: LICENSE
 
 pyCANON
 =======
 
-|made-with-python| |License| |Documentation Status|
+|License| |Documentation Status| |Pipeline Status|
 
-pyCANON is a library and CLI to assess the values of the paramenters
-associated with the most common privacy-preserving techniques.
+pyCANON is a Python library and CLI to assess the values of the parameters
+associated with the most common privacy-preserving techniques via anonymization.
 
 **Authors:** Judith Sáinz-Pardo Díaz and Álvaro López García (IFCA - CSIC).
 
 Installation
 ------------
 
 We recommend to use Python3 with
@@ -61,32 +60,34 @@
 ---------------
 
 Example using the `adult
 dataset <https://archive.ics.uci.edu/ml/datasets/adult>`__:
 
 .. code:: python
 
+   import pandas as pd
    from pycanon import anonymity, report
 
    FILE_NAME = "adult.csv"
    QI = ["age", "education", "occupation", "relationship", "sex", "native-country"]
    SA = ["salary-class"]
+   DATA = pd.read_csv(FILE_NAME)
 
    # Calculate k for k-anonymity:
-   k = anonymity.k_anonymity(FILE_NAME, QI)
+   k = anonymity.k_anonymity(DATA, QI)
 
    # Print the anonymity report:
-   report.print_report(FILE_NAME, QI, SA)
+   report.print_report(DATA, QI, SA)
 
 Description
 -----------
 
 pyCANON allows to check if the following privacy-preserving techniques
 are verified and the value of the parameters associated with each of
-them:
+them.
 
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 | Technique                 | pyCANON function            | Parameters | Notes                                               |
 +===========================+=============================+============+=====================================================+
 | k-anonymity               | ``k_anonymity``             | *k*: int   |                                                     |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 | (α, k)-anonymity          | ``alpha_k_anonymity``       | *α*: float |                                                     |
@@ -107,16 +108,30 @@
 |                           |                             |            | (one-dimensional Earth Mover’s Distance) is used.   |
 |                           |                             |            | For categorical attributes, the metric "Equal       |
 |                           |                             |            | Distance" is used.                                  |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 | δ-disclosure privacy      | ``delta_disclosure``        | *δ*: float |                                                     |
 +---------------------------+-----------------------------+------------+-----------------------------------------------------+
 
+More information can be found in this `paper <https://www.nature.com/articles/s41597-022-01894-2>`__.
+
+
+Citation
+-----------
+If you are using pyCANON you can cite it as follows:: 
+
+   @article{sainzpardo2022pycanon,
+      title={A Python library to check the level of anonymity of a dataset},
+      author={S{\'a}inz-Pardo D{\'\i}az, Judith and L{\'o}pez Garc{\'\i}a, {\'A}lvaro},
+      journal={Scientific Data},
+      volume={9},
+      number={1},
+      pages={785},
+      year={2022},
+      publisher={Nature Publishing Group UK London}}
 
-.. |made-with-python| image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg
-   :target: https://www.python.org/
 .. |License| image:: https://img.shields.io/badge/License-Apache_2.0-blue.svg
    :target: https://gitlab.ifca.es/sainzj/check-anonymity/-/blob/main/LICENSE
 .. |Documentation Status| image:: https://readthedocs.org/projects/pycanon/badge/?version=latest
    :target: https://pycanon.readthedocs.io/en/latest/?badge=latest
-
-
+.. |Pipeline Status| image:: https://gitlab.ifca.es/privacy-security/pycanon/badges/main/pipeline.svg
+   :target: https://gitlab.ifca.es/privacy-security/pycanon/-/pipelines
```

### Comparing `pycanon-1.0.0.post5/pycanon.egg-info/SOURCES.txt` & `pycanon-1.0.1/pycanon.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -20,8 +20,11 @@
 pycanon/anonymity/_t_closeness.py
 pycanon/anonymity/utils/__init__.py
 pycanon/anonymity/utils/aux_anonymity.py
 pycanon/anonymity/utils/aux_functions.py
 pycanon/report/__init__.py
 pycanon/report/base.py
 pycanon/report/json.py
-pycanon/report/pdf.py
+pycanon/report/pdf.py
+pycanon/report/pdf_utility_report.py
+tests/test_metrics.py
+tests/test_reports.py
```

### Comparing `pycanon-1.0.0.post5/setup.cfg` & `pycanon-1.0.1/setup.cfg`

 * *Files identical despite different names*

