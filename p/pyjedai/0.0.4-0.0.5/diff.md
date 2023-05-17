# Comparing `tmp/pyjedai-0.0.4.tar.gz` & `tmp/pyjedai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjedai-0.0.4.tar", last modified: Wed Oct  5 09:20:50 2022, max compression
+gzip compressed data, was "pyjedai-0.0.5.tar", last modified: Wed May 17 14:21:47 2023, max compression
```

## Comparing `pyjedai-0.0.4.tar` & `pyjedai-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-10-05 09:20:50.161357 pyjedai-0.0.4/
--rw-rw-rw-   0        0        0    11684 2022-09-21 14:32:22.000000 pyjedai-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     7378 2022-10-05 09:20:50.160355 pyjedai-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5701 2022-10-05 09:20:27.000000 pyjedai-0.0.4/README.md
--rw-rw-rw-   0        0        0     2428 2022-10-05 08:37:59.000000 pyjedai-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-05 09:20:50.161357 pyjedai-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-05 09:20:50.108845 pyjedai-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2022-10-05 09:20:50.130848 pyjedai-0.0.4/src/pyjedai/
--rw-rw-rw-   0        0        0        0 2022-07-19 14:45:04.000000 pyjedai-0.0.4/src/pyjedai/__init__.py
--rw-rw-rw-   0        0        0    11292 2022-09-16 11:27:56.000000 pyjedai-0.0.4/src/pyjedai/block_building.py
--rw-rw-rw-   0        0        0     8568 2022-09-23 14:52:58.000000 pyjedai-0.0.4/src/pyjedai/block_cleaning.py
--rw-rw-rw-   0        0        0     1639 2022-09-05 13:35:43.000000 pyjedai-0.0.4/src/pyjedai/clustering.py
--rw-rw-rw-   0        0        0    23780 2022-09-06 10:31:37.000000 pyjedai-0.0.4/src/pyjedai/comparison_cleaning.py
--rw-rw-rw-   0        0        0     5218 2022-09-05 13:52:51.000000 pyjedai-0.0.4/src/pyjedai/datamodel.py
--rw-rw-rw-   0        0        0    13713 2022-09-10 14:20:26.000000 pyjedai-0.0.4/src/pyjedai/evaluation.py
--rw-rw-rw-   0        0        0    12886 2022-09-06 11:06:49.000000 pyjedai-0.0.4/src/pyjedai/joins.py
--rw-rw-rw-   0        0        0     7977 2022-09-09 09:40:55.000000 pyjedai-0.0.4/src/pyjedai/matching.py
--rw-rw-rw-   0        0        0     2661 2022-09-05 12:07:48.000000 pyjedai-0.0.4/src/pyjedai/utils.py
--rw-rw-rw-   0        0        0    13521 2022-09-22 10:51:11.000000 pyjedai-0.0.4/src/pyjedai/vector_based_blocking.py
--rw-rw-rw-   0        0        0      955 2022-07-19 14:45:04.000000 pyjedai-0.0.4/src/pyjedai/visualization.py
--rw-rw-rw-   0        0        0    13359 2022-09-26 09:51:49.000000 pyjedai-0.0.4/src/pyjedai/workflow.py
-drwxrwxrwx   0        0        0        0 2022-10-05 09:20:50.158332 pyjedai-0.0.4/src/pyjedai.egg-info/
--rw-rw-rw-   0        0        0     7378 2022-10-05 09:20:50.000000 pyjedai-0.0.4/src/pyjedai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2022-10-05 09:20:50.000000 pyjedai-0.0.4/src/pyjedai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-05 09:20:50.000000 pyjedai-0.0.4/src/pyjedai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      405 2022-10-05 09:20:50.000000 pyjedai-0.0.4/src/pyjedai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-10-05 09:20:50.000000 pyjedai-0.0.4/src/pyjedai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 14:21:47.907971 pyjedai-0.0.5/
+-rw-rw-rw-   0        0        0    11684 2022-09-21 14:32:22.000000 pyjedai-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     7234 2023-05-17 14:21:47.906971 pyjedai-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5557 2023-05-17 14:11:07.000000 pyjedai-0.0.5/README.md
+-rw-rw-rw-   0        0        0     2428 2023-05-17 14:13:30.000000 pyjedai-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 14:21:47.908973 pyjedai-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 14:21:47.806873 pyjedai-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 14:21:47.853183 pyjedai-0.0.5/src/pyjedai/
+-rw-rw-rw-   0        0        0        0 2022-07-19 14:45:04.000000 pyjedai-0.0.5/src/pyjedai/__init__.py
+-rw-rw-rw-   0        0        0    18483 2023-05-05 17:55:55.000000 pyjedai-0.0.5/src/pyjedai/block_building.py
+-rw-rw-rw-   0        0        0     8520 2023-05-05 17:55:55.000000 pyjedai-0.0.5/src/pyjedai/block_cleaning.py
+-rw-rw-rw-   0        0        0     8107 2023-05-16 13:45:11.000000 pyjedai-0.0.5/src/pyjedai/clustering.py
+-rw-rw-rw-   0        0        0    29695 2023-05-15 12:18:45.000000 pyjedai-0.0.5/src/pyjedai/comparison_cleaning.py
+-rw-rw-rw-   0        0        0     9857 2023-05-15 14:47:19.000000 pyjedai-0.0.5/src/pyjedai/datamodel.py
+-rw-rw-rw-   0        0        0    18898 2023-05-15 10:36:29.000000 pyjedai-0.0.5/src/pyjedai/evaluation.py
+-rw-rw-rw-   0        0        0    14566 2023-05-17 08:37:13.000000 pyjedai-0.0.5/src/pyjedai/joins.py
+-rw-rw-rw-   0        0        0      774 2022-08-31 12:44:46.000000 pyjedai-0.0.5/src/pyjedai/logs.py
+-rw-rw-rw-   0        0        0    24233 2023-05-16 12:56:27.000000 pyjedai-0.0.5/src/pyjedai/matching.py
+-rw-rw-rw-   0        0        0     8156 2023-05-16 12:34:27.000000 pyjedai-0.0.5/src/pyjedai/utils.py
+-rw-rw-rw-   0        0        0    27635 2023-05-15 11:13:12.000000 pyjedai-0.0.5/src/pyjedai/vector_based_blocking.py
+-rw-rw-rw-   0        0        0      955 2022-07-19 14:45:04.000000 pyjedai-0.0.5/src/pyjedai/visualization.py
+-rw-rw-rw-   0        0        0    24786 2023-03-21 21:57:00.000000 pyjedai-0.0.5/src/pyjedai/workflow.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:21:47.903961 pyjedai-0.0.5/src/pyjedai.egg-info/
+-rw-rw-rw-   0        0        0     7234 2023-05-17 14:21:47.000000 pyjedai-0.0.5/src/pyjedai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-05-17 14:21:47.000000 pyjedai-0.0.5/src/pyjedai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 14:21:47.000000 pyjedai-0.0.5/src/pyjedai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      405 2023-05-17 14:21:47.000000 pyjedai-0.0.5/src/pyjedai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 14:21:47.000000 pyjedai-0.0.5/src/pyjedai.egg-info/top_level.txt
```

### Comparing `pyjedai-0.0.4/LICENSE` & `pyjedai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.4/PKG-INFO` & `pyjedai-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjedai
-Version: 0.0.4
+Version: 0.0.5
 Summary: An open-source library that builds powerful end-to-end Entity Resolution workflows.
 Author-email: Konstantinos Nikoletos <nikoletos.kon@gmail.com>, George Papadakis <gpapadis84@gmail.com>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://github.com/AI-team-UoA/pyJedAI
 Project-URL: Documentation, https://github.com/AI-team-UoA/pyJedAI/wiki
 Project-URL: Bug Tracker, https://github.com/AI-team-UoA/pyJedAI/issues
 Project-URL: Source code, https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai
@@ -40,20 +40,14 @@
 <br>
 <div align="center">
 An open-source library that leverages Python’s data science ecosystem to build <br> powerful end-to-end Entity Resolution workflows.
 </div>
 
 ---
 
-[![Tests](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml)
-[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
-[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
-[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-
 <!--
 [![DOI:10.1007/978-3-319-76207-4_15](https://zenodo.org/badge/DOI/10.1007/978-3-319-76207-4_15.svg)](https://doi.org/10.1007/978-3-319-76207-4_15)
 [![Citation Badge](https://api.juleskreuer.eu/citation-badge.php?doi=10.1126/science.1058040)](https://juleskreuer.eu/projekte/citation-badge/)
 --->
 
 
 # Overview
@@ -111,26 +105,35 @@
 </div>
 
 <br>
 <br>
 
 See the full list of dependencies and all versions used, in this [file](https://github.com/AI-team-UoA/pyJedAI/blob/main/requirements.txt).
 
+
+__Status__ 
+
+[![Tests](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml)
+[![made-with-python](https://readthedocs.org/projects/pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/?badge=latest)
+
+
+
 # Bugs, Discussions & News
 
 [GitHub Discussions](https://github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/AI-team-UoA/pyJedAI/issues).
 
 # Team & Authors
 
-<img align="right" src="https://www.di.uoa.gr/themes/corporate_lite/logo_en.png" alt="pyJedAI" width="400"/>
+<img align="right" src="https://github.com/AI-team-UoA/.github/blob/main/AI_LOGO.png?raw=true" alt="pyJedAI" width="200"/>
 
 - [Konstantinos Nikoletos](https://nikoletos-k.github.io)
+- Jakub Maciejewski
 - [George Papadakis](https://gpapadis.wordpress.com)
 - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/)
 
 Research and development is made under the supervision of Pr. Manolis Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the University of Athens.
 
 # License
 
 Released under the Apache-2.0 license [(see LICENSE.txt)](https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE).
 
-2022-2023 | AI-Team @ University of Athens
+2023 | AI-Team @ University of Athens
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyjedai Version: 0.0.4 Summary: An open-source
+Metadata-Version: 2.1 Name: pyjedai Version: 0.0.5 Summary: An open-source
 library that builds powerful end-to-end Entity Resolution workflows. Author-
 email: Konstantinos Nikoletos
 kon@gmail.com>, George Papadakis
 gmail.com> License: Apache Software License 2.0 Project-URL: Homepage, https://
 github.com/AI-team-UoA/pyJedAI Project-URL: Documentation, https://github.com/
 AI-team-UoA/pyJedAI/wiki Project-URL: Bug Tracker, https://github.com/AI-team-
 UoA/pyJedAI/issues Project-URL: Source code, https://github.com/AI-team-UoA/
@@ -24,33 +24,26 @@
 
                                    [pyJedAI]
 
 
   An open-source library that leverages Pythonâs data science ecosystem to
                                     build
                powerful end-to-end Entity Resolution workflows.
---- [![Tests](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/
-tests.yml/badge.svg?branch=main)](https://github.com/AI-team-UoA/pyJedAI/
-actions/workflows/tests.yml) [![Linux](https://svgshare.com/i/Zhy.svg)](https:/
-/svgshare.com/i/Zhy.svg) [![macOS](https://svgshare.com/i/ZjP.svg)](https://
-svgshare.com/i/ZjP.svg) [![Windows](https://svgshare.com/i/ZhY.svg)](https://
-svgshare.com/i/ZhY.svg) [![made-with-python](https://img.shields.io/badge/
-Made%20with-Python-1f425f.svg)](https://www.python.org/)  # Overview pyJedAI is
-a python framework, aiming to offer experts and novice users, robust and fast
-solutions for multiple types of Entity Resolution problems. It is builded using
-state-of-the-art python frameworks. pyJedAI constitutes the sole open-source
-Link Discovery tool that is capable of exploiting the latest breakthroughs in
-Deep Learning and NLP techniques, which are publicly available through the
-Python data science ecosystem. This applies to both blocking and matching, thus
-ensuring high time efficiency, high scalability as well as high effectiveness,
-without requiring any labelled instances from the user. ### Key-Features -
-Input data-type independent. Both structured and semi-structured data can be
-processed. - Various implemented algorithms. - Easy-to-use. - Utilizes some of
-the famous and cutting-edge machine learning packages.  __Open demo python
-notebook:__
+---  # Overview pyJedAI is a python framework, aiming to offer experts and
+novice users, robust and fast solutions for multiple types of Entity Resolution
+problems. It is builded using state-of-the-art python frameworks. pyJedAI
+constitutes the sole open-source Link Discovery tool that is capable of
+exploiting the latest breakthroughs in Deep Learning and NLP techniques, which
+are publicly available through the Python data science ecosystem. This applies
+to both blocking and matching, thus ensuring high time efficiency, high
+scalability as well as high effectiveness, without requiring any labelled
+instances from the user. ### Key-Features - Input data-type independent. Both
+structured and semi-structured data can be processed. - Various implemented
+algorithms. - Easy-to-use. - Utilizes some of the famous and cutting-edge
+machine learning packages.  __Open demo python notebook:__
        [https://nbviewer.org/static/img/nav_logo.svg]         [https://
             miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png]
 
 For more tutorials go to [pyJedAI/tutorials](https://github.com/AI-team-UoA/
 pyJedAI/tree/main/tutorials). # Install Install the latest version of pyjedai
 __[requires python >= 3.7]__: ``` pip install pyjedai ``` The source code is
 currently hosted on GitHub at: [AI-team-UoA/pyJedAI](https://github.com/AI-
@@ -70,20 +63,25 @@
  [https://www.kornosk.me/resources/language-model/featured.png]     [https://
    repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-
 745fdcbeffe8]     [https://networkx.org/_static/networkx_logo.svg]     [https:/
           /raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png]
 
 
 See the full list of dependencies and all versions used, in this [file](https:/
-/github.com/AI-team-UoA/pyJedAI/blob/main/requirements.txt). # Bugs,
-Discussions & News [GitHub Discussions](https://github.com/AI-team-UoA/pyJedAI/
-discussions) is the discussion forum for general questions and discussions and
-our recommended starting point. Please report any bugs that you find [here]
-(https://github.com/AI-team-UoA/pyJedAI/issues). # Team & Authors [pyJedAI] -
-[Konstantinos Nikoletos](https://nikoletos-k.github.io) - [George Papadakis]
-(https://gpapadis.wordpress.com) - [Manolis Koubarakis](https://cgi.di.uoa.gr/
-~koubarak/) Research and development is made under the supervision of Pr.
-Manolis Koubarakis. This is a research project by the [AI-Team](https://
-ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the
-University of Athens. # License Released under the Apache-2.0 license [(see
-LICENSE.txt)](https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE). 2022-
-2023 | AI-Team @ University of Athens
+/github.com/AI-team-UoA/pyJedAI/blob/main/requirements.txt). __Status__ [!
+[Tests](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml/
+badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/
+workflows/tests.yml) [![made-with-python](https://readthedocs.org/projects/
+pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/
+?badge=latest) # Bugs, Discussions & News [GitHub Discussions](https://
+github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum for general
+questions and discussions and our recommended starting point. Please report any
+bugs that you find [here](https://github.com/AI-team-UoA/pyJedAI/issues). #
+Team & Authors [pyJedAI] - [Konstantinos Nikoletos](https://nikoletos-
+k.github.io) - Jakub Maciejewski - [George Papadakis](https://
+gpapadis.wordpress.com) - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/
+) Research and development is made under the supervision of Pr. Manolis
+Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr)
+of the Department of Informatics and Telecommunications at the University of
+Athens. # License Released under the Apache-2.0 license [(see LICENSE.txt)]
+(https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE). 2023 | AI-Team @
+University of Athens
```

### Comparing `pyjedai-0.0.4/README.md` & `pyjedai-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,14 @@
 <br>
 <div align="center">
 An open-source library that leverages Python’s data science ecosystem to build <br> powerful end-to-end Entity Resolution workflows.
 </div>
 
 ---
 
-[![Tests](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml)
-[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
-[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
-[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-
 <!--
 [![DOI:10.1007/978-3-319-76207-4_15](https://zenodo.org/badge/DOI/10.1007/978-3-319-76207-4_15.svg)](https://doi.org/10.1007/978-3-319-76207-4_15)
 [![Citation Badge](https://api.juleskreuer.eu/citation-badge.php?doi=10.1126/science.1058040)](https://juleskreuer.eu/projekte/citation-badge/)
 --->
 
 
 # Overview
@@ -77,26 +71,35 @@
 </div>
 
 <br>
 <br>
 
 See the full list of dependencies and all versions used, in this [file](https://github.com/AI-team-UoA/pyJedAI/blob/main/requirements.txt).
 
+
+__Status__ 
+
+[![Tests](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml)
+[![made-with-python](https://readthedocs.org/projects/pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/?badge=latest)
+
+
+
 # Bugs, Discussions & News
 
 [GitHub Discussions](https://github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/AI-team-UoA/pyJedAI/issues).
 
 # Team & Authors
 
-<img align="right" src="https://www.di.uoa.gr/themes/corporate_lite/logo_en.png" alt="pyJedAI" width="400"/>
+<img align="right" src="https://github.com/AI-team-UoA/.github/blob/main/AI_LOGO.png?raw=true" alt="pyJedAI" width="200"/>
 
 - [Konstantinos Nikoletos](https://nikoletos-k.github.io)
+- Jakub Maciejewski
 - [George Papadakis](https://gpapadis.wordpress.com)
 - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/)
 
 Research and development is made under the supervision of Pr. Manolis Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the University of Athens.
 
 # License
 
 Released under the Apache-2.0 license [(see LICENSE.txt)](https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE).
 
-2022-2023 | AI-Team @ University of Athens
+2023 | AI-Team @ University of Athens
```

#### html2text {}

```diff
@@ -1,33 +1,26 @@
 
                                    [pyJedAI]
 
 
   An open-source library that leverages Pythonâs data science ecosystem to
                                     build
                powerful end-to-end Entity Resolution workflows.
---- [![Tests](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/
-tests.yml/badge.svg?branch=main)](https://github.com/AI-team-UoA/pyJedAI/
-actions/workflows/tests.yml) [![Linux](https://svgshare.com/i/Zhy.svg)](https:/
-/svgshare.com/i/Zhy.svg) [![macOS](https://svgshare.com/i/ZjP.svg)](https://
-svgshare.com/i/ZjP.svg) [![Windows](https://svgshare.com/i/ZhY.svg)](https://
-svgshare.com/i/ZhY.svg) [![made-with-python](https://img.shields.io/badge/
-Made%20with-Python-1f425f.svg)](https://www.python.org/)  # Overview pyJedAI is
-a python framework, aiming to offer experts and novice users, robust and fast
-solutions for multiple types of Entity Resolution problems. It is builded using
-state-of-the-art python frameworks. pyJedAI constitutes the sole open-source
-Link Discovery tool that is capable of exploiting the latest breakthroughs in
-Deep Learning and NLP techniques, which are publicly available through the
-Python data science ecosystem. This applies to both blocking and matching, thus
-ensuring high time efficiency, high scalability as well as high effectiveness,
-without requiring any labelled instances from the user. ### Key-Features -
-Input data-type independent. Both structured and semi-structured data can be
-processed. - Various implemented algorithms. - Easy-to-use. - Utilizes some of
-the famous and cutting-edge machine learning packages.  __Open demo python
-notebook:__
+---  # Overview pyJedAI is a python framework, aiming to offer experts and
+novice users, robust and fast solutions for multiple types of Entity Resolution
+problems. It is builded using state-of-the-art python frameworks. pyJedAI
+constitutes the sole open-source Link Discovery tool that is capable of
+exploiting the latest breakthroughs in Deep Learning and NLP techniques, which
+are publicly available through the Python data science ecosystem. This applies
+to both blocking and matching, thus ensuring high time efficiency, high
+scalability as well as high effectiveness, without requiring any labelled
+instances from the user. ### Key-Features - Input data-type independent. Both
+structured and semi-structured data can be processed. - Various implemented
+algorithms. - Easy-to-use. - Utilizes some of the famous and cutting-edge
+machine learning packages.  __Open demo python notebook:__
        [https://nbviewer.org/static/img/nav_logo.svg]         [https://
             miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png]
 
 For more tutorials go to [pyJedAI/tutorials](https://github.com/AI-team-UoA/
 pyJedAI/tree/main/tutorials). # Install Install the latest version of pyjedai
 __[requires python >= 3.7]__: ``` pip install pyjedai ``` The source code is
 currently hosted on GitHub at: [AI-team-UoA/pyJedAI](https://github.com/AI-
@@ -47,20 +40,25 @@
  [https://www.kornosk.me/resources/language-model/featured.png]     [https://
    repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-
 745fdcbeffe8]     [https://networkx.org/_static/networkx_logo.svg]     [https:/
           /raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png]
 
 
 See the full list of dependencies and all versions used, in this [file](https:/
-/github.com/AI-team-UoA/pyJedAI/blob/main/requirements.txt). # Bugs,
-Discussions & News [GitHub Discussions](https://github.com/AI-team-UoA/pyJedAI/
-discussions) is the discussion forum for general questions and discussions and
-our recommended starting point. Please report any bugs that you find [here]
-(https://github.com/AI-team-UoA/pyJedAI/issues). # Team & Authors [pyJedAI] -
-[Konstantinos Nikoletos](https://nikoletos-k.github.io) - [George Papadakis]
-(https://gpapadis.wordpress.com) - [Manolis Koubarakis](https://cgi.di.uoa.gr/
-~koubarak/) Research and development is made under the supervision of Pr.
-Manolis Koubarakis. This is a research project by the [AI-Team](https://
-ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the
-University of Athens. # License Released under the Apache-2.0 license [(see
-LICENSE.txt)](https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE). 2022-
-2023 | AI-Team @ University of Athens
+/github.com/AI-team-UoA/pyJedAI/blob/main/requirements.txt). __Status__ [!
+[Tests](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml/
+badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/
+workflows/tests.yml) [![made-with-python](https://readthedocs.org/projects/
+pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/
+?badge=latest) # Bugs, Discussions & News [GitHub Discussions](https://
+github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum for general
+questions and discussions and our recommended starting point. Please report any
+bugs that you find [here](https://github.com/AI-team-UoA/pyJedAI/issues). #
+Team & Authors [pyJedAI] - [Konstantinos Nikoletos](https://nikoletos-
+k.github.io) - Jakub Maciejewski - [George Papadakis](https://
+gpapadis.wordpress.com) - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/
+) Research and development is made under the supervision of Pr. Manolis
+Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr)
+of the Department of Informatics and Telecommunications at the University of
+Athens. # License Released under the Apache-2.0 license [(see LICENSE.txt)]
+(https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE). 2023 | AI-Team @
+University of Athens
```

### Comparing `pyjedai-0.0.4/pyproject.toml` & `pyjedai-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyjedai"
-version = "0.0.4"
+version = "0.0.5"
 description = "An open-source library that builds powerful end-to-end Entity Resolution workflows."
 readme = "README.md"
 authors = [
     { name = "Konstantinos Nikoletos", email = "nikoletos.kon@gmail.com" },
     { name = "George Papadakis", email = "gpapadis84@gmail.com" },
 ]
 license = {text = "Apache Software License 2.0"}
@@ -34,15 +34,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 keywords = ["deduplication", "entity-resolution", "link-discovery"]
 requires-python = ">=3.7"
 dependencies = [
     "gensim >= 4.2.0",
-    "matplotlib >= 3.5.2",
+    "matplotlib >= 3.1.3",
     "matplotlib-inline >= 0.1.3",
     "networkx >= 2.3",
     "nltk >= 3.7",
     "numpy >= 1.21",
     "pandas >= 0.25.3",
     "pandas-profiling >= 3.2",
     "pandocfilters >= 1.5",
```

### Comparing `pyjedai-0.0.4/src/pyjedai/block_cleaning.py` & `pyjedai-0.0.5/src/pyjedai/block_cleaning.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,224 +1,210 @@
-from time import time
-
-import numpy as np
-from tqdm.notebook import tqdm
-
-from .datamodel import Block, Data
-from .utils import create_entity_index, drop_single_entity_blocks
-
-
-class BlockFiltering:
-    """Retains every entity in a subset of its smallest blocks.
-    Filtering consists of 3 steps:
-     - Blocks sort in ascending cardinality
-     - Creation of Entity Index: inversed block dictionary
-     - Retain every entity in ratio % of its smallest blocks
-     - Blocks reconstruction
-    """
-
-    _method_name = "Block Filtering"
-    _method_info = "Retains every entity in a subset of its smallest blocks."
-
-    def __init__(self, ratio: float = 0.8) -> None:
-        if ratio > 1.0 or ratio < 0.0:
-            raise AttributeError("Ratio is a number between 0.0 and 1.0")
-        else:
-            self.ratio = ratio
-        self.blocks: dict
-        self.tqdm_disable: bool
-        self.data: Data
-        self._progress_bar: tqdm
-        self.execution_time: float
-
-    def __str__(self) -> str:
-        print(self._method_name + self._method_info)
-        print("Ratio: ", self.ratio)
-        return super().__str__()
-
-    def process(
-            self,
-            blocks: dict = None,
-            data: Data = None,
-            tqdm_disable: bool = False
-    ) -> dict:
-        """Main method of Block Filtering
-
-        Args:
-            blocks (dict, optional): dict of keys to Blocks. Defaults to None.
-            data (Data, optional): input dataset module. Defaults to None.
-            tqdm_disable (bool, optional): disable progress bars. Defaults to False.
-
-        Returns:
-            dict: dict of keys to Blocks
-        """
-        start_time, self.tqdm_disable, self.data = time(), tqdm_disable, data
-        self._progress_bar = tqdm(
-            total=3,
-            desc=self._method_name,
-            disable=self.tqdm_disable
-        )
-        sorted_blocks = sort_blocks_cardinality(blocks, self.data.is_dirty_er)
-        self._progress_bar.update(1)
-        entity_index = create_entity_index(sorted_blocks, self.data.is_dirty_er)
-        self._progress_bar.update(1)
-        filtered_blocks = {}
-        for entity_id, block_keys in entity_index.items():
-            # Create new blocks from the entity index
-            for key in block_keys[:int(round(self.ratio*len(block_keys)))]:
-                filtered_blocks.setdefault(key, Block())
-                # Entities ids start to 0 ... n-1 for 1st dataset
-                # and n ... m for 2nd dataset
-                if entity_id < self.data.dataset_limit:
-                    filtered_blocks[key].entities_D1.add(entity_id)
-                else:
-                    filtered_blocks[key].entities_D2.add(entity_id)
-        self._progress_bar.update(1)
-        self.blocks = drop_single_entity_blocks(filtered_blocks, self.data.is_dirty_er)
-        self._progress_bar.close()
-        self.execution_time = time() - start_time
-
-        return self.blocks
-
-    def method_configuration(self) -> dict:
-        """Returns configuration details
-        """
-        return {
-            "name" : self._method_name,
-            "parameters" : self._configuration(),
-            "runtime": self.execution_time
-        }
-
-    def _configuration(self) -> dict:
-        return {
-            "Ratio" : self.ratio
-        }
-
-    def report(self) -> None:
-        """Prints Block Building method configuration
-        """
-        print(
-            "Method name: " + self._method_name +
-            "\nMethod info: " + self._method_info +
-            "\nParameters: \n" + ''.join(['\t{0}: {1}\n'.format(k, v) for k, v in self._configuration().items()]) +
-            "\nRuntime: {:2.4f} seconds".format(self.execution_time)
-        )
-
-class BlockPurging:
-    """Discards the blocks exceeding a certain number of comparisons.
-    """
-
-    _method_name = "Block Purging"
-    _method_info = "Discards the blocks exceeding a certain number of comparisons."
-
-    def __init__(self, smoothing_factor: float = 1.025) -> any:
-        self.smoothing_factor: float = smoothing_factor
-        self.max_comparisons_per_block: float
-        self.execution_time: float
-        self.tqdm_disable: bool
-        self._progress_bar: tqdm
-        self.data: Data
-
-    def process(
-            self,
-            blocks: dict,
-            data: Data,
-            tqdm_disable: bool = False
-    ) -> dict:
-        """Main method of Block Purging
-
-        Args:
-            blocks (dict): _description_
-            data (Data): _description_
-            tqdm_disable (bool, optional): _description_. Defaults to False.
-
-        Returns:
-            dict: _description_
-        """
-        self.tqdm_disable, self.data, start_time = tqdm_disable, data, time()
-        self._progress_bar = tqdm(total=2*len(blocks), desc=self._method_name, disable=self.tqdm_disable)
-        if not blocks:
-            raise AttributeError("Empty dict of blocks was given as input!")
-        new_blocks = blocks.copy()
-        self._set_threshold(new_blocks)
-        all_keys = list(new_blocks.keys())
-        for key in all_keys:
-            if new_blocks[key].get_cardinality(self.data.is_dirty_er) > self.max_comparisons_per_block:
-                del new_blocks[key]
-            self._progress_bar.update(1)
-        self.execution_time = time() - start_time
-        self._progress_bar.close()
-
-        return new_blocks
-
-    def _set_threshold(self, blocks: dict) -> None:
-        """
-        TODO _summary_
-
-        Args:
-            blocks (dict): _description_
-        """
-        sorted_blocks = sort_blocks_cardinality(blocks, self.data.is_dirty_er)
-        distinct_comparisons_level = set(b.get_cardinality(self.data.is_dirty_er) \
-                                        for _, b in sorted_blocks.items())
-        block_assignments = np.empty([len(distinct_comparisons_level)])
-        comparisons_level = np.empty([len(distinct_comparisons_level)])
-        total_comparisons_per_level = np.empty([len(distinct_comparisons_level)])
-        index = -1
-        for _, block in sorted_blocks.items():
-            if index == -1:
-                index += 1
-                comparisons_level[index] = block.get_cardinality(self.data.is_dirty_er)
-                block_assignments[index] = 0
-                total_comparisons_per_level[index] = 0
-            elif block.get_cardinality(self.data.is_dirty_er) != comparisons_level[index]:
-                index += 1
-                comparisons_level[index] = block.get_cardinality(self.data.is_dirty_er)
-                block_assignments[index] = block_assignments[index-1]
-                total_comparisons_per_level[index] = total_comparisons_per_level[index-1]
-
-            block_assignments[index] += block.get_size()
-            total_comparisons_per_level[index] += block.get_cardinality(self.data.is_dirty_er)
-            self._progress_bar.update(1)
-
-        current_bc = current_cc = current_size = \
-            previous_bc = previous_cc = previous_size = 0
-        for i in range(len(block_assignments)-1, 0, -1):
-            previous_size = current_size
-            previous_bc = current_bc
-            previous_cc = current_cc
-            current_size = comparisons_level[i]
-            current_bc = block_assignments[i]
-            current_cc = total_comparisons_per_level[i]
-            if current_bc * previous_cc < self.smoothing_factor * current_cc * previous_bc:
-                break
-        self.max_comparisons_per_block = previous_size
-
-    def _satisfies_threshold(self, block: Block) -> bool:
-        return block.get_cardinality(self.data.is_dirty_er) <= self.max_comparisons_per_block
-
-    def method_configuration(self) -> dict:
-        return {
-            "name" : self._method_name,
-            "parameters" : self._configuration(),
-            "runtime": self.execution_time
-        }
-
-    def _configuration(self) -> dict:
-        return {
-            "Smoothing factor" : self.smoothing_factor,
-            "Max Comparisons per Block" : self.max_comparisons_per_block
-        }
-
-    def report(self) -> None:
-        """Prints method configuration
-        """
-        print(
-            "Method name: " + self._method_name +
-            "\nMethod info: " + self._method_info +
-            "\nParameters: \n" + ''.join(
-                ['\t{0}: {1}\n'.format(k, v) for k, v in self._configuration().items()]) +
-            "Runtime: {:2.4f} seconds".format(self.execution_time)
-        )
-
-def sort_blocks_cardinality(blocks: dict, is_dirty_er: bool) -> dict:
-    return dict(sorted(blocks.items(), key=lambda x: x[1].get_cardinality(is_dirty_er)))
+"""Block Cleaning Module
+Contains:
+ - BlockFiltering
+ - BlockPurging
+"""
+from abc import ABC
+from collections import defaultdict
+from time import time
+from typing import Tuple
+
+import numpy as np
+from tqdm.autonotebook import tqdm
+
+from .block_building import AbstractBlockProcessing
+from .datamodel import Block, Data
+from .utils import create_entity_index, drop_single_entity_blocks
+
+class AbstractBlockCleaning(AbstractBlockProcessing):
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def report(self) -> None:
+        """Prints Block Building method configuration
+        """
+        print(
+            "Method name: " + self._method_name +
+            "\nMethod info: " + self._method_info +
+            "\nParameters: \n" + ''.join(['\t{0}: {1}\n'.format(k, v) for k, v in self._configuration().items()]) +
+            "Runtime: {:2.4f} seconds".format(self.execution_time)
+        )
+
+class BlockFiltering(AbstractBlockCleaning):
+    """Retains every entity in a subset of its smallest blocks.
+
+        Filtering consists of 3 steps:
+        - Blocks sort in ascending cardinality
+        - Creation of Entity Index: inversed block dictionary
+        - Retain every entity in ratio % of its smallest blocks
+        - Blocks reconstruction
+    """
+
+    _method_name = "Block Filtering"
+    _method_short_name: str = "BF"
+    _method_info = "Retains every entity in a subset of its smallest blocks."
+
+    def __init__(self, ratio: float = 0.8) -> None:
+        super().__init__()
+        if ratio > 1.0 or ratio < 0.0:
+            raise AttributeError("Ratio is a number between 0.0 and 1.0")
+        else:
+            self.ratio = ratio
+        self.entity_index: dict
+
+    def __str__(self) -> str:
+        print(self._method_name + self._method_info)
+        print("Ratio: ", self.ratio)
+        return super().__str__()
+
+    def process(
+            self,
+            blocks: dict,
+            data: Data,
+            tqdm_disable: bool = False
+    ) -> Tuple[dict, dict]:
+        """Main method of Block Filtering.
+
+        Args:
+            blocks (dict): dict of keys to Blocks.
+            data (Data): input dataset.
+            tqdm_disable (bool, optional): disable progress bars. Defaults to False.
+
+        Returns:
+            Tuple[dict, dict]: dict of keys to Blocks, entity index (reversed blocks)
+        """
+        start_time, self.tqdm_disable, self.data = time(), tqdm_disable, data
+        self._progress_bar = tqdm(
+            total=3,
+            desc=self._method_name,
+            disable=self.tqdm_disable
+        )
+        sorted_blocks = _sort_blocks_cardinality(blocks, self.data.is_dirty_er)
+        self._progress_bar.update(1)
+        entity_index = create_entity_index(sorted_blocks, self.data.is_dirty_er)
+        self._progress_bar.update(1)
+        filtered_blocks = {}
+        for entity_id, block_keys in entity_index.items():
+            # Create new blocks from the entity index
+            # print(list(block_keys[:int(round(self.ratio*len(block_keys)))]))
+            block_keys = list(block_keys)
+            for key in list(block_keys[:int(round(self.ratio*len(block_keys)))]):
+                filtered_blocks.setdefault(key, Block())
+                # Entities ids start to 0 ... n-1 for 1st dataset
+                # and n ... m for 2nd dataset
+                _ = filtered_blocks[key].entities_D1.add(entity_id) if entity_id < self.data.dataset_limit \
+                    else filtered_blocks[key].entities_D2.add(entity_id)
+        self._progress_bar.update(1)
+        new_blocks = drop_single_entity_blocks(filtered_blocks, self.data.is_dirty_er)
+        self._progress_bar.close()
+        self.execution_time = time() - start_time
+        self.blocks = new_blocks
+        
+        return new_blocks
+
+    def _configuration(self) -> dict:
+        return {
+            "Ratio" : self.ratio
+        }
+
+
+class BlockPurging(AbstractBlockCleaning):
+    """Discards the blocks exceeding a certain number of comparisons.
+    """
+
+    _method_name = "Block Purging"
+    _method_short_name: str = "BP"
+    _method_info = "Discards the blocks exceeding a certain number of comparisons."
+
+    def __init__(self, smoothing_factor: float = 1.025) -> any:
+        super().__init__()
+        self.smoothing_factor: float = smoothing_factor
+        self.max_comparisons_per_block: float
+
+    def process(
+            self,
+            blocks: dict,
+            data: Data,
+            tqdm_disable: bool = False
+    ) -> dict:
+        """Main method of Block Purging.
+
+        Args:
+            blocks (dict): Blocks of entities.
+            data (Data): Data module. Contains all the information about the dataset.
+            tqdm_disable (bool, optional): Disable progress bar. Defaults to False.
+
+        Returns:
+            dict: Purged blocks.
+        """
+        self.tqdm_disable, self.data, start_time = tqdm_disable, data, time()
+        if not blocks:
+            raise AttributeError("Empty dict of blocks was given as input!")
+        else:
+            new_blocks = blocks.copy()
+        self._progress_bar = tqdm(total=2*len(new_blocks), desc=self._method_name, disable=self.tqdm_disable)            
+        self._set_threshold(new_blocks)
+        new_blocks = dict(filter(self._cardinality_threshold, blocks.items()))
+        self._progress_bar.close()
+        self.execution_time = time() - start_time
+        self.blocks = new_blocks
+
+        return new_blocks
+
+    def _cardinality_threshold(self, id_block_tuple) -> bool:
+        self._progress_bar.update(1)
+        return id_block_tuple[1].get_cardinality(self.data.is_dirty_er) <= self.max_comparisons_per_block
+
+    def _set_threshold(self, blocks: dict) -> None:
+        """Calculates the maximum number of comparisons per block, so in the next step to be purged.
+
+        Args:
+            blocks (dict): _description_
+        """
+        sorted_blocks = _sort_blocks_cardinality(blocks, self.data.is_dirty_er)
+        distinct_comparisons_level = set(b.get_cardinality(self.data.is_dirty_er) \
+                                        for _, b in sorted_blocks.items())
+        block_assignments = np.empty([len(distinct_comparisons_level)])
+        comparisons_level = np.empty([len(distinct_comparisons_level)])
+        total_comparisons_per_level = np.empty([len(distinct_comparisons_level)])
+        index = -1
+        for _, block in sorted_blocks.items():
+            if index == -1:
+                index += 1
+                comparisons_level[index] = block.get_cardinality(self.data.is_dirty_er)
+                block_assignments[index] = 0
+                total_comparisons_per_level[index] = 0
+            elif block.get_cardinality(self.data.is_dirty_er) != comparisons_level[index]:
+                index += 1
+                comparisons_level[index] = block.get_cardinality(self.data.is_dirty_er)
+                block_assignments[index] = block_assignments[index-1]
+                total_comparisons_per_level[index] = total_comparisons_per_level[index-1]
+
+            block_assignments[index] += block.get_size()
+            total_comparisons_per_level[index] += block.get_cardinality(self.data.is_dirty_er)
+            self._progress_bar.update(1)
+
+        current_bc = current_cc = current_size = \
+            previous_bc = previous_cc = previous_size = 0
+        for i in range(len(block_assignments)-1, 0, -1):
+            previous_size = current_size
+            previous_bc = current_bc
+            previous_cc = current_cc
+            current_size = comparisons_level[i]
+            current_bc = block_assignments[i]
+            current_cc = total_comparisons_per_level[i]
+            if current_bc * previous_cc < self.smoothing_factor * current_cc * previous_bc:
+                break
+        self.max_comparisons_per_block = previous_size
+
+    def _satisfies_threshold(self, block: Block) -> bool:
+        return block.get_cardinality(self.data.is_dirty_er) <= self.max_comparisons_per_block
+
+    def _configuration(self) -> dict:
+        return {
+            "Smoothing factor" : self.smoothing_factor,
+            "Max Comparisons per Block" : self.max_comparisons_per_block
+        }
+
+def _sort_blocks_cardinality(blocks: dict, is_dirty_er: bool) -> dict:
+    return dict(sorted(blocks.items(), key=lambda x: x[1].get_cardinality(is_dirty_er)))
```

### Comparing `pyjedai-0.0.4/src/pyjedai/comparison_cleaning.py` & `pyjedai-0.0.5/src/pyjedai/comparison_cleaning.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,40 @@
-from logging import warning
-import warnings
-import numpy as np
 import sys
-from time import time
+import warnings
+from itertools import chain
+from collections import defaultdict
+from logging import warning
 from math import log10
 from queue import PriorityQueue
-from tqdm.notebook import tqdm
-from .datamodel import Data
-from .utils import create_entity_index, chi_square
+from time import time
+
+import numpy as np
+from tqdm.autonotebook import tqdm
 
-class AbstractComparisonCleaning:
+from .evaluation import Evaluation
+
+from .datamodel import Data, PYJEDAIFeature
+from .utils import chi_square, create_entity_index
+
+from abc import ABC, abstractmethod
+
+
+class AbstractComparisonCleaning(PYJEDAIFeature):
     """Abstract class for Block cleaning
     """
 
     def __init__(self) -> None:
-        self.data: Data
+        super().__init__()
         self._limit: int
         self._num_of_blocks: int
         self._valid_entities: set() = set()
         self._entity_index: dict
-        self._progress_bar: tqdm
         self._weighting_scheme: str
-        self._blocks: dict() # initial blocks
+        self._blocks: dict # initial blocks
         self.blocks = dict() # blocks after CC
-        self.tqdm_disable: bool
-        self._progress_bar: tqdm
-        self.execution_time: float
         self._node_centric: bool
 
     def process(
             self,
             blocks: dict,
             data: Data,
             tqdm_disable: bool = False
@@ -41,37 +46,31 @@
             data (Data): dataset module
             tqdm_disable (bool, optional): Disables tqdm progress bars. Defaults to False.
 
         Returns:
             dict: cleaned blocks
         """
         start_time = time()
-        self.tqdm_disable, self.data = tqdm_disable, data, 
-        self._entity_index = create_entity_index(blocks, self.data.is_dirty_er)
-        self._num_of_blocks = len(blocks)
-        self._blocks: dict = blocks
+        self.tqdm_disable, self.data = tqdm_disable, data
         self._limit = self.data.num_of_entities \
-                    if self.data.is_dirty_er or self._node_centric else self.data.dataset_limit
+                if self.data.is_dirty_er or self._node_centric else self.data.dataset_limit
         self._progress_bar = tqdm(
             total=self._limit,
             desc=self._method_name,
             disable=self.tqdm_disable
         )
-        blocks = self._apply_main_processing()
+
+        self._entity_index = create_entity_index(blocks, self.data.is_dirty_er)
+        self._num_of_blocks = len(blocks)
+        self._blocks: dict = blocks
+        self._blocks = self._apply_main_processing()
         self.execution_time = time() - start_time
         self._progress_bar.close()
-        
-        return blocks
 
-    def method_configuration(self) -> dict:
-        return {
-            "name" : self._method_name,
-            "parameters" : self._configuration(),
-            "runtime": self.execution_time
-        }
+        return self._blocks
 
     def report(self) -> None:
         """Prints Block Building method configuration
         """
         print(
             "Method name: " + self._method_name +
             "\nMethod info: " + self._method_info +
@@ -79,19 +78,62 @@
             "Attributes from D1:\n\t" + ', '.join(c for c in (self.attributes_1 if self.attributes_1 is not None \
                 else self.data.dataset_1.columns)) +
             ("\nAttributes from D2:\n\t" + ', '.join(c for c in (self.attributes_2 if self.attributes_2 is not None \
                 else self.data.dataset_2.columns)) if not self.data.is_dirty_er else "") +
             "\nRuntime: {:2.4f} seconds".format(self.execution_time)
         )
 
-class AbstractMetablocking(AbstractComparisonCleaning):
-    """
-    Restructure a redundancy-positive block collection into a new
-    one that contains substantially lower number of redundant
-    and superfluous comparisons, while maintaining the original number of matching ones
+    @abstractmethod
+    def _apply_main_processing(self) -> dict:
+        pass
+
+    @abstractmethod
+    def _configuration(self) -> dict:
+        pass
+    
+    def stats(self) -> None:
+        pass
+
+    def evaluate(self,
+                 prediction,
+                 export_to_df: bool = False,
+                 export_to_dict: bool = False,
+                 with_classification_report: bool = False,
+                 verbose: bool = True) -> any:
+
+        if self.data is None:
+            raise AttributeError("Can not proceed to evaluation without data object.")
+
+        if self.data.ground_truth is None:
+            raise AttributeError("Can not proceed to evaluation without a ground-truth file. " +
+                    "Data object has not been initialized with the ground-truth file")
+
+        eval_obj = Evaluation(self.data)
+        true_positives = 0
+        total_matching_pairs = sum([len(block) for block in prediction.values()])
+        for _, (id1, id2) in self.data.ground_truth.iterrows():
+            id1 = self.data._ids_mapping_1[id1]
+            id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er \
+                                                else self.data._ids_mapping_2[id2]
+            if (id1 in prediction and id2 in prediction[id1]) or   \
+                (id2 in prediction and id1 in prediction[id2]):
+                true_positives += 1
+
+        eval_obj.calculate_scores(true_positives=true_positives, 
+                                  total_matching_pairs=total_matching_pairs)
+        return eval_obj.report(self.method_configuration(),
+                                export_to_df,
+                                export_to_dict,
+                                with_classification_report,
+                                verbose)
+
+class AbstractMetablocking(AbstractComparisonCleaning, ABC):
+    """Restructure a redundancy-positive block collection into a new
+        one that contains substantially lower number of redundant
+        and superfluous comparisons, while maintaining the original number of matching ones
     """
 
     def __init__(self) -> None:
         super().__init__()
         self._flags: np.array
         self._counters: np.array
         self._flags: np.array
@@ -107,14 +149,15 @@
 
     def _apply_main_processing(self) -> dict:
         self._counters = np.empty([self.data.num_of_entities], dtype=float)
         self._flags = np.empty([self.data.num_of_entities], dtype=int)
         if self.weighting_scheme == 'EJS':
             self._set_statistics()
         self._set_threshold()
+
         return self._prune_edges()
 
     def _get_weight(self, entity_id: int, neighbor_id: int) -> float:
         ws = self.weighting_scheme
         if ws == 'ARCS' or ws == 'CBS':
             return self._counters[neighbor_id]
         elif ws == 'ECBS':
@@ -129,80 +172,95 @@
         elif ws == 'EJS':
             probability = self._counters[neighbor_id] / (len(self._entity_index[entity_id]) + \
                             len(self._entity_index[neighbor_id]) - self._counters[neighbor_id])
             return float(probability * \
                     log10(self._distinct_comparisons / self._comparisons_per_entity[entity_id]) * \
                     log10(self._distinct_comparisons / self._comparisons_per_entity[neighbor_id]))
         elif ws == 'X2':
-            observed = [int(self._counters[neighbor_id]), 
+            observed = [int(self._counters[neighbor_id]),
                         int(len(self._entity_index[entity_id])-self._counters[neighbor_id])]
-            expected = [int(len(self._entity_index[neighbor_id])-observed[0]), 
+            expected = [int(len(self._entity_index[neighbor_id])-observed[0]),
                         int(self._num_of_blocks - (observed[0] + observed[1] - self._counters[neighbor_id]))]
             return chi_square(np.array([observed, expected]))
         else:
             raise ValueError("This weighting scheme does not exist")
 
     def _normalize_neighbor_entities(self, block_key: str, entity_id: int) -> None:
         self._neighbors.clear()
         if self.data.is_dirty_er:
             if not self._node_centric:
-                self._neighbors.update([neighbor_id for neighbor_id in self._blocks[block_key].entities_D1 if neighbor_id < entity_id])
+                self._neighbors.update(
+                    [neighbor_id for neighbor_id in self._blocks[block_key].entities_D1 \
+                        if neighbor_id < entity_id]
+                )
             else:
-                self._neighbors.update([neighbor_id for neighbor_id in self._blocks[block_key].entities_D1 if neighbor_id != entity_id])
+                self._neighbors.update(
+                    [neighbor_id for neighbor_id in self._blocks[block_key].entities_D1 \
+                        if neighbor_id != entity_id]
+                )
         else:
             if entity_id < self.data.dataset_limit:
                 self._neighbors.update(self._blocks[block_key].entities_D2)
             else:
                 self._neighbors.update(self._blocks[block_key].entities_D1)
 
     def _set_statistics(self) -> None:
         self._distinct_comparisons = 0
         self._comparisons_per_entity = np.empty([self.data.num_of_entities], dtype=float)
         distinct_neighbors = set()
         for entity_id in range(0, self.data.num_of_entities, 1):
             if entity_id in self._entity_index:
                 associated_blocks = self._entity_index[entity_id]
                 distinct_neighbors.clear()
-                for block_id in associated_blocks:
-                    distinct_neighbors = set.union(
-                        distinct_neighbors,
-                        self._get_neighbor_entities(block_id, entity_id)
-                    )
+                # distinct_neighbors = set().union(*[
+                #     self._get_neighbor_entities(block_id, entity_id) for block_id in associated_blocks
+                # ])
+                distinct_neighbors = set(chain.from_iterable(
+                    self._get_neighbor_entities(block_id, entity_id) for block_id in associated_blocks
+                ))
+                # for block_id in associated_blocks:
+                #     distinct_neighbors = set.union(
+                #         distinct_neighbors,
+                #         self._get_neighbor_entities(block_id, entity_id)
+                #     )
                 self._comparisons_per_entity[entity_id] = len(distinct_neighbors)
 
                 if self.data.is_dirty_er:
                     self._comparisons_per_entity[entity_id] -= 1
 
                 self._distinct_comparisons += self._comparisons_per_entity[entity_id]
         self._distinct_comparisons /= 2
 
     def _get_neighbor_entities(self, block_id: int, entity_id: int) -> set:
-        if not self.data.is_dirty_er and entity_id < self.data.dataset_limit:
-            return self._blocks[block_id].entities_D2
-        return self._blocks[block_id].entities_D1
-        
-class ComparisonPropagation(AbstractComparisonCleaning):
-    """_summary_
-    TODO ComparisonPropagation
-    Args:
-        AbstractComparisonCleaning (_type_): _description_
+        return self._blocks[block_id].entities_D2 \
+            if (not self.data.is_dirty_er and entity_id < self.data.dataset_limit) else \
+                self._blocks[block_id].entities_D1
 
-    Returns:
-        _type_: _description_
+    @abstractmethod
+    def _set_threshold(self):
+        pass
+
+    @abstractmethod
+    def _prune_edges(self) -> dict:
+        pass
+
+class ComparisonPropagation(AbstractComparisonCleaning):
+    """Comparison Propagation
     """
 
     _method_name = "Comparison Propagation"
+    _method_short_name: str = "CP"
     _method_info = "Eliminates all redundant comparisons from a set of overlapping blocks."
 
     def __init__(self) -> None:
         super().__init__()
         self._node_centric = False
 
     def _apply_main_processing(self) -> dict:
-        self.blocks = dict()
+        self.blocks = {}
         for i in range(0, self._limit):
             if i in self._entity_index:
                 self._valid_entities.clear()
                 associated_blocks = self._entity_index[i]
                 for block_index in associated_blocks:
                     if self.data.is_dirty_er:
                         self._valid_entities.update(
@@ -221,14 +279,15 @@
 
 class WeightedEdgePruning(AbstractMetablocking):
     """A Meta-blocking method that retains all comparisons \
         that have a weight higher than the average edge weight in the blocking graph.
     """
 
     _method_name = "Weighted Edge Pruning"
+    _method_short_name: str = "WEP"
     _method_info = "A Meta-blocking method that retains all comparisons " + \
                 "that have a weight higher than the average edge weight in the blocking graph."
 
     def __init__(self, weighting_scheme: str = 'CBS') -> None:
         super().__init__()
         self.weighting_scheme = weighting_scheme
         self._node_centric = False
@@ -273,58 +332,58 @@
         self._threshold = 0.0
 
         for i in range(0, self._limit):
             self._process_entity(i)
             self._update_threshold(i)
 
         self._threshold /= self._num_of_edges
-        
+
     def _verify_valid_entities(self, entity_id: int) -> None:    
         if entity_id not in self._entity_index:
             return
-            
+
         self._retained_neighbors.clear()
         for neighbor_id in self._valid_entities:
             weight = self._get_weight(entity_id, neighbor_id)
             if self._threshold <= weight:
                 self._retained_neighbors.add(neighbor_id)
 
         if len(self._retained_neighbors) > 0:
             self.blocks[entity_id] = self._retained_neighbors.copy()
 
     def _configuration(self) -> dict:
         return {
             "Node centric" : self._node_centric,
             "Weighting scheme" : self.weighting_scheme
         }
-        
+
 class CardinalityEdgePruning(WeightedEdgePruning):
     """A Meta-blocking method that retains the comparisons \
             that correspond to the top-K weighted edges in the blocking graph.
     """
 
     _method_name = "Cardinality Edge Pruning"
+    _method_short_name: str = "CEP"
     _method_info = "A Meta-blocking method that retains the comparisons " + \
                         "that correspond to the top-K weighted edges in the blocking graph."
 
     def __init__(self, weighting_scheme: str = 'JS') -> None:
         super().__init__(weighting_scheme)
         self._minimum_weight: float = sys.float_info.min
         self._top_k_edges: PriorityQueue
 
     def _prune_edges(self) -> dict:
-        self.blocks = dict()
+        self.blocks = defaultdict(set)
         self._top_k_edges = PriorityQueue(int(2*self._threshold))
         for i in range(0, self._limit):
             self._process_entity(i)
             self._verify_valid_entities(i)
             self._progress_bar.update(1)
         while not self._top_k_edges.empty():
             comparison = self._top_k_edges.get()
-            self.blocks.setdefault(comparison[1], set())
             self.blocks[comparison[1]].add(comparison[2])
 
         return self.blocks
 
     def _set_threshold(self) -> None:
         block_assignments = 0
         for block in self._blocks.values():
@@ -346,14 +405,15 @@
 
 class CardinalityNodePruning(CardinalityEdgePruning):
     """A Meta-blocking method that retains for every entity, \
         the comparisons that correspond to its top-k weighted edges in the blocking graph."
     """
 
     _method_name = "Cardinality Node Pruning"
+    _method_short_name: str = "CNP"
     _method_info = "A Meta-blocking method that retains for every entity, " + \
                     "the comparisons that correspond to its top-k weighted edges in the blocking graph."
 
     def __init__(self, weighting_scheme: str = 'CBS') -> None:
         super().__init__(weighting_scheme)
         self._nearest_entities: dict
         self._node_centric = True
@@ -380,15 +440,15 @@
 
     def _is_valid_comparison(self, entity_id: int, neighbor_id: int) -> bool:
         if neighbor_id not in self._nearest_entities:
             return True
         if entity_id in self._nearest_entities[neighbor_id]:
             return entity_id < neighbor_id
         return True
-        
+
     def _set_threshold(self) -> None:
         block_assignments = 0
         for block in self._blocks.values():
             block_assignments += block.get_size()
         self._threshold = max(1, block_assignments / self.data.num_of_entities)
 
     def _verify_valid_entities(self, entity_id: int) -> None:
@@ -413,14 +473,15 @@
 class ReciprocalCardinalityNodePruning(CardinalityNodePruning):
     """A Meta-blocking method that retains the comparisons \
         that correspond to edges in the blocking graph that are among the top-k weighted  \
         ones for both adjacent entities/nodes.
     """
 
     _method_name = "Reciprocal Cardinality Node Pruning"
+    _method_short_name: str = "RCNP"
     _method_info = "A Meta-blocking method that retains the comparisons " + \
                     "that correspond to edges in the blocking graph that are among " + \
                     "the top-k weighted ones for both adjacent entities/nodes."
 
     def __init__(self, weighting_scheme: str = 'ARCS') -> None:
         super().__init__(weighting_scheme)
 
@@ -434,14 +495,15 @@
 class WeightedNodePruning(WeightedEdgePruning):
     """A Meta-blocking method that retains for every entity, the comparisons \
         that correspond to edges in the blocking graph that are exceed \
         the average edge weight in the respective node neighborhood.
     """
 
     _method_name = "Weighted Node Pruning"
+    _method_short_name: str = "WNP"
     _method_info = "A Meta-blocking method that retains for every entity, the comparisons \
                     that correspond to edges in the blocking graph that are exceed \
                     the average edge weight in the respective node neighborhood."
 
     def __init__(self, weighting_scheme: str = 'CBS') -> None:
         super().__init__(weighting_scheme)
         self._average_weight: np.array
@@ -479,20 +541,20 @@
 
 class BLAST(WeightedNodePruning):
     """Meta-blocking method that retains the comparisons \
         that correspond to edges in the blocking graph that are exceed 1/4 of the sum \
         of the maximum edge weights in the two adjacent node neighborhoods.
     """
 
-    _method_name = "BLAST"
+    _method_name = _method_short_name = "BLAST"
     _method_info = "Meta-blocking method that retains the comparisons " + \
                 "that correspond to edges in the blocking graph that are exceed 1/4 of the sum " + \
                 "of the maximum edge weights in the two adjacent node neighborhoods."
 
-    def __init__(self, weighting_scheme: str = 'PEARSON_X2') -> None:
+    def __init__(self, weighting_scheme: str = 'X2') -> None:
         super().__init__(weighting_scheme)
 
     def _get_valid_weight(self, entity_id: int, neighbor_id: int) -> float:
         weight = self._get_weight(entity_id, neighbor_id)
         edge_threshold = (self._average_weight[entity_id] + self._average_weight[neighbor_id]) / 4
         return edge_threshold <= weight and entity_id < neighbor_id
 
@@ -507,38 +569,120 @@
 class ReciprocalWeightedNodePruning(WeightedNodePruning):
     """Meta-blocking method that retains the comparisons\
         that correspond to edges in the blocking graph that are \
         exceed the average edge weight in both adjacent node neighborhoods.
     """
 
     _method_name = "Reciprocal Weighted Node Pruning"
+    _method_short_name: str = "RWNP"
     _method_info = "Meta-blocking method that retains the comparisons " + \
                     "that correspond to edges in the blocking graph that are " + \
                     "exceed the average edge weight in both adjacent node neighborhoods."
 
     def __init__(self, weighting_scheme: str = 'ARCS') -> None:
         super().__init__(weighting_scheme)
 
     def _get_valid_weight(self, entity_id: int, neighbor_id: int) -> float:
         weight = self._get_weight(entity_id, neighbor_id)
         return weight if ((self._average_weight[entity_id] <= weight and \
                              self._average_weight[neighbor_id] <= weight) and
                                 entity_id < neighbor_id) else 0
 
-def get_meta_blocking_approach(acronym, w_scheme):
+class ProgressiveCardinalityEdgePruning(CardinalityEdgePruning):
+    def __init__(self, weighting_scheme: str = 'JS', budget: int = 0) -> None:
+        super().__init__(weighting_scheme)
+        self._budget = budget
+
+    def _set_threshold(self) -> None:
+        self._threshold = self._budget
+
+    def process(self, blocks: dict, data: Data, tqdm_disable: bool = False, cc: AbstractMetablocking = None) -> dict:
+
+        if(cc is None):
+            return super().process(blocks, data, tqdm_disable)
+        else:
+            self._threshold = self._budget
+            self._top_k_edges = PriorityQueue(int(2*self._threshold))
+            self._minimum_weight = sys.float_info.min            
+            self.trimmed_blocks : dict = defaultdict(set)
+
+            for entity_id, neighbors in blocks.items():
+                for neighbor_id in neighbors:
+                    weight = cc._get_weight(entity_id, neighbor_id)
+                    if weight >= self._minimum_weight:
+                        self._top_k_edges.put(
+                        (weight, entity_id, neighbor_id)
+                        )
+                        if self._threshold < self._top_k_edges.qsize():
+                            self._minimum_weight = self._top_k_edges.get()[0]
+
+            while not self._top_k_edges.empty():
+                comparison = self._top_k_edges.get()
+                self.trimmed_blocks[comparison[1]].add(comparison[2])
+
+            return self.trimmed_blocks
+
+class ProgressiveCardinalityNodePruning(CardinalityNodePruning):
+    def __init__(self, weighting_scheme: str = 'CBS', budget: int = 0) -> None:
+        super().__init__(weighting_scheme)
+        self._budget = budget
+
+    def _set_threshold(self) -> None:
+        self._threshold = max(1, 2 * self._budget / self.data.num_of_entities)
+
+    def process(self, blocks: dict, data: Data, tqdm_disable: bool = False, cc: AbstractMetablocking = None) -> dict:
+
+        if(cc is None):
+            return super().process(blocks, data, tqdm_disable)
+        else:
+            self._threshold = max(1, 2 * self._budget / data.num_of_entities)           
+            self.trimmed_blocks : dict = defaultdict(set)
+
+            for entity_id, neighbors in blocks.items():
+                self._minimum_weight = sys.float_info.min
+                self._top_k_edges = PriorityQueue(int(2*self._threshold))
+                for neighbor_id in neighbors:
+                    weight = cc._get_weight(entity_id, neighbor_id)
+                    if weight >= self._minimum_weight:
+                        self._top_k_edges.put(
+                        (weight, entity_id, neighbor_id)
+                        )
+                        if self._threshold < self._top_k_edges.qsize():
+                            self._minimum_weight = self._top_k_edges.get()[0]
+
+                while not self._top_k_edges.empty():
+                    comparison = self._top_k_edges.get()
+                    self.trimmed_blocks[entity_id].add(comparison[2])
+
+        return self.trimmed_blocks        
+
+def get_meta_blocking_approach(acronym: str, w_scheme: str, budget: int = 0) -> any:
+    """Return method by acronym
+
+    Args:
+        acronym (str): Method acronym
+        w_scheme (str): Weighting Scheme name
+
+    Returns:
+        any: Comparison Cleaning Method
+    """
     if acronym == "BLAST":
         return BLAST(w_scheme)
     elif acronym == "CEP":
         return CardinalityEdgePruning(w_scheme)
     elif acronym == "CNP":
         return CardinalityNodePruning(w_scheme)
     elif acronym == "RCNP":
         return ReciprocalCardinalityNodePruning(w_scheme)
     elif acronym == "RWNP":
         return ReciprocalWeightedNodePruning(w_scheme)
     elif acronym == "WEP":
         return WeightedEdgePruning(w_scheme)
     elif acronym == "WNP":
         return WeightedNodePruning(w_scheme)
+    elif acronym == "PCEP":
+        return ProgressiveCardinalityEdgePruning(w_scheme, budget)
+    elif acronym == "PCNP":
+        return ProgressiveCardinalityNodePruning(w_scheme, budget)
     else:
         warnings.warn("Wrong meta-blocking approach selected. Returning Comparison Propagation.")
         return ComparisonPropagation()
```

### Comparing `pyjedai-0.0.4/src/pyjedai/joins.py` & `pyjedai-0.0.5/src/pyjedai/joins.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,209 +1,216 @@
-import pandas as pd
-import tqdm
-from tqdm.notebook import tqdm
-import networkx
-from queue import PriorityQueue
-import nltk, re
-import numpy as np
+import itertools
 import math
-from time import time
+import re
+from collections import defaultdict
 from queue import PriorityQueue
-from .datamodel import Data
+from time import time
+
+import networkx
+import nltk
+import numpy as np
+import pandas as pd
+import tqdm
+from tqdm.autonotebook import tqdm
+
+from .datamodel import Data, PYJEDAIFeature
+from .evaluation import Evaluation
 
-class AbstractJoin:
+class AbstractJoin(PYJEDAIFeature):
     """Abstract class of Joins module
     """
 
     def __init__(
             self,
             metric: str,
             tokenization: str,
             qgrams: int = 2,
             similarity_threshold: float = None
     ) -> None:
+        """AbstractJoin Constructor
+
+        Args:
+            metric (str): String similarity metric
+            tokenization (str): Tokenizer
+            qgrams (int, optional): For Jaccard metric. Defaults to 2.
+            similarity_threshold (float, optional): Threshold for preserving pair. Defaults to None.
+        """
         self.metric = metric
         self.qgrams = qgrams
         self.tokenization = tokenization
         self._source_frequency: np.array
         self.similarity_threshold: float = similarity_threshold
-        self.data: Data
         self.reverse_order: bool
         self.attributes_1: list
         self.attributes_2: list
-        self.tqdm_disable: bool
-        self._progress_bar: tqdm
         self._flags: np.array
         self.pairs: networkx.Graph
 
-    def _tokenize_entity(self, entity: str) -> set:
-        if self.tokenization == 'qgrams':
-            return set([' '.join(grams) for grams in nltk.ngrams(entity.lower(), n=self.qgrams)])
-        elif self.tokenization == 'standard':
-            return set(filter(None, re.split('[\\W_]', entity.lower())))
-        elif self.tokenization == 'standard_multiset':
-            tok_ids_index = {}
-            multiset = set()
-            for tok in set(filter(None, re.split('[\\W_]', entity.lower()))):
-                tok_id =  tok_ids_index[tok] if tok in tok_ids_index else 0
-                multiset.add(tok+str(tok_id))
-                tok_ids_index[tok] = tok_id+1
-            return multiset
-        elif self.tokenization == 'qgrams_multiset':
-            grams_ids_index = {}
-            qgrams = set()
-            for gram in set([' '.join(grams) for grams in nltk.ngrams(entity.lower(), n=self.qgrams)]):
-                gram_id =  grams_ids_index[gram] if gram in grams_ids_index else 0
-                qgrams.add(gram+str(gram_id))
-                grams_ids_index[gram] = gram_id+1
-            return qgrams
-        else:
-            raise AttributeError("Tokenization not found")
-
-    def fit(
-            self,
+    def fit(self,
             data: Data,
             reverse_order: bool = False,
             attributes_1: list = None,
             attributes_2: list = None,
             tqdm_disable: bool = False
     ) -> networkx.Graph:
         """Joins main method
-        TODO
-        Args:
-            data (Data): dataset module
-            reverse_order (bool, optional): _description_. Defaults to False.
-            attributes_1 (list, optional): _description_. Defaults to None.
-            attributes_2 (list, optional): _description_. Defaults to None.
-            tqdm_disable (bool, optional): _description_. Defaults to False.
 
-        Returns:
-            networkx.Graph: _description_
+            Args:
+                data (Data): dataset module
+                reverse_order (bool, optional): _description_. Defaults to False.
+                attributes_1 (list, optional): _description_. Defaults to None.
+                attributes_2 (list, optional): _description_. Defaults to None.
+                tqdm_disable (bool, optional): _description_. Defaults to False.
+
+            Returns:
+                networkx.Graph: graph containg nodes as entities and edges as similarity score
         """
+        if reverse_order and data.is_dirty_er:
+            raise ValueError("Can't have reverse order in Dirty Entity Resolution")
+
         start_time = time()
         self.tqdm_disable, self.reverse_order, self.attributes_1, self.attributes_2, self.data = \
             tqdm_disable, reverse_order, attributes_1, attributes_2, data
-        if attributes_1:
-            isolated_attr_dataset_1 = data.dataset_1[attributes_1].apply(" ".join, axis=1)
-        if attributes_2:
-            isolated_attr_dataset_2 = data.dataset_2[attributes_1].apply(" ".join, axis=1)
-        if reverse_order and data.is_dirty_er:
-            raise ValueError("Can't have reverse order in Dity Entity Resolution")
-        if reverse_order:
-            num_of_entities = self.data.num_of_entities_2
-        else:
-            num_of_entities = self.data.num_of_entities_1
+
+        self._entities_d1 = data.dataset_1[attributes_1 if attributes_1 else data.attributes_1] \
+                            .apply(" ".join, axis=1) \
+                            .apply(self._tokenize_entity) \
+                            .values.tolist()
+
+        if not data.is_dirty_er:
+            self._entities_d2 = data.dataset_2[attributes_2 if attributes_2 else data.attributes_2] \
+                    .apply(" ".join, axis=1) \
+                    .apply(self._tokenize_entity) \
+                    .values.tolist()
+
+        num_of_entities = self.data.num_of_entities_2 if reverse_order else self.data.num_of_entities_1
+
         self._progress_bar = tqdm(
             total=self.data.num_of_entities if not self.data.is_dirty_er else num_of_entities*2,
             desc=self._method_name+" ("+self.metric+")", disable=self.tqdm_disable
         )
-        self._flags = np.empty([num_of_entities])
-        self._flags[:] = -1
-        self._counters = np.zeros([num_of_entities])
-        self._sims = np.empty([self.data.num_of_entities_1*self.data.num_of_entities_2])
-        self._source_frequency = np.empty([num_of_entities])
-
-        self.pairs = networkx.Graph()
-        if self.attributes_1 and isinstance(self.attributes_1, dict):
-            self.attributes_1 = list(self.attributes_1.keys())
-
-        if reverse_order:
-            entity_index = self._create_entity_index_d2()
-        else:
-            entity_index = self._create_entity_index_d1()
 
-        if self.attributes_2 and isinstance(self.attributes_2, dict):
-            self.attributes_2 = list(self.attributes_2.keys())
+        self._flags, \
+        self._counters, \
+        self._sims, \
+        self._source_frequency, \
+        self.pairs = np.empty([num_of_entities]), \
+                    np.zeros([num_of_entities]), \
+                    np.empty([self.data.num_of_entities_1*self.data.num_of_entities_2]), \
+                    np.empty([num_of_entities]), \
+                    networkx.Graph()
+        self._flags[:] = -1
+        entity_index = self._create_entity_index(
+                self._entities_d2 if reverse_order else self._entities_d1
+            )
 
         if self.data.is_dirty_er:
-            for i in range(0, self.data.num_of_entities_1):
+            eid = 0
+            for entity in self._entities_d1:
                 candidates = set()
-                record = isolated_attr_dataset_1.iloc[i] \
-                            if self.attributes_1 else self.data.entities_d1.iloc[i]
-                tokens = self._tokenize_entity(record)
-                for token in tokens:
+                for token in entity:
                     if token in entity_index:
                         current_candidates = entity_index[token]
                         for candidate_id in current_candidates:
-                            if self._flags[candidate_id] != i:
+                            if self._flags[candidate_id] != eid:
                                 self._counters[candidate_id] = 0
-                                self._flags[candidate_id] = i
+                                self._flags[candidate_id] = eid
                             self._counters[candidate_id] += 1
                             candidates.add(candidate_id)
-                            
-                self._process_candidates(candidates, i, len(tokens))
+                self._process_candidates(candidates, eid, len(entity))
                 self._progress_bar.update(1)
+                eid += 1
         else:
             if reverse_order:
-                dataset = self.data.dataset_1
-                entities = self.data.entities_d1
+                entities = self._entities_d1
                 num_of_entities = self.data.num_of_entities_1
-                attr = self.attributes_1
             else:
-                dataset = self.data.dataset_2
-                entities = self.data.entities_d2
+                entities = self._entities_d2
                 num_of_entities = self.data.num_of_entities_2
-                attr = self.attributes_2
-                
+
             for i in range(0, num_of_entities):
                 candidates = set()
-                record = dataset.iloc[i, attr] \
-                            if attr else entities.iloc[i]
-                tokens = self._tokenize_entity(record)
+                record = entities[i]
                 entity_id = i if reverse_order else i+self.data.dataset_limit
-                for token in tokens:
+                for token in record:
                     if token in entity_index:
                         current_candidates = entity_index[token]
                         for candidate_id in current_candidates:
                             if self._flags[candidate_id] != entity_id:
                                 self._counters[candidate_id] = 0
                                 self._flags[candidate_id] = entity_id
                             self._counters[candidate_id] += 1
                             candidates.add(candidate_id)
                 if 0 < len(candidates):
-                    self._process_candidates(candidates, entity_id, len(tokens))
+                    self._process_candidates(candidates, entity_id, len(record))
                 self._progress_bar.update(1)
         self._progress_bar.close()
         self.execution_time = time() - start_time
+
         return self.pairs
 
-    def _calc_similarity(self, common_tokens: int, source_frequency: int, tokens_size: int) -> float:
+    def _tokenize_entity(self, entity: str) -> set:
+        if self.tokenization == 'qgrams':
+            return set([' '.join(grams) for grams in nltk.ngrams(entity.lower(), n=self.qgrams)])
+        elif self.tokenization == 'standard':
+            return set(filter(None, re.split('[\\W_]', entity.lower())))
+        elif self.tokenization == 'standard_multiset':
+            tok_ids_index = {}
+            multiset = set()
+            for tok in set(filter(None, re.split('[\\W_]', entity.lower()))):
+                tok_id =  tok_ids_index[tok] if tok in tok_ids_index else 0
+                multiset.add(tok+str(tok_id))
+                tok_ids_index[tok] = tok_id+1
+            return multiset
+        elif self.tokenization == 'qgrams_multiset':
+            grams_ids_index = {}
+            qgrams = set()
+            for gram in set([' '.join(grams) for grams in nltk.ngrams(entity.lower(), n=self.qgrams)]):
+                gram_id =  grams_ids_index[gram] if gram in grams_ids_index else 0
+                qgrams.add(gram+str(gram_id))
+                grams_ids_index[gram] = gram_id+1
+            return qgrams
+        else:
+            raise AttributeError("Tokenization not found")
+
+    def _calc_similarity(
+            self,
+            common_tokens: int,
+            source_frequency: int,
+            tokens_size: int
+        ) -> float:
+        """Similarity score
+
+        Args:
+            common_tokens (int): number of common tokens
+            source_frequency (int): frequency
+            tokens_size (int): size of tokens
+
+        Returns:
+            float: similarity
+        """
         if self.metric == 'cosine':
             return common_tokens / math.sqrt(source_frequency*tokens_size)
         elif self.metric == 'dice':
             return 2 * common_tokens / (source_frequency+tokens_size)
         elif self.metric == 'jaccard':
-            return common_tokens / (source_frequency+tokens_size-common_tokens)        
+            return common_tokens / (source_frequency+tokens_size-common_tokens)
 
-    def _create_entity_index_d1(self):
-        entity_index_d1 = {}
-        for i in range(0, self.data.num_of_entities_1, 1):
-            record = self.data.dataset_1.iloc[i, self.attributes_1]  \
-                            if self.attributes_1 else self.data.entities_d1.iloc[i]
-            tokens = self._tokenize_entity(record)
-            for token in tokens:
-                entity_index_d1.setdefault(token, set())
-                entity_index_d1[token].add(i)
-            self._source_frequency[i] = len(tokens)
+    def _create_entity_index(self, entities: list) -> dict:
+        entity_index = defaultdict(set)
+        entity_id = itertools.count()
+        for entity in entities:
+            eid = next(entity_id)
+            for token in entity:
+                entity_index[token].add(eid)
+            self._source_frequency[eid] = len(entity)
             self._progress_bar.update(1)
-        return entity_index_d1
 
-    def _create_entity_index_d2(self):
-        entity_index = {}
-        for i in range(0, self.data.num_of_entities_2, 1):
-            record = self.data.dataset_2.iloc[i, self.attributes_2]  \
-                            if self.attributes_2 else self.data.entities_d2.iloc[i]
-            tokens = self._tokenize_entity(record)
-            for token in tokens:
-                entity_index.setdefault(token, set())
-                entity_index[token].add(i)
-            self._source_frequency[i] = len(tokens)
-            self._progress_bar.update(1)
         return entity_index
-    
+
 #     def _similarity(self, entity_id1: int, entity_id2: int, attributes: any=None) -> float:
 #         similarity: float = 0.0
 #         if isinstance(attributes, dict):
 #             for attribute, weight in self.attributes.items():
 #                 similarity += weight*self._metric(
 #                     self.data.entities.iloc[entity_id1][attribute],
 #                     self.data.entities.iloc[entity_id2][attribute]
@@ -223,69 +230,107 @@
 #                 self.data.entities.iloc[entity_id1].str.cat(sep=' '),
 #                 self.data.entities.iloc[entity_id2].str.cat(sep=' ')
 #             )
 #         return similarity
 
     def _insert_to_graph(self, entity_id1, entity_id2, similarity):
         if self.similarity_threshold <= similarity:
-            self.pairs.add_edge(entity_id1, entity_id2, weight=similarity)    
+            self.pairs.add_edge(entity_id1, entity_id2, weight=similarity)
+
+    def evaluate(self, prediction=None, export_to_df: bool = False,
+                 export_to_dict: bool = False, with_classification_report: bool = False,
+                 verbose: bool = True) -> any:
+        if self.data is None:
+            raise AttributeError("Can not proceed to evaluation without data object.")
+
+        if self.data.ground_truth is None:
+            raise AttributeError("Can not proceed to evaluation without a ground-truth file. " +
+                    "Data object has not been initialized with the ground-truth file")
+
+        eval_obj = Evaluation(self.data)
+        true_positives = 0
+        total_matching_pairs = prediction.number_of_edges()
+        for _, (id1, id2) in self.data.ground_truth.iterrows():
+            id1 = self.data._ids_mapping_1[id1]
+            id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er \
+                                                else self.data._ids_mapping_2[id2]
+            if (id1 in prediction and id2 in prediction[id1]) or   \
+                 (id2 in prediction and id1 in prediction[id2]):
+                true_positives += 1
+
+        eval_obj.calculate_scores(true_positives=true_positives, 
+                                  total_matching_pairs=total_matching_pairs)
+        return eval_obj.report(self.method_configuration(),
+                        export_to_df,
+                        export_to_dict,
+                        with_classification_report,
+                        verbose)
+
+    def stats(self) -> None:
+        pass
+
+    def _configuration(self) -> dict:
+        return {
+            "similarity_threshold" : self.similarity_threshold,
+            "metric" : self.metric,
+            "tokenization" : self.tokenization,
+            "qgrams": self.qgrams
+        }    
 
-class SchemaAgnosticΕJoin(AbstractJoin):
+class ΕJoin(AbstractJoin):
     """
-    TODO
+     Ε Join algorithm
     """
-    
-    _method_name = "Schema Agnostic Join"
-    # TODO _method_info = ""
+    _method_name = "EJoin"
+    _method_info = " ΕJoin algorithm"
+    _method_short_name = "EJ"
 
     def __init__(
         self,
-        threshold: float = 0.82,
+        similarity_threshold: float = 0.82,
         metric: str = 'cosine',
         tokenization: str = 'qgrams',
         qgrams: int = 2
     ) -> None:
-        super().__init__(metric, tokenization, qgrams, threshold)
+        super().__init__(metric, tokenization, qgrams, similarity_threshold)
 
     def _process_candidates(self, candidates: set, entity_id: int, tokens_size: int) -> None:
         for candidate_id in candidates:
             self._insert_to_graph(
-                candidate_id+self.data.dataset_limit if self.reverse_order and not self.data.is_dirty_er \
-                                else candidate_id,
-                entity_id, 
+                candidate_id+self.data.dataset_limit if self.reverse_order \
+                                                        and not self.data.is_dirty_er \
+                                                    else candidate_id,
+                entity_id,
                 self._calc_similarity(
-                    self._counters[candidate_id], 
+                    self._counters[candidate_id],
                     self._source_frequency[candidate_id],
                     tokens_size
                 )
             )
 
-class TopKSchemaAgnosticJoin(AbstractJoin):
-    """_summary_
-    TODO
-    Args:
-        AbstractJoin (_type_): _description_
+class TopKJoin(AbstractJoin):
+    """Top-K Join algorithm
     """
 
-    _method_name = "Top-K Schema Agnostic Join"
-    # TODO _method_info = ""
-
-    def __init__(
-            self, K: int,
-            metric: str,
-            tokenization: str,
-            qgrams: int = 2
-    ) -> None:
+    _method_name = "Top-K Join"
+    _method_info = "Top-K Join algorithm"
+    _method_short_name = "TopKJ"
+
+    def __init__(self,
+                 K: int,
+                 metric: str,
+                 tokenization: str,
+                 qgrams: int = 2
+        ) -> None:
         super().__init__(metric, tokenization, qgrams)
         self.K = K
 
     def _process_candidates(self, candidates: set, entity_id: int, tokens_size: int) -> None:
         minimum_weight=0
         pq = PriorityQueue()
-
         for candidate_id in candidates:
             sim = self._calc_similarity(
                 self._counters[candidate_id], self._source_frequency[candidate_id], tokens_size
             )
             if minimum_weight < sim:
                 pq.put(sim)
                 if self.K < pq.qsize():
@@ -299,7 +344,16 @@
                 entity_id,
                 self._calc_similarity(
                     self._counters[candidate_id], 
                     self._source_frequency[candidate_id],
                     tokens_size
                 )
             )
+
+    def _configuration(self) -> dict:
+        return {
+            "similarity_threshold" : self.similarity_threshold,
+            "K" : self.K,
+            "metric" : self.metric,
+            "tokenization" : self.tokenization,
+            "qgrams": self.qgrams
+        }
```

### Comparing `pyjedai-0.0.4/src/pyjedai/visualization.py` & `pyjedai-0.0.5/src/pyjedai/visualization.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.4/src/pyjedai.egg-info/PKG-INFO` & `pyjedai-0.0.5/src/pyjedai.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjedai
-Version: 0.0.4
+Version: 0.0.5
 Summary: An open-source library that builds powerful end-to-end Entity Resolution workflows.
 Author-email: Konstantinos Nikoletos <nikoletos.kon@gmail.com>, George Papadakis <gpapadis84@gmail.com>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://github.com/AI-team-UoA/pyJedAI
 Project-URL: Documentation, https://github.com/AI-team-UoA/pyJedAI/wiki
 Project-URL: Bug Tracker, https://github.com/AI-team-UoA/pyJedAI/issues
 Project-URL: Source code, https://github.com/AI-team-UoA/pyJedAI/tree/main/pyjedai
@@ -40,20 +40,14 @@
 <br>
 <div align="center">
 An open-source library that leverages Python’s data science ecosystem to build <br> powerful end-to-end Entity Resolution workflows.
 </div>
 
 ---
 
-[![Tests](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/tests.yml)
-[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
-[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
-[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-
 <!--
 [![DOI:10.1007/978-3-319-76207-4_15](https://zenodo.org/badge/DOI/10.1007/978-3-319-76207-4_15.svg)](https://doi.org/10.1007/978-3-319-76207-4_15)
 [![Citation Badge](https://api.juleskreuer.eu/citation-badge.php?doi=10.1126/science.1058040)](https://juleskreuer.eu/projekte/citation-badge/)
 --->
 
 
 # Overview
@@ -111,26 +105,35 @@
 </div>
 
 <br>
 <br>
 
 See the full list of dependencies and all versions used, in this [file](https://github.com/AI-team-UoA/pyJedAI/blob/main/requirements.txt).
 
+
+__Status__ 
+
+[![Tests](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml)
+[![made-with-python](https://readthedocs.org/projects/pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/?badge=latest)
+
+
+
 # Bugs, Discussions & News
 
 [GitHub Discussions](https://github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum for general questions and discussions and our recommended starting point. Please report any bugs that you find [here](https://github.com/AI-team-UoA/pyJedAI/issues).
 
 # Team & Authors
 
-<img align="right" src="https://www.di.uoa.gr/themes/corporate_lite/logo_en.png" alt="pyJedAI" width="400"/>
+<img align="right" src="https://github.com/AI-team-UoA/.github/blob/main/AI_LOGO.png?raw=true" alt="pyJedAI" width="200"/>
 
 - [Konstantinos Nikoletos](https://nikoletos-k.github.io)
+- Jakub Maciejewski
 - [George Papadakis](https://gpapadis.wordpress.com)
 - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/)
 
 Research and development is made under the supervision of Pr. Manolis Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the University of Athens.
 
 # License
 
 Released under the Apache-2.0 license [(see LICENSE.txt)](https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE).
 
-2022-2023 | AI-Team @ University of Athens
+2023 | AI-Team @ University of Athens
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyjedai Version: 0.0.4 Summary: An open-source
+Metadata-Version: 2.1 Name: pyjedai Version: 0.0.5 Summary: An open-source
 library that builds powerful end-to-end Entity Resolution workflows. Author-
 email: Konstantinos Nikoletos
 kon@gmail.com>, George Papadakis
 gmail.com> License: Apache Software License 2.0 Project-URL: Homepage, https://
 github.com/AI-team-UoA/pyJedAI Project-URL: Documentation, https://github.com/
 AI-team-UoA/pyJedAI/wiki Project-URL: Bug Tracker, https://github.com/AI-team-
 UoA/pyJedAI/issues Project-URL: Source code, https://github.com/AI-team-UoA/
@@ -24,33 +24,26 @@
 
                                    [pyJedAI]
 
 
   An open-source library that leverages Pythonâs data science ecosystem to
                                     build
                powerful end-to-end Entity Resolution workflows.
---- [![Tests](https://github.com/AI-team-UoA/pyJedAI/actions/workflows/
-tests.yml/badge.svg?branch=main)](https://github.com/AI-team-UoA/pyJedAI/
-actions/workflows/tests.yml) [![Linux](https://svgshare.com/i/Zhy.svg)](https:/
-/svgshare.com/i/Zhy.svg) [![macOS](https://svgshare.com/i/ZjP.svg)](https://
-svgshare.com/i/ZjP.svg) [![Windows](https://svgshare.com/i/ZhY.svg)](https://
-svgshare.com/i/ZhY.svg) [![made-with-python](https://img.shields.io/badge/
-Made%20with-Python-1f425f.svg)](https://www.python.org/)  # Overview pyJedAI is
-a python framework, aiming to offer experts and novice users, robust and fast
-solutions for multiple types of Entity Resolution problems. It is builded using
-state-of-the-art python frameworks. pyJedAI constitutes the sole open-source
-Link Discovery tool that is capable of exploiting the latest breakthroughs in
-Deep Learning and NLP techniques, which are publicly available through the
-Python data science ecosystem. This applies to both blocking and matching, thus
-ensuring high time efficiency, high scalability as well as high effectiveness,
-without requiring any labelled instances from the user. ### Key-Features -
-Input data-type independent. Both structured and semi-structured data can be
-processed. - Various implemented algorithms. - Easy-to-use. - Utilizes some of
-the famous and cutting-edge machine learning packages.  __Open demo python
-notebook:__
+---  # Overview pyJedAI is a python framework, aiming to offer experts and
+novice users, robust and fast solutions for multiple types of Entity Resolution
+problems. It is builded using state-of-the-art python frameworks. pyJedAI
+constitutes the sole open-source Link Discovery tool that is capable of
+exploiting the latest breakthroughs in Deep Learning and NLP techniques, which
+are publicly available through the Python data science ecosystem. This applies
+to both blocking and matching, thus ensuring high time efficiency, high
+scalability as well as high effectiveness, without requiring any labelled
+instances from the user. ### Key-Features - Input data-type independent. Both
+structured and semi-structured data can be processed. - Various implemented
+algorithms. - Easy-to-use. - Utilizes some of the famous and cutting-edge
+machine learning packages.  __Open demo python notebook:__
        [https://nbviewer.org/static/img/nav_logo.svg]         [https://
             miro.medium.com/max/1400/1*Edn_LpbSpLeNKfWkEdG2Jg.png]
 
 For more tutorials go to [pyJedAI/tutorials](https://github.com/AI-team-UoA/
 pyJedAI/tree/main/tutorials). # Install Install the latest version of pyjedai
 __[requires python >= 3.7]__: ``` pip install pyjedai ``` The source code is
 currently hosted on GitHub at: [AI-team-UoA/pyJedAI](https://github.com/AI-
@@ -70,20 +63,25 @@
  [https://www.kornosk.me/resources/language-model/featured.png]     [https://
    repository-images.githubusercontent.com/1349775/202c4680-8f7c-11e9-91c6-
 745fdcbeffe8]     [https://networkx.org/_static/networkx_logo.svg]     [https:/
           /raw.githubusercontent.com/RDFLib/OWL-RL/master/OWL-RL.png]
 
 
 See the full list of dependencies and all versions used, in this [file](https:/
-/github.com/AI-team-UoA/pyJedAI/blob/main/requirements.txt). # Bugs,
-Discussions & News [GitHub Discussions](https://github.com/AI-team-UoA/pyJedAI/
-discussions) is the discussion forum for general questions and discussions and
-our recommended starting point. Please report any bugs that you find [here]
-(https://github.com/AI-team-UoA/pyJedAI/issues). # Team & Authors [pyJedAI] -
-[Konstantinos Nikoletos](https://nikoletos-k.github.io) - [George Papadakis]
-(https://gpapadis.wordpress.com) - [Manolis Koubarakis](https://cgi.di.uoa.gr/
-~koubarak/) Research and development is made under the supervision of Pr.
-Manolis Koubarakis. This is a research project by the [AI-Team](https://
-ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the
-University of Athens. # License Released under the Apache-2.0 license [(see
-LICENSE.txt)](https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE). 2022-
-2023 | AI-Team @ University of Athens
+/github.com/AI-team-UoA/pyJedAI/blob/main/requirements.txt). __Status__ [!
+[Tests](https://github.com/Nikoletos-K/pyJedAI/actions/workflows/tests.yml/
+badge.svg?branch=main)](https://github.com/Nikoletos-K/pyJedAI/actions/
+workflows/tests.yml) [![made-with-python](https://readthedocs.org/projects/
+pyjedai/badge/?version=latest)](https://pyjedai.readthedocs.io/en/latest/
+?badge=latest) # Bugs, Discussions & News [GitHub Discussions](https://
+github.com/AI-team-UoA/pyJedAI/discussions) is the discussion forum for general
+questions and discussions and our recommended starting point. Please report any
+bugs that you find [here](https://github.com/AI-team-UoA/pyJedAI/issues). #
+Team & Authors [pyJedAI] - [Konstantinos Nikoletos](https://nikoletos-
+k.github.io) - Jakub Maciejewski - [George Papadakis](https://
+gpapadis.wordpress.com) - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/
+) Research and development is made under the supervision of Pr. Manolis
+Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr)
+of the Department of Informatics and Telecommunications at the University of
+Athens. # License Released under the Apache-2.0 license [(see LICENSE.txt)]
+(https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE). 2023 | AI-Team @
+University of Athens
```

### Comparing `pyjedai-0.0.4/src/pyjedai.egg-info/SOURCES.txt` & `pyjedai-0.0.5/src/pyjedai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/pyjedai/block_building.py
 src/pyjedai/block_cleaning.py
 src/pyjedai/clustering.py
 src/pyjedai/comparison_cleaning.py
 src/pyjedai/datamodel.py
 src/pyjedai/evaluation.py
 src/pyjedai/joins.py
+src/pyjedai/logs.py
 src/pyjedai/matching.py
 src/pyjedai/utils.py
 src/pyjedai/vector_based_blocking.py
 src/pyjedai/visualization.py
 src/pyjedai/workflow.py
 src/pyjedai.egg-info/PKG-INFO
 src/pyjedai.egg-info/SOURCES.txt
```

