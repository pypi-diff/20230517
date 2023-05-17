# Comparing `tmp/RiskLabAI-0.0.1.tar.gz` & `tmp/RiskLabAI-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RiskLabAI-0.0.1.tar", last modified: Tue Sep 13 05:51:16 2022, max compression
+gzip compressed data, was "RiskLabAI-0.0.4.tar", last modified: Wed May 17 13:40:23 2023, max compression
```

## Comparing `RiskLabAI-0.0.1.tar` & `RiskLabAI-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-09-13 05:51:16.925230 RiskLabAI-0.0.1/
--rw-rw-rw-   0        0        0     1727 2022-09-13 04:47:57.000000 RiskLabAI-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      635 2022-09-13 05:51:16.926230 RiskLabAI-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2022-09-13 04:47:57.000000 RiskLabAI-0.0.1/README.md
--rw-rw-rw-   0        0        0      765 2022-09-13 05:51:16.938221 RiskLabAI-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       67 2022-09-13 05:08:03.000000 RiskLabAI-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-13 05:51:16.873260 RiskLabAI-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2022-09-13 05:51:16.923232 RiskLabAI-0.0.1/src/RiskLabAI.egg-info/
--rw-rw-rw-   0        0        0      635 2022-09-13 05:51:16.000000 RiskLabAI-0.0.1/src/RiskLabAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2022-09-13 05:51:16.000000 RiskLabAI-0.0.1/src/RiskLabAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-13 05:51:16.000000 RiskLabAI-0.0.1/src/RiskLabAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2022-09-13 05:51:16.000000 RiskLabAI-0.0.1/src/RiskLabAI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2022-09-13 05:51:16.000000 RiskLabAI-0.0.1/src/RiskLabAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:40:23.697558 RiskLabAI-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-17 13:40:23.697558 RiskLabAI-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:40:23.689558 RiskLabAI-0.0.4/RiskLabAI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:40:23.689558 RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-17 13:40:23.000000 RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-17 13:40:23.000000 RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:40:23.000000 RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 13:40:23.000000 RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 13:40:23.000000 RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:40:23.689558 RiskLabAI-0.0.4/RiskLabAI/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:40:23.689558 RiskLabAI-0.0.4/RiskLabAI/data/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/structures/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/structures/hedging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/structures/infomation_driven_bars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/structures/standard_bars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/data/structures/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:40:23.697558 RiskLabAI-0.0.4/RiskLabAI/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/RiskLabAI/utils/smoothing_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-17 13:40:23.697558 RiskLabAI-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 13:40:09.000000 RiskLabAI-0.0.4/setup.py
```

### Comparing `RiskLabAI-0.0.1/LICENSE` & `RiskLabAI-0.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-BSD 3-Clause License
-
-Copyright (c) 2022, RiskLab AI (risklab.ai)
-All rights reserved.
-
-RiskLabAI includes codes and algorithms from Marcos López de Prado's books 
-"Advances in Financial Machine Learning" and 
-"Machine Learning for Asset Managers".
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2022, RiskLab AI (risklab.ai)
+All rights reserved.
+
+RiskLabAI includes codes and algorithms from Marcos López de Prado's books 
+"Advances in Financial Machine Learning" and 
+"Machine Learning for Asset Managers".
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `RiskLabAI-0.0.1/PKG-INFO` & `RiskLabAI-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-Metadata-Version: 2.1
-Name: RiskLabAI
-Version: 0.0.1
-Summary: Financial AI using Python.
-Home-page: https://github.com/RiskLabAI/RiskLabAI.py
-Author: RiskLab
-Author-email: research@risklab.ai
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/RiskLabAI/RiskLabAI.py/issues
-Project-URL: Changelog, https://github.com/RiskLabAI/RiskLabAI.py/releases
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: RiskLabAI
+Version: 0.0.4
+Summary: Financial AI using Python.
+Home-page: https://github.com/RiskLabAI/RiskLabAI.py
+Author: RiskLab
+Author-email: research@risklab.ai
+Project-URL: Bug Tracker, https://github.com/RiskLabAI/RiskLabAI.py/issues
+Project-URL: Changelog, https://github.com/RiskLabAI/RiskLabAI.py/releases
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
```

### Comparing `RiskLabAI-0.0.1/src/RiskLabAI.egg-info/PKG-INFO` & `RiskLabAI-0.0.4/RiskLabAI/RiskLabAI.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-Metadata-Version: 2.1
-Name: RiskLabAI
-Version: 0.0.1
-Summary: Financial AI using Python.
-Home-page: https://github.com/RiskLabAI/RiskLabAI.py
-Author: RiskLab
-Author-email: research@risklab.ai
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/RiskLabAI/RiskLabAI.py/issues
-Project-URL: Changelog, https://github.com/RiskLabAI/RiskLabAI.py/releases
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: RiskLabAI
+Version: 0.0.4
+Summary: Financial AI using Python.
+Home-page: https://github.com/RiskLabAI/RiskLabAI.py
+Author: RiskLab
+Author-email: research@risklab.ai
+Project-URL: Bug Tracker, https://github.com/RiskLabAI/RiskLabAI.py/issues
+Project-URL: Changelog, https://github.com/RiskLabAI/RiskLabAI.py/releases
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
```

