# Comparing `tmp/triglav-1.0.2.tar.gz` & `tmp/triglav-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triglav-1.0.2.tar", last modified: Tue May 16 22:07:49 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `triglav-1.0.2.tar` & `triglav-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:07:49.343427 triglav-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-16 22:07:35.000000 triglav-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-16 22:07:49.343427 triglav-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-16 22:07:35.000000 triglav-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-16 22:07:35.000000 triglav-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 22:07:49.343427 triglav-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:07:49.343427 triglav-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-16 22:07:35.000000 triglav-1.0.2/tests/test_triglav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:07:49.343427 triglav-1.0.2/triglav.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-16 22:07:49.000000 triglav-1.0.2/triglav.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 22:07:49.000000 triglav-1.0.2/triglav.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:07:49.000000 triglav-1.0.2/triglav.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-16 22:07:49.000000 triglav-1.0.2/triglav.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 22:07:49.000000 triglav-1.0.2/triglav.egg-info/top_level.txt
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 triglav-1.0.3/environment.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 triglav-1.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 triglav-1.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 triglav-1.0.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 triglav-1.0.3/.github/workflows/draft-pdf.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 triglav-1.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 triglav-1.0.3/docs/API.md
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 triglav-1.0.3/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0   139948 2020-02-02 00:00:00.000000 triglav-1.0.3/notebooks/01_random_dataset.ipynb
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 triglav-1.0.3/notebooks/README.md
+-rw-r--r--   0        0        0   148463 2020-02-02 00:00:00.000000 triglav-1.0.3/notebooks/Diseased-Gut-Analysis/16S_CD_stability.ipynb
+-rw-r--r--   0        0        0   541360 2020-02-02 00:00:00.000000 triglav-1.0.3/notebooks/Diseased-Gut-Analysis/16S_end_to_end.ipynb
+-rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 triglav-1.0.3/notebooks/Diseased-Gut-Analysis/stability.py
+-rw-r--r--   0        0        0  1481934 2020-02-02 00:00:00.000000 triglav-1.0.3/notebooks/Diseased-Gut-Analysis/Diseased Gut/ESV.table
+-rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 triglav-1.0.3/notebooks/Diseased-Gut-Analysis/Diseased Gut/metadata.csv
+-rw-r--r--   0        0        0   507476 2020-02-02 00:00:00.000000 triglav-1.0.3/notebooks/Diseased-Gut-Analysis/Diseased Gut/rdp.out.tmp
+-rw-r--r--   0        0        0    78793 2020-02-02 00:00:00.000000 triglav-1.0.3/paper/Figure 1.svg
+-rw-r--r--   0        0        0   975750 2020-02-02 00:00:00.000000 triglav-1.0.3/paper/Figure 2.svg
+-rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 triglav-1.0.3/paper/paper.bib
+-rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 triglav-1.0.3/paper/paper.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 triglav-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 triglav-1.0.3/tests/test_triglav.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 triglav-1.0.3/tests/data/expected_output.csv
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 triglav-1.0.3/triglav/__init__.py
+-rw-r--r--   0        0        0    37911 2020-02-02 00:00:00.000000 triglav-1.0.3/triglav/triglav.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 triglav-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 triglav-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 triglav-1.0.3/README.md
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 triglav-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 triglav-1.0.3/PKG-INFO
```

### Comparing `triglav-1.0.2/LICENSE` & `triglav-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `triglav-1.0.2/PKG-INFO` & `triglav-1.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Metadata-Version: 2.1
 Name: triglav
-Version: 1.0.2
+Version: 1.0.3
 Summary: Triglav: Iterative Refinement and Selection of Stable Features Using Shapley Values
+Project-URL: Homepage, https://github.com/jrudar/Triglav
+Project-URL: Repository, https://github.com/jrudar/Triglav.git
+Project-URL: Bug Tracker, https://github.com/jrudar/Triglav/issues
 Author: Peter Kruczkiewicz, G. Brian Golding, Oliver Lung
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
         
         Copyright (c) 2023 Josip Rudar, Peter Kruczkiewicz, Oliver Lung, G.Brian Golding, Mehrdad Hajibabaei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,34 +24,47 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/jrudar/Triglav
-Project-URL: Repository, https://github.com/jrudar/Triglav.git
-Project-URL: Bug Tracker, https://github.com/jrudar/Triglav/issues
-Keywords: ecology,multivariate statistics,feature selection,stability selection
+License-File: LICENSE
+Keywords: ecology,feature selection,multivariate statistics,stability selection
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Requires-Dist: imbalanced-learn>=0.10.1
+Requires-Dist: joblib>=1.1.0
+Requires-Dist: matplotlib>=3.4.3
+Requires-Dist: numpy==1.23.5
+Requires-Dist: sage-importance>=0.0.5
+Requires-Dist: scikit-bio>=0.5.8
+Requires-Dist: scikit-learn>=1.0.1
+Requires-Dist: scipy>=1.7.3
+Requires-Dist: shap>=0.40.0
+Requires-Dist: statsmodels>=0.12.0
 Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: twine; extra == 'dev'
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Description-Content-Type: text/markdown
 
 # Triglav - Feature Selection Using Iterative Refinement
 
 [![CI](https://github.com/jrudar/Triglav/actions/workflows/ci.yml/badge.svg)](https://github.com/jrudar/Triglav/actions/workflows/ci.yml)
 [![Draft PDF](https://github.com/jrudar/Triglav/actions/workflows/draft-pdf.yml/badge.svg)](https://github.com/jrudar/Triglav/actions/workflows/draft-pdf.yml)
 
 ## Overview
```

### Comparing `triglav-1.0.2/README.md` & `triglav-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `triglav-1.0.2/pyproject.toml` & `triglav-1.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+[build-system]
+build-backend = "hatchling.build"
+requires = ["hatchling"]
+
 [project]
 name = "triglav"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
     {name = "Peter Kruczkiewicz"},
     {name = "G. Brian Golding"},
     {name = "Oliver Lung"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
@@ -51,26 +55,19 @@
 
 [project.optional-dependencies]
 dev = [
     "black",
     "mypy",
     "ruff",
     "twine",
-    "wheel",
 ]
+
 test = [
     "pytest",
     "pytest-cov"
 ]
 
-[tool.setuptools]
-py-modules = ["triglav"]
-
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 70"
 
 [tool.coverage.run]
 source = ["triglav"]
-
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = ["setuptools", "wheel"]
```

### Comparing `triglav-1.0.2/tests/test_triglav.py` & `triglav-1.0.3/tests/test_triglav.py`

 * *Files identical despite different names*

