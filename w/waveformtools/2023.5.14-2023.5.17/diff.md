# Comparing `tmp/waveformtools-2023.5.14.tar.gz` & `tmp/waveformtools-2023.5.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveformtools-2023.5.14.tar", last modified: Mon May 15 05:06:51 2023, max compression
+gzip compressed data, was "waveformtools-2023.5.17.tar", last modified: Wed May 17 09:12:41 2023, max compression
```

## Comparing `waveformtools-2023.5.14.tar` & `waveformtools-2023.5.17.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 vaishakp  (1000) vaishakp  (1000)        0 2023-05-15 05:06:51.786130 waveformtools-2023.5.14/
--rwxrwxrwx   0 vaishakp  (1000) vaishakp  (1000)     1075 2021-03-27 09:49:21.000000 waveformtools-2023.5.14/LICENSE
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)     8561 2023-05-15 05:06:51.786130 waveformtools-2023.5.14/PKG-INFO
--rwxrwxrwx   0 vaishakp  (1000) vaishakp  (1000)      106 2021-07-01 03:03:09.000000 waveformtools-2023.5.14/README
--rwxrwxr-x   0 vaishakp  (1000) vaishakp  (1000)     7905 2023-05-11 16:28:22.000000 waveformtools-2023.5.14/README.md
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)     1090 2023-05-15 05:05:40.000000 waveformtools-2023.5.14/pyproject.toml
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)       38 2023-05-15 05:06:51.786130 waveformtools-2023.5.14/setup.cfg
--rwxrwxr-x   0 vaishakp  (1000) vaishakp  (1000)     1396 2023-05-15 04:58:27.000000 waveformtools-2023.5.14/setup.py
-drwxrwxr-x   0 vaishakp  (1000) vaishakp  (1000)        0 2023-05-15 05:06:51.782129 waveformtools-2023.5.14/waveformtools/
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)     5481 2023-05-11 16:28:22.000000 waveformtools-2023.5.14/waveformtools/BMS.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)     9131 2023-05-11 16:28:22.000000 waveformtools-2023.5.14/waveformtools/CoM.py
--rwxrwxr-x   0 vaishakp  (1000) vaishakp  (1000)     1285 2023-05-15 04:49:32.000000 waveformtools-2023.5.14/waveformtools/__init__.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)    10880 2023-05-15 04:49:32.000000 waveformtools-2023.5.14/waveformtools/compare.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)    52390 2023-05-15 04:49:32.000000 waveformtools-2023.5.14/waveformtools/dataIO.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)     1698 2023-05-11 16:28:22.000000 waveformtools-2023.5.14/waveformtools/diagnostics.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)    25350 2023-05-11 16:28:22.000000 waveformtools-2023.5.14/waveformtools/differentiate.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)     9106 2023-05-11 16:28:22.000000 waveformtools-2023.5.14/waveformtools/extrapolate.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)    14069 2023-05-11 16:28:22.000000 waveformtools-2023.5.14/waveformtools/grids.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)    10954 2023-05-11 16:28:22.000000 waveformtools-2023.5.14/waveformtools/integrate.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)     7204 2023-05-11 16:28:22.000000 waveformtools-2023.5.14/waveformtools/legacy.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)    53840 2023-05-11 16:28:22.000000 waveformtools-2023.5.14/waveformtools/simulations.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)     6478 2023-05-11 16:28:22.000000 waveformtools-2023.5.14/waveformtools/spherical.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)    10920 2023-05-11 16:28:22.000000 waveformtools-2023.5.14/waveformtools/transforms.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)    68396 2023-05-15 04:49:32.000000 waveformtools-2023.5.14/waveformtools/waveforms.py
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)    87949 2023-05-11 17:29:19.000000 waveformtools-2023.5.14/waveformtools/waveformtools.py
-drwxrwxr-x   0 vaishakp  (1000) vaishakp  (1000)        0 2023-05-15 05:06:51.786130 waveformtools-2023.5.14/waveformtools.egg-info/
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)     8561 2023-05-15 05:06:51.000000 waveformtools-2023.5.14/waveformtools.egg-info/PKG-INFO
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)      654 2023-05-15 05:06:51.000000 waveformtools-2023.5.14/waveformtools.egg-info/SOURCES.txt
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)        1 2023-05-15 05:06:51.000000 waveformtools-2023.5.14/waveformtools.egg-info/dependency_links.txt
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)      102 2023-05-15 05:06:51.000000 waveformtools-2023.5.14/waveformtools.egg-info/requires.txt
--rw-rw-r--   0 vaishakp  (1000) vaishakp  (1000)       14 2023-05-15 05:06:51.000000 waveformtools-2023.5.14/waveformtools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:12:41.616490 waveformtools-2023.5.17/
+-rwxrwxrwx   0 root         (0) root         (0)     1075 2023-05-17 09:11:57.000000 waveformtools-2023.5.17/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8708 2023-05-17 09:12:41.615490 waveformtools-2023.5.17/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      106 2023-05-17 09:11:57.000000 waveformtools-2023.5.17/README
+-rwxrwxrwx   0 root         (0) root         (0)     8052 2023-05-17 09:11:57.000000 waveformtools-2023.5.17/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 09:12:41.616490 waveformtools-2023.5.17/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1396 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:12:41.613490 waveformtools-2023.5.17/waveformtools/
+-rw-rw-rw-   0 root         (0) root         (0)     5480 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/BMS.py
+-rw-rw-rw-   0 root         (0) root         (0)     9130 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/CoM.py
+-rwxrwxrwx   0 root         (0) root         (0)     1284 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10875 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)    54085 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/dataIO.py
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/diagnostics.py
+-rw-rw-rw-   0 root         (0) root         (0)    25350 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/differentiate.py
+-rw-rw-rw-   0 root         (0) root         (0)     9106 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/extrapolate.py
+-rw-rw-rw-   0 root         (0) root         (0)    14069 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/grids.py
+-rw-rw-rw-   0 root         (0) root         (0)    10952 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     7204 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)    53835 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/simulations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6476 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/spherical.py
+-rw-rw-rw-   0 root         (0) root         (0)    12491 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/transforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    60703 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/waveforms.py
+-rw-rw-rw-   0 root         (0) root         (0)   110367 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/waveformtools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:12:41.615490 waveformtools-2023.5.17/waveformtools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8708 2023-05-17 09:12:41.000000 waveformtools-2023.5.17/waveformtools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-17 09:12:41.000000 waveformtools-2023.5.17/waveformtools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 09:12:41.000000 waveformtools-2023.5.17/waveformtools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-17 09:12:41.000000 waveformtools-2023.5.17/waveformtools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-17 09:12:41.000000 waveformtools-2023.5.17/waveformtools.egg-info/top_level.txt
```

### Comparing `waveformtools-2023.5.14/LICENSE` & `waveformtools-2023.5.17/LICENSE`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.14/PKG-INFO` & `waveformtools-2023.5.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: waveformtools
-Version: 2023.5.14
+Version: 2023.5.17
 Summary:  Tools for working with numerical relativity and waveforms data 
 Home-page: https://gitlab.com/vaishakp/waveformtools
 Author: Vaishak Prasad
 Author-email: Vaishak Prasad <vaishakprasad@gmail.com>
 Project-URL: Homepage, https://gitlab.com/vaishakp/waveformtools
 Project-URL: Bug Tracker, https://gitlab.com/vaishakp/waveformtools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: EXT
 License-File: LICENSE
 
-[![Project landing page](https://sites.google.com/view/waveformtools/home)]
+[[Project landing page]](https://sites.google.com/view/waveformtools/home)
 [![pipeline status](https://gitlab.com/vaishakp/waveformtools/badges/main/pipeline.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/waveformtools/badge/?version=latest)](https://waveformtools.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
+[![PyPI version](https://badge.fury.io/py/waveformtools.svg)](https://badge.fury.io/py/waveformtools)
 # Waveformtools 
 
 
 This is a python module for the handling and analysis of waveforms and data from Numerical Relativity codes, and for carrying out gravitational wave data analysis.  
 
 waveformtools is a numerical relativity data handling package that was written to aid the handling and analysis of numerical relativity data.
 
 This package contains implementations of customized algorithms and techniques.  Some of these contain the usage of existing python based library functions from pycbc, scipy, etc but effort has been made to keep these to a minimum.
 
  
-* Handling of numerical relativity data, and retreiving specific information about the physical system.
+* Handling of numerical relativity data, and retreiving specific information about the physical system. Presently, this supports the EinsteinToolkit data.
 
     The class container and methods "sim" can load NR data into convenient lists and dictionaries, which can be used to     retrieve specific data/ information about the numerical simulation. 
 
     This offers the following functionality, like retreiving:
 
     * Horizon masses, mass-ratios, and areas.
 
@@ -104,16 +104,16 @@
 
 
 
 # Citing this code
 
 Please cite the latest version of this code if used in your work. This code was developed for use in the following works:
 
-1. [`News from Horizons in Binary Black Hole Mergers`](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.125.121101)
-2. ['Tidal deformation of dynamical horizons in binary black hole mergers'](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.105.044019)
+1. [News from Horizons in Binary Black Hole Mergers](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.125.121101)
+2. [Tidal deformation of dynamical horizons in binary black hole mergers](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.105.044019)
 
 We request you to also cite these. Thanks!
```

### Comparing `waveformtools-2023.5.14/README.md` & `waveformtools-2023.5.17/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-[![Project landing page](https://sites.google.com/view/waveformtools/home)]
+[[Project landing page]](https://sites.google.com/view/waveformtools/home)
 [![pipeline status](https://gitlab.com/vaishakp/waveformtools/badges/main/pipeline.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/waveformtools/badge/?version=latest)](https://waveformtools.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
+[![PyPI version](https://badge.fury.io/py/waveformtools.svg)](https://badge.fury.io/py/waveformtools)
 # Waveformtools 
 
 
 This is a python module for the handling and analysis of waveforms and data from Numerical Relativity codes, and for carrying out gravitational wave data analysis.  
 
 waveformtools is a numerical relativity data handling package that was written to aid the handling and analysis of numerical relativity data.
 
 This package contains implementations of customized algorithms and techniques.  Some of these contain the usage of existing python based library functions from pycbc, scipy, etc but effort has been made to keep these to a minimum.
 
  
-* Handling of numerical relativity data, and retreiving specific information about the physical system.
+* Handling of numerical relativity data, and retreiving specific information about the physical system. Presently, this supports the EinsteinToolkit data.
 
     The class container and methods "sim" can load NR data into convenient lists and dictionaries, which can be used to     retrieve specific data/ information about the numerical simulation. 
 
     This offers the following functionality, like retreiving:
 
     * Horizon masses, mass-ratios, and areas.
 
@@ -87,16 +87,16 @@
 
 
 
 # Citing this code
 
 Please cite the latest version of this code if used in your work. This code was developed for use in the following works:
 
-1. [`News from Horizons in Binary Black Hole Mergers`](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.125.121101)
-2. ['Tidal deformation of dynamical horizons in binary black hole mergers'](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.105.044019)
+1. [News from Horizons in Binary Black Hole Mergers](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.125.121101)
+2. [Tidal deformation of dynamical horizons in binary black hole mergers](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.105.044019)
 
 We request you to also cite these. Thanks!
```

### Comparing `waveformtools-2023.5.14/pyproject.toml` & `waveformtools-2023.5.17/pyproject.toml`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.14/setup.py` & `waveformtools-2023.5.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # requiremnts directly from toml
 # mreq, oreq = get_requirements()
 
 
 
 setuptools.setup(
     name="waveformtools",
- 	version="2023.05.14",
+ 	version="2023.05.17",
     author="Vaishak Prasad",
     author_email="vaishakprasad@gmail.com",
     description="Functions for handling waveform and numerical relativity data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/vaishakp/waveformtools",
     packages=setuptools.find_packages(),
```

### Comparing `waveformtools-2023.5.14/waveformtools/BMS.py` & `waveformtools-2023.5.17/waveformtools/BMS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ The implementation of BMS transformations on the waveforms. """
 
-
 #############################
 # Imports
 #############################
 
 import numpy as np
 
 from waveformtools.waveformtools import message
```

### Comparing `waveformtools-2023.5.14/waveformtools/CoM.py` & `waveformtools-2023.5.17/waveformtools/CoM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """ Centre of mass correction for the waveforms. """
 
 #################
 # Imports
 #################
 
-
 import numpy as np
 
 
 def X_com_moments(time_axis, Xcom, order):
     """Compute the nth order temporal moment of the COM coordinates.
 
     Parameters
```

### Comparing `waveformtools-2023.5.14/waveformtools/__init__.py` & `waveformtools-2023.5.17/waveformtools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copyright (c) 2020, Vaishak Prasad
 # See [LICENSE](https://gitlab.com/vaishakp/waveformtools/-/blob/main/LICENSE) file for details.
-
 """
 Module for the analysis and handling of numerical relativity and gravitational waveform data.
 
 Classes
 -------
 sim: Base class for NR simulations data.
                 This is needed to retrieve and handle Numerical Relativity data.
@@ -35,8 +34,8 @@
         print("This is not a git repo! please use the version attribute instead!")
     # with open(package_directory + "/../public/date.txt", "r") as vers_file:
     # vers = vers_file.read()[:10]
 
     return vers
 
 
-__version__ = "2023.05.14"
+__version__ = "2023.05.17"
```

### Comparing `waveformtools-2023.5.14/waveformtools/compare.py` & `waveformtools-2023.5.17/waveformtools/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # Plot settings
 fontsize = 16
 labelsize = 16
 labelpad = 14
 
 matplotlib.rcParams.update(matplotlib.rcParamsDefault)
 
-
 # plt.rcParams.update({'font.size': fontsize})
 plt.rcParams.update({"figure.figsize": (8, 6)})
 # plt.rcParams.update({"axes.grid" : True})
 plt.rcParams.update({"axes.labelpad": labelpad})
 plt.rcParams.update({"axes.labelsize": labelsize})
 plt.rcParams.update({"figure.autolayout": True})
 plt.rcParams.update({"grid.alpha": 0.3})
@@ -39,15 +38,15 @@
                               to plot.
     nmodes:     int
                             The number of modes to plot.
     xlim : list
            [xmin, xmax] limits to plot.
     tol:    float
                     The tolerance to detect the modes.
-    
+
     Returns
     -------
     Plots.
     """
 
     from waveformtools.waveformtools import xtract_cphase
```

### Comparing `waveformtools-2023.5.14/waveformtools/dataIO.py` & `waveformtools-2023.5.17/waveformtools/dataIO.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 
 def _key_gen(ell, emm, extras=None):
     """Generates strings to be used as keys for
     managing h5 datasets.
 
     Parameters
     ----------
-    ell:    int
-                    The polar angular mode number
-                    :math:`\\ell`.
+    ell:	int
+                                    The polar angular mode number
+                                    :math:`\\ell`.
     emm : int
-              The aximuthal angular mode number
-              :math:`m`.
+                      The aximuthal angular mode number
+                      :math:`m`.
     extras: str
-                Any extra string to be appended
-                to the end of the key.
+                            Any extra string to be appended
+                            to the end of the key.
 
     Returns
     -------
-    key:     str
-                     A string key.
+    key:	 str
+                                     A string key.
     """
 
     key = f"l{ell}_m{emm}"
 
     if extras is not None:
         key += f"_{extras}"
         # message('adding rext')
@@ -54,20 +54,20 @@
 
 
 def get_ell_max_from_keys(all_keys):
     """Get ell max from a list of keys.
 
     Parameters
     ----------
-    all_keys :  list
-            A list of strings string containing the modes keys.
+    all_keys :	list
+                    A list of strings string containing the modes keys.
     Returns
     -------
     ell_max : int
-              The maximum available ell.
+                      The maximum available ell.
     """
 
     # available mode numbers
     all_ell_modes = set({})
 
     # Get mode numbers
     for item in all_keys:
@@ -89,28 +89,28 @@
 
 
 def get_ell_max_from_file(data_dir, var_type="Psi4", file_name="*.h5"):
     """Get the largest available mode number from available data in files.
 
     Parameters
     ----------
-    data_dir :  string
-                A string containing the directory path where the mode files can be found.
+    data_dir :	string
+                            A string containing the directory path where the mode files can be found.
     var_type: string, optional
-            A string that denotes the variable that is being loaded. Options are Psi4 and strain.
-            The former is the default.
+                    A string that denotes the variable that is being loaded. Options are Psi4 and strain.
+                    The former is the default.
     file_name : string, optional
-              The h5 file that contains the modes data. It defaults to the only file in the directory.
-              If there are multiple files, it throws an error.
+                      The h5 file that contains the modes data. It defaults to the only file in the directory.
+                      If there are multiple files, it throws an error.
     Returns
     -------
     ell_max : int
-              The maximum available ell.
+                      The maximum available ell.
     keys_list : list
-                A list of data access keys.
+                            A list of data access keys.
 
     Notes
     -----
     Reads in various ASCII dat files for RIT Psi4, h5 files for RIT strain and gen strain.
     """
 
     if var_type == "Psi4":
@@ -142,23 +142,23 @@
 
 def _get_modes_list_from_keys(keys_list, r_ext):
     """Get the modes list from the keys list
     of an hdf file.
 
     Parameters
     ----------
-    keys_list:      list
-                    The list containing all the keys
-    r_ext:      float
-                The extraction radius of the data.
+    keys_list:		list
+                                    The list containing all the keys
+    r_ext:		float
+                            The extraction radius of the data.
 
     Returns
     -------
     modes_list: list
-                    The list of modes.
+                                    The list of modes.
     """
 
     # Sort the keys to ensure a nice
     # modes list structure.
     keys_list_orig = sorted(keys_list)
 
     if r_ext != -1:
@@ -206,23 +206,23 @@
 
 def _get_ell_emm_from_key(key):
     """Get the :math:`\\ell` and :math:`m` values
     from a given key string of an hdf file.
 
     Parameters
     ----------
-    key:    str
-            The input key string
+    key:	str
+                    The input key string
 
     Returns
     -------
-    ell_value:      int
-                    The :math:`\\ell` value
-    emm_value:      int
-                    The :math:`m` value.
+    ell_value:		int
+                                    The :math:`\\ell` value
+    emm_value:		int
+                                    The :math:`m` value.
 
     Notes
     -----
 
     Assumes that the input string has :math:`\\ell` and :math:`m` values
     in the form `l{int}m{int}`.
 
@@ -245,21 +245,21 @@
 
 def get_iteration_numbers_from_keys(keys_list):
     """Get the iteration number from keys.
 
     Parameters
     ----------
     keys_list: list
-               The list of keys.
+                       The list of keys.
 
     Returns
     -------
     iteration_numbers: list
-                        The list containing the iteration
-                        numbers.
+                                            The list containing the iteration
+                                            numbers.
     """
     import re
 
     iteration_numbers = []
 
     for key in keys_list:
         str_match = re.search(" it=\d* ", key)
@@ -275,23 +275,23 @@
     """
     Construct a modes list in the form [[ell1, [emm1, emm2, ...], [ell2, [emm..]],..]
     given the :math:`\\ell_{max}.`
 
     Parameters
     ----------
     spin_weight : int
-                The spin weight of the modes.
+                            The spin weight of the modes.
     ell_max : int
-              The :math:`\\ell_{max}` of the modes list.
+                      The :math:`\\ell_{max}` of the modes list.
 
     Returns
     -------
 
     modes_list : list
-                 A list containg the mode indices lists.
+                             A list containg the mode indices lists.
 
     Notes
     -----
     The modes list is the form which the `waveform` object understands.
     """
 
     # The modes list.
@@ -302,25 +302,25 @@
         modes_list.append([ell_index, list(range(-ell_index, ell_index + 1))])
 
     return modes_list
 
 
 def sort_keys(modes_keys_list):
     """Sort the keys in a list based on
-        its iteration number
+            its iteration number
 
     Parameters
     ----------
     modes_keys_list: str
-                     The list of keys.
+                                     The list of keys.
 
     Returns
     -------
     sorted_modes_keys_list: str
-                            The sorted list.
+                                                    The sorted list.
     """
 
     iteration_numbers = get_iteration_numbers_from_keys(modes_keys_list)
 
     sargs = np.argsort(iteration_numbers)
 
     sorted_modes_keys_list = np.array(modes_keys_list)[sargs]
@@ -335,83 +335,81 @@
     ell_max=None,
     modes_list=None,
     save_as_ma=False,
     spin_weight=-2,
     resam_type="finest",
     interp_kind="cubic",
     crop=False,
-    centre=False
+    centre=False,
 ):
     """Load the Psi4 waveforms from the RIT catalogue
     from ASCII files from disk.
 
     Parameters
     ----------
-    wfa  :  waveforms
-            An instance of the waveforms class. Updates this instance if provided, else creates a new instance.
-    data_dir :  string
-            A string containing the directory path where the mode files can be found.
+    wfa  :	waveforms
+                    An instance of the waveforms class. Updates this instance if provided, else creates a new instance.
+    data_dir :	string
+                    A string containing the directory path where the mode files can be found.
     label : string, optional
-            The label of the modes_array object.
+                    The label of the modes_array object.
     ell_max : int, optional
-                The maximum mode number to load. If not specified,
-                then all available modes are loaded.
+                            The maximum mode number to load. If not specified,
+                            then all available modes are loaded.
     save_as_ma : bool, optional
-                 Save to disk again as a modes_array h5 file?
+                             Save to disk again as a modes_array h5 file?
     spin_weight : int, optional
-                  The spin weight of the object. Used for filtering modes.
-                  Defaults to -2.
+                              The spin weight of the object. Used for filtering modes.
+                              Defaults to -2.
     resam_type : string, float, optional
-                 The type of resampling to do. Options are finest and coarsest, and user input float.
+                             The type of resampling to do. Options are finest and coarsest, and user input float.
     interp_kind : string, optional
-                  The interpolation type to use. Default is cubic.
+                              The interpolation type to use. Default is cubic.
 
     Returns
     -------
 
     rit_modes_array : modes_array
-                        A modes_array instance containing the loaded modes.
+                                            A modes_array instance containing the loaded modes.
 
     Notes
     -----
     It seems like the time axis of individual modes are identical to each other. Hence, one need not worry about
     choosing the time domain. This may change in future.
     """
     message("Loading RIT Psi4 type data.", message_verbosity=1)
     from waveformtools.waveforms import modes_array
 
     if not wfa:
         wfa = modes_array(label=label, data_dir=data_dir, modes_list=wf_modes_list)
 
     if modes_list is None:
-    
+
         # Max available mode l.
         if ell_max is None:
             ell_max, _ = get_ell_max_from_file(data_dir)
 
         # Construct a modes list
         wf_modes_list = construct_mode_list(ell_max=ell_max, spin_weight=spin_weight)
-    
+
         message("The modes list is", wf_modes_list, message_verbosity=2)
 
     else:
         ell_max = max([item[0] for item in modes_list])
         wf_modes_list = modes_list
-    
+
     wfa.ell_max = ell_max
     wfa.modes_list = wf_modes_list
     wfa.r_ext = np.inf
     # For interpolation
     from scipy.interpolate import interp1d
 
     # Alias of the modes_array
     # label = 'q1a0_a'
     # Create a modes array
-    
-    
     # Enforce only l>2 modes.
     wf_modes_list = [item for item in wf_modes_list if item[0] >= abs(spin_weight)]
 
     # tend = []
     # tstart = []
 
     ##########################################
@@ -499,31 +497,31 @@
 
             ###################################
             # Load the modes data
             ###################################
 
             wfa.set_mode_data(ell, emm, wfmode)
 
-    wfa.actions+='->load_modes'
+    wfa.actions += "->load_modes"
 
     if crop is not False or centre is True:
         # Trim or recenter
-        if crop is True or centre is True: 
+        if crop is True or centre is True:
             wfa.trim(trim_upto_time=0)
             wfa.centered = True
-            wfa.actions+='->recenter'
+            wfa.actions += "->recenter"
 
         elif isinstance(crop, float):
             wfa.trim(trim_upto_time=crop)
-            wfa.actions+='->crop'
-    
+            wfa.actions += "->crop"
+
         if save_as_ma is True:
             # Save the modes array as waveforms hdf file
             wfa.save_modes(out_file_name="{label}_resam.h5")
-            wfa.actions+='->save_as_wfh5'
+            wfa.actions += "->save_as_wfh5"
     return wfa
 
 
 def load_RIT_Strain_data_from_disk(
     wfa=None,
     data_dir="./",
     file_name="*",
@@ -541,37 +539,37 @@
 ):
     """Load the RIT or strain waveforms from the RIT/ MAYA catalogue data,
     from hdf5 files from disk.
 
     Parameters
     ----------
     wfa  : waveforms
-           An instance of the waveforms class. Creates a new one if not provided.
-    data_dir :  string
-            A string containing the directory path where the mode files can be found.
+               An instance of the waveforms class. Creates a new one if not provided.
+    data_dir :	string
+                    A string containing the directory path where the mode files can be found.
     label : string, optional
-            The label of the modes_array object.
+                    The label of the modes_array object.
     ell_max : int, optional
-                The maximum mode number to load. If not specified,
-                then all available modes are loaded.
+                            The maximum mode number to load. If not specified,
+                            then all available modes are loaded.
     save_as_ma : bool, optional
-                 Save to disk again as a modes_array h5 file?
+                             Save to disk again as a modes_array h5 file?
     spin_weight : int, optional
-                  The spin weight of the object. Used for filtering modes.
-                  Defaults to -2.
+                              The spin weight of the object. Used for filtering modes.
+                              Defaults to -2.
     resam_type : string, float, optional
-                 The type of resampling to do. Options are finest and coarsest, and user input float.
+                             The type of resampling to do. Options are finest and coarsest, and user input float.
     interp_kind : string, optional
-                  The interpolation type to use. Default is cubic.
+                              The interpolation type to use. Default is cubic.
 
     Returns
     -------
 
     rit_modes_array : modes_array
-                        A modes_array instance containing the loaded modes.
+                                            A modes_array instance containing the loaded modes.
 
     Notes
     -----
     It seems like the time axis of individual modes are identical to each other. Hence, one need not worry about
     choosing the time domain. This may change in future.
     """
     message("Loading RIT strain data.", message_verbosity=1)
@@ -581,14 +579,15 @@
     # Initialize the interpolator
     if isinstance(interp_kind, int):
         message("Interpolating using InterpolatedUnivariateSpline", message_verbosity=2)
         interpolator = partial(interp, k=interp_kind)
 
     elif isinstance(interp_kind, str):
         from scipy.interpolate import interp1d
+
         message("Interpolating using interp1d", message_verbosity=2)
         interpolator = partial(interp1d, kind=interp_kind)
 
     from waveformtools.waveforms import modes_array
 
     # Max available mode l.
     ell_max_act, keys_list = get_ell_max_from_file(data_dir=data_dir, var_type="Strain", file_name=file_name)
@@ -635,15 +634,15 @@
         wfa.file_name = file_name
 
     if not ell_max:
         ell_max = wfa.ell_max
     else:
         wfa.ell_max = ell_max
 
-    # ell_max        = 12
+    # ell_max		 = 12
     if not modes_list:
         if not wfa.modes_list:
             message("Constructing the modes list")
             modes_list = construct_mode_list(ell_max=ell_max, spin_weight=wfa.spin_weight)
         else:
             modes_list = wfa.modes_list
     else:
@@ -704,31 +703,42 @@
                     # For MAYA data type
                     time_axis = Tphase
                     # dt_auto = time_axis[1]-time_axis[0]
                     from scipy.stats import mode
 
                     dt_auto = mode(np.diff(time_axis))[0][0]
 
-                # min_dt = round(min(np.diff(wf_psi4_time)), 2)
-                # max_dt = round(max(np.diff(wf_psi4_time)), 2)
-                message(f"Default dt is {dt_auto}")
+                min_dt = round(min(np.diff(time_axis)), 2)
+                max_dt = round(max(np.diff(time_axis)), 2)
+                message(f"Default dt is {dt_auto}", message_verbosity=2)
 
                 if resam_type == "auto":
                     # Choose finest available timestep
                     # for upto 3 decimal digits.
                     m_dt = dt_auto
-                    message("Sampling at the default timestep", m_dt)
+                    message("Sampling at the default timestep", m_dt, message_verbosity=2)
 
-                if isinstance(resam_type, float):
+                elif resam_type == "finest":
+                    m_dt = min_dt
+                    message("Sampling at the finest available timestep", m_dt, message_verbosity=2)
+
+                elif resam_type == "coarsest":
+                    m_dt = max_dt
+                    message("Sampling at the coarsest available timestep", m_dt, message_verbosity=2)
+
+                elif isinstance(resam_type, float):
                     m_dt = resam_type
-                    message("Resampling at user defined timestep", m_dt)
+                    message("Resampling at user defined timestep", m_dt, message_verbosity=2)
 
                     # New (resampled) time axis
                     time_axis = np.arange(time_axis[0], time_axis[-1], m_dt)
 
+                else:
+                    raise NotImplementedError(f"Unknown resampling parameter {resam_type}")
+
                 # Length of data.
                 data_len = len(time_axis)
 
                 # Create a modes array object
                 wfa.create_modes_array(ell_max=ell_max, data_len=data_len)
 
                 # Assign to it the time axis
@@ -736,15 +746,15 @@
                 # message(wfa.time_axis)
             # message(wfa.time_axis - wf_psi4_time)
             # continue
             ###################################
             # Uniform sampling
             ###################################
             # message('Wfa time axis', wfa.time_axis)
-            
+
             Yphase_interp_fun = interpolator(Tphase, Yphase)
             # Yphase_interp_fun = interpolator(Tphase, Yphase, k=3)
 
             # Resample
 
             Yphase_resam = Yphase_interp_fun(time_axis)
 
@@ -763,44 +773,44 @@
             # Resample
 
             Yamp_resam = Yamp_interp_fun(time_axis)
 
             wfmode = Yamp_resam * np.exp(1j * Yphase_resam)
 
             # if not (Tphase==Tamp).all():
-            #    raise ValueError('The time axis of the amps and phase are different!')
+            # 	 raise ValueError('The time axis of the amps and phase are different!')
 
             # wfmode = interp_resam_wfs(wf_c, Tphase, time_axis, k=4)
 
             ###################################
             # Load the modes data
             ###################################
 
             wfa.set_mode_data(ell, emm, r_ext_factor * wfmode)
 
     data_file.close()
 
     #####################
     # Finishing touches
     #####################
-    wfa.actions+='->load_modes'
+    wfa.actions += "->load_modes"
 
     # Trim or recenter
     if centre is True:
         wfa.trim(trim_upto_time=0)
-        wfa.actions+='->center'
+        wfa.actions += "->center"
 
     if isinstance(crop, float):
         wfa.trim(trim_upto_time=crop)
-        wfa.actions+='->crop'
+        wfa.actions += "->crop"
 
     if save_as_ma is True:
         # Save the modes array as waveforms hdf file
         wfa.save_modes(out_file_name=f"{label}_resam.h5")
-        wfa.actions+='->save_as_wfh5'
+        wfa.actions += "->save_as_wfh5"
 
     if debug is True:
         return wfa, wf_nl
     else:
         return wfa
 
 
@@ -826,36 +836,36 @@
     **kwargs,
 ):
     """Load the RIT strain waveforms from the RIT catalogue,
     from hdf5 files from disk.
 
     Parameters
     ----------
-    data_dir :  string
-            A string containing the directory path where the mode files can be found.
+    data_dir :	string
+                    A string containing the directory path where the mode files can be found.
     label : string, optional
-            The label of the modes_array object.
+                    The label of the modes_array object.
     ell_max : int, optional
-                The maximum mode number to load. If not specified,
-                then all available modes are loaded.
+                            The maximum mode number to load. If not specified,
+                            then all available modes are loaded.
     save_as_ma : bool, optional
-                 Save to disk again as a modes_array h5 file?
+                             Save to disk again as a modes_array h5 file?
     spin_weight : int, optional
-                  The spin weight of the object. Used for filtering modes.
-                  Defaults to -2.
+                              The spin weight of the object. Used for filtering modes.
+                              Defaults to -2.
     resam_type : string, float, optional
-                 The type of resampling to do. Options are finest and coarsest, and user input float.
+                             The type of resampling to do. Options are finest and coarsest, and user input float.
     interp_kind : string, optional
-                  The interpolation type to use. Default is cubic.
+                              The interpolation type to use. Default is cubic.
 
     Returns
     -------
 
     rit_modes_array : modes_array
-                        A modes_array instance containing the loaded modes.
+                                            A modes_array instance containing the loaded modes.
 
     Notes
     -----
     It seems like the time axis of individual modes are identical to each other. Hence, one need not worry about
     choosing the time domain. This may change in future.
 
     """
@@ -864,31 +874,31 @@
 
     # Max available mode l.
     if not wfa:
         # Create a modes array
         wfa = modes_array(label=label, data_dir=data_dir, modes_list=modes_list, ell_max=ell_max)
 
     # if not data_dir:
-    #   data_dir = wfa.data_dir
+    # 	data_dir = wfa.data_dir
     # else:
-    #   wfa.data_dir = data_dir
+    # 	wfa.data_dir = data_dir
 
     # if not file_name:
-    #   file_name = wfa.file_name
+    # 	file_name = wfa.file_name
     # else:
-    #   wfa.file_name = file_name
+    # 	wfa.file_name = file_name
 
     # if not ell_max:
-    #   ell_max = wfa.ell_max
+    # 	ell_max = wfa.ell_max
     # else:
-    #   wfa.ell_max = ell_max
+    # 	wfa.ell_max = ell_max
 
     # if not label:
-    #   label = wfa.label
-    # ell_max        = 12
+    # 	label = wfa.label
+    # ell_max		 = 12
     # Max available mode l.
 
     full_path = f"{data_dir}/{file_name}"
     message(f"Loading data from {full_path}")
     # Enforce only l>2 modes.
     # wf_modes_list = [item for item in wf_modes_list if item[0]>=abs(spin_weight)]
 
@@ -1066,19 +1076,19 @@
 
             wfa.trim(trim_upto_time=crop_time)
 
         # maxloc = np.argmax(np.absolute(self.mode(2, 2)))
         # maxtime = time_axis[shift + maxloc]
 
         # if wfa.maxtime is None:
-        #    wfa.maxtime = maxtime
+        # 	 wfa.maxtime = maxtime
         # message("Max time is", maxtime)
 
         # if centre:
-        #    wfa.time_axis = time_axis[shift:] - maxtime
+        # 	 wfa.time_axis = time_axis[shift:] - maxtime
         # message(wfa.file_name)
         return wfa
 
 
 ########################################################################################################################
 # SpEC
 ########################################################################################################################
@@ -1102,37 +1112,37 @@
     debug=False,
 ):
     """Load the SpEC waveform to modes_array,from hdf5 files from disk.
 
     Parameters
     ----------
     wfa : modes_array, optional
-          The modes array to which to store the loaded waveform to. A new modes array will be returned
-          if not provided.
-    data_dir :  string
-            A string containing the directory path where the mode files can be found.
+              The modes array to which to store the loaded waveform to. A new modes array will be returned
+              if not provided.
+    data_dir :	string
+                    A string containing the directory path where the mode files can be found.
     file_name : string
-            The name of the file containing the waveform data.
+                    The name of the file containing the waveform data.
     label : string, optional
-            The label of the modes_array object.
+                    The label of the modes_array object.
     ell_max : int, optional
-                The maximum mode number to load. If not specified,
-                then all available modes are loaded.
+                            The maximum mode number to load. If not specified,
+                            then all available modes are loaded.
     save_as_ma : bool, optional
-                 Save to disk again as a modes_array h5 file?
+                             Save to disk again as a modes_array h5 file?
     resam_type : string, float, optional
-                 The type of resampling to do. Options are finest and coarsest, and user input float.
+                             The type of resampling to do. Options are finest and coarsest, and user input float.
     interp_kind : string, optional
-                  The interpolation type to use. Default is cubic.
+                              The interpolation type to use. Default is cubic.
 
     Returns
     -------
 
     modes_array : modes_array
-                  A modes_array instance containing the loaded modes.
+                              A modes_array instance containing the loaded modes.
 
 
     """
     message("Loading SpEC data.", message_verbosity=1)
 
     from waveformtools.waveforms import modes_array
 
@@ -1197,15 +1207,15 @@
         wfa.file_name = file_name
 
     if not ell_max:
         ell_max = wfa.ell_max
     else:
         wfa.ell_max = ell_max
 
-    # ell_max        = 12
+    # ell_max		 = 12
     if not modes_list:
         if not wfa.modes_list:
             message("Constructing the modes list")
             # sys.exit(0)
             modes_list = construct_mode_list(ell_max=ell_max, spin_weight=wfa.spin_weight)
         else:
             modes_list = wfa.modes_list
@@ -1292,15 +1302,15 @@
 
             # Interpolate and resamplea
             # Note
             # Interpolating in amplitude and phase is better
             # and has lower interpolation errors
             # but is slower due to unwrapping of phases.
 
-            wf_int = interp_resam_wfs(wf_data_c, wf_time, time_axis, kind='cubic', k=None)
+            wf_int = interp_resam_wfs(wf_data_c, wf_time, time_axis, kind="cubic", k=None)
 
             # amp_int = interp_resam_wfs(wf_amp, wf_time, time_axis)
             # phase_int = interp_resam_wfs(wf_phase, wf_time, time_axis)
 
             # re_int = interp1d(wf_time, wf_data_re)
             # message(wf_time[0], wf_time[-1], time_axis[0], time_axis[-1])
             # re_dat = re_int(time_axis)
@@ -1365,37 +1375,37 @@
     compression_opts=0,
 ):
     """Load the SpECTRE or SpEC CCE waveform to modes_array,from hdf5 files from disk.
 
     Parameters
     ----------
     wfa : modes_array, optional
-          The modes array to which to store the loaded waveform to. A new modes array will be returned
-          if not provided.
-    data_dir :  string
-            A string containing the directory path where the mode files can be found.
+              The modes array to which to store the loaded waveform to. A new modes array will be returned
+              if not provided.
+    data_dir :	string
+                    A string containing the directory path where the mode files can be found.
     file_name : string
-            The name of the file containing the waveform data.
+                    The name of the file containing the waveform data.
     label : string, optional
-            The label of the modes_array object.
+                    The label of the modes_array object.
     ell_max : int, optional
-                The maximum mode number to load. If not specified,
-                then all available modes are loaded.
+                            The maximum mode number to load. If not specified,
+                            then all available modes are loaded.
     save_as_ma : bool, optional
-                 Save to disk again as a modes_array h5 file?
+                             Save to disk again as a modes_array h5 file?
     resam_type : string, float, optional
-                 The type of resampling to do. Options are finest and coarsest, and user input float.
+                             The type of resampling to do. Options are finest and coarsest, and user input float.
     interp_kind : string, optional
-                  The interpolation type to use. Default is cubic.
+                              The interpolation type to use. Default is cubic.
 
     Returns
     -------
 
     modes_array : modes_array
-                  A modes_array instance containing the loaded modes.
+                              A modes_array instance containing the loaded modes.
 
 
     """
     spin_weight = -2
     message("Loading SpECTRE data.", message_verbosity=1)
     from waveformtools.waveforms import modes_array
 
@@ -1440,15 +1450,15 @@
         wfa.file_name = file_name
 
     if not ell_max:
         ell_max = wfa.ell_max
     else:
         wfa.ell_max = ell_max
 
-    # ell_max        = 12
+    # ell_max		 = 12
     if not modes_list:
         if not wfa.modes_list:
             message("Constructing the modes list")
             # sys.exit(0)
             modes_list = construct_mode_list(ell_max=ell_max, spin_weight=spin_weight)
         else:
             modes_list = wfa.modes_list
@@ -1552,30 +1562,30 @@
     compression_opts=0,
     r_ext=None,
 ):
     """Save the waveform mode data to an hdf file.
 
     Parameters
     ----------
-    pre_key:    str, optional
-                            A string containing the key of the group in
-                            the HDF file in which the modes` dataset exists.
-                            It defaults to `None`.
-    mode_numbers:   list
-                                    The mode numbers to load from the file.
-                                    Each item in the list is a list that
-                                    contains two integrer numbers, one for
-                                    the mode index :math:`\\ell` and the
-                                    other for the mode index :math:`m`.
+    pre_key:	str, optional
+                                                    A string containing the key of the group in
+                                                    the HDF file in which the modes` dataset exists.
+                                                    It defaults to `None`.
+    mode_numbers:	list
+                                                                    The mode numbers to load from the file.
+                                                                    Each item in the list is a list that
+                                                                    contains two integrer numbers, one for
+                                                                    the mode index :math:`\\ell` and the
+                                                                    other for the mode index :math:`m`.
 
     Returns
     -------
-    waveform_obj:   3d array
-                                    Sets the three dimensional array `waveform.modes` that contains
-                                    the required :math:`\\ell, m` modes.
+    waveform_obj:	3d array
+                                                                    Sets the three dimensional array `waveform.modes` that contains
+                                                                    the required :math:`\\ell, m` modes.
 
     Examples
     --------
     >>> from waveformtools.waveforms import modes_array
     >>> wf = modes_array()
     >>> wf.data_dir = './'
     >>> wf.filename = 'data_file.h5'
```

### Comparing `waveformtools-2023.5.14/waveformtools/diagnostics.py` & `waveformtools-2023.5.17/waveformtools/diagnostics.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.14/waveformtools/differentiate.py` & `waveformtools-2023.5.17/waveformtools/differentiate.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.14/waveformtools/extrapolate.py` & `waveformtools-2023.5.17/waveformtools/extrapolate.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.14/waveformtools/grids.py` & `waveformtools-2023.5.17/waveformtools/grids.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.14/waveformtools/integrate.py` & `waveformtools-2023.5.17/waveformtools/integrate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """ Methods to integrate functions """
 
-
 #################################################
 # Imports
 ################################################
 
-
 import numpy as np
 
 from waveformtools.waveformtools import message
 
 ##################################################
 # Fixed frequency integration
 ##################################################
```

### Comparing `waveformtools-2023.5.14/waveformtools/legacy.py` & `waveformtools-2023.5.17/waveformtools/legacy.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.14/waveformtools/simulations.py` & `waveformtools-2023.5.17/waveformtools/simulations.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 from waveformtools.waveformtools import cleandata, message
 
 # import waveformtools
 
 
 class sim:
-
     """A data container for simulation data.
 
     Arrtibutes
     ----------
 
     ROOTDIR:	string
                             Root directory as a string containing the simulation folders.
@@ -363,18 +362,18 @@
                         The definition of time end of junk radiation. Default is 200.
 
         Notes
         -----
         Computes:
 
         self.indjn:	dict
-                                        A dictionary containing the index location 
+                                        A dictionary containing the index location
                                         corresponding to timestamp tjn.
         self.distjn:	dict
-                                        A dictionary containing the normalized co-ordinate 
+                                        A dictionary containing the normalized co-ordinate
                                         distance between the two BHs at tjn.
 
         """
 
         # Find the starting distance at t = 200M.
         # Initialize the directory.
         self.indjn = {}
@@ -445,15 +444,14 @@
         log_deltmult = {}
         for alias in self.aliases:
             message(alias)
             # Multipole data
             item = np.transpose(self.multipoles[alias])
             """Length of multipoles"""
             ml_length = len(item[:, 0])
-
             """Check the lengths of multipole and distance data"""
             if ml_length < self.comm_data_length[alias]:
                 """Reset the datalengths"""
                 self.comm_data_length[alias] = ml_length
                 """Resize the distance array"""
                 self.distance[alias] = self.distance[alias][:ml_length]
             message(item.shape)
@@ -506,15 +504,14 @@
         log_deltmult = {}
         for alias in self.aliases:
             message(alias)
             # Multipole data
             item = np.transpose(self.multipoles[alias])
             """Length of multipoles"""
             ml_length = len(item[:, 0])
-
             """Check the lengths of multipole and distance data"""
             if ml_length < self.comm_data_length[alias]:
                 """Reset the datalengths"""
                 self.comm_data_length[alias] = ml_length
                 """Resize the distance array"""
                 self.distance[alias] = self.distance[alias][:ml_length]
             message(item.shape)
```

### Comparing `waveformtools-2023.5.14/waveformtools/spherical.py` & `waveformtools-2023.5.17/waveformtools/spherical.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ Methods to handle functions on a sphere. """
 
-
 ##################################
 # Imports
 #################################
 
 import numpy as np
 
 
@@ -72,15 +71,14 @@
     phi = gridinfo.phi(ntheta=ntheta, nphi=nphi)
 
     # decomposed_waveforms = {}
 
     multipoles_all = {}
     for item in waveform:
         # Integrate on the sphere for decomposition into SWSHs
-
         """This should be fixed with summation over ell"""
 
         # define m values.
         if emm_list == "all":
             emm_list = np.arange(-ell_max, ell_max + 1)
 
         # Convert input to arrays.
```

### Comparing `waveformtools-2023.5.14/waveformtools/transforms.py` & `waveformtools-2023.5.17/waveformtools/transforms.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """ Methods to transform the waveform """
 
-
 import numpy as np
-
+from waveformtools.waveformtools import message
 # from numba import jit, njit
 
 
 # @njit(parallel=True)
 def compute_fft(udata_x, delta_x):
     """Find the FFT of the samples in time-space, and return with the frequencies.
 
     Parameters
     ----------
 
     udata_x:	1d array
-                            The samples in time-space.
+                                                    The samples in time-space.
 
     delta_x:	float
-                            The stepping delta_x
+                                                    The stepping delta_x
 
     Returns
     -------
 
     freqs:	1d array
-                    The frequency axis, shifted approriately.
+                                    The frequency axis, shifted approriately.
     utilde:	1d array
-                            The samples in frequency space, with conventions applied.
+                                                    The samples in frequency space, with conventions applied.
 
     """
 
     # import necessary libraries.
     from numpy.fft import fft
 
     # FFT
@@ -56,27 +55,27 @@
 def compute_ifft(utilde, delta_f):
     """Find the inverse FFT of the samples in frequency-space, and return with the time axis.
 
     Parameters
     ----------
 
     utilde	:	1d array
-                            The samples in frequency-space.
+                                                    The samples in frequency-space.
 
     delta_f:	float
-                            The frequency stepping
+                                                    The frequency stepping
 
     Returns
     -------
 
     time_axis:	1d array
-                            The time axis.
+                                                    The time axis.
 
     udata_time:	1d array
-                                    The samples in time domain.
+                                                                    The samples in time domain.
 
     """
 
     # import necessary libraries.
     from numpy.fft import ifft
 
     # FFT
@@ -101,28 +100,28 @@
 
     return time_axis, udata_time
 
 
 # @njit(parallel=True)
 def set_fft_conven(utilde_orig):
     """Make a numppy fft consistent with the chosen conventions.
-            This takes care of the zero mode factor and array position.
-            Also, it shifts the negative frequencies using numpy's fftshift.
+                    This takes care of the zero mode factor and array position.
+                    Also, it shifts the negative frequencies using numpy's fftshift.
 
     Parameters
     ----------
 
     utilde_orig:	1d array
-                                    The result of a numpy fft.
+                                                                    The result of a numpy fft.
 
     Returns
     -------
 
     utilde_conven:	1d array
-                                    The fft with set conventions.
+                                                                    The fft with set conventions.
     """
 
     # Multiply by 2, take conjugate.
     utilde_conven = 2 * np.conj(utilde_orig) / len(utilde_orig)
     # Restore the zero mode.
     utilde_conven[0] = utilde_conven[0] / 2
     # Shift the frequency axis.
@@ -130,22 +129,22 @@
 
     return utilde_conven
 
 
 # @njit(parallel=True)
 def unset_fft_conven(utilde_conven):
     """Make an actual conventional fft consistent with numpy's conventions.
-            The inverse of set_conv.
+                    The inverse of set_conv.
 
 
     Parameters
     ----------
 
     utilde_conven:	1d array
-                                    The conventional fft data vector.
+                                                                    The conventional fft data vector.
 
     Returns
     -------
 
     utilde_np
     """
 
@@ -156,257 +155,297 @@
     utilde_np[0] *= 2
     # message(utilde_original[0])
 
     return utilde_np
 
 
 def Yslm(spin_weight, ell, emm, theta, phi):
-    """Spin-weighted spherical harmonics data defined as a function of zeta and phi, for qlm data decomposition.
+    """Spin-weighted spherical harmonics fast evaluation.
 
-    Inputs
-    -----------
+    Parameters
+    ----------
 
-    spin_weight :   int
-                    The Spin weight.
-    ell :   int
-            The mode number :math:`\\ell'.
-    emm :   int
-            The azimuthal mode number :math:`m'.
+    spin_weight :	int
+                                    The Spin weight.
+    ell :	int
+                    The mode number :math:`\\ell'.
+    emm :	int
+                    The azimuthal mode number :math:`m'.
     theta : float
-            The polar angle  :math:`\\theta` in radians,
-    phi :   float
-            The aximuthal angle :math:`\\phi' in radians.
+                    The polar angle  :math:`\\theta` in radians,
+    phi :	float
+                    The aximuthal angle :math:`\\phi' in radians.
 
     Returns
     --------
-    Yslm :  float
-            The value of Yslm at :math:`\\theta, phi'.
+    Yslm :	float
+                    The value of Yslm at :math:`\\theta, phi'.
+
+            Note
+            ----
+            This is accurate upto 14 decimals for L upto 25.
 
     """
     import sympy as sp
 
     # theta, phi = sp.symbols('theta phi')
 
     fact = np.math.factorial
     # fact = sp.factorial
     Sum = 0
 
-    spin_weight = abs(spin_weight)
-
-    for aar in range(ell - spin_weight + 1):
-        if (aar + spin_weight - emm) < 0 or (ell - aar - spin_weight) < 0:
-            # message('Continuing')
+    factor = 1
+    if spin_weight < 0:
+        factor = (-1) ** ell
+        theta = np.pi - theta
+        phi += np.pi
+
+    abs_spin_weight = abs(spin_weight)
+
+    for aar in range(ell - abs_spin_weight + 1):
+        if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
+            message(f"Skippin r {aar}", message_verbosity=3)
             continue
         else:
-            # message('r, l, s, m', r, l, s, m)
-            # a1 = sp.binomial(ell - spin_weight, aar)
-            # message(a1)
-            # a2 = sp.binomial(ell + spin_weight, aar + spin_weight - emm)
-            # message(a2)
-            # a3 = np.exp(1j * emm * phi)
-            # message(a3)
-            # a4 = np.tan(theta / 2)
-            # message(a4)
-
             Sum += (
-                sp.binomial(ell - spin_weight, aar)
-                * sp.binomial(ell + spin_weight, aar + spin_weight - emm)
-                * np.power((-1), (ell - aar - spin_weight))
+                sp.binomial(ell - abs_spin_weight, aar)
+                * sp.binomial(ell + abs_spin_weight, aar + abs_spin_weight - emm)
+                * np.power((-1), (ell - aar - abs_spin_weight))
                 * np.exp(1j * emm * phi)
-                / np.power(np.tan(theta / 2), (2 * aar + spin_weight - emm))
+                / np.power(np.tan(theta / 2), (2 * aar + abs_spin_weight - emm))
             )
 
     Sum = complex(Sum)
-    # message(type(m))
-    # message((-1)**int(m))
-    # message(np.sin(th/2)**(2*l))
     Yslm = (-1) ** emm * (
         np.sqrt(
             fact(ell + emm)
             * fact(ell - emm)
             * (2 * ell + 1)
-            / (4 * np.pi * fact(ell + spin_weight) * fact(ell - spin_weight))
+            / (4 * np.pi * fact(ell + abs_spin_weight) * fact(ell - abs_spin_weight))
         )
         * np.sin(theta / 2) ** (2 * ell)
         * Sum
     )
 
-    return Yslm
+    return factor * Yslm
 
 
 def Yslm_vec(spin_weight, ell, emm, theta_grid, phi_grid):
-    """Spin-weighted spherical harmonics data defined as a function of zeta and phi, for qlm data decomposition.
+    """Spin-weighted spherical harmonics fast evaluations on numpy arrays for vectorized evaluations.
 
     Inputs
     -----------
 
-    spin_weight :   int
-                    The Spin weight.
-    ell :   int
-            The mode number :math:`\\ell'.
-    emm :   int
-            The azimuthal mode number :math:`m'.
+    spin_weight :	int
+                                    The Spin weight.
+    ell :	int
+                    The mode number :math:`\\ell'.
+    emm :	int
+                    The azimuthal mode number :math:`m'.
     theta : float
-            The polar angle  :math:`\\theta` in radians,
-    phi :   float
-            The aximuthal angle :math:`\\phi' in radians.
+                    The polar angle  :math:`\\theta` in radians,
+    phi :	float
+                    The aximuthal angle :math:`\\phi' in radians.
 
     Returns
     --------
-    Yslm :  float
-            The value of Yslm at :math:`\\theta, phi'.
+    Yslm :	float
+                    The value of Yslm at :math:`\\theta, phi'.
 
+            Note
+            ----
+            This is accurate upto 14 decimals for L upto 25.
     """
 
-    # spin_weight = abs(spin_weight)
-    # theta, phi = sp.symbols('theta phi')
     from math import comb
 
-    # import sympy as sp
     fact = np.math.factorial
 
     theta_grid = np.array(theta_grid)
     phi_grid = np.array(phi_grid)
 
     Sum = 0 + 1j * 0
 
-    spin_weight = abs(spin_weight)
+    factor = 1
+    if spin_weight < 0:
+        factor = (-1) ** ell
+        theta = np.pi - theta
+        phi += np.pi
+
+    abs_spin_weight = abs(spin_weight)
 
-    for aar in range(0, ell - spin_weight + 1):
-        # message('aar', aar)
+    for aar in range(0, ell - abs_spin_weight + 1):
         subterm = 0
 
-        if (aar + spin_weight - emm) < 0 or (ell - aar - spin_weight) < 0:
-            # message('Continuing')
+        if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
+            message(f"Skipping r {aar}", message_verbosity=3)
             continue
         else:
-            # message(aar + spin_weight-emm)
 
-            term1 = comb(ell - spin_weight, aar)
-            term2 = comb(ell + spin_weight, aar + spin_weight - emm)
-            term3 = np.power(float(-1), (ell - aar - spin_weight))
-            # term3 = (-1)**(ell-aar-spin_weight)
+            term1 = comb(ell - abs_spin_weight, aar)
+            term2 = comb(ell + abs_spin_weight, aar + abs_spin_weight - emm)
+            term3 = np.power(float(-1), (ell - aar - abs_spin_weight))
             term4 = np.exp(1j * emm * phi_grid)
-            term5 = np.power(np.tan(theta_grid / 2), (-2 * aar - spin_weight + emm))
+            term5 = np.power(np.tan(theta_grid / 2), (-2 * aar - abs_spin_weight + emm))
             subterm = term1 * term2 * term3 * term4 * term5
 
-            # message(term1, term2, term3, term4)
-
             Sum += subterm
-            # message('arr, subterm', aar, subterm)
 
-    # message(ell+emm, ell+spin_weight, ell-spin_weight)
     Yslmv = float(-1) ** emm * (
         np.sqrt(
             fact(ell + emm)
             * fact(ell - emm)
             * (2 * ell + 1)
-            / (4 * np.pi * fact(ell + spin_weight) * fact(ell - spin_weight))
+            / (4 * np.pi * fact(ell + abs_spin_weight) * fact(ell - abs_spin_weight))
         )
         * np.sin(theta_grid / 2) ** (2 * ell)
         * Sum
     )
 
-    return Yslmv
+    return factor * Yslmv
 
 
-def Yslm_prec(spin_weight, ell, emm, theta, phi, pres=16):
-    """Spin-weighted spherical harmonics data defined as a function of zeta and phi, for qlm data decomposition.
+def Yslm_prec(spin_weight, ell, emm, theta, phi, prec=24):
+    """Spin-weighted spherical harmonics function with precise computations.
+                            Uses a symbolic method evaluated at the degree of precision requested
+                            by the user.
+    Parameters
+    ----------
 
-    Inputs
-    -----------
+    spin_weight :	int
+                                    The Spin weight.
+    ell :	int
+                    The mode number :math:`\\ell'.
+    emm :	int
+                    The azimuthal mode number :math:`m'.
+    theta : float
+                    The polar angle  :math:`\\theta` in radians,
+    phi :	float
+                    The aximuthal angle :math:`\\phi' in radians.
+    pres : int, optional
+               The precision i.e. number of digits to compute
+               upto. Default value is 16.
+    Returns
+    --------
+    Yslm :	float
+                    The value of Yslm at :math:`\\theta, phi'.
+
+    """
+    import sympy as sp
+
+    # tv, pv = theta, phi
+    th, ph = sp.symbols("theta phi")
+
+    Yslm_expr = Yslm_prec_sym(spin_weight, ell, emm)
+
+    if spin_weight < 0:
+        theta = np.pi - theta
+        phi = np.pi + phi
+
+    return Yslm_expr.evalf(prec, subs={th: sp.Float(f"{theta}"), ph: sp.Float(f"{phi}")})
 
-    spin_weight :   int
-                    The Spin weight.
-    ell :   int
-            The mode number :math:`\\ell'.
-    emm :   int
-            The azimuthal mode number :math:`m'.
+
+def Yslm_prec_sym(spin_weight, ell, emm):
+    """Spin-weighted spherical harmonics precise, symbolic computation for deferred evaluations.
+       Is dependent on variables th: theta and ph:phi.
+    Parameters
+    ----------
+
+    spin_weight :	int
+                                    The Spin weight.
+    ell :	int
+                    The mode number :math:`\\ell'.
+    emm :	int
+                    The azimuthal mode number :math:`m'.
     theta : float
-            The polar angle  :math:`\\theta` in radians,
-    phi :   float
-            The aximuthal angle :math:`\\phi' in radians.
+                    The polar angle  :math:`\\theta` in radians,
+    phi :	float
+                    The aximuthal angle :math:`\\phi' in radians.
     pres : int, optional
-           The precision i.e. number of digits to compute
-           upto. Default value is 16.
+               The precision i.e. number of digits to compute
+               upto. Default value is 16.
+
     Returns
     --------
-    Yslm :  float
-            The value of Yslm at :math:`\\theta, phi'.
+    Yslm :	sym
+                    The value of Yslm at :math:`\\theta, phi'.
 
     """
     import sympy as sp
 
-    tv, pv = theta, phi
-    theta, phi = sp.symbols("theta phi")
+    th, ph = sp.symbols("theta phi")
 
-    # fact = np.math.factorial
     fact = sp.factorial
     Sum = 0
 
-    spin_weight = abs(spin_weight)
+    abs_spin_weight = abs(spin_weight)
+    # To get negative spin weight SWSH
+    # in terms of positive spin weight
+    factor = 1
+    if spin_weight < 0:
+        factor = sp.Pow(-1, ell)
 
-    for aar in range(ell - spin_weight + 1):
+    for aar in range(ell - abs_spin_weight + 1):
 
-        if (aar + spin_weight - emm) < 0 or (ell - aar - spin_weight) < 0:
+        if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
             # message('Continuing')
             continue
         else:
             # message('r, l, s, m', r, l, s, m)
             # a1 = sp.binomial(ell - spin_weight, aar)
             # message(a1)
             # a2 = sp.binomial(ell + spin_weight, aar + spin_weight - emm)
             # message(a2)
             # a3 = sp.exp(1j * emm * phi)
             # message(a3)
             # a4 = sp.tan(theta / 2)
             # message(a4)
 
             Sum += (
-                sp.binomial(ell - spin_weight, aar)
-                * sp.binomial(ell + spin_weight, aar + spin_weight - emm)
-                * sp.Pow((-1), (ell - aar - spin_weight))
-                * sp.exp(1j * emm * phi)
-                / sp.Pow(sp.tan(theta / 2), (2 * aar + spin_weight - emm))
+                sp.binomial(ell - abs_spin_weight, aar)
+                * sp.binomial(ell + abs_spin_weight, aar + abs_spin_weight - emm)
+                * sp.Pow((-1), (ell - aar - abs_spin_weight))
+                * sp.exp(sp.I * emm * ph)
+                * sp.Pow(sp.cot(th / 2), (2 * aar + abs_spin_weight - emm))
             )
 
     Yslm_expr = sp.Pow(-1, emm) * (
         sp.sqrt(
             fact(ell + emm)
             * fact(ell - emm)
             * (2 * ell + 1)
-            / (4 * sp.pi * fact(ell + spin_weight) * fact(ell - spin_weight))
+            / (4 * sp.pi * fact(ell + abs_spin_weight) * fact(ell - abs_spin_weight))
         )
-        * sp.Pow(sp.sin(theta / 2), (2 * ell))
+        * sp.Pow(sp.sin(th / 2), (2 * ell))
         * Sum
     )
 
-    Yslm_expr = sp.simplify(Yslm_expr)
+    Yslm_expr = factor * sp.simplify(Yslm_expr)
 
-    return Yslm_expr.evalf(pres, subs={theta: sp.Float(f"{tv}"), phi: sp.Float(f"{pv}")})
+    return Yslm_expr
 
 
 def rotate_polarizations(wf, alpha):
     """Rotate the polarizations of the time domain
     observer waveform by :math:`2\alpha`
 
     Parameters
     ----------
     wf : 1d array
-         The complex observer waveform to rotate.
+             The complex observer waveform to rotate.
     alpha : float
-            The coordinate angle to rotate the polarizations
-            in radians. Note that the polarizarions would
-            rotate by :math:`2 \alpha` on a cordinate
-            rotation of :math:`\alpha`.
+                    The coordinate angle to rotate the polarizations
+                    in radians. Note that the polarizarions would
+                    rotate by :math:`2 \alpha` on a cordinate
+                    rotation of :math:`\alpha`.
 
     Returns
     -------
     rot_wf : 1d array
-             The rotated waveform.
+                     The rotated waveform.
     """
 
     h1, h2 = wf.real, wf.imag
 
     rh1 = np.cos(2 * alpha) * h1 - np.sin(2 * alpha) * h2
     rh2 = np.sin(2 * alpha) * h1 + np.cos(2 * alpha) * h2
```

### Comparing `waveformtools-2023.5.14/waveformtools.egg-info/PKG-INFO` & `waveformtools-2023.5.17/waveformtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: waveformtools
-Version: 2023.5.14
+Version: 2023.5.17
 Summary:  Tools for working with numerical relativity and waveforms data 
 Home-page: https://gitlab.com/vaishakp/waveformtools
 Author: Vaishak Prasad
 Author-email: Vaishak Prasad <vaishakprasad@gmail.com>
 Project-URL: Homepage, https://gitlab.com/vaishakp/waveformtools
 Project-URL: Bug Tracker, https://gitlab.com/vaishakp/waveformtools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: EXT
 License-File: LICENSE
 
-[![Project landing page](https://sites.google.com/view/waveformtools/home)]
+[[Project landing page]](https://sites.google.com/view/waveformtools/home)
 [![pipeline status](https://gitlab.com/vaishakp/waveformtools/badges/main/pipeline.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/waveformtools/badge/?version=latest)](https://waveformtools.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
+[![PyPI version](https://badge.fury.io/py/waveformtools.svg)](https://badge.fury.io/py/waveformtools)
 # Waveformtools 
 
 
 This is a python module for the handling and analysis of waveforms and data from Numerical Relativity codes, and for carrying out gravitational wave data analysis.  
 
 waveformtools is a numerical relativity data handling package that was written to aid the handling and analysis of numerical relativity data.
 
 This package contains implementations of customized algorithms and techniques.  Some of these contain the usage of existing python based library functions from pycbc, scipy, etc but effort has been made to keep these to a minimum.
 
  
-* Handling of numerical relativity data, and retreiving specific information about the physical system.
+* Handling of numerical relativity data, and retreiving specific information about the physical system. Presently, this supports the EinsteinToolkit data.
 
     The class container and methods "sim" can load NR data into convenient lists and dictionaries, which can be used to     retrieve specific data/ information about the numerical simulation. 
 
     This offers the following functionality, like retreiving:
 
     * Horizon masses, mass-ratios, and areas.
 
@@ -104,16 +104,16 @@
 
 
 
 # Citing this code
 
 Please cite the latest version of this code if used in your work. This code was developed for use in the following works:
 
-1. [`News from Horizons in Binary Black Hole Mergers`](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.125.121101)
-2. ['Tidal deformation of dynamical horizons in binary black hole mergers'](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.105.044019)
+1. [News from Horizons in Binary Black Hole Mergers](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.125.121101)
+2. [Tidal deformation of dynamical horizons in binary black hole mergers](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.105.044019)
 
 We request you to also cite these. Thanks!
```

### Comparing `waveformtools-2023.5.14/waveformtools.egg-info/SOURCES.txt` & `waveformtools-2023.5.17/waveformtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

