# Comparing `tmp/Pulse3D-0.33.4.tar.gz` & `tmp/Pulse3D-0.33.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pulse3D-0.33.4.tar", last modified: Thu May 11 22:58:29 2023, max compression
+gzip compressed data, was "Pulse3D-0.33.5.tar", last modified: Wed May 17 19:31:07 2023, max compression
```

## Comparing `Pulse3D-0.33.4.tar` & `Pulse3D-0.33.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.858380 Pulse3D-0.33.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-11 22:58:29.858380 Pulse3D-0.33.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/mantarray-magnet-finding/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-11 22:57:22.000000 Pulse3D-0.33.4/mantarray-magnet-finding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/mantarray-magnet-finding/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 22:57:22.000000 Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-11 22:57:22.000000 Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 22:57:22.000000 Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-05-11 22:57:22.000000 Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-11 22:57:22.000000 Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-11 22:58:29.858380 Pulse3D-0.33.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/src/Pulse3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-11 22:58:29.000000 Pulse3D-0.33.4/src/Pulse3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-11 22:58:29.000000 Pulse3D-0.33.4/src/Pulse3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 22:58:14.000000 Pulse3D-0.33.4/src/Pulse3D.egg-info/not-zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 22:57:52.000000 Pulse3D-0.33.4/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-11 22:57:52.000000 Pulse3D-0.33.4/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 22:57:52.000000 Pulse3D-0.33.4/src/mantarray_magnet_finding/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-05-11 22:57:52.000000 Pulse3D-0.33.4/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-11 22:57:52.000000 Pulse3D-0.33.4/src/mantarray_magnet_finding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/src/pulse3D/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/compression_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    46466 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34854 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/nb_peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    33716 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/plate_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.834094 Pulse3D-0.33.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-17 19:30:05.000000 Pulse3D-0.33.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-17 19:31:07.834094 Pulse3D-0.33.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.830094 Pulse3D-0.33.5/mantarray-magnet-finding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-17 19:30:09.000000 Pulse3D-0.33.5/mantarray-magnet-finding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.830094 Pulse3D-0.33.5/mantarray-magnet-finding/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.830094 Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 19:30:09.000000 Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-17 19:30:09.000000 Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 19:30:09.000000 Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-05-17 19:30:09.000000 Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-17 19:30:09.000000 Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-17 19:31:07.834094 Pulse3D-0.33.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.830094 Pulse3D-0.33.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.834094 Pulse3D-0.33.5/src/Pulse3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-17 19:31:07.000000 Pulse3D-0.33.5/src/Pulse3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-17 19:31:07.000000 Pulse3D-0.33.5/src/Pulse3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:30:53.000000 Pulse3D-0.33.5/src/Pulse3D.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.830094 Pulse3D-0.33.5/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 19:30:30.000000 Pulse3D-0.33.5/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-17 19:30:30.000000 Pulse3D-0.33.5/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 19:30:30.000000 Pulse3D-0.33.5/src/mantarray_magnet_finding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-05-17 19:30:30.000000 Pulse3D-0.33.5/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-17 19:30:30.000000 Pulse3D-0.33.5/src/mantarray_magnet_finding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:31:07.834094 Pulse3D-0.33.5/src/pulse3D/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/compression_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46466 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34854 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/nb_peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33716 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/plate_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-17 19:30:06.000000 Pulse3D-0.33.5/src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.33.4/LICENSE` & `Pulse3D-0.33.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/PKG-INFO` & `Pulse3D-0.33.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.4
+Version: 0.33.5
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 License-File: LICENSE
```

### Comparing `Pulse3D-0.33.4/mantarray-magnet-finding/setup.py` & `Pulse3D-0.33.5/mantarray-magnet-finding/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 """Setup configuration."""
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name="mantarray_magnet_finding",
-    version="0.5.1",
+    version="0.5.2",
     description="Magnet Finding",
     url="https://github.com/CuriBio/mantarray-magnet-finding",
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=[
         "nptyping==1.4.4",
         "numpy==1.23.4",  # Tanner (12/3/21): pinned for numba compatibility
         "scipy==1.9.3",
-        "numba==0.56.4",
+        "numba==0.57.0",
         "stdlib_utils>=0.4.4",
         "labware-domain-models>=0.3.1",
         "h5py>=3.7.0",
         "immutabledict>=2.2.1",
     ],
     zip_safe=False,
     include_package_data=True,
@@ -31,13 +31,14 @@
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
 )
```

### Comparing `Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.5/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/setup.py` & `Pulse3D-0.33.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,48 +18,49 @@
 extensions = [Extension("pulse3D.compression_cy", [os.path.join("src", "pulse3D", "compression_cy") + ext])]
 if USE_CYTHON:
     # cythonizing compression_cy.pyx with kwarg annotate=True will help when optimizing the code by enabling generation of the html annotation file
     extensions = cythonize(extensions, annotate=False)
 
 setup(
     name="Pulse3D",
-    version="0.33.4",
+    version="0.33.5",
     description="Pulse3D Analysis Platform",
     url="https://github.com/CuriBio/Pulse3D",
     project_urls={"Documentation": "https://pulse3D.readthedocs.io/en/latest/"},
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     package_dir={"": "src"},
     include_dirs=[np.get_include()],
     packages=find_packages("src"),
     install_requires=[
-        "h5py>=3.7.0",
+        "h5py>=3.8.0",
         "nptyping==1.4.4",  # Tanner (4/7/22): pinning for now, can upgrade to 2.0.0 once there is time to refactor
-        "numpy>=1.23.4",
+        "numpy>=1.23.4",  # there is also a numpy version pinned in requirements-dev.txt since it is required to run this setup.py file
         "scipy==1.9.3",
-        "numba==0.56.4",
+        "numba==0.57.0",
         "immutabledict>=1.2.0",
         "XlsxWriter>=1.3.8",
         "openpyxl>=3.0.7",
         "stdlib_utils>=0.4.4",
         "labware-domain-models>=0.3.1",
         "requests>=2.25.1",
         "semver>=2.13.0",
-        "pandas>=1.3.4",
+        "pandas==1.5.3",
+        "pyarrow==12.0.0",
         'importlib-metadata >= 3.7.3 ; python_version < "3.8"',
     ],
     zip_safe=False,
     include_package_data=True,
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
     ],
     ext_modules=extensions,
 )
```

### Comparing `Pulse3D-0.33.4/src/Pulse3D.egg-info/PKG-INFO` & `Pulse3D-0.33.5/src/Pulse3D.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.4
+Version: 0.33.5
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 License-File: LICENSE
```

### Comparing `Pulse3D-0.33.4/src/Pulse3D.egg-info/SOURCES.txt` & `Pulse3D-0.33.5/src/Pulse3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.5/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.5/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/pulse3D/compression_cy.pyx` & `Pulse3D-0.33.5/src/pulse3D/compression_cy.pyx`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/pulse3D/constants.py` & `Pulse3D-0.33.5/src/pulse3D/constants.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/pulse3D/excel_writer.py` & `Pulse3D-0.33.5/src/pulse3D/excel_writer.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/pulse3D/exceptions.py` & `Pulse3D-0.33.5/src/pulse3D/exceptions.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/pulse3D/magnet_finding.py` & `Pulse3D-0.33.5/src/pulse3D/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/pulse3D/metrics.py` & `Pulse3D-0.33.5/src/pulse3D/metrics.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/pulse3D/nb_peak_detection.py` & `Pulse3D-0.33.5/src/pulse3D/nb_peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/pulse3D/peak_detection.py` & `Pulse3D-0.33.5/src/pulse3D/peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/pulse3D/plate_recording.py` & `Pulse3D-0.33.5/src/pulse3D/plate_recording.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/pulse3D/plotting.py` & `Pulse3D-0.33.5/src/pulse3D/plotting.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/pulse3D/stimulation.py` & `Pulse3D-0.33.5/src/pulse3D/stimulation.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/pulse3D/transforms.py` & `Pulse3D-0.33.5/src/pulse3D/transforms.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.4/src/pulse3D/utils.py` & `Pulse3D-0.33.5/src/pulse3D/utils.py`

 * *Files identical despite different names*

