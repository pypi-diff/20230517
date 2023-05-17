# Comparing `tmp/tad_dftd3-0.1.0.tar.gz` & `tmp/tad_dftd3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_dftd3-0.1.0.tar", last modified: Mon Jan 16 12:32:47 2023, max compression
+gzip compressed data, was "tad_dftd3-0.1.1.tar", last modified: Wed May 17 06:06:17 2023, max compression
```

## Comparing `tad_dftd3-0.1.0.tar` & `tad_dftd3-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-01-16 12:32:47.987167 tad_dftd3-0.1.0/
--rw-rw-r--   0 friede    (1000) friede    (1000)    11358 2022-11-18 09:32:35.000000 tad_dftd3-0.1.0/LICENSE
--rw-rw-r--   0 friede    (1000) friede    (1000)    10108 2023-01-16 12:32:47.987167 tad_dftd3-0.1.0/PKG-INFO
--rw-rw-r--   0 friede    (1000) friede    (1000)     9320 2023-01-16 12:09:34.000000 tad_dftd3-0.1.0/README.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)      623 2023-01-16 12:09:34.000000 tad_dftd3-0.1.0/pyproject.toml
--rw-rw-r--   0 friede    (1000) friede    (1000)     1095 2023-01-16 12:32:47.987167 tad_dftd3-0.1.0/setup.cfg
--rw-rw-r--   0 friede    (1000) friede    (1000)       69 2023-01-16 12:09:34.000000 tad_dftd3-0.1.0/setup.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-01-16 12:32:47.983167 tad_dftd3-0.1.0/src/
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-01-16 12:32:47.983167 tad_dftd3-0.1.0/src/tad_dftd3/
--rw-rw-r--   0 friede    (1000) friede    (1000)     5802 2023-01-13 15:56:16.000000 tad_dftd3-0.1.0/src/tad_dftd3/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)      842 2022-11-18 09:32:35.000000 tad_dftd3-0.1.0/src/tad_dftd3/constants.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-01-16 12:32:47.987167 tad_dftd3-0.1.0/src/tad_dftd3/damping/
--rw-rw-r--   0 friede    (1000) friede    (1000)      180 2023-01-13 15:56:16.000000 tad_dftd3-0.1.0/src/tad_dftd3/damping/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3377 2023-01-13 15:56:16.000000 tad_dftd3-0.1.0/src/tad_dftd3/damping/atm.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1260 2023-01-13 15:56:16.000000 tad_dftd3-0.1.0/src/tad_dftd3/damping/rational.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    75725 2023-01-16 12:09:34.000000 tad_dftd3-0.1.0/src/tad_dftd3/data.py
--rw-rw-r--   0 friede    (1000) friede    (1000)      579 2023-01-13 15:56:16.000000 tad_dftd3-0.1.0/src/tad_dftd3/defaults.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     7352 2023-01-16 12:09:34.000000 tad_dftd3-0.1.0/src/tad_dftd3/disp.py
--rw-rw-r--   0 friede    (1000) friede    (1000)      774 2023-01-13 15:56:16.000000 tad_dftd3-0.1.0/src/tad_dftd3/exception.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3805 2023-01-16 12:09:34.000000 tad_dftd3-0.1.0/src/tad_dftd3/model.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5107 2023-01-16 12:09:34.000000 tad_dftd3-0.1.0/src/tad_dftd3/ncoord.py
--rw-rw-r--   0 friede    (1000) friede    (1000)   893128 2022-11-18 09:32:35.000000 tad_dftd3-0.1.0/src/tad_dftd3/reference-c6.npy
--rw-rw-r--   0 friede    (1000) friede    (1000)    11703 2023-01-16 12:09:34.000000 tad_dftd3-0.1.0/src/tad_dftd3/reference.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1442 2023-01-16 12:09:34.000000 tad_dftd3-0.1.0/src/tad_dftd3/typing.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4894 2023-01-13 15:56:16.000000 tad_dftd3-0.1.0/src/tad_dftd3/util.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-01-16 12:32:47.983167 tad_dftd3-0.1.0/src/tad_dftd3.egg-info/
--rw-rw-r--   0 friede    (1000) friede    (1000)    10108 2023-01-16 12:32:47.000000 tad_dftd3-0.1.0/src/tad_dftd3.egg-info/PKG-INFO
--rw-rw-r--   0 friede    (1000) friede    (1000)      634 2023-01-16 12:32:47.000000 tad_dftd3-0.1.0/src/tad_dftd3.egg-info/SOURCES.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)        1 2023-01-16 12:32:47.000000 tad_dftd3-0.1.0/src/tad_dftd3.egg-info/dependency_links.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)      100 2023-01-16 12:32:47.000000 tad_dftd3-0.1.0/src/tad_dftd3.egg-info/requires.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)       10 2023-01-16 12:32:47.000000 tad_dftd3-0.1.0/src/tad_dftd3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:06:17.512986 tad_dftd3-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-05-17 06:06:17.512986 tad_dftd3-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-17 06:06:17.512986 tad_dftd3-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:06:17.504986 tad_dftd3-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:06:17.508986 tad_dftd3-0.1.1/src/tad_dftd3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:06:17.508986 tad_dftd3-0.1.1/src/tad_dftd3/damping/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/damping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/damping/atm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/damping/rational.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75725 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/ncoord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:06:17.508986 tad_dftd3-0.1.1/src/tad_dftd3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-05-17 06:06:17.000000 tad_dftd3-0.1.1/src/tad_dftd3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-17 06:06:17.000000 tad_dftd3-0.1.1/src/tad_dftd3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 06:06:17.000000 tad_dftd3-0.1.1/src/tad_dftd3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 06:06:17.000000 tad_dftd3-0.1.1/src/tad_dftd3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 06:06:17.000000 tad_dftd3-0.1.1/src/tad_dftd3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:06:17.512986 tad_dftd3-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/tests/test_dftd3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/tests/test_disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/tests/test_ncoord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/tests/test_utils.py
```

### Comparing `tad_dftd3-0.1.0/LICENSE` & `tad_dftd3-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.0/PKG-INFO` & `tad_dftd3-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad_dftd3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Torch autodiff DFT-D3 implementation
 License: Apache-2.0
 Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
 Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -69,14 +69,27 @@
 `dispax <https://github.com/awvwgk/dispax>`__:
   Implementation of the DFT-D3 dispersion model in Jax M.D.
 
 
 Installation
 ------------
 
+pip
+~~~
+
+The project can easily be installed with ``pip``.
+
+.. code::
+
+   pip install tad-dftd3
+
+
+From source
+~~~~~~~~~~~
+
 This project is hosted on GitHub at `dftd3/tad-dftd3 <https://github.com/dftd3/tad-dftd3>`__.
 Obtain the source by cloning the repository with
 
 .. code::
 
    git clone https://github.com/dftd3/tad-dftd3
    cd tad-dftd3
```

### Comparing `tad_dftd3-0.1.0/README.rst` & `tad_dftd3-0.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,27 @@
 `dispax <https://github.com/awvwgk/dispax>`__:
   Implementation of the DFT-D3 dispersion model in Jax M.D.
 
 
 Installation
 ------------
 
+pip
+~~~
+
+The project can easily be installed with ``pip``.
+
+.. code::
+
+   pip install tad-dftd3
+
+
+From source
+~~~~~~~~~~~
+
 This project is hosted on GitHub at `dftd3/tad-dftd3 <https://github.com/dftd3/tad-dftd3>`__.
 Obtain the source by cloning the repository with
 
 .. code::
 
    git clone https://github.com/dftd3/tad-dftd3
    cd tad-dftd3
```

### Comparing `tad_dftd3-0.1.0/pyproject.toml` & `tad_dftd3-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -20,11 +20,10 @@
 warn_unreachable = true
 warn_unused_ignores = false
 
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["./src"]
-omit = ["./src/dxtb/exlibs/*"]
 
 [tool.coverage.report]
 fail_under = 80
```

### Comparing `tad_dftd3-0.1.0/setup.cfg` & `tad_dftd3-0.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tad_dftd3
-version = 0.1.0
+version = 0.1.1
 description = Torch autodiff DFT-D3 implementation
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 license = Apache-2.0
 license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: Apache Software License
```

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3/__init__.py` & `tad_dftd3-0.1.1/src/tad_dftd3/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3/constants.py` & `tad_dftd3-0.1.1/src/tad_dftd3/constants.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3/damping/atm.py` & `tad_dftd3-0.1.1/src/tad_dftd3/damping/atm.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,16 @@
         Exponent of zero damping function. Defaults to `14.0`.
 
     Returns
     -------
     Tensor
         Atom-resolved ATM dispersion energy.
     """
+    dd = {"device": positions.device, "dtype": positions.dtype}
+
     s9 = s9.type(positions.dtype).to(positions.device)
     rs9 = rs9.type(positions.dtype).to(positions.device)
     alp = alp.type(positions.dtype).to(positions.device)
 
     cutoff2 = cutoff * cutoff
     srvdw = rs9 * rvdw
 
@@ -81,15 +83,15 @@
     # very slow: (pos.unsqueeze(-2) - pos.unsqueeze(-3)).pow(2).sum(-1)
     distances = torch.pow(
         torch.where(
             real_pairs(numbers, diagonal=False),
             torch.cdist(
                 positions, positions, p=2, compute_mode="use_mm_for_euclid_dist"
             ),
-            positions.new_tensor(torch.finfo(positions.dtype).eps),
+            torch.tensor(torch.finfo(positions.dtype).eps, **dd),
         ),
         2.0,
     )
 
     r2ij = distances.unsqueeze(-1)
     r2ik = distances.unsqueeze(-2)
     r2jk = distances.unsqueeze(-3)
@@ -103,12 +105,12 @@
     s = (r2ij + r2jk - r2ik) * (r2ij - r2jk + r2ik) * (-r2ij + r2jk + r2ik)
     ang = torch.where(
         real_triples(numbers, diagonal=False)
         * (r2ij <= cutoff2)
         * (r2jk <= cutoff2)
         * (r2jk <= cutoff2),
         0.375 * s / r5 + 1.0 / r3,
-        positions.new_tensor(0.0),
+        torch.tensor(0.0, **dd),
     )
 
     energy = ang * fdamp * c9
     return torch.sum(energy, dim=(-2, -1)) / 6.0
```

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3/damping/rational.py` & `tad_dftd3-0.1.1/src/tad_dftd3/damping/rational.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,10 +39,12 @@
         DFT-D3 damping parameters.
 
     Returns
     -------
     Tensor
         Values of the damping function.
     """
-    a1 = param.get("a1", distances.new_tensor(defaults.A1))
-    a2 = param.get("a2", distances.new_tensor(defaults.A1))
+    dd = {"device": distances.device, "dtype": distances.dtype}
+
+    a1 = param.get("a1", torch.tensor(defaults.A1, **dd))
+    a2 = param.get("a2", torch.tensor(defaults.A2, **dd))
     return 1.0 / (distances.pow(order) + (a1 * torch.sqrt(qq) + a2).pow(order))
```

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3/data.py` & `tad_dftd3-0.1.1/src/tad_dftd3/data.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3/defaults.py` & `tad_dftd3-0.1.1/src/tad_dftd3/defaults.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3/disp.py` & `tad_dftd3-0.1.1/src/tad_dftd3/disp.py`

 * *Files 11% similar despite different names*

```diff
@@ -88,16 +88,18 @@
         Van der Waals radii of the atoms in the system.
     r4r2 : Tensor
         r⁴ over r² expectation values of the atoms in the system.
     damping_function : Callable
         Damping function evaluate distance dependent contributions.
         Additional arguments are passed through to the function.
     """
+    dd = {"device": positions.device, "dtype": positions.dtype}
+
     if cutoff is None:
-        cutoff = positions.new_tensor(50.0)
+        cutoff = torch.tensor(50.0, **dd)
     if r4r2 is None:
         r4r2 = (
             data.sqrt_z_r4_over_r2[numbers].type(positions.dtype).to(positions.device)
         )
     if numbers.shape != positions.shape[:-1]:
         raise ValueError(
             "Shape of positions is not consistent with atomic numbers.",
@@ -151,40 +153,42 @@
         Atomic C6 dispersion coefficients.
     r4r2 : Tensor
         r⁴ over r² expectation values of the atoms in the system.
     damping_function : Callable
         Damping function evaluate distance dependent contributions.
         Additional arguments are passed through to the function.
     """
+    dd = {"device": positions.device, "dtype": positions.dtype}
+
     mask = real_pairs(numbers, diagonal=False)
     distances = torch.where(
         mask,
         torch.cdist(positions, positions, p=2, compute_mode="use_mm_for_euclid_dist"),
-        positions.new_tensor(torch.finfo(positions.dtype).eps),
+        torch.tensor(torch.finfo(positions.dtype).eps, **dd),
     )
 
     qq = 3 * r4r2.unsqueeze(-1) * r4r2.unsqueeze(-2)
     c8 = c6 * qq
 
     t6 = torch.where(
         mask * (distances <= cutoff),
         damping_function(6, distances, qq, param, **kwargs),
-        positions.new_tensor(0.0),
+        torch.tensor(0.0, **dd),
     )
     t8 = torch.where(
         mask * (distances <= cutoff),
         damping_function(8, distances, qq, param, **kwargs),
-        positions.new_tensor(0.0),
+        torch.tensor(0.0, **dd),
     )
 
     e6 = -0.5 * torch.sum(c6 * t6, dim=-1)
     e8 = -0.5 * torch.sum(c8 * t8, dim=-1)
 
-    s6 = param.get("s6", positions.new_tensor(defaults.S6))
-    s8 = param.get("s8", positions.new_tensor(defaults.S8))
+    s6 = param.get("s6", torch.tensor(defaults.S6, **dd))
+    s8 = param.get("s8", torch.tensor(defaults.S8, **dd))
     return s6 * e6 + s8 * e8
 
 
 def dispersion3(
     numbers: Tensor,
     positions: Tensor,
     param: Dict[str, Tensor],
@@ -216,12 +220,14 @@
         Scaling for van-der-Waals radii in damping function. Defaults to `4.0/3.0`.
 
     Returns
     -------
     Tensor
         Atom-resolved three-body dispersion energy.
     """
-    alp = param.get("alp", positions.new_tensor(14.0))
-    s9 = param.get("s9", positions.new_tensor(14.0))
+    dd = {"device": positions.device, "dtype": positions.dtype}
+
+    alp = param.get("alp", torch.tensor(14.0, **dd))
+    s9 = param.get("s9", torch.tensor(1.0, **dd))
     rs9 = rs9.type(positions.dtype).to(positions.device)
 
     return dispersion_atm(numbers, positions, c6, rvdw, cutoff, s9, rs9, alp)
```

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3/exception.py` & `tad_dftd3-0.1.1/src/tad_dftd3/exception.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3/model.py` & `tad_dftd3-0.1.1/src/tad_dftd3/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,12 +125,12 @@
     """
 
     mask = reference.cn[numbers] >= 0
 
     weights = torch.where(
         mask,
         weighting_function(reference.cn[numbers] - cn.unsqueeze(-1), **kwargs),
-        cn.new_tensor(0.0),
+        torch.tensor(0.0, device=cn.device, dtype=cn.dtype),
     )
     norms = torch.add(torch.sum(weights, dim=-1), epsilon)
 
     return weights / norms.unsqueeze(-1)
```

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3/ncoord.py` & `tad_dftd3-0.1.1/src/tad_dftd3/ncoord.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,33 +112,34 @@
     cutoff : float
         Real-space cutoff for the evaluation of counting function
 
     Returns
     -------
         Tensor: The coordination number of each atom in the system.
     """
+    dd = {"device": positions.device, "dtype": positions.dtype}
+
     if cutoff is None:
-        cutoff = positions.new_tensor(25.0)
+        cutoff = torch.tensor(25.0, **dd)
     if rcov is None:
         rcov = data.covalent_rad_d3[numbers].type(positions.dtype).to(positions.device)
     if numbers.shape != rcov.shape:
         raise ValueError(
             "Shape of covalent radii is not consistent with atomic numbers"
         )
     if numbers.shape != positions.shape[:-1]:
         raise ValueError("Shape of positions is not consistent with atomic numbers")
 
-    eps = positions.new_tensor(torch.finfo(positions.dtype).eps)
     mask = real_pairs(numbers, diagonal=False)
     distances = torch.where(
         mask,
         torch.cdist(positions, positions, p=2, compute_mode="use_mm_for_euclid_dist"),
-        eps,
+        torch.tensor(torch.finfo(positions.dtype).eps, **dd),
     )
 
     rc = rcov.unsqueeze(-2) + rcov.unsqueeze(-1)
     cf = torch.where(
         mask * (distances <= cutoff),
         counting_function(distances, rc.type(distances.dtype), **kwargs),
-        positions.new_tensor(0.0),
+        torch.tensor(0.0, **dd),
     )
     return torch.sum(cf, dim=-1)
```

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3/reference.py` & `tad_dftd3-0.1.1/src/tad_dftd3/reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,14 @@
     ]
 
     def __init__(
         self,
         cn: Optional[Tensor] = None,
         c6: Optional[Tensor] = None,
     ):
-
         if cn is None:
             cn = _load_cn()
         self.cn = cn
         if c6 is None:
             c6 = _load_c6()
         self.c6 = c6
```

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3/typing.py` & `tad_dftd3-0.1.1/src/tad_dftd3/typing.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3/util.py` & `tad_dftd3-0.1.1/src/tad_dftd3/util.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.0/src/tad_dftd3.egg-info/PKG-INFO` & `tad_dftd3-0.1.1/src/tad_dftd3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad-dftd3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Torch autodiff DFT-D3 implementation
 License: Apache-2.0
 Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
 Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -69,14 +69,27 @@
 `dispax <https://github.com/awvwgk/dispax>`__:
   Implementation of the DFT-D3 dispersion model in Jax M.D.
 
 
 Installation
 ------------
 
+pip
+~~~
+
+The project can easily be installed with ``pip``.
+
+.. code::
+
+   pip install tad-dftd3
+
+
+From source
+~~~~~~~~~~~
+
 This project is hosted on GitHub at `dftd3/tad-dftd3 <https://github.com/dftd3/tad-dftd3>`__.
 Obtain the source by cloning the repository with
 
 .. code::
 
    git clone https://github.com/dftd3/tad-dftd3
    cd tad-dftd3
```

