# Comparing `tmp/noise2read-0.0.83.tar.gz` & `tmp/noise2read-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noise2read-0.0.83.tar", last modified: Wed May 17 10:00:06 2023, max compression
+gzip compressed data, was "noise2read-0.0.85.tar", last modified: Wed May 17 10:42:43 2023, max compression
```

## Comparing `noise2read-0.0.83.tar` & `noise2read-0.0.85.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:00:06.666115 noise2read-0.0.83/
--rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.83/LICENSE
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-17 10:00:06.667656 noise2read-0.0.83/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.83/README.rst
--rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.83/pyproject.toml
--rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-17 10:00:06.670689 noise2read-0.0.83/setup.cfg
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:00:06.522770 noise2read-0.0.83/src/
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:00:06.614696 noise2read-0.0.83/src/noise2read/
--rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-17 09:59:03.000000 noise2read-0.0.83/src/noise2read/__init__.py
--rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.83/src/noise2read/classifier.py
--rw-r--r--   0 pping    (55472) Research  (5010)    17130 2023-05-17 06:03:22.000000 noise2read-0.0.83/src/noise2read/config.py
--rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.83/src/noise2read/coverage.py
--rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.83/src/noise2read/data_analysis.py
--rw-r--r--   0 pping    (55472) Research  (5010)    45704 2023-05-16 13:16:54.000000 noise2read-0.0.83/src/noise2read/data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.83/src/noise2read/data_preprocessing.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.83/src/noise2read/encoding.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30699 2023-04-20 03:30:20.000000 noise2read-0.0.83/src/noise2read/error_orrection.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.83/src/noise2read/isolates_correction.py
--rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.83/src/noise2read/noise2read.py
--rw-r--r--   0 pping    (55472) Research  (5010)    34363 2023-05-17 09:58:46.000000 noise2read-0.0.83/src/noise2read/reads2vectors.py
--rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.83/src/noise2read/simulation.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.83/src/noise2read/umitest.py
--rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.83/src/noise2read/utils.py
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:00:06.647514 noise2read-0.0.83/src/noise2read.egg-info/
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-17 10:00:06.000000 noise2read-0.0.83/src/noise2read.egg-info/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-17 10:00:06.000000 noise2read-0.0.83/src/noise2read.egg-info/SOURCES.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-17 10:00:06.000000 noise2read-0.0.83/src/noise2read.egg-info/dependency_links.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-17 10:00:06.000000 noise2read-0.0.83/src/noise2read.egg-info/entry_points.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.83/src/noise2read.egg-info/not-zip-safe
--rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-17 10:00:06.000000 noise2read-0.0.83/src/noise2read.egg-info/requires.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-17 10:00:06.000000 noise2read-0.0.83/src/noise2read.egg-info/top_level.txt
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:00:06.661646 noise2read-0.0.83/tests/
--rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.83/tests/test_data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.83/tests/test_reads2vector.py
--rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.83/tests/test_utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:42:43.756609 noise2read-0.0.85/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.85/LICENSE
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-17 10:42:43.758719 noise2read-0.0.85/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.85/README.rst
+-rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.85/pyproject.toml
+-rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-17 10:42:43.762772 noise2read-0.0.85/setup.cfg
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:42:43.609934 noise2read-0.0.85/src/
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:42:43.701669 noise2read-0.0.85/src/noise2read/
+-rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-17 10:40:53.000000 noise2read-0.0.85/src/noise2read/__init__.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.85/src/noise2read/classifier.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    17130 2023-05-17 06:03:22.000000 noise2read-0.0.85/src/noise2read/config.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.85/src/noise2read/coverage.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.85/src/noise2read/data_analysis.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    49753 2023-05-17 10:38:46.000000 noise2read-0.0.85/src/noise2read/data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.85/src/noise2read/data_preprocessing.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.85/src/noise2read/encoding.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30699 2023-04-20 03:30:20.000000 noise2read-0.0.85/src/noise2read/error_orrection.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.85/src/noise2read/isolates_correction.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.85/src/noise2read/noise2read.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    34363 2023-05-17 09:58:46.000000 noise2read-0.0.85/src/noise2read/reads2vectors.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.85/src/noise2read/simulation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.85/src/noise2read/umitest.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.85/src/noise2read/utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:42:43.735936 noise2read-0.0.85/src/noise2read.egg-info/
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-17 10:42:43.000000 noise2read-0.0.85/src/noise2read.egg-info/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-17 10:42:43.000000 noise2read-0.0.85/src/noise2read.egg-info/SOURCES.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-17 10:42:43.000000 noise2read-0.0.85/src/noise2read.egg-info/dependency_links.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-17 10:42:43.000000 noise2read-0.0.85/src/noise2read.egg-info/entry_points.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.85/src/noise2read.egg-info/not-zip-safe
+-rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-17 10:42:43.000000 noise2read-0.0.85/src/noise2read.egg-info/requires.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-17 10:42:43.000000 noise2read-0.0.85/src/noise2read.egg-info/top_level.txt
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-17 10:42:43.751609 noise2read-0.0.85/tests/
+-rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.85/tests/test_data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.85/tests/test_reads2vector.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.85/tests/test_utils.py
```

### Comparing `noise2read-0.0.83/LICENSE` & `noise2read-0.0.85/LICENSE`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/PKG-INFO` & `noise2read-0.0.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.83
+Version: 0.0.85
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.83/README.rst` & `noise2read-0.0.85/README.rst`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/setup.cfg` & `noise2read-0.0.85/setup.cfg`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read/classifier.py` & `noise2read-0.0.85/src/noise2read/classifier.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read/config.py` & `noise2read-0.0.85/src/noise2read/config.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read/coverage.py` & `noise2read-0.0.85/src/noise2read/coverage.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read/data_analysis.py` & `noise2read-0.0.85/src/noise2read/data_analysis.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read/data_generation.py` & `noise2read-0.0.85/src/noise2read/data_generation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-16 15:52:44
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-16 23:16:54
+# @Last Modified time: 2023-05-17 20:38:46
 
 import editdistance
 import networkx as nx
 import os
 import csv
 from tqdm import tqdm
 from noise2read.utils import *
 from mpire import WorkerPool
 import matplotlib.pyplot as plt
 from networkx.drawing.nx_agraph import graphviz_layout
 from collections import Counter
 import sys
 import pandas as pd
+from multiprocessing import Pool
 
 class DataGneration():
     """
     A class to generate genuine and ambiguous errors from 1nt/2nt-edit-distance-based graphs construted from short reads dataset
     """
     def __init__(self, logger, config):
         """
@@ -255,42 +256,42 @@
             DataFrame: two pandas dataframes saving genuine and ambiguous errors
         """
         if edit_dis == 1:
             genu_columns = ["StartRead","StartReadCount", "StartDegree", "ErrorTye","ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"]
             ambiguous_df= pd.DataFrame(columns=["idx", "StartRead","StartReadCount", "StartDegree", "ErrorTye","ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"])
             genuine_csv = self.config.result_dir + "genuine1.csv"
             ambiguous_csv = self.config.result_dir + "ambiguous1.csv"
-        elif edit_dis == 2 or edit_dis == 3:
+        elif edit_dis == 2: #or edit_dis == 3:
             genu_columns = ["StartRead","StartReadCount", "StartDegree", "EndRead", "EndReadCount", "EndDegree"]
             ambiguous_df= pd.DataFrame(columns=["idx", "StartRead", "StartReadCount", "StartDegree", "EndRead", "EndReadCount", "EndDegree"])
             genuine_csv = self.config.result_dir + "genuine2.csv"
             ambiguous_csv = self.config.result_dir + "ambiguous2.csv"  
 
-        genuine_lst = []
-        ambiguous_lst = []
-        subgraph_num = len(subgraphs)
-        shared_obs = subgraphs, edit_dis
-        idx = 0
+        # genuine_lst = []
+        # ambiguous_lst = []
+        # subgraph_num = len(subgraphs)
+        # shared_obs = subgraphs, edit_dis
+        
         self.logger.info("Extracting genuine and ambiguous errors...")
-        with WorkerPool(self.config.num_workers, shared_objects=shared_obs, start_method='fork') as pool:
-            for genu_ambi_lst in pool.imap(self.extract_genuine_ambi_errs_subgraph, range(subgraph_num), progress_bar=self.config.verbose):
-                if genu_ambi_lst[0]:
-                    genuine_lst.extend(genu_ambi_lst[0])
-                    ambiguous_lst.extend(genu_ambi_lst[1])
-        self.logger.info("Done!")                    
+
+        pool = Pool(processes=self.config.num_workers)
+        # Process the subgraphs in parallel
+        results = [pool.apply_async(self.extract_genuine_ambi_errs_subgraph, (subgraph, edit_dis)) for subgraph in subgraphs]
+        genuine_lst, ambiguous_lst = zip(*results)
+
         # with WorkerPool(self.config.num_workers, shared_objects=shared_obs, start_method='fork') as pool:
-        #     with tqdm(total=subgraph_num, desc=self.logger.info("Extract samples with genuine errors"), miniters=int(subgraph_num/self.config.min_iters)) as pbar:   
-        #         for genu_ambi_lst in pool.imap(self.extract_genuine_ambi_errs_subgraph, range(subgraph_num)):
-        #             if genu_ambi_lst[0]:
-        #                 genuine_lst.extend(genu_ambi_lst[0])
-        #                 ambiguous_lst.extend(genu_ambi_lst[1])
-        #             pbar.update()
+        #     for genu_ambi_lst in pool.imap(self.extract_genuine_ambi_errs_subgraph, range(subgraph_num), progress_bar=self.config.verbose):
+        #         if genu_ambi_lst[0]:
+        #             genuine_lst.extend(genu_ambi_lst[0])
+        #             ambiguous_lst.extend(genu_ambi_lst[1])
+        self.logger.info("Done!")                    
 
         genuine_df = pd.DataFrame(genuine_lst, columns=genu_columns)
 
+        idx = 0
         for a_item in ambiguous_lst:
             for sub_item in a_item:
                 sub_item.insert(0, idx)
                 ambiguous_df.loc[len(ambiguous_df)] = sub_item
             idx += 1
                 
         if self.config.verbose:
@@ -331,93 +332,94 @@
         for a_item in item_lst:
             for sub_item in a_item:
                 sub_item.insert(0, idx)
                 tmp_df.loc[len(tmp_df)] = sub_item
             idx += 1
         return tmp_df
 
-    def extract_genuine_ambi_errs_subgraph(self, shared_obs, ii):
+    def extract_genuine_ambi_errs_subgraph(self, sub_graphs, edit_dis):
         gen_lst = []
         ambi_lst = []
-        sub_graphs, edit_dis = shared_obs 
-        sub_graph = sub_graphs[ii]
-        edges_lst = [e for e in sub_graph.edges()]
-        if len(edges_lst) > 0:
-            nodes_lst = list(sub_graph.nodes)
-            for node in nodes_lst:
-                node_count = sub_graph.nodes[node]['count']
-                node_degree = sub_graph.degree[node]
-                if node_count <= self.config.max_error_freq and not sub_graph.nodes[node]['flag']:
-                    node_neis = [n for n in sub_graph.neighbors(node)]
-                    if node_degree == 1:
-                        nei = node_neis[0]
-                        nei_count = sub_graph.nodes[nei]['count']
-                        nei_degree = sub_graph.degree[nei]
-                        # if nei_count >= self.config.high_freq_thre:
-                        if nei_count > self.config.high_freq_thre:
-                            line = [nei, nei_count, nei_degree, node, node_count, node_degree]
-                            if edit_dis == 1:
-                                newline = self.err_type_classification(line)
-                                # gen_df.loc[len(gen_df)] = newline
-                                gen_lst.append(newline)
-                                del line, newline 
-                            else:
-                                # gen_df.loc[len(gen_df)] = line 
-                                gen_lst.append(line)
-                                del line                                   
-                    # elif node_degree <= self.config.ambiguous_error_node_degree: # comment this line on 13 May 2023
-                    else:
-                        high_num = 0
-                        nei2count = []
-                        for nei in node_neis:
+        # sub_graphs, edit_dis = shared_obs 
+        # sub_graph = sub_graphs[ii]
+        for sub_graph in sub_graphs:
+            edges_lst = [e for e in sub_graph.edges()]
+            if len(edges_lst) > 0:
+                nodes_lst = list(sub_graph.nodes)
+                for node in nodes_lst:
+                    node_count = sub_graph.nodes[node]['count']
+                    node_degree = sub_graph.degree[node]
+                    if node_count <= self.config.max_error_freq and not sub_graph.nodes[node]['flag']:
+                        node_neis = [n for n in sub_graph.neighbors(node)]
+                        if node_degree == 1:
+                            nei = node_neis[0]
                             nei_count = sub_graph.nodes[nei]['count']
                             nei_degree = sub_graph.degree[nei]
                             # if nei_count >= self.config.high_freq_thre:
                             if nei_count > self.config.high_freq_thre:
-                                high_num += 1
-                                nei2count.append((nei, nei_count))
-                        if high_num == 1:             
-                            nei2count.sort(key=lambda x:x[1], reverse=True)
-                            first_nei, first_nei_count = nei2count[0]
-                            first_nei_degree = sub_graph.degree[first_nei]
-                            # if first_nei_count >= self.config.high_freq_thre:
-                            if first_nei_count > self.config.high_freq_thre:
-                                line = [first_nei, first_nei_count, first_nei_degree, node, node_count, node_degree]
+                                line = [nei, nei_count, nei_degree, node, node_count, node_degree]
                                 if edit_dis == 1:
                                     newline = self.err_type_classification(line)
                                     # gen_df.loc[len(gen_df)] = newline
                                     gen_lst.append(newline)
-                                    del line, newline  
+                                    del line, newline 
                                 else:
                                     # gen_df.loc[len(gen_df)] = line 
                                     gen_lst.append(line)
-                                    del line
+                                    del line                                   
+                        # elif node_degree <= self.config.ambiguous_error_node_degree: # comment this line on 13 May 2023
                         else:
-                            # ambiguous errors
-                            tmp_lst = []
-                            for cre_nei, cur_nei_count in nei2count:
-                                # if cur_nei_count >= self.config.high_freq_thre:
-                                if cur_nei_count > self.config.high_freq_thre:
-                                    cur_nei_degree = sub_graph.degree[nei]
-                                    line = [cre_nei, cur_nei_count, cur_nei_degree, node, node_count, node_degree]
+                            high_num = 0
+                            nei2count = []
+                            for nei in node_neis:
+                                nei_count = sub_graph.nodes[nei]['count']
+                                nei_degree = sub_graph.degree[nei]
+                                # if nei_count >= self.config.high_freq_thre:
+                                if nei_count > self.config.high_freq_thre:
+                                    high_num += 1
+                                    nei2count.append((nei, nei_count))
+                            if high_num == 1:             
+                                nei2count.sort(key=lambda x:x[1], reverse=True)
+                                first_nei, first_nei_count = nei2count[0]
+                                first_nei_degree = sub_graph.degree[first_nei]
+                                # if first_nei_count >= self.config.high_freq_thre:
+                                if first_nei_count > self.config.high_freq_thre:
+                                    line = [first_nei, first_nei_count, first_nei_degree, node, node_count, node_degree]
                                     if edit_dis == 1:
                                         newline = self.err_type_classification(line)
+                                        # gen_df.loc[len(gen_df)] = newline
+                                        gen_lst.append(newline)
+                                        del line, newline  
                                     else:
-                                        newline = line
-                                    # newline.insert(0, idx)
-                                    # ambi_df.loc[len(ambi_df)] = newline
-                                    tmp_lst.append(newline)
-                                    del newline 
-                            if tmp_lst:
-                                ambi_lst.append(tmp_lst)  
-                            # idx += 1 
-                    sub_graph.nodes[node]['flag'] = True        
-                else:
-                    continue
-        return [gen_lst, ambi_lst]
+                                        # gen_df.loc[len(gen_df)] = line 
+                                        gen_lst.append(line)
+                                        del line
+                            else:
+                                # ambiguous errors
+                                tmp_lst = []
+                                for cre_nei, cur_nei_count in nei2count:
+                                    # if cur_nei_count >= self.config.high_freq_thre:
+                                    if cur_nei_count > self.config.high_freq_thre:
+                                        cur_nei_degree = sub_graph.degree[nei]
+                                        line = [cre_nei, cur_nei_count, cur_nei_degree, node, node_count, node_degree]
+                                        if edit_dis == 1:
+                                            newline = self.err_type_classification(line)
+                                        else:
+                                            newline = line
+                                        # newline.insert(0, idx)
+                                        # ambi_df.loc[len(ambi_df)] = newline
+                                        tmp_lst.append(newline)
+                                        del newline 
+                                if tmp_lst:
+                                    ambi_lst.append(tmp_lst)  
+                                # idx += 1 
+                        sub_graph.nodes[node]['flag'] = True        
+                    else:
+                        continue
+        return gen_lst, ambi_lst
 
     def data_files(self, edit_dis):
         """
         function to return the results produced by DataGneration class
 
         Args:
             edit_dis (int): set edit distance 1 or 2 to search edges for constructing graph
@@ -590,24 +592,14 @@
             if edit_dis == 1:
                 for edge_lst in pool.imap(self.real_ed1_seqs, high_freq, progress_bar=self.config.verbose):
                     edges_lst.extend(edge_lst)
             elif edit_dis == 2:
                 for edge_lst in pool.imap(self.real_ed2_seqs, high_freq, progress_bar=self.config.verbose):
                     edges_lst.extend(edge_lst)
 
-        # with WorkerPool(self.config.num_workers, shared_objects=shared_unique_seqs, start_method='fork') as pool:
-        #     with tqdm(total=len(high_freq), desc=self.logger.info("Searching Edges"), miniters=int(len(high_freq)/self.config.min_iters)) as pbar:   
-        #         if edit_dis == 1:
-        #             for edge_lst in pool.imap(self.real_ed1_seqs, high_freq):
-        #                 edges_lst.extend(edge_lst)
-        #                 pbar.update()
-        #         elif edit_dis == 2:
-        #             for edge_lst in pool.imap(self.real_ed2_seqs, high_freq):
-        #                 edges_lst.extend(edge_lst)
-        #                 pbar.update()
         if len(edges_lst) > 0:
             self.logger.debug(len(edges_lst))
             self.logger.debug(edges_lst[0])
             graph.add_edges_from(edges_lst)
         self.logger.info(str(edit_dis) + "nt-edit-distance read graph construction finished.")
         ########################################################
         # save graphs
@@ -802,14 +794,15 @@
             del edges_lst
         if self.config.verbose:
             high_ambiguous_csv = self.config.result_dir + "high_ambiguous_1nt.csv"
             high_ambiguous_df.to_csv(high_ambiguous_csv, index=False)  
         self.logger.info("Done!")
         return high_ambiguous_df
 
+
 '''
     def extract_genuine_ambi_errs(self, subgraphs, edit_dis):
         """
         extract genuine and ambiguous errors from read graph
 
         Args:
             subgraphs (class): Subgraphs of graph constructed using NetworkX.
@@ -890,8 +883,90 @@
                         sub_graph.nodes[node]['flag'] = True        
                     else:
                         continue
         if self.config.verbose:
             genuine_df.to_csv(genuine_csv, index=False)  
             ambiguous_df.to_csv(ambiguous_csv, index=False)    
         return genuine_df, ambiguous_df
+'''
+
+'''
+    def extract_genuine_ambi_errs_subgraph(self, shared_obs, ii):
+        gen_lst = []
+        ambi_lst = []
+        sub_graphs, edit_dis = shared_obs 
+        sub_graph = sub_graphs[ii]
+        edges_lst = [e for e in sub_graph.edges()]
+        if len(edges_lst) > 0:
+            nodes_lst = list(sub_graph.nodes)
+            for node in nodes_lst:
+                node_count = sub_graph.nodes[node]['count']
+                node_degree = sub_graph.degree[node]
+                if node_count <= self.config.max_error_freq and not sub_graph.nodes[node]['flag']:
+                    node_neis = [n for n in sub_graph.neighbors(node)]
+                    if node_degree == 1:
+                        nei = node_neis[0]
+                        nei_count = sub_graph.nodes[nei]['count']
+                        nei_degree = sub_graph.degree[nei]
+                        # if nei_count >= self.config.high_freq_thre:
+                        if nei_count > self.config.high_freq_thre:
+                            line = [nei, nei_count, nei_degree, node, node_count, node_degree]
+                            if edit_dis == 1:
+                                newline = self.err_type_classification(line)
+                                # gen_df.loc[len(gen_df)] = newline
+                                gen_lst.append(newline)
+                                del line, newline 
+                            else:
+                                # gen_df.loc[len(gen_df)] = line 
+                                gen_lst.append(line)
+                                del line                                   
+                    # elif node_degree <= self.config.ambiguous_error_node_degree: # comment this line on 13 May 2023
+                    else:
+                        high_num = 0
+                        nei2count = []
+                        for nei in node_neis:
+                            nei_count = sub_graph.nodes[nei]['count']
+                            nei_degree = sub_graph.degree[nei]
+                            # if nei_count >= self.config.high_freq_thre:
+                            if nei_count > self.config.high_freq_thre:
+                                high_num += 1
+                                nei2count.append((nei, nei_count))
+                        if high_num == 1:             
+                            nei2count.sort(key=lambda x:x[1], reverse=True)
+                            first_nei, first_nei_count = nei2count[0]
+                            first_nei_degree = sub_graph.degree[first_nei]
+                            # if first_nei_count >= self.config.high_freq_thre:
+                            if first_nei_count > self.config.high_freq_thre:
+                                line = [first_nei, first_nei_count, first_nei_degree, node, node_count, node_degree]
+                                if edit_dis == 1:
+                                    newline = self.err_type_classification(line)
+                                    # gen_df.loc[len(gen_df)] = newline
+                                    gen_lst.append(newline)
+                                    del line, newline  
+                                else:
+                                    # gen_df.loc[len(gen_df)] = line 
+                                    gen_lst.append(line)
+                                    del line
+                        else:
+                            # ambiguous errors
+                            tmp_lst = []
+                            for cre_nei, cur_nei_count in nei2count:
+                                # if cur_nei_count >= self.config.high_freq_thre:
+                                if cur_nei_count > self.config.high_freq_thre:
+                                    cur_nei_degree = sub_graph.degree[nei]
+                                    line = [cre_nei, cur_nei_count, cur_nei_degree, node, node_count, node_degree]
+                                    if edit_dis == 1:
+                                        newline = self.err_type_classification(line)
+                                    else:
+                                        newline = line
+                                    # newline.insert(0, idx)
+                                    # ambi_df.loc[len(ambi_df)] = newline
+                                    tmp_lst.append(newline)
+                                    del newline 
+                            if tmp_lst:
+                                ambi_lst.append(tmp_lst)  
+                            # idx += 1 
+                    sub_graph.nodes[node]['flag'] = True        
+                else:
+                    continue
+        return [gen_lst, ambi_lst]
 '''
```

### Comparing `noise2read-0.0.83/src/noise2read/data_preprocessing.py` & `noise2read-0.0.85/src/noise2read/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read/encoding.py` & `noise2read-0.0.85/src/noise2read/encoding.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read/error_orrection.py` & `noise2read-0.0.85/src/noise2read/error_orrection.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read/isolates_correction.py` & `noise2read-0.0.85/src/noise2read/isolates_correction.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read/noise2read.py` & `noise2read-0.0.85/src/noise2read/noise2read.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read/reads2vectors.py` & `noise2read-0.0.85/src/noise2read/reads2vectors.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read/simulation.py` & `noise2read-0.0.85/src/noise2read/simulation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read/umitest.py` & `noise2read-0.0.85/src/noise2read/umitest.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read/utils.py` & `noise2read-0.0.85/src/noise2read/utils.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/src/noise2read.egg-info/PKG-INFO` & `noise2read-0.0.85/src/noise2read.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.83
+Version: 0.0.85
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.83/src/noise2read.egg-info/SOURCES.txt` & `noise2read-0.0.85/src/noise2read.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/tests/test_data_generation.py` & `noise2read-0.0.85/tests/test_data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/tests/test_reads2vector.py` & `noise2read-0.0.85/tests/test_reads2vector.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.83/tests/test_utils.py` & `noise2read-0.0.85/tests/test_utils.py`

 * *Files identical despite different names*

