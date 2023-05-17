# Comparing `tmp/mcmc_statphys-0.1.2.tar.gz` & `tmp/mcmc_statphys-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcmc_statphys-0.1.2.tar", last modified: Mon May 15 01:43:56 2023, max compression
+gzip compressed data, was "mcmc_statphys-0.2.1.tar", last modified: Wed May 17 14:26:05 2023, max compression
```

## Comparing `mcmc_statphys-0.1.2.tar` & `mcmc_statphys-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 01:43:56.892957 mcmc_statphys-0.1.2/
--rw-rw-rw-   0        0        0      170 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3721 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      651 2023-05-15 01:23:48.000000 mcmc_statphys-0.1.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3541 2023-05-15 01:43:56.893955 mcmc_statphys-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2052 2023-05-15 01:32:18.000000 mcmc_statphys-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-15 01:43:56.744356 mcmc_statphys-0.1.2/docs/
--rw-rw-rw-   0        0        0      634 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/authors.rst
--rw-rw-rw-   0        0        0     5006 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/history.rst
--rw-rw-rw-   0        0        0      333 2023-05-15 01:23:54.000000 mcmc_statphys-0.1.2/docs/index.rst
--rw-rw-rw-   0        0        0     1209 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/installation.rst
--rwxrwxrwx   0        0        0      811 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/readme.rst
--rw-rw-rw-   0        0        0       88 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-05-15 01:43:56.761309 mcmc_statphys-0.1.2/mcmc_statphys/
--rw-rw-rw-   0        0        0      143 2023-05-14 12:02:25.000000 mcmc_statphys-0.1.2/mcmc_statphys/__init__.py
--rw-rw-rw-   0        0        0      434 2023-05-14 12:02:25.000000 mcmc_statphys-0.1.2/mcmc_statphys/cli.py
--rw-rw-rw-   0        0        0    16697 2023-05-14 15:53:48.000000 mcmc_statphys-0.1.2/mcmc_statphys/method.py
--rw-rw-rw-   0        0        0     8200 2023-05-14 15:40:25.000000 mcmc_statphys-0.1.2/mcmc_statphys/model.py
-drwxrwxrwx   0        0        0        0 2023-05-15 01:43:56.876003 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/
--rw-rw-rw-   0        0        0     3541 2023-05-15 01:43:56.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      655 2023-05-15 01:43:56.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 01:43:56.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-15 01:43:56.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-05-15 01:43:56.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-15 01:43:56.000000 mcmc_statphys-0.1.2/mcmc_statphys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      408 2023-05-15 01:43:56.901934 mcmc_statphys-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1556 2023-05-15 01:20:36.000000 mcmc_statphys-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 01:43:56.890964 mcmc_statphys-0.1.2/tests/
--rw-rw-rw-   0        0        0       44 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0      920 2023-05-14 15:52:21.000000 mcmc_statphys-0.1.2/tests/test_mcmc_statphys.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:26:05.115743 mcmc_statphys-0.2.1/
+-rw-rw-rw-   0        0        0      170 2023-05-14 13:37:58.000000 mcmc_statphys-0.2.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3721 2023-05-14 13:37:58.000000 mcmc_statphys-0.2.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1236 2023-05-17 14:25:52.000000 mcmc_statphys-0.2.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1089 2023-05-14 13:37:58.000000 mcmc_statphys-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-05-14 13:37:58.000000 mcmc_statphys-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4161 2023-05-17 14:26:05.116741 mcmc_statphys-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2087 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 14:26:04.963154 mcmc_statphys-0.2.1/docs/
+-rw-rw-rw-   0        0        0      634 2023-05-14 13:37:58.000000 mcmc_statphys-0.2.1/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.2.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     5006 2023-05-14 13:37:58.000000 mcmc_statphys-0.2.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-05-14 13:37:58.000000 mcmc_statphys-0.2.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.2.1/docs/history.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 14:26:04.970135 mcmc_statphys-0.2.1/docs/img/
+-rw-rw-rw-   0        0        0    12977 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png
+-rw-rw-rw-   0        0        0      333 2023-05-16 16:00:10.000000 mcmc_statphys-0.2.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1209 2023-05-14 13:37:58.000000 mcmc_statphys-0.2.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      811 2023-05-14 13:37:58.000000 mcmc_statphys-0.2.1/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-05-14 13:37:58.000000 mcmc_statphys-0.2.1/docs/readme.rst
+-rw-rw-rw-   0        0        0    17063 2023-05-17 14:25:54.000000 mcmc_statphys-0.2.1/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 14:26:05.003046 mcmc_statphys-0.2.1/mcmc_statphys/
+-rw-rw-rw-   0        0        0      247 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/mcmc_statphys/__init__.py
+-rw-rw-rw-   0        0        0    32646 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/mcmc_statphys/algorithm.py
+-rw-rw-rw-   0        0        0     1406 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/mcmc_statphys/analysis.py
+-rw-rw-rw-   0        0        0      434 2023-05-14 12:02:25.000000 mcmc_statphys-0.2.1/mcmc_statphys/cli.py
+-rw-rw-rw-   0        0        0     2900 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/mcmc_statphys/draw.py
+-rw-rw-rw-   0        0        0     8023 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/mcmc_statphys/model.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:26:05.061888 mcmc_statphys-0.2.1/mcmc_statphys.egg-info/
+-rw-rw-rw-   0        0        0     4161 2023-05-17 14:26:04.000000 mcmc_statphys-0.2.1/mcmc_statphys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      903 2023-05-17 14:26:04.000000 mcmc_statphys-0.2.1/mcmc_statphys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 14:26:04.000000 mcmc_statphys-0.2.1/mcmc_statphys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-17 14:26:04.000000 mcmc_statphys-0.2.1/mcmc_statphys.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-14 13:46:13.000000 mcmc_statphys-0.2.1/mcmc_statphys.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-05-17 14:26:04.000000 mcmc_statphys-0.2.1/mcmc_statphys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-17 14:26:04.000000 mcmc_statphys-0.2.1/mcmc_statphys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      408 2023-05-17 14:26:05.119732 mcmc_statphys-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1556 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:26:05.090810 mcmc_statphys-0.2.1/tests/
+-rw-rw-rw-   0        0        0       44 2023-05-14 13:37:58.000000 mcmc_statphys-0.2.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:26:05.108761 mcmc_statphys-0.2.1/tests/test/
+-rw-rw-rw-   0        0        0      229 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/tests/test/__init__.py
+-rw-rw-rw-   0        0        0    32668 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/tests/test/algorithm.py
+-rw-rw-rw-   0        0        0     1406 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/tests/test/analysis.py
+-rw-rw-rw-   0        0        0      434 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/tests/test/cli.py
+-rw-rw-rw-   0        0        0     2900 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/tests/test/draw.py
+-rw-rw-rw-   0        0        0     8383 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/tests/test/model.py
+-rw-rw-rw-   0        0        0    15793 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/tests/test.ipynb
+-rw-rw-rw-   0        0        0     1046 2023-05-17 14:16:19.000000 mcmc_statphys-0.2.1/tests/test_mcmc_statphys.py
```

### Comparing `mcmc_statphys-0.1.2/CONTRIBUTING.rst` & `mcmc_statphys-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.2/LICENSE` & `mcmc_statphys-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.2/PKG-INFO` & `mcmc_statphys-0.2.1/mcmc_statphys.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mcmc_statphys
-Version: 0.1.2
+Name: mcmc-statphys
+Version: 0.2.1
 Summary: A library project of Monte Carlo simulation algorithms for some statistical physics models (in particular, the Ising model and its variants).
 Home-page: https://github.com/uynajgi/mcmc_statphys
 Author: Uynaj GI
 Author-email: suquan12148@outlook.com
 License: MIT license
 Keywords: mcmc_statphys
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -48,30 +48,33 @@
 --------
 
 A simple Ising model simulation.
 
 .. code-block:: python
 
     >>> import mcmc_statphys as mcsp
-    >>> import matplotlib.pyplot as plt # We have not yet produced a built-in plotting module. Stay tuned.
-    >>> model = mcsp.model.Ising(16)
-    >>> simulator = mcsp.method.Simulation(model)
-    >>> energy, magnetization, _ = simulator.metropolis_sample(T=1, max_iter=10000)
-    >>> plt.plot(energy)
+    >>> model = mcsp.model.Ising(12) # 12x12 Ising model
+    >>> algorithm = mcsp.method.Metropolis(model) # Metropolis algorithm
+    >>> uid = algorithm.equil_sample(T=1, max_iter=1000) # sample until equilibrium
+    >>> fig = mcsp.draw.Plot(algorithm) 
+    >>> fig.curve(uid=uid, comlumn='energy') # plot the energy curve
 
-Install the latest version of mcmc_statphys: 
+Install
+-------
+
+the latest version of mcmc_statphys: 
 
 .. code-block:: console
 
     $ pip install mcmc_statphys
 
 Bugs
 ----
 
-Please report any bugs that you find `here`_. Or, even better, fork the repository on `GitHub` and create a pull request (PR). We welcome all changes, big or small, and we will help you make the PR if you are new to git (just ask on the issue and/or see `CONTRIBUTING`).
+Please report any bugs that you find `here`_. Or, even better, fork the repository on `GitHub`_ and create a pull request (PR). We welcome all changes, big or small, and we will help you make the PR if you are new to git (just ask on the issue and/or see `CONTRIBUTING`_).
 
 .. _here: https://github.com/uynajgi/mcmc_statphys/issues
 .. _GitHub: https://github.com/uynajgi/mcmc_statphys/
 .. _CONTRIBUTING: https://mcmc-statphys.readthedocs.io/en/latest/contributing.html
 
 Credits
 -------
@@ -90,27 +93,54 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 [Unreleased]
 ------------
 
+[0.2.1] - 2023-05-17
+---------------------
+
+Fixed
+~~~~~
+
+* Fix the bug of saving `_get_per_magnetization` in `_save_data` in `algorithm`
+
+Added
+~~~~~
+
+* Add moudle `analysis` to analyze the data
+* Add moudle `draw` to draw the figures
+* Add method `setspin` in `model`
+* Add tqmd to show the progress bar
+
+Doc
+~~~
+
+* Add documentation to README
+* Add documentation to Usages
+
+Changed
+~~~~~~~
+
+* Change the methods in the `analysis` module: removed the `Sample` and `ParameterSample` classes, added `Metropolis`, `Wolff`, `Anneal` classes and several methods
+
 [0.1.2] - 2023-05-15
 --------------------
 
 Security
->>>>>>>>>
+~~~~~~~~
 
 * Add function annotations to all functions
 * Add type hints to all functions
 * Add type hints to all variables
 * Change `mcmc_statphys.py` to `method.py`
 
 Doc
->>>
+~~~
 
 * Add documentation to README
 
 [0.1.1] - 2023-05-14
 --------------------
 
 * First release on PyPI.
```

### Comparing `mcmc_statphys-0.1.2/README.rst` & `mcmc_statphys-0.2.1/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -27,30 +27,33 @@
 --------
 
 A simple Ising model simulation.
 
 .. code-block:: python
 
     >>> import mcmc_statphys as mcsp
-    >>> import matplotlib.pyplot as plt # We have not yet produced a built-in plotting module. Stay tuned.
-    >>> model = mcsp.model.Ising(16)
-    >>> simulator = mcsp.method.Simulation(model)
-    >>> energy, magnetization, _ = simulator.metropolis_sample(T=1, max_iter=10000)
-    >>> plt.plot(energy)
+    >>> model = mcsp.model.Ising(12) # 12x12 Ising model
+    >>> algorithm = mcsp.method.Metropolis(model) # Metropolis algorithm
+    >>> uid = algorithm.equil_sample(T=1, max_iter=1000) # sample until equilibrium
+    >>> fig = mcsp.draw.Plot(algorithm) 
+    >>> fig.curve(uid=uid, comlumn='energy') # plot the energy curve
 
-Install the latest version of mcmc_statphys: 
+Install
+-------
+
+the latest version of mcmc_statphys: 
 
 .. code-block:: console
 
     $ pip install mcmc_statphys
 
 Bugs
 ----
 
-Please report any bugs that you find `here`_. Or, even better, fork the repository on `GitHub` and create a pull request (PR). We welcome all changes, big or small, and we will help you make the PR if you are new to git (just ask on the issue and/or see `CONTRIBUTING`).
+Please report any bugs that you find `here`_. Or, even better, fork the repository on `GitHub`_ and create a pull request (PR). We welcome all changes, big or small, and we will help you make the PR if you are new to git (just ask on the issue and/or see `CONTRIBUTING`_).
 
 .. _here: https://github.com/uynajgi/mcmc_statphys/issues
 .. _GitHub: https://github.com/uynajgi/mcmc_statphys/
 .. _CONTRIBUTING: https://mcmc-statphys.readthedocs.io/en/latest/contributing.html
 
 Credits
 -------
```

### Comparing `mcmc_statphys-0.1.2/docs/Makefile` & `mcmc_statphys-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.2/docs/conf.py` & `mcmc_statphys-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.2/docs/installation.rst` & `mcmc_statphys-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.2/docs/make.bat` & `mcmc_statphys-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.2/mcmc_statphys/model.py` & `mcmc_statphys-0.2.1/tests/test/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,20 @@
         '''Get the delta energy of the site'''
         old_site_energy = self._get_site_energy(index)
         self._change_site_spin(index)
         new_site_energy = self._get_site_energy(index)
         detle_energy = new_site_energy - old_site_energy
         return detle_energy
 
+    def set_spin(self, spin):
+        # TODO[0.3.0]: 增加 spin 格式审查
+        self.spin = spin
+        self._get_total_energy()
+        self._get_total_magnetization()
+
 
 class Heisenberg(Ising):
 
     def __init__(self, L, Jij=1, H=0, *args, **kwargs):
         super().__init__(L, Jij, H, dimension=3, *args, **kwargs)
         self._init_spin(type='heisenberg')
```

### Comparing `mcmc_statphys-0.1.2/mcmc_statphys.egg-info/PKG-INFO` & `mcmc_statphys-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mcmc-statphys
-Version: 0.1.2
+Name: mcmc_statphys
+Version: 0.2.1
 Summary: A library project of Monte Carlo simulation algorithms for some statistical physics models (in particular, the Ising model and its variants).
 Home-page: https://github.com/uynajgi/mcmc_statphys
 Author: Uynaj GI
 Author-email: suquan12148@outlook.com
 License: MIT license
 Keywords: mcmc_statphys
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -48,30 +48,33 @@
 --------
 
 A simple Ising model simulation.
 
 .. code-block:: python
 
     >>> import mcmc_statphys as mcsp
-    >>> import matplotlib.pyplot as plt # We have not yet produced a built-in plotting module. Stay tuned.
-    >>> model = mcsp.model.Ising(16)
-    >>> simulator = mcsp.method.Simulation(model)
-    >>> energy, magnetization, _ = simulator.metropolis_sample(T=1, max_iter=10000)
-    >>> plt.plot(energy)
+    >>> model = mcsp.model.Ising(12) # 12x12 Ising model
+    >>> algorithm = mcsp.method.Metropolis(model) # Metropolis algorithm
+    >>> uid = algorithm.equil_sample(T=1, max_iter=1000) # sample until equilibrium
+    >>> fig = mcsp.draw.Plot(algorithm) 
+    >>> fig.curve(uid=uid, comlumn='energy') # plot the energy curve
 
-Install the latest version of mcmc_statphys: 
+Install
+-------
+
+the latest version of mcmc_statphys: 
 
 .. code-block:: console
 
     $ pip install mcmc_statphys
 
 Bugs
 ----
 
-Please report any bugs that you find `here`_. Or, even better, fork the repository on `GitHub` and create a pull request (PR). We welcome all changes, big or small, and we will help you make the PR if you are new to git (just ask on the issue and/or see `CONTRIBUTING`).
+Please report any bugs that you find `here`_. Or, even better, fork the repository on `GitHub`_ and create a pull request (PR). We welcome all changes, big or small, and we will help you make the PR if you are new to git (just ask on the issue and/or see `CONTRIBUTING`_).
 
 .. _here: https://github.com/uynajgi/mcmc_statphys/issues
 .. _GitHub: https://github.com/uynajgi/mcmc_statphys/
 .. _CONTRIBUTING: https://mcmc-statphys.readthedocs.io/en/latest/contributing.html
 
 Credits
 -------
@@ -90,27 +93,54 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 [Unreleased]
 ------------
 
+[0.2.1] - 2023-05-17
+---------------------
+
+Fixed
+~~~~~
+
+* Fix the bug of saving `_get_per_magnetization` in `_save_data` in `algorithm`
+
+Added
+~~~~~
+
+* Add moudle `analysis` to analyze the data
+* Add moudle `draw` to draw the figures
+* Add method `setspin` in `model`
+* Add tqmd to show the progress bar
+
+Doc
+~~~
+
+* Add documentation to README
+* Add documentation to Usages
+
+Changed
+~~~~~~~
+
+* Change the methods in the `analysis` module: removed the `Sample` and `ParameterSample` classes, added `Metropolis`, `Wolff`, `Anneal` classes and several methods
+
 [0.1.2] - 2023-05-15
 --------------------
 
 Security
->>>>>>>>>
+~~~~~~~~
 
 * Add function annotations to all functions
 * Add type hints to all functions
 * Add type hints to all variables
 * Change `mcmc_statphys.py` to `method.py`
 
 Doc
->>>
+~~~
 
 * Add documentation to README
 
 [0.1.1] - 2023-05-14
 --------------------
 
 * First release on PyPI.
```

### Comparing `mcmc_statphys-0.1.2/setup.py` & `mcmc_statphys-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='mcmc_statphys',
     name='mcmc_statphys',
     packages=find_packages(include=['mcmc_statphys', 'mcmc_statphys.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/uynajgi/mcmc_statphys',
-    version='0.1.2',
+    version='0.2.1',
     zip_safe=False,
 )
```

