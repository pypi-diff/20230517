# Comparing `tmp/fast_poisson_solver-0.1.1.tar.gz` & `tmp/fast_poisson_solver-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_poisson_solver-0.1.1.tar", max compression
+gzip compressed data, was "fast_poisson_solver-0.1.2.tar", max compression
```

## Comparing `fast_poisson_solver-0.1.1.tar` & `fast_poisson_solver-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      875 2023-05-16 12:29:28.632704 fast_poisson_solver-0.1.1/fast_poisson_solver/__init__.py
--rw-r--r--   0        0        0     6142 2023-05-16 15:17:14.183908 fast_poisson_solver-0.1.1/fast_poisson_solver/analyze.py
--rw-r--r--   0        0        0    15699 2023-05-17 07:05:24.430390 fast_poisson_solver-0.1.1/fast_poisson_solver/data.py
--rw-r--r--   0        0        0     7662 2023-05-15 08:15:52.798338 fast_poisson_solver-0.1.1/fast_poisson_solver/data_utils/source_functions.py
--rw-r--r--   0        0        0     2037 2023-02-07 12:41:32.954182 fast_poisson_solver-0.1.1/fast_poisson_solver/diff_matrices.py
--rw-r--r--   0        0        0     6705 2023-05-15 08:15:52.618334 fast_poisson_solver-0.1.1/fast_poisson_solver/model.py
--rw-r--r--   0        0        0     6300 2023-05-17 08:23:50.210866 fast_poisson_solver-0.1.1/fast_poisson_solver/numeric_solver.py
--rw-r--r--   0        0        0    17864 2023-05-16 15:17:14.219909 fast_poisson_solver-0.1.1/fast_poisson_solver/plotter.py
--rw-r--r--   0        0        0    14052 2023-05-17 07:23:46.769675 fast_poisson_solver-0.1.1/fast_poisson_solver/solver.py
--rw-r--r--   0        0        0     6890 2023-05-16 15:17:14.147907 fast_poisson_solver-0.1.1/fast_poisson_solver/utils.py
--rw-r--r--   0        0        0    35823 2023-05-14 14:36:23.182354 fast_poisson_solver-0.1.1/LICENSE
--rw-r--r--   0        0        0     1316 2023-05-17 09:52:14.756574 fast_poisson_solver-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5400 2023-05-17 09:51:11.819440 fast_poisson_solver-0.1.1/README.md
--rw-r--r--   0        0        0     7050 1970-01-01 00:00:00.000000 fast_poisson_solver-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      875 2023-05-16 12:29:28.632704 fast_poisson_solver-0.1.2/fast_poisson_solver/__init__.py
+-rw-r--r--   0        0        0     6142 2023-05-16 15:17:14.183908 fast_poisson_solver-0.1.2/fast_poisson_solver/analyze.py
+-rw-r--r--   0        0        0    15699 2023-05-17 07:05:24.430390 fast_poisson_solver-0.1.2/fast_poisson_solver/data.py
+-rw-r--r--   0        0        0     7662 2023-05-15 08:15:52.798338 fast_poisson_solver-0.1.2/fast_poisson_solver/data_utils/source_functions.py
+-rw-r--r--   0        0        0     2037 2023-02-07 12:41:32.954182 fast_poisson_solver-0.1.2/fast_poisson_solver/diff_matrices.py
+-rw-r--r--   0        0        0     6705 2023-05-15 08:15:52.618334 fast_poisson_solver-0.1.2/fast_poisson_solver/model.py
+-rw-r--r--   0        0        0     6300 2023-05-17 08:23:50.210866 fast_poisson_solver-0.1.2/fast_poisson_solver/numeric_solver.py
+-rw-r--r--   0        0        0    17864 2023-05-16 15:17:14.219909 fast_poisson_solver-0.1.2/fast_poisson_solver/plotter.py
+-rw-r--r--   0        0        0    14052 2023-05-17 07:23:46.769675 fast_poisson_solver-0.1.2/fast_poisson_solver/solver.py
+-rw-r--r--   0        0        0     6890 2023-05-16 15:17:14.147907 fast_poisson_solver-0.1.2/fast_poisson_solver/utils.py
+-rw-r--r--   0        0        0    35823 2023-05-14 14:36:23.182354 fast_poisson_solver-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1316 2023-05-17 09:55:27.612680 fast_poisson_solver-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5164 2023-05-17 09:54:46.480390 fast_poisson_solver-0.1.2/README.md
+-rw-r--r--   0        0        0     6814 1970-01-01 00:00:00.000000 fast_poisson_solver-0.1.2/PKG-INFO
```

### Comparing `fast_poisson_solver-0.1.1/fast_poisson_solver/__init__.py` & `fast_poisson_solver-0.1.2/fast_poisson_solver/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_poisson_solver-0.1.1/fast_poisson_solver/analyze.py` & `fast_poisson_solver-0.1.2/fast_poisson_solver/analyze.py`

 * *Files identical despite different names*

### Comparing `fast_poisson_solver-0.1.1/fast_poisson_solver/data.py` & `fast_poisson_solver-0.1.2/fast_poisson_solver/data.py`

 * *Files identical despite different names*

### Comparing `fast_poisson_solver-0.1.1/fast_poisson_solver/data_utils/source_functions.py` & `fast_poisson_solver-0.1.2/fast_poisson_solver/data_utils/source_functions.py`

 * *Files identical despite different names*

### Comparing `fast_poisson_solver-0.1.1/fast_poisson_solver/diff_matrices.py` & `fast_poisson_solver-0.1.2/fast_poisson_solver/diff_matrices.py`

 * *Files identical despite different names*

### Comparing `fast_poisson_solver-0.1.1/fast_poisson_solver/model.py` & `fast_poisson_solver-0.1.2/fast_poisson_solver/model.py`

 * *Files identical despite different names*

### Comparing `fast_poisson_solver-0.1.1/fast_poisson_solver/numeric_solver.py` & `fast_poisson_solver-0.1.2/fast_poisson_solver/numeric_solver.py`

 * *Files identical despite different names*

### Comparing `fast_poisson_solver-0.1.1/fast_poisson_solver/plotter.py` & `fast_poisson_solver-0.1.2/fast_poisson_solver/plotter.py`

 * *Files identical despite different names*

### Comparing `fast_poisson_solver-0.1.1/fast_poisson_solver/solver.py` & `fast_poisson_solver-0.1.2/fast_poisson_solver/solver.py`

 * *Files identical despite different names*

### Comparing `fast_poisson_solver-0.1.1/fast_poisson_solver/utils.py` & `fast_poisson_solver-0.1.2/fast_poisson_solver/utils.py`

 * *Files identical despite different names*

### Comparing `fast_poisson_solver-0.1.1/LICENSE` & `fast_poisson_solver-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_poisson_solver-0.1.1/pyproject.toml` & `fast_poisson_solver-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast-poisson-solver"
-version = "0.1.1"
+version = "0.1.2"
 description = "A fast solver for the Poisson equation."
 authors = ["Matthias Neuwirth"]
 readme = "README.md"
 packages = [{include = "fast_poisson_solver"}]
 license = "GNUv3"
 keywords = ["Poisson", "solver", "fast", "python"]
 repository = "https://github.com/matthiasnwt/fast-poisson-solver"
```

### Comparing `fast_poisson_solver-0.1.1/README.md` & `fast_poisson_solver-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,14 @@
 This module comes with an easy-to-use method for solving arbitrary 2D Poisson problems.
 It also includes a numerical solver and an analyzing function to quantify the results.
 For visual inspection, the module offers a plotting function.
 
 In its current version this module supports only 2D Poisson problems with Dirichlet boundary conditions.
 The boundary conditions should be a constant value.
 
-## Table of Contents
-1. [Installation](#installation)
-2. [Basic Usage](#basic-usage)
-3. [Contributing](#contributing)
-4. [License](#license)
-5. [Contact](#contact)
-6. [Roadmap and Future Enhancements](#roadmap-and-future-enhancements)
-
 ## Installation
 
 This project is available on PyPI and can be installed with pip.
 
 ```bash
 pip install fast-poisson-solver
 ```
```

### Comparing `fast_poisson_solver-0.1.1/PKG-INFO` & `fast_poisson_solver-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-poisson-solver
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fast solver for the Poisson equation.
 Home-page: https://github.com/matthiasnwt/fast-poisson-solver
 License: GNUv3
 Keywords: Poisson,solver,fast,python
 Author: Matthias Neuwirth
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -63,22 +63,14 @@
 This module comes with an easy-to-use method for solving arbitrary 2D Poisson problems.
 It also includes a numerical solver and an analyzing function to quantify the results.
 For visual inspection, the module offers a plotting function.
 
 In its current version this module supports only 2D Poisson problems with Dirichlet boundary conditions.
 The boundary conditions should be a constant value.
 
-## Table of Contents
-1. [Installation](#installation)
-2. [Basic Usage](#basic-usage)
-3. [Contributing](#contributing)
-4. [License](#license)
-5. [Contact](#contact)
-6. [Roadmap and Future Enhancements](#roadmap-and-future-enhancements)
-
 ## Installation
 
 This project is available on PyPI and can be installed with pip.
 
 ```bash
 pip install fast-poisson-solver
 ```
```

