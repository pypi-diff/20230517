# Comparing `tmp/pyqmc-0.5.1.tar.gz` & `tmp/pyqmc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqmc-0.5.1.tar", last modified: Sat Dec  3 15:40:45 2022, max compression
+gzip compressed data, was "pyqmc-0.6.0.tar", last modified: Wed May 17 14:16:55 2023, max compression
```

## Comparing `pyqmc-0.5.1.tar` & `pyqmc-0.6.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 15:40:45.306050 pyqmc-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2022-12-03 15:40:32.000000 pyqmc-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2022-12-03 15:40:45.306050 pyqmc-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2022-12-03 15:40:32.000000 pyqmc-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 15:40:45.306050 pyqmc-0.5.1/pyqmc/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/accumulators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/addwf.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/coord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/determinant_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    19130 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/dmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10461 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/eval_ecp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17758 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/ewald.py
--rw-r--r--   0 runner    (1001) docker     (123)    18675 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/func3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/hdftools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/j3.py
--rw-r--r--   0 runner    (1001) docker     (123)    23157 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/jastrowspin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/linemin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/mc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/multiplywf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/obdm.py
--rw-r--r--   0 runner    (1001) docker     (123)    22591 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/optimize_excited_states.py
--rw-r--r--   0 runner    (1001) docker     (123)    26531 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/optimize_ortho.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/optvariance.py
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/orbitals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/pbc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/pbc_eval_gto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/pyscftools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/reblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16632 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/slater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/supercell.py
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/tbdm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11110 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/testwf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/twists.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2022-12-03 15:40:32.000000 pyqmc-0.5.1/pyqmc/wftools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 15:40:45.306050 pyqmc-0.5.1/pyqmc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2022-12-03 15:40:45.000000 pyqmc-0.5.1/pyqmc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      786 2022-12-03 15:40:45.000000 pyqmc-0.5.1/pyqmc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 15:40:45.000000 pyqmc-0.5.1/pyqmc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-03 15:40:45.000000 pyqmc-0.5.1/pyqmc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-03 15:40:45.000000 pyqmc-0.5.1/pyqmc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-03 15:40:45.306050 pyqmc-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2022-12-03 15:40:32.000000 pyqmc-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:16:55.397704 pyqmc-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 14:16:43.000000 pyqmc-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-17 14:16:55.397704 pyqmc-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-17 14:16:43.000000 pyqmc-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:16:55.397704 pyqmc-0.6.0/pyqmc/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/accumulators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/addwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/determinant_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19392 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/dmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/eval_ecp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/ewald.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/func3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/geminaljastrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/hdftools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23163 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/jastrowspin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/linemin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/mc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/multiplywf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/obdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23007 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/optimize_excited_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27711 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/optimize_ortho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/optvariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14343 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/orbitals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/pbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/pyscftools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/reblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/slater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/supercell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/tbdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/testwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22293 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/three_body_jastrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/twists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-05-17 14:16:43.000000 pyqmc-0.6.0/pyqmc/wftools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:16:55.397704 pyqmc-0.6.0/pyqmc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-17 14:16:55.000000 pyqmc-0.6.0/pyqmc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-17 14:16:55.000000 pyqmc-0.6.0/pyqmc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:16:55.000000 pyqmc-0.6.0/pyqmc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 14:16:55.000000 pyqmc-0.6.0/pyqmc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 14:16:55.000000 pyqmc-0.6.0/pyqmc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:16:55.397704 pyqmc-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-17 14:16:43.000000 pyqmc-0.6.0/setup.py
```

### Comparing `pyqmc-0.5.1/LICENSE` & `pyqmc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqmc-0.5.1/PKG-INFO` & `pyqmc-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqmc
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python library for real space quantum Monte Carlo
 Home-page: https://github.com/WagnerGroup/pyqmc
 Maintainer: Lucas Wagner
 Maintainer-email: lkwagner@illinois.edu
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyqmc-0.5.1/README.md` & `pyqmc-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqmc-0.5.1/pyqmc/accumulators.py` & `pyqmc-0.6.0/pyqmc/accumulators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pyqmc.gpu as gpu
 import pyqmc.energy as energy
 import pyqmc.ewald as ewald
 import pyqmc.eval_ecp as eval_ecp
+import copy
 
 
 def gradient_generator(mol, wf, to_opt=None, nodal_cutoff=1e-3, **ewald_kwargs):
     return PGradTransform(
         EnergyAccumulator(mol, **ewald_kwargs),
         LinearTransform(wf.parameters, to_opt),
         nodal_cutoff=nodal_cutoff,
@@ -58,19 +59,18 @@
     """
     Linearize a dictionary of wf parameters.
 
     :parameter dict parameters: the wave function parameters
     :parameter dict to_opt: is a dictionary with the keys to optimize, and its values are boolean arrays indicating which specific elements to optimize
 
     Note:
-        to_opt[k] can't be boolean scalar; it has to be an array with the same dimension as parameters[k].
 
-        to_opt doesn't have to have all the keys of parameters, but all keys of to_opt must be keys of parameters.
-
-        If you change wf.parameters, then all serializations will be out of date. For example, if you serialize, then change wf.paramaters, then deserialize, the deserialization will be incorrect.
+    * to_opt[k] can't be boolean scalar; it has to be an array with the same dimension as parameters[k].
+    * to_opt doesn't have to have all the keys of parameters, but all keys of to_opt must be keys of parameters.
+    * If you change wf.parameters, then all serializations will be out of date. For example, if you serialize, then change wf.paramaters, then deserialize, the deserialization will be incorrect.
     """
 
     def __init__(self, parameters, to_opt=None):
         parameters = {k: gpu.asnumpy(v) for k, v in parameters.items()}
         if to_opt is None:
             to_opt = {k: np.ones(p.shape, dtype=bool) for k, p in parameters.items()}
         self.to_opt = {k: o for k, o in to_opt.items() if np.any(o)}
@@ -215,43 +215,95 @@
 
 
 class SqAccumulator:
     r"""
     Accumulates structure factor
 
     .. math:: S(\vec{q}) = \langle \rho_{\vec{q}} \rho_{-\vec{q}} \rangle
-                         = \langle \left| \sum_{j=1}^{N_e} e^{i\vec{q}\cdot\vec{r}_j} \right| \rangle
+                         = \langle \left| \sum_{j=1}^{N_e} e^{i\vec{q}\cdot\vec{r}_j} \right|^2 \rangle
+    .. math:: S_{\rm spin}(\vec{q}) = \langle \left| \sum_{j=1}^{N_e} s_j e^{i\vec{q}\cdot\vec{r}_j} \right|^2 \rangle
 
     """
 
-    def __init__(self, qlist=None, Lvecs=None, nq=4):
+    def __init__(self, cell, nq=4, qlist=None):
         """
         Inputs:
-            qlist: (n, 3) array-like. If qlist is provided, Lvecs and nq are ignored
-            Lvecs: (3, 3) array-like of lattice vectors. Required if qlist is None
-            nq: int, if qlist is nonzero, use a uniform grid of shape (nq, nq, nq)
+            cell: pyscf Cell object
+            nq: int. If qlist is nonzero, use a uniform grid of shape (nq, nq, nq)
+            qlist: (n, 3) array-like. If qlist is provided, nq is ignored
         """
         if qlist is not None:
             self.qlist = qlist
         else:
-            assert (
-                Lvecs is not None
-            ), "need to provide either list of q vectors or lattice vectors"
-            Gvecs = np.linalg.inv(Lvecs).T * 2 * np.pi
-            qvecs = list(map(np.ravel, np.meshgrid(*[np.arange(nq)] * 3)))
-            qvecs = np.stack(qvecs, axis=1)
-            self.qlist = np.dot(qvecs, Gvecs)
+            recvec = np.linalg.inv(cell.lattice_vectors()).T
+            self.qlist = ewald.generate_positive_gpoints(nq, recvec)
+        nup = cell.nelec[0]
+        self.nelec = sum(cell.nelec)
+        self.spins = np.ones((2, self.nelec))
+        self.spins[1, nup:] = -1
 
     def __call__(self, configs, wf):
-        nelec = configs.configs.shape[1]
         exp_iqr = np.exp(1j * np.inner(configs.configs, self.qlist))
-        sum_exp_iqr = exp_iqr.sum(axis=1)
-        return {"Sq": (sum_exp_iqr.real**2 + sum_exp_iqr.imag**2) / nelec}
+        sum_exp_iqr = np.einsum("ijk,sj->sik", exp_iqr, self.spins)
+        Sq = (sum_exp_iqr.real**2 + sum_exp_iqr.imag**2) / self.nelec
+        return {"Sq": Sq[0], "spinSq": Sq[1]}
+
+    def avg(self, configs, wf):
+        exp_iqr = np.exp(1j * np.inner(configs.configs, self.qlist))
+        sum_exp_iqr = np.einsum("ijk,sj->sik", exp_iqr, self.spins)
+        Sq = (sum_exp_iqr.real**2 + sum_exp_iqr.imag**2).mean(axis=1) / self.nelec
+        return {"Sq": Sq[0], "spinSq": Sq[1]}
+
+    def keys(self):
+        return set(["Sq", "spinSq"])
+
+    def shapes(self):
+        return {"Sq": (len(self.qlist),), "spinSq": (len(self.qlist),)}
+
+
+class SymmetryAccumulator:
+    """
+    Evaluates S * Psi(R) / Psi(R) for each many-body symmetry operator S given in a dictionary
+    Makes use of the equivariance property S * Psi(R) = Psi(S * R) by transforming all electron coordinates R and recomputing the wf
+    When defining a SymmetryAccumulator object, pass in a dictionary of symmetry operator names and their respective 3x3 unitary matrices
+    For example, to evaluate a rotation of angle theta about the z-axis and mirror reflection about the yz plane, use the code
+
+    rotation_z = np.array(
+        [
+            [np.cos(theta), -np.sin(theta), 0],
+            [np.sin(theta), np.cos(theta), 0],
+            [0, 0, 1],
+        ]
+    )
+    reflection_yz = np.array([[-1, 0, 0], [0, 1, 0], [0, 0, 1]])
+    symmetry_operators = {"rotation_z": rotation_z, "reflection_yz": reflection_yz}
+    acc = {"symmetry": SymmetryAccumulator(symmetry_operators=symmetry_operators)}
+    """
+
+    def __init__(self, symmetry_operators):
+        """
+        Inputs:
+            symmetry_operators: dictionary of symmetry operator names and their respective unitary transformation matrices of shape (3,3)
+        """
+        self.symmetry_operators = symmetry_operators
+
+    def __call__(self, configs, wf):
+        symmetry_observables = {}
+        original_wf_value = wf.value()
+        configs_copy = copy.deepcopy(configs)
+        for S_name, S_matrix in self.symmetry_operators.items():
+            configs_copy.configs = np.einsum("ijk,kl->ijl", configs.configs, S_matrix)
+            transformed_wf_value = wf.recompute(configs_copy)
+            symmetry_observables[S_name] = (
+                transformed_wf_value[0] / original_wf_value[0]
+            ) * np.exp(transformed_wf_value[1] - original_wf_value[1])
+        wf.recompute(configs)
+        return symmetry_observables
 
     def avg(self, configs, wf):
         return {k: np.mean(it, axis=0) for k, it in self(configs, wf).items()}
 
     def keys(self):
-        return set(["Sq"])
+        return self.shapes().keys()
 
     def shapes(self):
-        return {"Sq": (len(self.qlist),)}
+        return {S: () for S in self.symmetry_operators.keys()}
```

### Comparing `pyqmc-0.5.1/pyqmc/addwf.py` & `pyqmc-0.6.0/pyqmc/addwf.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     def __init__(self, coeffs, wf_components):
         """
         The wave function is sum coeffs[i] wf_components[i].
         """
         self.coeffs = coeffs
         self.wf_components = wf_components
         self.parameters = Parameters([wf.parameters for wf in wf_components])
-        self.iscomplex = bool(
-            sum(wf.iscomplex for wf in wf_components)
+        iscomplex = bool(
+            sum(wf.dtype == complex for wf in wf_components)
             + sum([isinstance(c, complex) * 1 for c in coeffs])
         )
-        self.dtype = complex if self.iscomplex else float
+        self.dtype = complex if iscomplex else float
 
     def recompute(self, configs):
         """
         Recompute the quantity :math:`ln(|\psi(R)|)` and the phase/sign of the wave function.
         """
         wf_vals = np.array([wf.recompute(configs) for wf in self.wf_components])
         ref = np.amax(wf_vals[:, 1, :]).real
```

### Comparing `pyqmc-0.5.1/pyqmc/api.py` & `pyqmc-0.6.0/pyqmc/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,7 +9,8 @@
 from pyqmc.reblock import reblock as avg_reblock
 from pyqmc.wftools import generate_wf, read_wf, generate_jastrow, generate_slater
 from pyqmc.pyscftools import recover_pyscf
 from pyqmc.slater import Slater
 from pyqmc.jastrowspin import JastrowSpin
 from pyqmc.multiplywf import MultiplyWF
 from pyqmc.addwf import AddWF
+from pyqmc.twists import create_supercell_twists
```

### Comparing `pyqmc-0.5.1/pyqmc/coord.py` & `pyqmc-0.6.0/pyqmc/coord.py`

 * *Files identical despite different names*

### Comparing `pyqmc-0.5.1/pyqmc/determinant_tools.py` & `pyqmc-0.6.0/pyqmc/determinant_tools.py`

 * *Files identical despite different names*

### Comparing `pyqmc-0.5.1/pyqmc/distance.py` & `pyqmc-0.6.0/pyqmc/distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         n2 = config2.shape[1]
         if n1 == 0 or n2 == 0:
             return np.zeros((config1.shape[0], 0, 3)), []
         vs = []
         ij = []
         for i in range(n2):
             vs.append(self.dist_i(config1, config2[:, i, :]))
-            ij.extend([(i, j) for j in range(n1)])
+            ij.extend([(j, i) for j in range(n1)])
         vs = np.concatenate(vs, axis=1)
 
         return vs, ij
 
 
 class MinimalImageDistance(RawDistance):
     """Compute distance vectors under a minimal image condition
```

### Comparing `pyqmc-0.5.1/pyqmc/dmc.py` & `pyqmc-0.6.0/pyqmc/dmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     new_grad = limdrift(np.real(g.T), tstep)
     forward = np.sum(gauss**2, axis=1)
     backward = np.sum((gauss + grad + new_grad) ** 2, axis=1)
     t_prob = np.exp(1 / (2 * tstep) * (forward - backward))
 
     # Acceptance -- fixed-node: reject if wf changes sign
     ratio = np.abs(wfratio) ** 2 * t_prob
-    if not wf.iscomplex:
+    if wf.dtype == float:
         ratio *= np.sign(wfratio)
     accept = ratio > np.random.rand(nconfig)
     r2 = np.sum((gauss + grad) ** 2, axis=1)
 
     return newepos, accept, r2, saved
 
 
@@ -205,14 +205,19 @@
 
     df_ret["weight"] = np.mean(weight)
 
     return df_ret, configs, weights
 
 
 def compute_S(e_trial, e_est, branchcut, v2, tau, eloc, nelec):
+    r"""
+    .. math:: S = E_T - E_{\rm est} + \frac{f_{\rm sat}(E_{\rm est} - E_L; c_{\rm branch})}{1 + \frac{v^2\tau}{n_{\rm elec}}}
+
+    :math:`f_{\rm sat}(x; c)` is the saturation function: :math:`x` if :math:`|x| < c` and :math:`c{\rm sign}(x)` otherwise.
+    """
     e_cut = e_est - eloc
     mask = np.abs(e_cut) > branchcut
     e_cut[mask] = branchcut * np.sign(e_cut[mask])
     denominator = 1 + (v2 * tau / nelec) ** 2
 
     return e_trial - e_est + e_cut / denominator
 
@@ -483,15 +488,15 @@
         df_["weight_std"] = np.std(weights)
         df_["nsteps"] = branchtime
 
         configs, weights, branch_info = branch(configs, weights)
         df_.update(branch_info)
         df.append(df_)
         dmc_file(hdf_file, df_, {}, configs, weights)
-        
+
         e_est = estimate_energy(hdf_file, df, ekey)
         e_trial = e_est - feedback * np.log(np.mean(weights)).real
 
         if verbose:
             print(
                 "energy",
                 df_[ekey[0] + ekey[1]],
```

### Comparing `pyqmc-0.5.1/pyqmc/energy.py` & `pyqmc-0.6.0/pyqmc/energy.py`

 * *Files identical despite different names*

### Comparing `pyqmc-0.5.1/pyqmc/eval_ecp.py` & `pyqmc-0.6.0/pyqmc/eval_ecp.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 
 
 def ecp(mol, configs, wf, threshold, naip=None):
     """
     :returns: ECP value, summed over all the electrons and atoms.
     """
     nconf, nelec = configs.configs.shape[0:2]
-    ecp_tot = np.zeros(nconf, dtype=complex if wf.iscomplex else float)
+    ecp_tot = np.zeros(nconf, dtype=wf.dtype)
     if mol._ecp != {}:
         for atom in mol._atom:
             if atom[0] in mol._ecp.keys():
                 for e in range(nelec):
                     ecp_tot += ecp_ea(mol, configs, wf, e, atom, threshold, naip)[
                         "total"
                     ]
     return ecp_tot
 
 
 def compute_tmoves(mol, configs, wf, e, threshold, tau, naip=None):
     """
     For a given electron, evaluate all possible t-moves.
 
-    returns a dictionary: 
+    returns a dictionary:
        ratio: psi(R')/psi(R) for each move
        weight: The symmetric part of Eqn 31 in Anderson and Umrigar (i.e., ratio * weight gives the amplitude for the t-move)
        configs: positions of the move
     """
     nconfig = configs.configs.shape[0]
     if mol._ecp != {}:
         data = [
@@ -61,15 +61,15 @@
 
 def ecp_ea(mol, configs, wf, e, atom, threshold, naip=None):
     """
     :returns: the ECP value between electron e and atom at, local+nonlocal.
     TODO: update documentation
     """
     nconf = configs.configs.shape[0]
-    ecp_val = np.zeros(nconf, dtype=complex if wf.iscomplex else float)
+    ecp_val = np.zeros(nconf, dtype=wf.dtype)
 
     at_name, apos = atom
     apos = np.asarray(apos)
 
     r_ea_vec = configs.dist.dist_i(apos, configs.configs[:, e, :]).reshape((-1, 3))
     r_ea = np.linalg.norm(r_ea_vec, axis=-1)
 
@@ -232,17 +232,18 @@
     :rtype:  ((naip,) array, (nconf, naip, 3) array)
     """
 
     if nconf > 0:  # get around a bug(?) when there are zero configurations.
         rot = scipy.spatial.transform.Rotation.random(nconf).as_matrix()
     else:
         rot = np.zeros((0, 3, 3))
+    quadrature_grid = generate_quadrature_grids()
 
     if naip not in quadrature_grid.keys():
-        raise ValueError("Do not support naip!= 6 or 12")
+        raise ValueError(f"Possible AIPs are one of {quadrature_grid.keys()}")
     points, weights = quadrature_grid[naip]
     rot_vec = np.einsum("jkl,ik->jil", rot, points)
     return weights, rot_vec
 
 
 def generate_quadrature_grids():
     """
@@ -300,8 +301,7 @@
     qgrid[50] = (OABCD, repeat("O", 4 / 315, 64 / 2835, 27 / 1280, 14641 / 725760))
     qgrid[12] = (IAB, repeat("I", 1 / 12, 1 / 12))
     qgrid[32] = (IABC, repeat("I", 5 / 168, 5 / 168, 27 / 840))
 
     return qgrid
 
 
-quadrature_grid = generate_quadrature_grids()
```

### Comparing `pyqmc-0.5.1/pyqmc/ewald.py` & `pyqmc-0.6.0/pyqmc/ewald.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,36 +117,16 @@
         recvec = np.linalg.inv(self.latvec).T
 
         # Determine alpha
         smallestheight = np.amin(1 / np.linalg.norm(recvec, axis=1))
         self.alpha = 5.0 / smallestheight
 
         # Determine G points to include in reciprocal Ewald sum
-        gptsXpos = gpu.cp.meshgrid(
-            gpu.cp.arange(1, ewald_gmax + 1),
-            *[gpu.cp.arange(-ewald_gmax, ewald_gmax + 1)] * 2,
-            indexing="ij"
-        )
-        zero = gpu.cp.asarray([0])
-        gptsX0Ypos = gpu.cp.meshgrid(
-            zero,
-            gpu.cp.arange(1, ewald_gmax + 1),
-            gpu.cp.arange(-ewald_gmax, ewald_gmax + 1),
-            indexing="ij",
-        )
-        gptsX0Y0Zpos = gpu.cp.meshgrid(
-            zero, zero, gpu.cp.arange(1, ewald_gmax + 1), indexing="ij"
-        )
-        gs = zip(
-            *[
-                select_big(x, cellvolume, recvec, self.alpha)
-                for x in (gptsXpos, gptsX0Ypos, gptsX0Y0Zpos)
-            ]
-        )
-        self.gpoints, self.gweight = [gpu.cp.concatenate(x, axis=0) for x in gs]
+        gpoints = generate_positive_gpoints(ewald_gmax, recvec)
+        self.gpoints, self.gweight = select_big(gpoints, cellvolume, self.alpha)
         self.set_ewald_constants(cellvolume)
 
     def set_ewald_constants(self, cellvolume):
         r"""
         Compute Ewald constants (independent of particle positions): self energy and charged-system energy. Here we compute the combined terms. These terms are independent of the convergence parameters `gmax` and `nlatvec`, but do depend on the partitioning parameter :math:`\alpha`.
 
         We define two constants, `squareconst`, the coefficient of the squared charges,
@@ -289,15 +269,15 @@
 
         # Real space electron-electron part
         ee_real_separated = gpu.cp.zeros((nconf, nelec))
         if nelec > 1:
             ee_distances, ee_inds = configs.dist.dist_matrix(configs.configs)
             ee_cij = self._real_cij(ee_distances)
 
-            for ((i, j), val) in zip(ee_inds, ee_cij.T):
+            for (i, j), val in zip(ee_inds, ee_cij.T):
                 ee_real_separated[:, i] += val
                 ee_real_separated[:, j] += val
             ee_real_separated /= 2
 
         ee_recip, ei_recip = self.reciprocal_space_electron(configs.configs)
         ee = ee_real_separated.sum(axis=1) + ee_recip
         ei = ei_real_separated.sum(axis=1) + ei_recip
@@ -376,16 +356,24 @@
         :rtype: (nelec,) array
         """
         raise NotImplementedError("ewalde_separated is currently not computed anywhere")
         nelec = configs.configs.shape[1]
         return self.e_single(nelec) + self.ewalde_separated
 
 
-def select_big(gpts, cellvolume, recvec, alpha):
-    gpoints = gpu.cp.einsum(
-        "j...,jk->...k", gpu.cp.asarray(gpts), gpu.cp.asarray(recvec) * 2 * np.pi
-    )
-    gsquared = gpu.cp.einsum("...k,...k->...", gpoints, gpoints)
+def select_big(gpoints, cellvolume, alpha):
+    gsquared = gpu.cp.einsum("jk,jk->j", gpoints, gpoints)
     gweight = 4 * np.pi * gpu.cp.exp(-gsquared / (4 * alpha**2))
     gweight /= cellvolume * gsquared
     bigweight = gweight > 1e-10
     return gpoints[bigweight], gweight[bigweight]
+
+
+def generate_positive_gpoints(gmax, recvec):
+    gXpos = gpu.cp.mgrid[1 : gmax + 1, -gmax : gmax + 1, -gmax : gmax + 1].reshape(
+        3, -1
+    )
+    gX0Ypos = gpu.cp.mgrid[0:1, 1 : gmax + 1, -gmax : gmax + 1].reshape(3, -1)
+    gX0Y0Zpos = gpu.cp.mgrid[0:1, 0:1, 1 : gmax + 1].reshape(3, -1)
+    gpts = gpu.cp.concatenate([gXpos, gX0Ypos, gX0Y0Zpos], axis=1)
+    gpoints = gpu.cp.einsum("ji,jk->ik", gpts, gpu.cp.asarray(recvec) * 2 * np.pi)
+    return gpoints
```

### Comparing `pyqmc-0.5.1/pyqmc/hdftools.py` & `pyqmc-0.6.0/pyqmc/hdftools.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,17 +24,15 @@
     for k, it in data.items():
         if k not in data.keys():
             f.create_dataset(
                 k, (0, *it.shape), maxshape=(None, *it.shape), dtype=it.dtype
             )
         currshape = f[k].shape
         f[k].resize((currshape[0] + 1, *currshape[1:]))
-        f[k][
-            -1,
-        ] = it
+        f[k][-1,] = it
 
 
 if __name__ == "__main__":
     f = h5py.File("testfile.hdf5", "a")
     test = {"a": np.arange(1, 5)}
     attr = {"testval": 3.0}
     setup_hdf(f, test, attr)
```

### Comparing `pyqmc-0.5.1/pyqmc/j3.py` & `pyqmc-0.6.0/pyqmc/geminaljastrow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 import numpy as np
 import pyqmc.gpu as gpu
 import pyqmc.orbitals
+import pyqmc.supercell
 
 
-class J3:
+class GeminalJastrow:
+    """
+    Jastrow factor defined by Casula, Attaccalite, and Sorella, J. Chem. Phys. 121, 7110 (2004); https://doi.org/10.1063/1.1794632
+    """
+
     def __init__(self, mol, orbitals=None):
-        if hasattr(mol, "lattice_vectors"):
-            raise NotImplementedError("J3 is not implemented for periodic systems")
-        self.mol = mol
         if orbitals is None:
-            self.orbitals = pyqmc.orbitals.MoleculeOrbitalEvaluator(mol, [0, 0])
+            if hasattr(mol, "lattice_vectors"):
+                if not hasattr(mol, "original_cell"):
+                    mol = pyqmc.supercell.get_supercell(mol, np.eye(3))
+                else:
+                    mol = make_pbc_supercell_for_gamma_aos(mol)
+                kpts = [[0, 0, 0]]
+                self.orbitals = pyqmc.orbitals.PBCOrbitalEvaluatorKpoints(
+                    mol, kpts=kpts
+                )
+            else:
+                self.orbitals = pyqmc.orbitals.MoleculeOrbitalEvaluator(mol, [0, 0])
         else:
             self.orbitals = orbitals
         randpos = np.random.random((1, 3))
         dim = mol.eval_gto("GTOval_cart", randpos).shape[-1]
         self.parameters = {"gcoeff": gpu.cp.zeros((dim, dim))}
-        self.iscomplex = False
+        self.dtype = float
         self.optimize = "greedy"
 
     def recompute(self, configs):
         nconf, self.nelec = configs.configs.shape[:2]
         # shape of arrays:
         # ao_val: (nconf, nelec, nbasis)
         aos = self.orbitals.aos("GTOval_cart", configs)
@@ -121,7 +133,36 @@
             "mn, c...n, cim -> c...",
             self.parameters["gcoeff"],
             new_ao_val,
             masked_ao_val[:, e + 1 :, :],
             optimize=self.optimize,
         )
         return gpu.asnumpy(gpu.cp.exp((new_val.T - curr_val).T)), new_ao_val
+
+
+def make_pbc_supercell_for_gamma_aos(scell, S=None, **kwargs):
+    import pyscf.pbc.gto as gto
+
+    cell = scell.original_cell
+    if S is None:
+        S = scell.S
+    scale = np.abs(int(np.round(np.linalg.det(S))))
+    superlattice = np.dot(S, cell.lattice_vectors())
+    Rpts = pyqmc.supercell.get_supercell_copies(cell.lattice_vectors(), S)
+    atom = []
+    for name, xyz in cell._atom:
+        atom.extend([(name, xyz + R) for R in Rpts])
+
+    newcell = gto.Cell(
+        atom=atom,
+        a=superlattice,
+        unit="Bohr",
+        spin=cell.spin * scale,
+    )
+    for k in ["basis", "ecp", "exp_to_discard"]:
+        if k not in kwargs.keys() and k in cell.__dict__.keys():
+            kwargs[k] = cell.__dict__[k]
+    for k, v in kwargs.items():
+        newcell.__dict__[k] = v
+    newcell.build()
+    newsupercell = pyqmc.supercell.get_supercell(newcell, np.eye(3))
+    return newsupercell
```

### Comparing `pyqmc-0.5.1/pyqmc/jastrowspin.py` & `pyqmc-0.6.0/pyqmc/jastrowspin.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.a_basis = a_basis
         self.b_basis = b_basis
         self.parameters = {}
         self._nelec = np.sum(mol.nelec)
         self._mol = mol
         self.parameters["bcoeff"] = gpu.cp.zeros((len(b_basis), 3))
         self.parameters["acoeff"] = gpu.cp.zeros((self._mol.natm, len(a_basis), 2))
-        self.iscomplex = False
+        self.dtype = float
 
     def recompute(self, configs):
         r"""
 
         _avalues is the array for current configurations :math:`A_{Iks} = \sum_s a_{k}(r_{Is})` where :math:`s` indexes over :math:`\uparrow` (:math:`\alpha`) and :math:`\downarrow` (:math:`\beta`) sums.
         _bvalues is the array for current configurations :math:`B_{ls} = \sum_s b_{l}(r_{s})` where :math:`s` indexes over :math:`\uparrow\uparrow` (:math:`\alpha_1 < \alpha_2`), :math:`\uparrow\downarrow` (:math:`\alpha, \beta`), and :math:`\downarrow\downarrow` (:math:`\beta_1 < \beta_2`)  sums.
 
@@ -90,15 +90,16 @@
         u += gpu.cp.einsum("ijkl,jkl->i", self._avalues, self.parameters["acoeff"])
         return (np.ones(len(u)), gpu.asnumpy(u))
 
     def updateinternals(self, e, epos, configs, mask=None, saved_values=None):
         r"""Update a and b sums.
         _avalues is the array for current configurations :math:`A_{Iks} = \sum_s a_{k}(r_{Is})` where :math:`s` indexes over :math:`\uparrow` (:math:`\alpha`) and :math:`\downarrow` (:math:`\beta`) sums.
         _bvalues is the array for current configurations :math:`B_{ls} = \sum_s b_{l}(r_{s})` where :math:`s` indexes over :math:`\uparrow\uparrow` (:math:`\alpha_1 < \alpha_2`), :math:`\uparrow\downarrow` (:math:`\alpha, \beta`), and :math:`\downarrow\downarrow` (:math:`\beta_1 < \beta_2`)  sums.
-        The update for _avalues and _b_values from moving one electron only requires computing the new sum for that electron. The sums for the electron in the current configuration are stored in _a_partial and _b_partial"""
+        The update for _avalues and _b_values from moving one electron only requires computing the new sum for that electron. The sums for the electron in the current configuration are stored in _a_partial and _b_partial
+        """
         if mask is None:
             mask = [True] * self._configscurrent.configs.shape[0]
         edown = int(e >= self._mol.nelec[0])
         if saved_values is None:
             aupdate = self._a_update(e, epos, mask)
             bupdate, bvals = self._b_update(e, epos, mask)
         else:
```

### Comparing `pyqmc-0.5.1/pyqmc/linemin.py` & `pyqmc-0.6.0/pyqmc/linemin.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,24 +132,37 @@
         update_kws = {}
     if warmup_options is None:
         warmup_options = dict(nblocks=1, nsteps_per_block=100)
     if "tstep" not in warmup_options and "tstep" in vmcoptions:
         warmup_options["tstep"] = vmcoptions["tstep"]
     assert npts >= 3, f"linemin npts={npts}; need npts >= 3 for correlated sampling"
 
-    # Restart
     iteration_offset = 0
-    if hdf_file is not None and os.path.isfile(hdf_file):
+    if hdf_file is not None and os.path.isfile(hdf_file):  # restarting -- read in data
         with h5py.File(hdf_file, "r") as hdf:
             if "wf" in hdf.keys():
                 grp = hdf["wf"]
                 for k in grp.keys():
                     wf.parameters[k] = gpu.cp.asarray(grp[k])
             if "iteration" in hdf.keys():
                 iteration_offset = np.max(hdf["iteration"][...]) + 1
+            coords.load_hdf(hdf)
+    else:  # not restarting -- VMC warm up period
+        if verbose:
+            print("starting warmup")
+        _, coords = pyqmc.mc.vmc(
+            wf,
+            coords,
+            accumulators={},
+            client=client,
+            npartitions=npartitions,
+            **warmup_options,
+        )
+        if verbose:
+            print("finished warmup", flush=True)
 
     # Attributes for linemin
     attr = dict(max_iterations=max_iterations, npts=npts, steprange=steprange)
 
     def gradient_energy_function(x, coords):
         newparms = pgrad_acc.transform.deserialize(wf, x)
         for k in newparms:
@@ -176,27 +189,14 @@
                 print(nm, quant)
             raise ValueError("NaN detected in derivatives")
 
         return coords, grad, Sij, en, en_err, sigma
 
     x0 = pgrad_acc.transform.serialize_parameters(wf.parameters)
 
-    # VMC warm up period
-    if verbose:
-        print("starting warmup")
-    _, coords = pyqmc.mc.vmc(
-        wf,
-        coords,
-        accumulators={},
-        client=client,
-        npartitions=npartitions,
-        **warmup_options,
-    )
-    if verbose:
-        print("finished warmup", flush=True)
     df = []
     # Gradient descent cycles
     for it in range(max_iterations):
         # Calculate gradient accurately
         coords, pgrad, Sij, en, en_err, sigma = gradient_energy_function(x0, coords)
         step_data = {}
         step_data["energy"] = en
@@ -262,15 +262,17 @@
     :returns: a single dict with indices [parameter, values]
 
     """
 
     data = []
     psi0 = wf.recompute(configs)[1]  # recompute gives logdet
 
+    current_state = np.random.get_state()
     for p in params:
+        np.random.set_state(current_state)
         newparms = pgrad_acc.transform.deserialize(wf, p)
         for k in newparms:
             wf.parameters[k] = newparms[k]
         psi = wf.recompute(configs)[1]  # recompute gives logdet
         rawweights = np.exp(2 * (psi - psi0))  # convert from log(|psi|) to |psi|**2
         df = pgrad_acc.enacc(configs, wf)
         df["weight"] = rawweights
```

### Comparing `pyqmc-0.5.1/pyqmc/mc.py` & `pyqmc-0.6.0/pyqmc/mc.py`

 * *Files identical despite different names*

### Comparing `pyqmc-0.5.1/pyqmc/multiplywf.py` & `pyqmc-0.6.0/pyqmc/multiplywf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 
 class Parameters:
     def __init__(self, dicts):
         self.data = {}
         self.wf_count = len(dicts)
-        for (i, d) in enumerate(dicts):
+        for i, d in enumerate(dicts):
             self.data["wf" + str(i + 1)] = d
 
     def __setitem__(self, idx, value):
         k1 = idx[0:3]
         k2 = idx[3:]
         self.data[k1][k2] = value
 
@@ -58,16 +58,16 @@
     """
     A general representation of a wavefunction as a product of multiple wf_factors
     """
 
     def __init__(self, *wf_factors):
         self.wf_factors = [*wf_factors]
         self.parameters = Parameters([wf.parameters for wf in wf_factors])
-        self.iscomplex = bool(sum(wf.iscomplex for wf in wf_factors))
-        self.dtype = complex if self.iscomplex else float
+        iscomplex = bool(sum(wf.dtype == complex for wf in wf_factors))
+        self.dtype = complex if iscomplex else float
 
     def recompute(self, configs):
         signs = np.ones(len(configs.configs))
         vals = np.zeros(len(configs.configs))
         for wf in self.wf_factors:
             results = wf.recompute(configs)
             signs = signs * results[0]
```

### Comparing `pyqmc-0.5.1/pyqmc/obdm.py` & `pyqmc-0.6.0/pyqmc/obdm.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         tstep=0.50,
         warmup=100,
         naux=None,
         spin=None,
         electrons=None,
         kpts=None,
     ):
-
         if spin is not None:
             if spin == 0:
                 self._electrons = np.arange(0, mol.nelec[0])
             elif spin == 1:
                 self._electrons = np.arange(mol.nelec[0], np.sum(mol.nelec))
             else:
                 raise ValueError("Spin not equal to 0 or 1")
@@ -80,15 +79,15 @@
         else:
             if not hasattr(mol, "original_cell"):
                 mol = supercell.get_supercell(mol, np.eye(3))
             self.orbitals = pyqmc.orbitals.PBCOrbitalEvaluatorKpoints(
                 mol, [orb_coeff, orb_coeff], kpts
             )
 
-        self.iscomplex = self.orbitals.iscomplex
+        self.dtype = self.orbitals.mo_dtype
 
         self._tstep = tstep
         self.nelec = len(self._electrons)
         self._nsweeps = nsweeps
         self._nstep = nsweeps * self.nelec
         self._warmup = warmup
         self._naux = naux
@@ -114,17 +113,16 @@
 
         nconf = configs.configs.shape[0]
         if not self._warmed_up:
             naux = nconf if self._naux is None else self._naux
             self.warm_up(naux)
             self._warmed_up = True
 
-        dtype = complex if self.iscomplex else float
         results = {
-            "value": np.zeros((nconf, self.norb, self.norb), dtype=dtype),
+            "value": np.zeros((nconf, self.norb, self.norb), dtype=self.dtype),
             "norm": np.zeros((nconf, self.norb)),
         }
         naux = self._extra_config.configs.shape[0]
 
         auxassignments = np.random.randint(0, naux, size=(self._nsweeps, nconf))
         accept, extra_configs, borb_aux = sample_onebody(
             self._extra_config,
```

### Comparing `pyqmc-0.5.1/pyqmc/optimize_excited_states.py` & `pyqmc-0.6.0/pyqmc/optimize_excited_states.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-from scipy.stats.stats import WeightedTauResult
 import pyqmc.mc as mc
 import scipy.stats
 import pyqmc.linemin as linemin
 
 """
 TODO:
 
@@ -299,15 +298,19 @@
             avg[("dp2", wfi)][:, wfi, wfi] - avg[("dp", wfi)][:, wfi, wfi] ** 2
         )
     ret["energy"] = avg["total"]
     return ret
 
 
 def objective_function_derivative(
-    terms, overlap_penalty, norm_penalty, offdiagonal_energy_penalty
+    terms,
+    overlap_penalty,
+    norm_penalty,
+    offdiagonal_energy_penalty,
+    lagrange_multiplier,
 ):
     """
     terms are output from generate_terms
     lam is the penalty
     norm_relative_penalty is the prefactor on the norm
     offdiagonal_energy_penalty is the penalty on the off-diagonal matrix elements.
     """
@@ -315,27 +318,29 @@
 
     return [
         terms[("dp_energy", i)][:, i, i]
         + overlap_penalty
         * 2
         * np.sum(np.triu(terms[("dp_overlap", i)] * terms["overlap"], 1), axis=(1, 2))
         + norm_penalty * 2 * (terms["norm"][i] - 1) * terms[("dp_norm", i)]
+        + np.sum(
+            np.triu(lagrange_multiplier * terms[("dp_overlap", i)], 1), axis=(1, 2)
+        )
         + offdiagonal_energy_penalty
         * 2.0
         * np.sum(np.triu(terms["energy"] * terms[("dp_energy", i)], 1), axis=(1, 2))
         for i in range(nwf)
     ]
 
 
 import pyqmc.hdftools as hdftools
 import h5py
 
 
 def hdf_save(hdf_file, data, attr, wfs):
-
     if hdf_file is not None:
         with h5py.File(hdf_file, "a") as hdf:
             if "energy" not in hdf.keys():
                 hdftools.setup_hdf(hdf, data, attr)
                 for wfi, wf in enumerate(wfs):
                     for k, it in wf.parameters.items():
                         hdf.create_dataset(f"wf/{wfi}/" + k, data=it)
@@ -403,15 +408,17 @@
     log_vals = np.real(log_vals)  # should already be real
     ref = np.max(log_vals, axis=0)
     rho = np.mean(np.nan_to_num(np.exp(2 * (log_vals - ref))), axis=0)
     nconfig = configs.configs.shape[0]
 
     energy_final = []
     overlap_final = []
+    current_state = np.random.get_state()
     for p, parameter in enumerate(parameters):
+        np.random.set_state(current_state)
         for wf, transform, wf_parm in zip(wfs, transforms, parameter):
             for k, it in transform.deserialize(wf, wf_parm).items():
                 wf.parameters[k] = it
 
         phase, log_vals = [
             np.nan_to_num(np.array(x))
             for x in zip(*[wf.recompute(configs) for wf in wfs])
@@ -438,14 +445,15 @@
 
 def find_move_from_line(
     x,
     data,
     overlap_penalty,
     norm_penalty,
     offdiagonal_energy_penalty,
+    lagrange_multiplier,
     max_norm_deviation=0.2,
 ):
     """
     Given the data from correlated sampling, find the best move.
 
     Return:
     cost function
@@ -459,14 +467,15 @@
     # print("energy cost", np.sum(energy.diagonal(axis1=1,axis2=2),axis=1))
     # print("overlap cost",np.sum(np.triu(overlap**2,1),axis=(1,2)) )
     # print("offdiagonal_energy", energy)
     # print("norm",np.einsum('ijj->i', (overlap-1)**2 ))
     cost = (
         np.sum(energy.diagonal(axis1=1, axis2=2), axis=1)
         + overlap_penalty * np.sum(np.triu(overlap**2, 1), axis=(1, 2))
+        + np.sum(lagrange_multiplier * np.triu(overlap, 1), axis=(1, 2))
         + offdiagonal_energy_penalty * np.sum(np.triu(energy**2, 1), axis=(1, 2))
         + norm_penalty * np.einsum("ijj->i", (overlap - 1) ** 2)
     )
 
     # good_norms = np.prod(np.einsum('ijj->ij',np.abs(overlap-1) < max_norm_deviation),axis=1)
     # print("good norms", good_norms, 'cost', cost[good_norms])
     xmin = linemin.stable_fit(x, cost)
@@ -481,14 +490,15 @@
 def optimize(
     wfs,
     configs,
     energy,
     transforms,
     hdf_file,
     overlap_penalty=0.5,
+    lagrange_multiplier=0.0,
     nsteps=40,
     max_tstep=0.1,
     condition_epsilon=0.1,
     norm_penalty=0.01,
     offdiagonal_energy_penalty=0.1,
     vmc_options=None,
     client=None,
@@ -521,15 +531,19 @@
         )
         avg, error = average(data_weighted, data_unweighted)
         print("energy", avg["total"], error["total"])
         terms = collect_terms(avg, error)
         print("norm", terms["norm"])
         print("overlap", terms["overlap"][0, 1])
         derivative = objective_function_derivative(
-            terms, overlap_penalty, norm_penalty, offdiagonal_energy_penalty
+            terms,
+            overlap_penalty,
+            norm_penalty,
+            offdiagonal_energy_penalty,
+            lagrange_multiplier,
         )
         derivative_conditioned = [
             d / (terms[("condition", i)] + condition_epsilon)
             for i, d in enumerate(derivative)
         ]
         print("|gradient|", [np.linalg.norm(d) for d in derivative_conditioned])
 
@@ -551,14 +565,15 @@
         )
         xmin, cost = find_move_from_line(
             x,
             correlated_data,
             overlap_penalty,
             norm_penalty,
             offdiagonal_energy_penalty,
+            lagrange_multiplier,
         )
         print("line search", x, cost)
         print("choosing to move", xmin)
         parameters = [p - xmin * d for p, d in zip(parameters, derivative_conditioned)]
         for wf, transform, parm in zip(wfs, transforms, parameters):
             for k, it in transform.deserialize(wf, parm).items():
                 wf.parameters[k] = it
```

### Comparing `pyqmc-0.5.1/pyqmc/optimize_ortho.py` & `pyqmc-0.6.0/pyqmc/optimize_ortho.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import pyqmc.linemin
 import pyqmc.hdftools as hdftools
 import pyqmc.mc as mc
 import os
 
 
 def ortho_hdf(hdf_file, data, attr, configs, parameters):
-
     if hdf_file is not None:
         with h5py.File(hdf_file, "a") as hdf:
             if "configs" not in hdf.keys():
                 hdftools.setup_hdf(hdf, data, attr)
                 hdf.create_dataset("configs", configs.configs.shape)
                 for k, it in parameters.items():
                     hdf.create_dataset("wf/" + k, data=it)
@@ -259,24 +258,26 @@
     ref = np.max(log_values0)
     normalized_values = phase0 * np.exp(log_values0 - ref)
     denominator = np.sum(np.exp(2 * (log_values0 - ref)), axis=0)
     rhoprime_ = np.sum(np.exp(2 * (log_values0[:-1] - ref)), axis=0)
 
     wt0 = 1.0 / np.sum(np.exp(-2 * (log_values0[:, np.newaxis] - log_values0)), axis=1)
     weight = np.mean(wt0, axis=1)
-    dtype = complex if wfs[-1].iscomplex else float
+    dtype = wfs[-1].dtype
 
     data = {
         "total": np.zeros(nparms),
         "weight": np.zeros(nparms),
         "overlap": np.zeros((nparms, len(wfs)), dtype=dtype),
         "rhoprime": np.zeros(nparms),
     }
     data["base_weight"] = weight
+    current_state = np.random.get_state()
     for p, parameter in enumerate(parameters):
+        np.random.set_state(current_state)
         wf = wfs[-1]
         for k, it in pgrad.transform.deserialize(wf, parameter).items():
             wf.parameters[k] = it
         wf.recompute(configs)
         val = wf.value()
         dat = pgrad.enacc(configs, wf)
 
@@ -293,15 +294,14 @@
 
     for k, it in pgrad.transform.deserialize(wf, p0).items():
         wfs[-1].parameters[k] = it
     return data
 
 
 def dist_correlated_sample(wfs, configs, *args, client, npartitions=None, **kwargs):
-
     if npartitions is None:
         npartitions = sum(client.nthreads().values())
 
     coord = configs.split(npartitions)
     allruns = []
     for nodeconfigs in coord:
         allruns.append(
@@ -350,39 +350,46 @@
 def evaluate(return_data, warmup):
     """
     For wave functions wfs and coordinate set coords, evaluate the overlap and energy of the last wave function.
 
     Returns a dictionary with relevant information.
     """
     avg_data = {}
+    error_data = {}
     for k, it in return_data.items():
         avg_data[k] = np.average(it[warmup:], axis=0)
+        error_data[k] = np.std(it[warmup:], axis=0) / np.sqrt(it[warmup:].shape[0] - 1)
     N = np.abs(avg_data["overlap"].diagonal())
+    N_error = np.abs(error_data["overlap"].diagonal())
     # Derivatives are only for the optimized wave function, so they miss
     # an index
     N_derivative = 2 * np.real(avg_data["overlap_gradient"][-1])
     Nij = np.sqrt(np.outer(N, N))
     S = avg_data["overlap"] / Nij
+    S_error = error_data["overlap"] / Nij
     S_derivative = avg_data["overlap_gradient"] / Nij[-1, :, np.newaxis] - np.einsum(
         "j,m->jm", 0.5 * avg_data["overlap"][-1, :] / Nij[-1, :], N_derivative / N[-1]
     )
     energy_derivative = 2.0 * np.real(
         avg_data["dpH"] - avg_data["total"] * avg_data["dppsi"]
     )
     dp = avg_data["dppsi"]
     condition = np.real(avg_data["dpidpj"] - np.einsum("i,j->ij", dp, dp))
 
     return {
         "N": N,
+        "N_error": N_error,
         "S": S,
+        "S_error": S_error,
         "S_derivative": S_derivative,
         "energy_derivative": energy_derivative,
         "N_derivative": N_derivative,
         "condition": condition,
         "total": np.real(avg_data["total"]),
+        "total_error": np.real(error_data["total"]),
     }
 
 
 def optimize_orthogonal(
     wfs,
     coords,
     pgrad,
@@ -507,15 +514,14 @@
         Ntarget=Ntarget,
         max_step=max_step,
     )
     conditioner = pyqmc.linemin.sd_update
     if npartitions is None:
         npartitions = sum(client.nthreads().values())
 
-
     if sample_options is None:
         sample_options = {}
     if correlated_options is None:
         correlated_options = {}
 
     if client is None:
         sampler = sample_overlap
@@ -541,65 +547,77 @@
         client=client,
         npartitions=npartitions,
         **warmup_options
     )
 
     # One set of configurations for every wave function
     allcoords = [coords.copy() for _ in wfs[:-1]]
-    dtype = np.complex if wfs[-1].iscomplex else np.float
+    dtype = wfs[-1].dtype
 
     for step in range(max_iterations):
         # we iterate until the normalization is reasonable
         # One could potentially save a little time here by not computing the gradients
         # every time, but typically we don't have to renormalize if the moves are good
 
         # Memory efficient implementation
         nwf = len(wfs)
         normalization = np.zeros(nwf - 1)
+        normalization_error = np.zeros(nwf - 1)
         total_energy = 0
+        total_energy_error_squared = 0
         # energy_derivative = np.zeros(len(parameters))
         N_derivative = np.zeros(len(parameters))
         condition = np.zeros((len(parameters), len(parameters)))
         overlaps = np.zeros(nwf - 1, dtype=dtype)
+        overlap_errors = np.zeros(nwf - 1, dtype=dtype)
         overlap_derivatives = np.zeros((nwf - 1, len(parameters)), dtype=dtype)
 
         while True:
             return_data, _ = sampler(
                 [wfs[0], wfs[-1]], allcoords[0], pgrad, **sample_options
             )
             tmp_deriv = evaluate(return_data, warmup)
             N = tmp_deriv["N"][-1]
 
             if verbose:
                 print("Normalization", N, flush=True)
             if abs(N - Ntarget) < Ntol:
                 normalization[0] = tmp_deriv["N"][-1]
+                normalization_error[0] = tmp_deriv["N_error"][-1]
                 total_energy += tmp_deriv["total"] / (nwf - 1)
+                total_energy_error_squared += (
+                    tmp_deriv["total_error"] / (nwf - 1)
+                ) ** 2
                 energy_derivative = tmp_deriv["energy_derivative"] / (nwf - 1)
                 N_derivative += tmp_deriv["N_derivative"] / (nwf - 1)
                 condition += tmp_deriv["condition"] / (nwf - 1)
                 overlaps[0] = tmp_deriv["S"][-1, 0]
+                overlap_errors[0] = tmp_deriv["S_error"][-1, 0]
                 overlap_derivatives[0] = tmp_deriv["S_derivative"][0, :]
                 break
             else:
                 renormalize([wfs[0], wfs[-1]], N)
                 parameters = pgrad.transform.serialize_parameters(wfs[-1].parameters)
 
         for i, wf in enumerate(wfs[1:-1]):
             return_data, _ = sampler(
                 [wf, wfs[-1]], allcoords[i + 1], pgrad, **sample_options
             )
             deriv_data = evaluate(return_data, warmup)
             normalization[i + 1] = deriv_data["N"][-1]
+            normalization_error[i + 1] = deriv_data["N_error"][-1]
             total_energy += deriv_data["total"] / (nwf - 1)
+            total_energy_error_squared += (deriv_data["total_error"] / (nwf - 1)) ** 2
             energy_derivative += deriv_data["energy_derivative"] / (nwf - 1)
             N_derivative += deriv_data["N_derivative"] / (nwf - 1)
             condition += deriv_data["condition"] / (nwf - 1)
             overlaps[i + 1] = deriv_data["S"][-1, 0]
+            overlap_errors[i + 1] = deriv_data["S_error"][-1, 0]
             overlap_derivatives[i + 1] = deriv_data["S_derivative"][0, :]
+        total_energy_error = np.sqrt(np.sum(total_energy_error_squared))
         if verbose:
             print("normalization", normalization)
 
         delta = overlaps - Starget
         delta_phase = delta / np.abs(delta)
         overlap_derivative = np.einsum(
             "j,jk->k",
@@ -704,20 +722,23 @@
             tstep *= 0.5
 
         for k, it in pgrad.transform.deserialize(wfs[-1], parameters).items():
             wfs[-1].parameters[k] = it
 
         save_data = {
             "energy": total_energy,
+            "energy_error": total_energy_error,
             "overlap": overlaps,
+            "overlap_error": overlap_errors,
             "gradient": total_derivative,
             "N": N,
             "parameters": parameters,
             "iteration": step + step_offset,
             "normalization": normalization,
+            "normalization_error": normalization_error,
             "overlap_derivatives": overlap_derivatives,
             "energy_derivative": energy_derivative,
             "line_tsteps": test_tsteps,
             "line_cost": cost,
             "line_norm": line_data["weight"],
         }
```

### Comparing `pyqmc-0.5.1/pyqmc/optvariance.py` & `pyqmc-0.6.0/pyqmc/optvariance.py`

 * *Files identical despite different names*

### Comparing `pyqmc-0.5.1/pyqmc/orbitals.py` & `pyqmc-0.6.0/pyqmc/orbitals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import numpy as np
 import pyqmc.gpu as gpu
 import pyqmc.pbc as pbc
 import pyqmc.supercell as supercell
-import pyqmc.pbc_eval_gto as pbc_eval_gto
 import pyqmc.determinant_tools
-import pyscf.pbc.dft.gen_grid
-
+import pyscf.pbc.gto.eval_gto
+import pyscf.lib
+import pyqmc.pbc
+import pyqmc.twists as twists
 
 """
 The evaluators have the concept of a 'set' of atomic orbitals, that may apply to 
 different sets of molecular orbitals
 
 For example, for the PBC evaluator, each k-point is a set, since each molecular 
 orbital is only a sum over the k-point of its type.
@@ -44,40 +45,36 @@
     You cannot pass both mc/tol and determinants.
 
     Returns:
     an orbital evaluator chosen based on the inputs.
     """
 
     if hasattr(mol, "a"):
-        if mc is not None:
-            if not hasattr(mc, "orbitals") or mc.orbitals is None:
-                mc.orbitals = np.arange(mc.ncore, mc.ncore + mc.ncas)
-            determinants = pyqmc.determinant_tools.pbc_determinants_from_casci(
-                mc, mc.orbitals
-            )
         return PBCOrbitalEvaluatorKpoints.from_mean_field(
-            mol, mf, twist, determinants=determinants, tol=tol
+            mol, mf, mc=mc, twist=twist, determinants=determinants, tol=tol
         )
     if mc is None:
         return MoleculeOrbitalEvaluator.from_pyscf(
             mol, mf, determinants=determinants, tol=tol
         )
     return MoleculeOrbitalEvaluator.from_pyscf(
         mol, mf, mc, determinants=determinants, tol=tol
     )
 
 
 class MoleculeOrbitalEvaluator:
     def __init__(self, mol, mo_coeff):
-        self.iscomplex = False
         self.parameters = {
             "mo_coeff_alpha": gpu.cp.asarray(mo_coeff[0]),
             "mo_coeff_beta": gpu.cp.asarray(mo_coeff[1]),
         }
         self.parm_names = ["_alpha", "_beta"]
+        iscomplex = bool(sum(map(gpu.cp.iscomplexobj, self.parameters.values())))
+        self.ao_dtype = True
+        self.mo_dtype = complex if iscomplex else float
 
         self._mol = mol
 
     @classmethod
     def from_pyscf(self, mol, mf, mc=None, tol=-1, determinants=None):
         """
         mol: A Mole object
@@ -137,22 +134,14 @@
             gpu.cp.array(
                 [self.parameters[f"mo_coeff{self.parm_names[spin]}"].shape[1]]
             ),
             ao,
         )
 
 
-def get_k_indices(cell, mf, kpts, tol=1e-6):
-    """Given a list of kpts, return inds such that mf.kpts[inds] is a list of kpts equivalent to the input list"""
-    kdiffs = mf.kpts[np.newaxis] - kpts[:, np.newaxis]
-    frac_kdiffs = np.dot(kdiffs, cell.lattice_vectors().T) / (2 * np.pi)
-    kdiffs = np.mod(frac_kdiffs + 0.5, 1) - 0.5
-    return np.nonzero(np.linalg.norm(kdiffs, axis=-1) < tol)[1]
-
-
 def pbc_single_determinant(mf, kinds):
     detcoeff = np.array([1.0])
     det_map = np.array([[0], [0]])
 
     if len(mf.mo_coeff[0][0].shape) == 2:
         occup_k = [
             [[list(np.argwhere(mf.mo_occ[spin][k] > 0.5)[:, 0])] for k in kinds]
@@ -162,30 +151,34 @@
         occup_k = [
             [[list(np.argwhere(mf.mo_occ[k] > 1.5 - spin)[:, 0])] for k in kinds]
             for spin in [0, 1]
         ]
     return detcoeff, det_map, occup_k
 
 
-def select_orbitals_kpoints(determinants, mf, kinds):
+def select_orbitals_kpoints(determinants, mo_coeff, kinds):
     """
     Based on the k-point indices in `kinds`, select the MO coefficients that correspond to those k-points,
     and the determinants.
     The determinant indices are flattened so that the indices refer to the concatenated MO coefficients.
     """
     max_orb = [
         [[np.max(orb_k) + 1 if len(orb_k) > 0 else 0 for orb_k in spin] for spin in det]
         for wt, det in determinants
     ]
     max_orb = np.amax(max_orb, axis=0)
 
-    if len(mf.mo_coeff[0][0].shape) == 2:
-        mf_mo_coeff = mf.mo_coeff
-    elif len(mf.mo_coeff[0][0].shape) == 1:
-        mf_mo_coeff = [mf.mo_coeff, mf.mo_coeff]
+    if len(mo_coeff[0][0].shape) == 2:
+        mf_mo_coeff = mo_coeff
+    elif len(mo_coeff[0][0].shape) == 1:
+        mf_mo_coeff = [mo_coeff, mo_coeff]
+    else:
+        raise ValueError(
+            f"mo_coeff[0][0] has unexpected number of array dimensions: {mo_coeff[0][0].shape}"
+        )
     mo_coeff = [
         [mf_mo_coeff[s][k][:, 0 : max_orb[s][k]] for ki, k in enumerate(kinds)]
         for s in range(2)
     ]
 
     # and finally, we remove the k-index from determinants
     determinants_flat = []
@@ -209,36 +202,51 @@
     Evaluate orbitals from a PBC object.
     cell is expected to be one made with make_supercell().
     mo_coeff should be in [spin][k][ao,mo] order
     kpts should be a list of the k-points corresponding to mo_coeff
 
     """
 
-    def __init__(self, cell, mo_coeff, kpts=None):
-        self.iscomplex = True
+    def __init__(self, cell, mo_coeff=None, kpts=None):
+        """
+        :parameter cell: PyQMC supercell object (from get_supercell)
+        :parameter mo_coeff: (2, nk, nao, nelec) array. MO coefficients for all kpts of primitive cell. If None, this object can't evaluate mos(), but can still evaluate aos().
+        :parameter kpts: list of kpts to evaluate AOs
+        """
         self._cell = cell.original_cell
         self.S = cell.S
         self.Lprim = self._cell.lattice_vectors()
 
         self._kpts = [0, 0, 0] if kpts is None else kpts
-        self.param_split = [
-            np.cumsum(np.asarray([m.shape[1] for m in mo_coeff[spin]]))
-            for spin in [0, 1]
-        ]
-        self.parm_names = ["_alpha", "_beta"]
-        self.parameters = {
-            "mo_coeff_alpha": gpu.cp.asarray(np.concatenate(mo_coeff[0], axis=1)),
-            "mo_coeff_beta": gpu.cp.asarray(np.concatenate(mo_coeff[1], axis=1)),
-        }
+        # If gamma-point only, AOs are real-valued
+        isgamma = np.abs(self._kpts).sum() < 1e-9
+        if mo_coeff is not None:
+            nelec_per_kpt = [np.asarray([m.shape[1] for m in mo]) for mo in mo_coeff]
+            self.param_split = [np.cumsum(nelec_per_kpt[spin]) for spin in [0, 1]]
+            self.parm_names = ["_alpha", "_beta"]
+            self.parameters = {
+                "mo_coeff_alpha": gpu.cp.asarray(np.concatenate(mo_coeff[0], axis=1)),
+                "mo_coeff_beta": gpu.cp.asarray(np.concatenate(mo_coeff[1], axis=1)),
+            }
+            iscomplex = (not isgamma) or bool(
+                sum(map(gpu.cp.iscomplexobj, self.parameters.values()))
+            )
+        else:
+            iscomplex = not isgamma
 
-        self.Ls = pbc_eval_gto.get_lattice_Ls(self._cell)
-        self.rcut = pbc_eval_gto._estimate_rcut(self._cell)
+        self.ao_dtype = float if isgamma else complex
+        self.mo_dtype = complex if iscomplex else float
+        Ls = self._cell.get_lattice_Ls(dimension=3)
+        self.Ls = Ls[np.argsort(pyscf.lib.norm(Ls, axis=1))]
+        self.rcut = pyscf.pbc.gto.eval_gto._estimate_rcut(self._cell)
 
     @classmethod
-    def from_mean_field(self, cell, mf, twist=None, determinants=None, tol=None):
+    def from_mean_field(
+        self, cell, mf, mc=None, twist=None, determinants=None, tol=None
+    ):
         """
         mf is expected to be a KUHF, KRHF, or equivalent DFT objects.
         Selects occupied orbitals from a given twist
         If cell is a supercell, will automatically choose the folded k-points that correspond to that twist.
 
         """
 
@@ -246,40 +254,50 @@
             cell
             if hasattr(cell, "original_cell")
             else supercell.get_supercell(
                 cell, np.asarray([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
             )
         )
         if twist is None:
-            twist = np.zeros(3)
-        else:
-            twist = np.dot(np.linalg.inv(cell.a), np.mod(twist, 1.0)) * 2 * np.pi
+            twist = 0
         if not hasattr(mf, "kpts"):
             mf.kpts = np.zeros((1, 3))
             if len(mf.mo_occ.shape) == 1:
                 mf.mo_coeff = [mf.mo_coeff]
                 mf.mo_occ = [mf.mo_occ]
             elif len(mf.mo_occ.shape) == 2:
                 mf.mo_coeff = [[c] for c in mf.mo_coeff]
                 mf.mo_occ = [[o] for o in mf.mo_occ]
-        kinds = list(
-            set(get_k_indices(cell, mf, supercell.get_supercell_kpts(cell) + twist))
-        )
+
+        kinds = twists.create_supercell_twists(cell, mf)["primitive_ks"][twist]
         if len(kinds) != cell.scale:
             raise ValueError(
                 f"Found {len(kinds)} k-points but should have found {cell.scale}."
             )
         kpts = mf.kpts[kinds]
 
         if determinants is None:
-            determinants = [
-                (1.0, pyqmc.determinant_tools.create_pbc_determinant(cell, mf, []))
-            ]
+            if mc is not None:
+                if not hasattr(mc, "orbitals") or mc.orbitals is None:
+                    mc.orbitals = np.arange(mc.ncore, mc.ncore + mc.ncas)
+                determinants = pyqmc.determinant_tools.pbc_determinants_from_casci(
+                    mc, mc.orbitals
+                )
+            else:
+                determinants = [
+                    (1.0, pyqmc.determinant_tools.create_pbc_determinant(cell, mf, []))
+                ]
 
-        mo_coeff, determinants_flat = select_orbitals_kpoints(determinants, mf, kinds)
+        if mc is not None:
+            mo_coeff = [mc.mo_coeff]  # kpt list
+        else:
+            mo_coeff = mf.mo_coeff
+        mo_coeff, determinants_flat = select_orbitals_kpoints(
+            determinants, mo_coeff, kinds
+        )
         detcoeff, occup, det_map = pyqmc.determinant_tools.create_packed_objects(
             determinants_flat, format="list", tol=tol
         )
         # Check
         for s, (occ_s, nelec_s) in enumerate(zip(occup, cell.nelec)):
             for determinant in occ_s:
                 if len(determinant) != nelec_s:
@@ -307,32 +325,34 @@
         if a derivative is requested, will instead return [k,d,...,orbital].
 
         The ... is the total length of mycoords. You'll need to reshape if you want the original shape
         """
         mycoords = configs.configs if mask is None else configs.configs[mask]
         mycoords = mycoords.reshape((-1, mycoords.shape[-1]))
         primcoords, primwrap = pbc.enforce_pbc(self.Lprim, mycoords)
-        # coordinate, dimension
-        wrap = configs.wrap if mask is None else configs.wrap[mask]
-        wrap = np.dot(wrap, self.S)
-        wrap = wrap.reshape((-1, wrap.shape[-1])) + primwrap
-        kdotR = np.linalg.multi_dot(
-            (self._kpts, self._cell.lattice_vectors().T, wrap.T)
-        )
-        # k, coordinate
-        wrap_phase = get_wrapphase_complex(kdotR)
-        # k,coordinate, orbital
         ao = gpu.cp.asarray(
-            self._cell.eval_gto(
+            pyscf.pbc.gto.eval_gto.eval_gto(
+                self._cell,
                 "PBC" + eval_str,
                 primcoords,
                 kpts=self._kpts,
+                rcut=self.rcut,
+                Ls=self.Ls,
             )
         )
-        ao = gpu.cp.einsum("k...,k...a->k...a", wrap_phase, ao)
+        if self.ao_dtype == complex:
+            wrap = configs.wrap if mask is None else configs.wrap[mask]
+            wrap = np.dot(wrap, self.S)
+            wrap = wrap.reshape((-1, wrap.shape[-1])) + primwrap
+            kdotR = np.linalg.multi_dot(
+                (self._kpts, self._cell.lattice_vectors().T, wrap.T)
+            )
+            # k, coordinate
+            wrap_phase = get_wrapphase_complex(kdotR)
+            ao = gpu.cp.einsum("k...,k...a->k...a", wrap_phase, ao)
         if len(ao.shape) == 4:  # if derivatives are included
             return ao.reshape(
                 (ao.shape[0], ao.shape[1], *mycoords.shape[:-1], ao.shape[-1])
             )
         else:
             return ao.reshape((ao.shape[0], *mycoords.shape[:-1], ao.shape[-1]))
 
@@ -343,17 +363,20 @@
         In the derivative case, returns [d,..., mo]
         """
         p = np.split(
             self.parameters[f"mo_coeff{self.parm_names[spin]}"],
             self.param_split[spin],
             axis=-1,
         )
-        return gpu.cp.concatenate(
-            [ak.dot(mok) for ak, mok in zip(ao, p[0:-1])], axis=-1
-        )
+        ps = [0] + list(self.param_split[spin])
+        nelec = self.parameters[f"mo_coeff{self.parm_names[spin]}"].shape[1]
+        out = gpu.cp.zeros([nelec, *ao[0].shape[:-1]], dtype=self.mo_dtype)
+        for i, ak, mok in zip(range(len(ao)), ao, p[:-1]):
+            gpu.cp.einsum("...a,an->n...", ak, mok, out=out[ps[i] : ps[i + 1]])
+        return out.transpose([*np.arange(1, len(out.shape)), 0])
 
     def pgradient(self, ao, spin):
         """
         returns:
         N sets of atomic orbitals
         split: which molecular orbitals correspond to which set
```

### Comparing `pyqmc-0.5.1/pyqmc/pbc.py` & `pyqmc-0.6.0/pyqmc/pbc.py`

 * *Files identical despite different names*

### Comparing `pyqmc-0.5.1/pyqmc/pyscftools.py` & `pyqmc-0.6.0/pyqmc/pyscftools.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         if len(mo_occ_shape) == 2:
             mf = pyscf.scf.UHF(mol)
         elif len(mo_occ_shape) == 1:
             mf = pyscf.scf.ROHF(mol) if mol.spin != 0 else pyscf.scf.RHF(mol)
         else:
             raise Exception("Couldn't determine type from chkfile")
     else:
-
         mol = pyscf.pbc.lib.chkfile.load_cell(chkfile)
         with h5py.File(chkfile, "r") as f:
             has_kpts = "mo_occ__from_list__" in f["/scf"].keys()
             if has_kpts:
                 rhf = "000000" in f["/scf/mo_occ__from_list__/"].keys()
             else:
                 rhf = len(f["/scf/mo_occ"].shape) == 1
@@ -57,14 +56,16 @@
             mf = pyscf.pbc.scf.ROHF(mol) if mol.spin != 0 else pyscf.pbc.scf.RHF(mol)
         else:
             mf = pyscf.pbc.scf.UHF(mol)
     mf.__dict__.update(pyscf.scf.chkfile.load(chkfile, "scf"))
 
     if ci_checkfile is not None:
         casdict = pyscf.lib.chkfile.load(ci_checkfile, "ci")
+        if casdict is None:
+            casdict = pyscf.lib.chkfile.load(ci_checkfile, "mcscf")
         with h5py.File(ci_checkfile, "r") as f:
             hci = "ci/_strs" in f.keys()
         if hci:
             mc = pyscf.hci.SCI(mol)
         else:
             if len(casdict["mo_coeff"].shape) == 3:
                 mc = pyscf.mcscf.UCASCI(mol, casdict["ncas"], casdict["nelecas"])
```

### Comparing `pyqmc-0.5.1/pyqmc/reblock.py` & `pyqmc-0.6.0/pyqmc/reblock.py`

 * *Files identical despite different names*

### Comparing `pyqmc-0.5.1/pyqmc/recipes.py` & `pyqmc-0.6.0/pyqmc/recipes.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,15 +71,17 @@
                 )[0]
             )
         # wfs = [wftools.read_wf(copy.deepcopy(wf), a) for a in anchors]
         wfs.append(wf)
         optimize_ortho.optimize_orthogonal(wfs, configs, acc, **linemin_kws)
 
 
-def generate_accumulators(mol, mf, energy=True, rdm1=False, extra_accumulators=None):
+def generate_accumulators(
+    mol, mf, energy=True, rdm1=False, extra_accumulators=None, twist=0
+):
     acc = {} if extra_accumulators is None else extra_accumulators
 
     if hasattr(mf, "kpts") and len(mf.mo_coeff[0][0].shape) < 2:
         mo_coeff = [mf.mo_coeff, mf.mo_coeff]
     elif hasattr(mf.mo_coeff, "shape") and len(mf.mo_coeff.shape) == 2:
         mo_coeff = [mf.mo_coeff, mf.mo_coeff]
     else:
@@ -87,18 +89,22 @@
 
     if energy:
         if "energy" in acc.keys():
             raise Exception("Found energy in extra_accumulators and energy is True")
         acc["energy"] = pyqmc.accumulators.EnergyAccumulator(mol)
     if rdm1:
         if hasattr(mol, "a"):
-            from pyqmc.orbitals import get_k_indices
+            from pyqmc.twists import create_supercell_twists
 
-            kinds = list(set(get_k_indices(mol, mf, supercell.get_supercell_kpts(mol))))
+            kinds = create_supercell_twists(mol, mf)["primitive_ks"][twist]
             kpts = mf.kpts[kinds]
+            mo_coeff = [
+                [mo_coeff[0][k] for k in kinds],
+                [mo_coeff[1][k] for k in kinds],
+            ]
         else:
             kpts = None
 
         if "rdm1_up" in acc.keys() or "rdm1_down" in acc.keys():
             raise Exception(
                 "Found rdm1_up or rdm1_down in extra_accumulators and rdm1 is True"
             )
@@ -180,19 +186,16 @@
     nodal_cutoff=1e-3,
 ):
     if ci_checkfile is None:
         mol, mf = pyscftools.recover_pyscf(dft_checkfile)
         mc = None
     else:
         mol, mf, mc = pyscftools.recover_pyscf(dft_checkfile, ci_checkfile=ci_checkfile)
-        if not hasattr(mc.ci, "shape"):
+        if not hasattr(mc.ci, "shape") or len(mc.ci.shape) == 3:
             mc.ci = mc.ci[target_root]
-        elif mc.orbitals is None:
-            mc.orbitals = np.arange(mc.ncore, mc.ncore + mc.ncas)
-            print("Warning: 'orbitals' not found in mc object; using default")
 
     if S is not None:
         mol = supercell.get_supercell(mol, np.asarray(S))
 
     wf, to_opt = wftools.generate_wf(
         mol, mf, mc=mc, jastrow_kws=jastrow_kws, slater_kws=slater_kws
     )
@@ -203,15 +206,19 @@
     if opt_wf:
         acc = pyqmc.accumulators.gradient_generator(
             mol, wf, to_opt, nodal_cutoff=nodal_cutoff
         )
     else:
         if accumulators == None:
             accumulators = {}
-        acc = generate_accumulators(mol, mf, **accumulators)
+        if slater_kws is not None and "twist" in slater_kws.keys():
+            twist = slater_kws["twist"]
+        else:
+            twist = 0
+        acc = generate_accumulators(mol, mf, twist=twist, **accumulators)
 
     return wf, configs, acc
 
 
 def read_opt(fname):
     with h5py.File(fname) as f:
         return pd.DataFrame(
```

### Comparing `pyqmc-0.5.1/pyqmc/slater.py` & `pyqmc-0.6.0/pyqmc/slater.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     inv_ratio = inv[:, :, :, e] / ratio[:, :, np.newaxis]
     invnew = inv - np.einsum("kdi,kdj->kdij", inv_ratio, tmp)
     invnew[:, :, :, e] = inv_ratio
     return ratio, invnew
 
 
 class Slater:
-    """
+    r"""
     A multi-determinant wave function object initialized
     via an SCF calculation.
 
     How to use with hci
 
     .. code-block:: python
 
@@ -92,16 +92,52 @@
         cisolver.select_cutoff=0.1
         nmo = mf.mo_coeff.shape[1]
         nelec = mol.nelec
         h1 = mf.mo_coeff.T.dot(mf.get_hcore()).dot(mf.mo_coeff)
         h2 = pyscf.ao2mo.full(mol, mf.mo_coeff)
         e, civec = cisolver.kernel(h1, h2, nmo, nelec, verbose=4)
         cisolver.ci = civec[0]
-        wf = pyqmc.multislater.MultiSlater(mol, mf, cisolver, tol=0.1)
+        wf = pyqmc.slater.Slater(mol, mf, cisolver, tol=0.1)
+
+    How to use with CASCI/CASSCF
+
+    .. code-block:: python
+
+        cell, mf = pyq.recover_pyscf(scf_checkfile, cancel_outputs=False)
+        mc = mcscf.CASCI(mf, 2, 2)
+        mc.kernel()
+        wf = pyqmc.slater.Slater(mol, mf, mc, tol=0.1)
+
+    To use saved results, attributes of CASCI/CASSCF objects need to be saved
+
+    .. code-block:: python
+
+        cell, mf = pyq.recover_pyscf(scf_checkfile, cancel_outputs=False)
 
+        mc = mcscf.CASCI(mf, 2, 2)
+        mc.kernel()
+        with h5py.File(casci_checkfile, "a") as f:
+            f.create_group("ci")
+            f["ci/nelecas"] = list(mc.nelecas)
+            f["ci/ci"] = mc.ci
+            f["ci/ncas"] = mc.ncas
+            f["ci/mo_coeff"] = mc.mo_coeff
+
+        mc = mcscf.CASSCF(mf, 2, 2)
+        mc.chkfile = casscf_checkfile # only CASSCF saves results
+        mc.kernel()
+        with h5py.File(casscf_checkfile, "a") as f:
+            f["mcscf/nelecas"] = list(mc.nelecas)
+            f["mcscf/ci"] = mc.ci
+
+    Note that when using CASCI/CASSCF, the ``mc`` object needs to have these four attributes: 
+        * ``nelecas``: list of 2 ints
+        * ``ci``: :math:`(N_{\rm det}, N_{\rm det})` matrix of ci coefficients 
+        * ``ncas``: int
+        * ``mo_coeff``: :math:`(N_{\rm AO}, N_{\rm AO})` array
 
     """
 
     def __init__(self, mol, mf, mc=None, tol=None, twist=None, determinants=None):
         """
         determinants should be a list of tuples, for example
         [ (1.0, [0,1],[0,1]),
@@ -110,15 +146,15 @@
 
         determinants overrides any information in mc, if passed.
         """
         self.tol = -1 if tol is None else tol
         self._mol = mol
         if hasattr(mc, "nelecas"):
             # In case nelecas overrode the information from the molecule object.
-            ncore = mc.ncore 
+            ncore = mc.ncore
             if not hasattr(ncore, "__len__"):
                 ncore = [ncore, ncore]
             self._nelec = (mc.nelecas[0] + ncore[0], mc.nelecas[1] + ncore[1])
         else:
             self._nelec = mol.nelec
 
         self.myparameters = {}
@@ -129,19 +165,19 @@
             self.orbitals,
         ) = pyqmc.orbitals.choose_evaluator_from_pyscf(
             mol, mf, mc, twist=twist, determinants=determinants, tol=self.tol
         )
 
         self.parameters = JoinParameters([self.myparameters, self.orbitals.parameters])
 
-        self.iscomplex = self.orbitals.iscomplex or bool(
+        iscomplex = self.orbitals.mo_dtype == complex or bool(
             sum(map(gpu.cp.iscomplexobj, self.parameters.values()))
         )
-        self.dtype = complex if self.iscomplex else float
-        self.get_phase = get_complex_phase if self.iscomplex else gpu.cp.sign
+        self.dtype = complex if iscomplex else float
+        self.get_phase = get_complex_phase if iscomplex else gpu.cp.sign
 
     def recompute(self, configs):
         """This computes the value from scratch. Returns the logarithm of the wave function as
         (phase,logdet). If the wf is real, phase will be +/- 1."""
 
         nconf, nelec, ndim = configs.configs.shape
         aos = self.orbitals.aos("GTOval_sph", configs)
```

### Comparing `pyqmc-0.5.1/pyqmc/supercell.py` & `pyqmc-0.6.0/pyqmc/supercell.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     """
     import pyscf.pbc
 
     scale = np.abs(int(np.round(np.linalg.det(S))))
     superlattice = np.dot(S, cell.lattice_vectors())
     Rpts = get_supercell_copies(cell.lattice_vectors(), S)
     atom = []
-    for (name, xyz) in cell._atom:
+    for name, xyz in cell._atom:
         atom.extend([(name, xyz + R) for R in Rpts])
     supercell = pyscf.pbc.gto.Cell()
     supercell.a = superlattice
     supercell.atom = atom
     supercell.ecp = cell.ecp
     supercell.basis = cell.basis
     supercell.exp_to_discard = cell.exp_to_discard
```

### Comparing `pyqmc-0.5.1/pyqmc/tbdm.py` & `pyqmc-0.6.0/pyqmc/tbdm.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         nsweeps=4,
         tstep=0.50,
         warmup=200,
         naux=None,
         ijkl=None,
         kpts=None,
     ):
-
         self._mol = mol
         self._tstep = tstep
         self._nsweeps = nsweeps
         self._spin = spin
         self._naux = naux
         self._warmup = warmup
 
@@ -77,15 +76,15 @@
                 mol = supercell.get_supercell(mol, np.eye(3))
             self.orbitals = pyqmc.orbitals.PBCOrbitalEvaluatorKpoints(
                 mol, orb_coeff, kpts
             )
             norb_up = np.sum([o.shape[1] for o in orb_coeff[0]])
             norb_down = np.sum([o.shape[1] for o in orb_coeff[1]])
 
-        self.dtype = complex if self.orbitals.iscomplex else float
+        self.dtype = self.orbitals.mo_dtype
         self._spin_sector = spin
         self._electrons = [
             np.arange(spin[s] * mol.nelec[0], mol.nelec[0] + spin[s] * mol.nelec[1])
             for s in [0, 1]
         ]
 
         # Default to full 2rdm if ijkl not specified
```

### Comparing `pyqmc-0.5.1/pyqmc/testwf.py` & `pyqmc-0.6.0/pyqmc/testwf.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,38 +11,40 @@
         mask = np.random.randint(0, 2, num_e).astype(bool)
     ratio, _ = wf.testvalue(e, epos, mask)
     ratio_ref = wf.testvalue(e, epos)[0][mask]
     error = np.abs((ratio - ratio_ref) / np.abs(np.max(ratio)))
     assert np.all(error < tolerance)
     print("testcase for test_value() with mask passed")
 
-def test_testvalue_many(wf,configs,tol=1e-6):
+
+def test_testvalue_many(wf, configs, tol=1e-6):
     """
     :parameter wf: a wave function object to be tested
     :parameter configs: electron positions
     :type configs: (nconf, nelec, 3) array
     :returns: max abs errors
     :rtype: dictionary
 
     """
     nconf, ne, ndim = configs.configs.shape
     val1 = wf.recompute(configs)
     wfcopy = copy.copy(wf)
 
-    delta=1e-2
-    tval = np.zeros((nconf,ne))
+    delta = 1e-2
+    tval = np.zeros((nconf, ne))
     epos = configs.make_irreducible(0, configs.configs[:, 0, :] + delta)
     for e in range(ne):
-        tval[:,e], savedvals = wf.testvalue(e, epos)
-    
+        tval[:, e], savedvals = wf.testvalue(e, epos)
+
     e_all = np.arange(ne)
 
-    tmany= wfcopy.testvalue_many(e_all,epos)
-    terr=tmany-tval
-    assert np.max(np.abs(terr))<tol
+    tmany = wfcopy.testvalue_many(e_all, epos)
+    terr = tmany - tval
+    assert np.max(np.abs(terr)) < tol
+
 
 def test_updateinternals(wf, configs):
     """
     :parameter wf: a wave function object to be tested
     :parameter configs: electron positions
     :type configs: (nconf, nelec, 3) array
     :returns: max abs errors
@@ -50,18 +52,17 @@
 
     """
     import pyqmc.mc as mc
 
     nconf, ne, ndim = configs.configs.shape
     delta = 1e-2
 
-    iscomplex = 1j if wf.iscomplex else 1
-    updatevstest = np.zeros((ne, nconf)) * iscomplex
-    recomputevstest = np.zeros((ne, nconf)) * iscomplex
-    recomputevsupdate = np.zeros((ne, nconf)) * iscomplex
+    updatevstest = np.zeros((ne, nconf), dtype=wf.dtype)
+    recomputevstest = np.zeros((ne, nconf), dtype=wf.dtype)
+    recomputevsupdate = np.zeros((ne, nconf), dtype=wf.dtype)
     wfcopy = copy.copy(wf)
     val1 = wf.recompute(configs)
     for e in range(ne):
         print("#### Electron", e)
         # val1 = wf.recompute(configs)
         epos = configs.make_irreducible(e, configs.configs[:, e, :] + delta)
         ratio, savedvals = wf.testvalue(e, epos)
@@ -114,19 +115,18 @@
     wf.testvalue(e,epos) should return a ratio: the wf value at the position where electron e is moved to epos divided by the current value
     wf.gradient(e,epos) should return grad ln Psi(epos), while keeping all the other electrons at current position. epos may be different from the current position of electron e
 
     :returns: max abs errors
     :rtype: dictionary
     """
     nconf, nelec = configs.configs.shape[0:2]
-    iscomplex = 1j if wf.iscomplex else 1
     wf.recompute(configs)
     maxerror = 0
-    grad = np.zeros(configs.configs.shape) * iscomplex
-    numeric = np.zeros(configs.configs.shape) * iscomplex
+    grad = np.zeros(configs.configs.shape, dtype=wf.dtype)
+    numeric = np.zeros(configs.configs.shape, dtype=wf.dtype)
     for e in range(nelec):
         grad[:, e, :] = wf.gradient(e, configs.electron(e)).T
         for d in range(0, 3):
             epos = configs.make_irreducible(
                 e, configs.configs[:, e, :] + delta * np.eye(3)[d]
             )
             plusval, _ = wf.testvalue(e, epos)
@@ -136,23 +136,22 @@
             minuval, _ = wf.testvalue(e, epos)
             numeric[:, e, d] = (plusval - minuval) / (2 * delta)
     maxerror = np.amax(np.abs(grad - numeric))
     return maxerror
 
 
 def test_wf_pgradient(wf, configs, delta=1e-5):
-    dtype = complex if wf.iscomplex else float
     baseval = wf.recompute(configs)
     gradient = wf.pgradient()
     error = {}
     for k in gradient.keys():  # We only check the gradients that are exposed.
         flt = wf.parameters[k].reshape(-1)
         # print(flt.shape,wf.parameters[k].shape,gradient[k].shape)
         nparms = len(flt)
-        numgrad = np.zeros((configs.configs.shape[0], nparms), dtype=dtype)
+        numgrad = np.zeros((configs.configs.shape[0], nparms), dtype=wf.dtype)
         for i, c in enumerate(flt):
             flt[i] += delta
             wf.parameters[k] = flt.reshape(wf.parameters[k].shape)
             plusval = wf.recompute(configs)
             flt[i] -= 2 * delta
             wf.parameters[k] = flt.reshape(wf.parameters[k].shape)
             minuval = wf.recompute(configs)
@@ -187,19 +186,18 @@
     wf.gradient(e,epos) should return grad ln Psi(epos), while keeping all the other electrons at current position. epos may be different from the current position of electron e
     wf.laplacian(e,epos) should behave the same as gradient, except lap(Psi(epos))/Psi(epos)
 
     :returns: max abs errors
     :rtype: dictionary
     """
     nconf, nelec = configs.configs.shape[0:2]
-    iscomplex = 1j if wf.iscomplex else 1
     wf.recompute(configs)
     maxerror = 0
-    lap = np.zeros(configs.configs.shape[:2]) * iscomplex
-    numeric = np.zeros(configs.configs.shape[:2]) * iscomplex
+    lap = np.zeros(configs.configs.shape[:2], dtype=wf.dtype)
+    numeric = np.zeros(configs.configs.shape[:2], dtype=wf.dtype)
 
     for e in range(nelec):
         lap[:, e] = wf.laplacian(e, configs.electron(e))
 
         for d in range(3):
             epos = configs.make_irreducible(
                 e, configs.configs[:, e, :] + delta * np.eye(3)[d]
@@ -215,21 +213,20 @@
 
     maxerror = np.amax(np.abs(lap - numeric))
     return maxerror
 
 
 def test_wf_gradient_laplacian(wf, configs):
     nconf, nelec = configs.configs.shape[0:2]
-    iscomplex = 1j if wf.iscomplex else 1
     wf.recompute(configs)
     maxerror = 0
-    lap = np.zeros(configs.configs.shape[:2]) * iscomplex
-    grad = np.zeros(configs.configs.shape).transpose((1, 2, 0)) * iscomplex
-    andlap = np.zeros(configs.configs.shape[:2]) * iscomplex
-    andgrad = np.zeros(configs.configs.shape).transpose((1, 2, 0)) * iscomplex
+    lap = np.zeros(configs.configs.shape[:2], dtype=wf.dtype)
+    grad = np.zeros(configs.configs.shape, dtype=wf.dtype).transpose((1, 2, 0))
+    andlap = np.zeros(configs.configs.shape[:2], dtype=wf.dtype)
+    andgrad = np.zeros(configs.configs.shape, dtype=wf.dtype).transpose((1, 2, 0))
 
     tsep = 0
     ttog = 0
     for e in range(nelec):
         ts0 = time.perf_counter()
         lap[:, e] = wf.laplacian(e, configs.electron(e))
         grad[e] = wf.gradient(e, configs.electron(e))
@@ -256,22 +253,21 @@
     else:
         a = [compare_nested_saved_vals(s1, s2) for s1, s2 in zip(saved1, saved2)]
         return np.amax(np.abs(a))
 
 
 def test_wf_gradient_value(wf, configs):
     nconf, nelec = configs.configs.shape[0:2]
-    iscomplex = 1j if wf.iscomplex else 1
     wf.recompute(configs)
     maxerror = 0
-    val = np.zeros(configs.configs.shape[:2]) * iscomplex
-    grad = np.zeros(configs.configs.shape).transpose((1, 2, 0)) * iscomplex
-    andval = np.zeros(configs.configs.shape[:2]) * iscomplex
-    andgrad = np.zeros(configs.configs.shape).transpose((1, 2, 0)) * iscomplex
-    saved_diff = np.zeros(configs.configs.shape[0])
+    val = np.zeros(configs.configs.shape[:2], dtype=wf.dtype)
+    grad = np.zeros(configs.configs.shape, dtype=wf.dtype).transpose((1, 2, 0))
+    andval = np.zeros(configs.configs.shape[:2], dtype=wf.dtype)
+    andgrad = np.zeros(configs.configs.shape, dtype=wf.dtype).transpose((1, 2, 0))
+    saved_diff = np.zeros(configs.configs.shape[0], dtype=wf.dtype)
 
     tsep = 0
     ttog = 0
     for e in range(nelec):
         ts0 = time.perf_counter()
         val[:, e], savedv = wf.testvalue(e, configs.electron(e))
         grad[e] = wf.gradient(e, configs.electron(e))
```

### Comparing `pyqmc-0.5.1/pyqmc/wftools.py` & `pyqmc-0.6.0/pyqmc/wftools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pyqmc import three_body_jastrow
 import pyqmc.slater as slater
 import pyqmc.multiplywf as multiplywf
 import pyqmc.addwf as addwf
 import pyqmc.jastrowspin as jastrowspin
 import pyqmc.func3d as func3d
 import pyqmc.gpu as gpu
 import numpy as np
@@ -102,14 +103,21 @@
     if len(ion_cusp) > 0:
         to_opt["acoeff"][:, 0, :] = False  # Cusp conditions
     to_opt["bcoeff"] = np.ones(jastrow.parameters["bcoeff"].shape).astype(bool)
     to_opt["bcoeff"][0, [0, 1, 2]] = False  # Cusp conditions
     return jastrow, to_opt
 
 
+def generate_jastrow3(mol, na=4, nb=3, rcut=None):
+    abasis, bbasis = default_jastrow_basis(mol, False, na, nb, rcut)
+    wf = three_body_jastrow.ThreeBodyJastrow(mol, abasis, bbasis)
+    to_opt = {"ccoeff": np.ones(wf.parameters["ccoeff"].shape).astype(bool)}
+    return wf, to_opt
+
+
 def generate_sj(mol, mf, optimize_orbitals=False, twist=None, **jastrow_kws):
     wf1, to_opt1 = generate_slater(mol, mf, optimize_orbitals, twist)
     wf2, to_opt2 = generate_jastrow(mol, **jastrow_kws)
     wf = multiplywf.MultiplyWF(wf1, wf2)
     to_opt = {"wf1" + x: opt for x, opt in to_opt1.items()}
     to_opt.update({"wf2" + x: opt for x, opt in to_opt2.items()})
```

### Comparing `pyqmc-0.5.1/pyqmc.egg-info/PKG-INFO` & `pyqmc-0.6.0/pyqmc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqmc
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python library for real space quantum Monte Carlo
 Home-page: https://github.com/WagnerGroup/pyqmc
 Maintainer: Lucas Wagner
 Maintainer-email: lkwagner@illinois.edu
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyqmc-0.5.1/setup.py` & `pyqmc-0.6.0/setup.py`

 * *Files identical despite different names*

