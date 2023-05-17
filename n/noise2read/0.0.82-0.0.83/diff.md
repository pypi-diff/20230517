# Comparing `tmp/noise2read-0.0.82.tar.gz` & `tmp/noise2read-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noise2read-0.0.82.tar", last modified: Wed May 17 06:05:52 2023, max compression
+gzip compressed data, was "noise2read-0.0.83.tar", last modified: Wed May 17 10:00:06 2023, max compression
```

## Comparing `noise2read-0.0.82.tar` & `noise2read-0.0.83.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 06:05:52.494170 noise2read-0.0.82/
--rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.82/LICENSE
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-17 06:05:52.504366 noise2read-0.0.82/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.82/README.rst
--rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.82/pyproject.toml
--rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-17 06:05:52.507324 noise2read-0.0.82/setup.cfg
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 06:05:52.340234 noise2read-0.0.82/src/
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 06:05:52.435361 noise2read-0.0.82/src/noise2read/
--rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-17 06:03:37.000000 noise2read-0.0.82/src/noise2read/__init__.py
--rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.82/src/noise2read/classifier.py
--rw-r--r--   0 pping    (55472) Research  (5010)    17130 2023-05-17 06:03:22.000000 noise2read-0.0.82/src/noise2read/config.py
--rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.82/src/noise2read/coverage.py
--rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.82/src/noise2read/data_analysis.py
--rw-r--r--   0 pping    (55472) Research  (5010)    45704 2023-05-16 13:16:54.000000 noise2read-0.0.82/src/noise2read/data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.82/src/noise2read/data_preprocessing.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.82/src/noise2read/encoding.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30699 2023-04-20 03:30:20.000000 noise2read-0.0.82/src/noise2read/error_orrection.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.82/src/noise2read/isolates_correction.py
--rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.82/src/noise2read/noise2read.py
--rw-r--r--   0 pping    (55472) Research  (5010)    34335 2023-05-16 12:55:31.000000 noise2read-0.0.82/src/noise2read/reads2vectors.py
--rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.82/src/noise2read/simulation.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.82/src/noise2read/umitest.py
--rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.82/src/noise2read/utils.py
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 06:05:52.467130 noise2read-0.0.82/src/noise2read.egg-info/
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-17 06:05:52.000000 noise2read-0.0.82/src/noise2read.egg-info/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-17 06:05:52.000000 noise2read-0.0.82/src/noise2read.egg-info/SOURCES.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-17 06:05:52.000000 noise2read-0.0.82/src/noise2read.egg-info/dependency_links.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-17 06:05:52.000000 noise2read-0.0.82/src/noise2read.egg-info/entry_points.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.82/src/noise2read.egg-info/not-zip-safe
--rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-17 06:05:52.000000 noise2read-0.0.82/src/noise2read.egg-info/requires.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-17 06:05:52.000000 noise2read-0.0.82/src/noise2read.egg-info/top_level.txt
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 06:05:52.482066 noise2read-0.0.82/tests/
--rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.82/tests/test_data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.82/tests/test_reads2vector.py
--rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.82/tests/test_utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:00:06.666115 noise2read-0.0.83/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.83/LICENSE
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-17 10:00:06.667656 noise2read-0.0.83/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.83/README.rst
+-rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.83/pyproject.toml
+-rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-17 10:00:06.670689 noise2read-0.0.83/setup.cfg
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:00:06.522770 noise2read-0.0.83/src/
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:00:06.614696 noise2read-0.0.83/src/noise2read/
+-rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-17 09:59:03.000000 noise2read-0.0.83/src/noise2read/__init__.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.83/src/noise2read/classifier.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    17130 2023-05-17 06:03:22.000000 noise2read-0.0.83/src/noise2read/config.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.83/src/noise2read/coverage.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.83/src/noise2read/data_analysis.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    45704 2023-05-16 13:16:54.000000 noise2read-0.0.83/src/noise2read/data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.83/src/noise2read/data_preprocessing.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.83/src/noise2read/encoding.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30699 2023-04-20 03:30:20.000000 noise2read-0.0.83/src/noise2read/error_orrection.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.83/src/noise2read/isolates_correction.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.83/src/noise2read/noise2read.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    34363 2023-05-17 09:58:46.000000 noise2read-0.0.83/src/noise2read/reads2vectors.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.83/src/noise2read/simulation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.83/src/noise2read/umitest.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.83/src/noise2read/utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:00:06.647514 noise2read-0.0.83/src/noise2read.egg-info/
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-17 10:00:06.000000 noise2read-0.0.83/src/noise2read.egg-info/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-17 10:00:06.000000 noise2read-0.0.83/src/noise2read.egg-info/SOURCES.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-17 10:00:06.000000 noise2read-0.0.83/src/noise2read.egg-info/dependency_links.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-17 10:00:06.000000 noise2read-0.0.83/src/noise2read.egg-info/entry_points.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.83/src/noise2read.egg-info/not-zip-safe
+-rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-17 10:00:06.000000 noise2read-0.0.83/src/noise2read.egg-info/requires.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-17 10:00:06.000000 noise2read-0.0.83/src/noise2read.egg-info/top_level.txt
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:00:06.661646 noise2read-0.0.83/tests/
+-rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.83/tests/test_data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.83/tests/test_reads2vector.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.83/tests/test_utils.py
```

### Comparing `noise2read-0.0.82/LICENSE` & `noise2read-0.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/PKG-INFO` & `noise2read-0.0.83/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.82
+Version: 0.0.83
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.82/README.rst` & `noise2read-0.0.83/README.rst`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/setup.cfg` & `noise2read-0.0.83/setup.cfg`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read/classifier.py` & `noise2read-0.0.83/src/noise2read/classifier.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read/config.py` & `noise2read-0.0.83/src/noise2read/config.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read/coverage.py` & `noise2read-0.0.83/src/noise2read/coverage.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read/data_analysis.py` & `noise2read-0.0.83/src/noise2read/data_analysis.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read/data_generation.py` & `noise2read-0.0.83/src/noise2read/data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read/data_preprocessing.py` & `noise2read-0.0.83/src/noise2read/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read/encoding.py` & `noise2read-0.0.83/src/noise2read/encoding.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read/error_orrection.py` & `noise2read-0.0.83/src/noise2read/error_orrection.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read/isolates_correction.py` & `noise2read-0.0.83/src/noise2read/isolates_correction.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read/noise2read.py` & `noise2read-0.0.83/src/noise2read/noise2read.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read/reads2vectors.py` & `noise2read-0.0.83/src/noise2read/reads2vectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-16 22:55:31
+# @Last Modified time: 2023-05-17 19:58:46
 
 from typing import Counter
 import numpy as np
 # import os
 from sklearn.preprocessing import StandardScaler
 from noise2read.encoding import EncodeScheme
 from mpire import WorkerPool
@@ -165,28 +165,28 @@
             cur_kmer2 = row['EndErrKmer']
             cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
             cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
             cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
             negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, row["StartDegree"]
 
         # isolates negative
-        for idx, row in negative_df.iterrows():
-            read = row['StartRead']
-            pos_reads = enumerate_ed1_seqs(read)
-            for read2 in pos_reads:
-                negtive_reads_lst1.append(read) 
-                negtive_reads_lst2.append(read2)  
-                cur_err_tye_kmers = error_type_classification(read, read2)
-                cur_err_tye = cur_err_tye_kmers[0]
-                cur_kmer1 = cur_err_tye_kmers[1]
-                cur_kmer2 = cur_err_tye_kmers[2]
-                cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
-                cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
-                cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
-                negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])  
+        # for idx, row in negative_df.iterrows():
+        #     read = row['StartRead']
+        #     pos_reads = enumerate_ed1_seqs(read)
+        #     for read2 in pos_reads:
+        #         negtive_reads_lst1.append(read) 
+        #         negtive_reads_lst2.append(read2)  
+        #         cur_err_tye_kmers = error_type_classification(read, read2)
+        #         cur_err_tye = cur_err_tye_kmers[0]
+        #         cur_kmer1 = cur_err_tye_kmers[1]
+        #         cur_kmer2 = cur_err_tye_kmers[2]
+        #         cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
+        #         cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
+        #         cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
+        #         negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])  
 
         for idx, row in ambiguous_df.iterrows():
             ambiguous_reads_lst1.append(row['StartRead'])
             ambiguous_reads_lst2.append(row['EndRead'])
             cur_err_tye = row['ErrorTye']
             cur_kmer1 = row['StartErrKmer']
             cur_kmer2 = row['EndErrKmer']
```

### Comparing `noise2read-0.0.82/src/noise2read/simulation.py` & `noise2read-0.0.83/src/noise2read/simulation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read/umitest.py` & `noise2read-0.0.83/src/noise2read/umitest.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read/utils.py` & `noise2read-0.0.83/src/noise2read/utils.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/src/noise2read.egg-info/PKG-INFO` & `noise2read-0.0.83/src/noise2read.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.82
+Version: 0.0.83
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.82/src/noise2read.egg-info/SOURCES.txt` & `noise2read-0.0.83/src/noise2read.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/tests/test_data_generation.py` & `noise2read-0.0.83/tests/test_data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/tests/test_reads2vector.py` & `noise2read-0.0.83/tests/test_reads2vector.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.82/tests/test_utils.py` & `noise2read-0.0.83/tests/test_utils.py`

 * *Files identical despite different names*

