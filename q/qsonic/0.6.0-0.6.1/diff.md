# Comparing `tmp/qsonic-0.6.0.tar.gz` & `tmp/qsonic-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsonic-0.6.0.tar", last modified: Fri May 12 19:16:25 2023, max compression
+gzip compressed data, was "qsonic-0.6.1.tar", last modified: Wed May 17 21:41:20 2023, max compression
```

## Comparing `qsonic-0.6.0.tar` & `qsonic-0.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:16:25.790731 qsonic-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 19:16:07.000000 qsonic-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-12 19:16:25.790731 qsonic-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-12 19:16:07.000000 qsonic-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:16:25.786731 qsonic-0.6.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:16:25.786731 qsonic-0.6.0/py/qsonic/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49789 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/picca_continuum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:16:25.790731 qsonic-0.6.0/py/qsonic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/scripts/qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/scripts/qsonic_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:16:25.790731 qsonic-0.6.0/py/qsonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-12 19:16:25.000000 qsonic-0.6.0/py/qsonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-12 19:16:25.000000 qsonic-0.6.0/py/qsonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:16:25.000000 qsonic-0.6.0/py/qsonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-12 19:16:25.000000 qsonic-0.6.0/py/qsonic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-12 19:16:25.000000 qsonic-0.6.0/py/qsonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 19:16:25.000000 qsonic-0.6.0/py/qsonic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 19:16:07.000000 qsonic-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 19:16:07.000000 qsonic-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-12 19:16:25.790731 qsonic-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:16:07.000000 qsonic-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:16:25.790731 qsonic-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_picca_continuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:41:20.536775 qsonic-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 21:41:07.000000 qsonic-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-17 21:41:20.536775 qsonic-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-17 21:41:07.000000 qsonic-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:41:20.532775 qsonic-0.6.1/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:41:20.536775 qsonic-0.6.1/py/qsonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49929 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/picca_continuum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:41:20.536775 qsonic-0.6.1/py/qsonic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/scripts/qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/scripts/qsonic_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25509 2023-05-17 21:41:07.000000 qsonic-0.6.1/py/qsonic/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:41:20.536775 qsonic-0.6.1/py/qsonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-17 21:41:20.000000 qsonic-0.6.1/py/qsonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-17 21:41:20.000000 qsonic-0.6.1/py/qsonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:41:20.000000 qsonic-0.6.1/py/qsonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-17 21:41:20.000000 qsonic-0.6.1/py/qsonic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-17 21:41:20.000000 qsonic-0.6.1/py/qsonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 21:41:20.000000 qsonic-0.6.1/py/qsonic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 21:41:07.000000 qsonic-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-17 21:41:07.000000 qsonic-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-17 21:41:20.536775 qsonic-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:41:07.000000 qsonic-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:41:20.536775 qsonic-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_picca_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-17 21:41:07.000000 qsonic-0.6.1/tests/test_spectrum.py
```

### Comparing `qsonic-0.6.0/LICENSE` & `qsonic-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/PKG-INFO` & `qsonic-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.6.0
+Version: 0.6.1
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
```

### Comparing `qsonic-0.6.0/README.rst` & `qsonic-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/py/qsonic/calibration.py` & `qsonic-0.6.1/py/qsonic/calibration.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/py/qsonic/catalog.py` & `qsonic-0.6.1/py/qsonic/catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/py/qsonic/io.py` & `qsonic-0.6.1/py/qsonic/io.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/py/qsonic/masks.py` & `qsonic-0.6.1/py/qsonic/masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/py/qsonic/mathtools.py` & `qsonic-0.6.1/py/qsonic/mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/py/qsonic/mpi_utils.py` & `qsonic-0.6.1/py/qsonic/mpi_utils.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/py/qsonic/picca_continuum.py` & `qsonic-0.6.1/py/qsonic/picca_continuum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Continuum fitting module."""
 import argparse
 
 import numpy as np
+from numba import njit
 import fitsio
 from iminuit import Minuit
 from scipy.optimize import minimize, curve_fit
 from scipy.interpolate import UnivariateSpline
 from scipy.special import legendre
 
 from mpi4py import MPI
@@ -773,14 +774,29 @@
             fts = fitsio.FITS(
                 f"{self.outdir}/continuum_chi2_catalog.fits", 'rw',
                 clobber=True)
             fts.write(all_catalog, extname='CHI2_CAT')
             fts.close()
 
 
+@njit("f8[:, :](i8[:], f8[:], f8[:], i8)")
+def _fast_weighted_vector_bincount(x, delta, var, minlength):
+    xvec = np.zeros((4, minlength), dtype=np.float_)
+    y = delta**2
+    y2 = y**2
+
+    for i in range(x.size):
+        xvec[0, x[i]] += delta[i]
+        xvec[1, x[i]] += y[i]
+        xvec[2, x[i]] += y2[i]
+        xvec[3, x[i]] += var[i]
+
+    return xvec
+
+
 class VarLSSFitter():
     """ Variance fitter for the large-scale fluctuations.
 
     Input wavelengths and variances are the bin edges, so centers will be
     shifted. Valid bins require at least 500 pixels from 50 quasars. Assumes no
     spectra has `wave < w1obs` or `wave > w2obs`.
 
@@ -964,20 +980,16 @@
         all_indx = ivar_indx + wave_indx * (self.nvarbins + 2)
         var = np.zeros_like(ivar)
         w = ivar > 0
         var[w] = 1. / ivar[w]
 
         npix = np.bincount(all_indx, minlength=self.minlength)
         self._num_pixels += npix
-        xvec = np.array([
-            np.bincount(all_indx, weights=delta, minlength=self.minlength),
-            np.bincount(all_indx, weights=delta**2, minlength=self.minlength),
-            np.bincount(all_indx, weights=delta**4, minlength=self.minlength),
-            np.bincount(all_indx, weights=var, minlength=self.minlength)
-        ])
+        xvec = _fast_weighted_vector_bincount(
+            all_indx, delta, var, self.minlength)
         self.subsampler.add_measurement(xvec, npix)
 
         npix[npix > 0] = 1
         self._num_qso += npix
 
     def _allreduce(self):
         """ Sums statistics from all MPI process in place."""
```

### Comparing `qsonic-0.6.0/py/qsonic/scripts/qsonic_calib.py` & `qsonic-0.6.1/py/qsonic/scripts/qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/py/qsonic/scripts/qsonic_fit.py` & `qsonic-0.6.1/py/qsonic/scripts/qsonic_fit.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/py/qsonic/spectrum.py` & `qsonic-0.6.1/py/qsonic/spectrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,14 +423,16 @@
 
         for arm, reso_arm in self.forestreso.items():
             weight = self.forestweight[arm].copy()
             weight[weight == 0] = 1e-8
 
             reso_arm = self.forestreso[arm]
             ddia = max_ndia - reso_arm.shape[0]
+            # Assumption ddia cannot be odd
+            ddia = ddia // 2
             if ddia > 0:
                 reso_arm = np.pad(reso_arm, ((ddia, ddia), (0, 0)))
 
             coadd_reso[:, idxes[arm]] += weight * reso_arm
             creso_norm[idxes[arm]] += weight
 
         coadd_reso /= creso_norm
@@ -489,26 +491,25 @@
         coadd_flux[w] /= coadd_norm[w]
         coadd_ivar[w] = coadd_norm[w]**2 / coadd_ivar[w]
 
         self._forestwave = {'brz': coadd_wave}
         self._forestflux = {'brz': coadd_flux}
         self._forestivar = {'brz': coadd_ivar}
         self.cont_params['cont'] = {'brz': coadd_cont}
+        if self.forestreso:
+            self._coadd_arms_reso(nwaves, idxes)
 
         self.set_smooth_ivar(self._smoothing_scale)
         self._forestweight = {}
         self.set_forest_weight(varlss_interp, eta_interp)
 
         mean_snr = np.dot(
             np.sqrt(coadd_ivar), coadd_flux) / np.sum(coadd_ivar > 0)
         self.mean_snr = {'brz': mean_snr}
 
-        if self.forestreso:
-            self._coadd_arms_reso(nwaves, idxes)
-
     def mean_resolution(self, arm, weight=None):
         """ Returns the weighted mean Gaussian sigma of the spectrograph
         resolution.
 
         Arguments
         ---------
         arm: str
```

### Comparing `qsonic-0.6.0/py/qsonic.egg-info/PKG-INFO` & `qsonic-0.6.1/py/qsonic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.6.0
+Version: 0.6.1
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
```

### Comparing `qsonic-0.6.0/py/qsonic.egg-info/SOURCES.txt` & `qsonic-0.6.1/py/qsonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/setup.cfg` & `qsonic-0.6.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.6.0
+current_version = 0.6.1
 commit = True
 tag = True
 
 [bumpversion:file:py/qsonic/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
```

### Comparing `qsonic-0.6.0/tests/test_catalog.py` & `qsonic-0.6.1/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/tests/test_io.py` & `qsonic-0.6.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/tests/test_masks.py` & `qsonic-0.6.1/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/tests/test_mathtools.py` & `qsonic-0.6.1/tests/test_mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/tests/test_mpi_utils.py` & `qsonic-0.6.1/tests/test_mpi_utils.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/tests/test_picca_continuum.py` & `qsonic-0.6.1/tests/test_picca_continuum.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/tests/test_qsonic_calib.py` & `qsonic-0.6.1/tests/test_qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.0/tests/test_spectrum.py` & `qsonic-0.6.1/tests/test_spectrum.py`

 * *Files identical despite different names*

