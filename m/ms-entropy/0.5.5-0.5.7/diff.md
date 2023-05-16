# Comparing `tmp/ms_entropy-0.5.5.tar.gz` & `tmp/ms_entropy-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_entropy-0.5.5.tar", last modified: Tue May 16 22:18:27 2023, max compression
+gzip compressed data, was "ms_entropy-0.5.7.tar", last modified: Tue May 16 23:36:49 2023, max compression
```

## Comparing `ms_entropy-0.5.5.tar` & `ms_entropy-0.5.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 22:18:27.214484 ms_entropy-0.5.5/
--rw-r--r--   0 yli       (1000) yli       (1000)    11357 2023-03-18 01:04:19.000000 ms_entropy-0.5.5/LICENSE
--rw-rw-r--   0 yli       (1000) yli       (1000)       68 2023-05-10 07:52:05.000000 ms_entropy-0.5.5/MANIFEST.in
--rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-16 22:18:27.214484 ms_entropy-0.5.5/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)     3264 2023-03-29 23:15:55.000000 ms_entropy-0.5.5/README.md
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 22:18:27.214484 ms_entropy-0.5.5/ms_entropy/
--rw-rw-r--   0 yli       (1000) yli       (1000)      177 2023-05-13 02:10:56.000000 ms_entropy-0.5.5/ms_entropy/__init__.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 22:18:27.214484 ms_entropy-0.5.5/ms_entropy/entropy_search/
--rw-rw-r--   0 yli       (1000) yli       (1000)      196 2023-05-10 21:32:05.000000 ms_entropy-0.5.5/ms_entropy/entropy_search/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    20160 2023-05-15 19:49:33.000000 ms_entropy-0.5.5/ms_entropy/entropy_search/flash_entropy_search.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    27891 2023-05-10 07:39:35.000000 ms_entropy-0.5.5/ms_entropy/entropy_search/flash_entropy_search_core.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     5661 2023-05-10 07:39:35.000000 ms_entropy-0.5.5/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 22:18:27.214484 ms_entropy-0.5.5/ms_entropy/file_io/
--rw-rw-r--   0 yli       (1000) yli       (1000)       62 2023-05-10 23:13:55.000000 ms_entropy-0.5.5/ms_entropy/file_io/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     2047 2023-05-10 07:39:40.000000 ms_entropy-0.5.5/ms_entropy/file_io/lbm2_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     1690 2023-05-10 07:39:40.000000 ms_entropy-0.5.5/ms_entropy/file_io/mgf_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     1930 2023-05-10 07:39:40.000000 ms_entropy-0.5.5/ms_entropy/file_io/msp_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     2230 2023-05-16 22:17:35.000000 ms_entropy-0.5.5/ms_entropy/file_io/mzml_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)      920 2023-05-10 07:39:40.000000 ms_entropy-0.5.5/ms_entropy/file_io/shared.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     5722 2023-05-15 19:09:34.000000 ms_entropy-0.5.5/ms_entropy/file_io/spec_file.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 22:18:27.214484 ms_entropy-0.5.5/ms_entropy/tools/
--rw-rw-r--   0 yli       (1000) yli       (1000)      118 2023-05-10 07:39:45.000000 ms_entropy-0.5.5/ms_entropy/tools/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)   903746 2023-05-10 07:43:19.000000 ms_entropy-0.5.5/ms_entropy/tools/fast_entropy.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     3183 2023-05-10 07:39:45.000000 ms_entropy-0.5.5/ms_entropy/tools/fast_entropy.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)   895888 2023-05-10 07:43:20.000000 ms_entropy-0.5.5/ms_entropy/tools/fast_spectrum.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     4978 2023-05-10 07:39:45.000000 ms_entropy-0.5.5/ms_entropy/tools/fast_spectrum.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)     4318 2023-05-10 07:39:45.000000 ms_entropy-0.5.5/ms_entropy/tools/tools.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 22:18:27.214484 ms_entropy-0.5.5/ms_entropy.egg-info/
--rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-16 22:18:27.000000 ms_entropy-0.5.5/ms_entropy.egg-info/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)     1404 2023-05-16 22:18:27.000000 ms_entropy-0.5.5/ms_entropy.egg-info/SOURCES.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-05-16 22:18:27.000000 ms_entropy-0.5.5/ms_entropy.egg-info/dependency_links.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       84 2023-05-16 22:18:27.000000 ms_entropy-0.5.5/ms_entropy.egg-info/requires.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-05-16 22:18:27.000000 ms_entropy-0.5.5/ms_entropy.egg-info/top_level.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-03-24 01:05:23.000000 ms_entropy-0.5.5/pyproject.toml
--rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-05-16 22:18:27.218484 ms_entropy-0.5.5/setup.cfg
--rw-rw-r--   0 yli       (1000) yli       (1000)     1648 2023-05-16 22:18:22.000000 ms_entropy-0.5.5/setup.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/
+-rw-r--r--   0 yli       (1000) yli       (1000)    11357 2023-03-18 01:04:19.000000 ms_entropy-0.5.7/LICENSE
+-rw-rw-r--   0 yli       (1000) yli       (1000)       68 2023-05-10 07:52:05.000000 ms_entropy-0.5.7/MANIFEST.in
+-rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3264 2023-03-29 23:15:55.000000 ms_entropy-0.5.7/README.md
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 23:36:49.007383 ms_entropy-0.5.7/ms_entropy/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      177 2023-05-13 02:10:56.000000 ms_entropy-0.5.7/ms_entropy/__init__.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/ms_entropy/entropy_search/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      196 2023-05-10 21:32:05.000000 ms_entropy-0.5.7/ms_entropy/entropy_search/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    20160 2023-05-15 19:49:33.000000 ms_entropy-0.5.7/ms_entropy/entropy_search/flash_entropy_search.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    28087 2023-05-16 23:34:52.000000 ms_entropy-0.5.7/ms_entropy/entropy_search/flash_entropy_search_core.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5661 2023-05-10 07:39:35.000000 ms_entropy-0.5.7/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/ms_entropy/file_io/
+-rw-rw-r--   0 yli       (1000) yli       (1000)       62 2023-05-10 23:13:55.000000 ms_entropy-0.5.7/ms_entropy/file_io/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     2047 2023-05-10 07:39:40.000000 ms_entropy-0.5.7/ms_entropy/file_io/lbm2_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1690 2023-05-10 07:39:40.000000 ms_entropy-0.5.7/ms_entropy/file_io/mgf_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1930 2023-05-10 07:39:40.000000 ms_entropy-0.5.7/ms_entropy/file_io/msp_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3916 2023-05-16 23:31:01.000000 ms_entropy-0.5.7/ms_entropy/file_io/mzml_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)      920 2023-05-10 07:39:40.000000 ms_entropy-0.5.7/ms_entropy/file_io/shared.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5722 2023-05-15 19:09:34.000000 ms_entropy-0.5.7/ms_entropy/file_io/spec_file.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/ms_entropy/tools/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      118 2023-05-10 07:39:45.000000 ms_entropy-0.5.7/ms_entropy/tools/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)   903746 2023-05-10 07:43:19.000000 ms_entropy-0.5.7/ms_entropy/tools/fast_entropy.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3183 2023-05-10 07:39:45.000000 ms_entropy-0.5.7/ms_entropy/tools/fast_entropy.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)   895888 2023-05-10 07:43:20.000000 ms_entropy-0.5.7/ms_entropy/tools/fast_spectrum.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4978 2023-05-10 07:39:45.000000 ms_entropy-0.5.7/ms_entropy/tools/fast_spectrum.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4318 2023-05-10 07:39:45.000000 ms_entropy-0.5.7/ms_entropy/tools/tools.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/ms_entropy.egg-info/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-16 23:36:48.000000 ms_entropy-0.5.7/ms_entropy.egg-info/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1404 2023-05-16 23:36:48.000000 ms_entropy-0.5.7/ms_entropy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-05-16 23:36:48.000000 ms_entropy-0.5.7/ms_entropy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       85 2023-05-16 23:36:48.000000 ms_entropy-0.5.7/ms_entropy.egg-info/requires.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-05-16 23:36:48.000000 ms_entropy-0.5.7/ms_entropy.egg-info/top_level.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-03-24 01:05:23.000000 ms_entropy-0.5.7/pyproject.toml
+-rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-05-16 23:36:49.011383 ms_entropy-0.5.7/setup.cfg
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1682 2023-05-16 23:36:30.000000 ms_entropy-0.5.7/setup.py
```

### Comparing `ms_entropy-0.5.5/LICENSE` & `ms_entropy-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/README.md` & `ms_entropy-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/ms_entropy/entropy_search/flash_entropy_search.py` & `ms_entropy-0.5.7/ms_entropy/entropy_search/flash_entropy_search.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/ms_entropy/entropy_search/flash_entropy_search_core.py` & `ms_entropy-0.5.7/ms_entropy/entropy_search/flash_entropy_search_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
                             set it to 2 for searching only when search_array is True (or 1).
         :param search_spectra_idx_min:  The minimum index of the MS/MS spectra to search, required when search_type is 1.
         :param search_spectra_idx_max:  The maximum index of the MS/MS spectra to search, required when search_type is 1.
         :param search_array:    The array of the MS/MS spectra to search, required when search_type is 2.
         """
         if not self.index:
             return np.zeros(0, dtype=np.float32)
+        if len(peaks) == 0:
+            return np.zeros(self.total_spectra_num, dtype=np.float32)
 
         # Check peaks
         assert ms2_tolerance_in_da <= self.max_ms2_tolerance_in_da, "The MS2 tolerance is larger than the maximum MS2 tolerance."
         assert abs(np.sum(peaks[:, 1])-1) < 1e-4, "The peaks are not normalized to sum to 1."
         assert peaks.shape[0] <= 1 or np.min(peaks[1:, 0] - peaks[:-1, 0]) > self.max_ms2_tolerance_in_da * 2, \
             "The peaks array should be sorted by m/z, and the m/z difference between two adjacent peaks should be larger than 2 * max_ms2_tolerance_in_da."
         all_ions_mz_idx_start, all_ions_mz, all_ions_intensity, all_ions_spec_idx, \
@@ -138,14 +140,16 @@
         :param target: The target to perform the search. "cpu" for CPU, "gpu" for GPU.
         :param precursor_mz: The precursor m/z of the MS/MS spectra.
         :param peaks: The peaks of the MS/MS spectra, needs to be cleaned with the "clean_spectrum" function.
         :param ms2_tolerance_in_da: The MS/MS tolerance in Da.
         """
         if not self.index:
             return np.zeros(0, dtype=np.float32)
+        if len(peaks) == 0:
+            return np.zeros(self.total_spectra_num, dtype=np.float32)
 
         # Check peaks
         assert ms2_tolerance_in_da <= self.max_ms2_tolerance_in_da, "The MS2 tolerance is larger than the maximum MS2 tolerance."
         assert abs(np.sum(peaks[:, 1])-1) < 1e-4, "The peaks are not normalized to sum to 1."
         assert peaks.shape[0] <= 1 or np.min(peaks[1:, 0] - peaks[:-1, 0]) > self.max_ms2_tolerance_in_da * 2, \
             "The peaks array should be sorted by m/z, and the m/z difference between two adjacent peaks should be larger than 2 * max_ms2_tolerance_in_da."
         all_ions_mz_idx_start, all_ions_mz, all_ions_intensity, all_ions_spec_idx, \
```

### Comparing `ms_entropy-0.5.5/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py` & `ms_entropy-0.5.7/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/ms_entropy/file_io/lbm2_file.py` & `ms_entropy-0.5.7/ms_entropy/file_io/lbm2_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/ms_entropy/file_io/mgf_file.py` & `ms_entropy-0.5.7/ms_entropy/file_io/mgf_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/ms_entropy/file_io/msp_file.py` & `ms_entropy-0.5.7/ms_entropy/file_io/msp_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/ms_entropy/file_io/shared.py` & `ms_entropy-0.5.7/ms_entropy/file_io/shared.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/ms_entropy/file_io/spec_file.py` & `ms_entropy-0.5.7/ms_entropy/file_io/spec_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/ms_entropy/tools/fast_entropy.c` & `ms_entropy-0.5.7/ms_entropy/tools/fast_entropy.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/ms_entropy/tools/fast_entropy.pyx` & `ms_entropy-0.5.7/ms_entropy/tools/fast_entropy.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/ms_entropy/tools/fast_spectrum.c` & `ms_entropy-0.5.7/ms_entropy/tools/fast_spectrum.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/ms_entropy/tools/fast_spectrum.pyx` & `ms_entropy-0.5.7/ms_entropy/tools/fast_spectrum.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/ms_entropy/tools/tools.py` & `ms_entropy-0.5.7/ms_entropy/tools/tools.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/ms_entropy.egg-info/SOURCES.txt` & `ms_entropy-0.5.7/ms_entropy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.5/setup.py` & `ms_entropy-0.5.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 import os
 
 
 os.environ['CFLAGS'] = '-O3 -Wno-cpp -Wno-unused-function'
 
 setup(
     name='ms_entropy',
-    version='0.5.5',
+    version='0.5.7',
     license='Apache License 2.0',
     author='Yuanyue Li',
     url='https://github.com/YuanyueLi/SpectralEntropy',
     packages=find_packages(where='.', exclude=['tests', 'docs', 'examples', 'manuscript', 'dist', 'build']),
     python_requires='>=3.8',
     install_requires=[
         "numpy >= 1.18",
         "cython >= 0.29",
-        "lz4>=4.3.2",
-        "msgpack>=1.0.5",
-        "pymzml>=2.5.2"
+        "lz4 >= 4.3.2",
+        "msgpack >= 1.0.5",
+        # "pymzml>=2.5.2",
+        "pyteomics == 4.6"
     ],
     extras_require={
         "gpu": ["cupy >= 8.3.0"]
     },
     keywords=[
         "ms entropy",
         "ms spectral entropy",
```

