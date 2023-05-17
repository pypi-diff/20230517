# Comparing `tmp/umierrorcorrect-0.26.tar.gz` & `tmp/umierrorcorrect-0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/xsteto/new/umierrorcorrect/dist/tmpzdatilqv/umierrorcorrect-0.26.tar", last modified: Fri Apr 14 12:15:47 2023, max compression
+gzip compressed data, was "/home/xsteto/new/umierrorcorrect/dist/tmpatp2bmun/umierrorcorrect-0.28.tar", last modified: Wed May 17 07:35:20 2023, max compression
```

## Comparing `umierrorcorrect-0.26.tar` & `umierrorcorrect-0.28.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/
-drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-14 12:15:46.000000 umierrorcorrect-0.26/umierrorcorrect/
-drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/umierrorcorrect/src/
--rw-rw-r--   0 xsteto    (1208) unix       (110)        0 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/src/__init__.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     4943 2023-04-14 12:03:38.000000 umierrorcorrect-0.26/umierrorcorrect/src/check_args.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    12262 2022-03-16 12:25:44.000000 umierrorcorrect-0.26/umierrorcorrect/src/get_cons_info.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    18485 2023-04-06 11:29:48.000000 umierrorcorrect-0.26/umierrorcorrect/src/get_consensus3.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     3756 2022-03-22 07:54:18.000000 umierrorcorrect-0.26/umierrorcorrect/src/get_regions_from_bed.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     6566 2022-08-30 07:25:37.000000 umierrorcorrect-0.26/umierrorcorrect/src/group.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)      868 2022-03-22 13:55:44.000000 umierrorcorrect-0.26/umierrorcorrect/src/handle_sequences.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     7529 2023-03-30 12:01:41.000000 umierrorcorrect-0.26/umierrorcorrect/src/umi_cluster.py
--rw-rw-r--   0 xsteto    (1208) unix       (110)        0 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/__init__.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     7853 2023-04-06 10:10:04.000000 umierrorcorrect-0.26/umierrorcorrect/call_variants.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     2889 2022-01-12 10:39:15.000000 umierrorcorrect-0.26/umierrorcorrect/downsampling_plots.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1165 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/filter_bam.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1895 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/filter_cons.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     2669 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/filter_cons2.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1806 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/filter_vcf.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     4254 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/fit_background_model.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    12378 2023-03-30 12:01:41.000000 umierrorcorrect-0.26/umierrorcorrect/get_consensus_statistics.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    12645 2022-02-01 13:00:49.000000 umierrorcorrect-0.26/umierrorcorrect/get_consensus_statistics2.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1798 2022-03-22 09:26:19.000000 umierrorcorrect-0.26/umierrorcorrect/get_umi_cluster_info.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    11999 2023-04-14 12:03:38.000000 umierrorcorrect-0.26/umierrorcorrect/preprocess.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     5643 2023-03-30 12:01:41.000000 umierrorcorrect-0.26/umierrorcorrect/run_mapping.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     9404 2023-04-14 12:03:38.000000 umierrorcorrect-0.26/umierrorcorrect/run_umierrorcorrect.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     3226 2021-11-24 14:09:38.000000 umierrorcorrect-0.26/umierrorcorrect/test_cons_info_indel.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    25529 2023-04-14 12:03:38.000000 umierrorcorrect-0.26/umierrorcorrect/umi_error_correct.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)       19 2023-04-14 12:12:43.000000 umierrorcorrect-0.26/umierrorcorrect/version.py
-drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/
--rw-rw-r--   0 xsteto    (1208) unix       (110)     3129 2023-04-14 12:15:44.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/PKG-INFO
--rw-rw-r--   0 xsteto    (1208) unix       (110)     1156 2023-04-14 12:15:45.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/SOURCES.txt
--rw-rw-r--   0 xsteto    (1208) unix       (110)        1 2023-04-14 12:15:44.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/dependency_links.txt
--rw-rw-r--   0 xsteto    (1208) unix       (110)        1 2022-01-24 15:00:25.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/not-zip-safe
--rw-rw-r--   0 xsteto    (1208) unix       (110)       30 2023-04-14 12:15:44.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/requires.txt
--rw-rw-r--   0 xsteto    (1208) unix       (110)       16 2023-04-14 12:15:44.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/top_level.txt
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1065 2021-11-29 10:11:37.000000 umierrorcorrect-0.26/LICENSE.txt
--rw-rw-r--   0 xsteto    (1208) unix       (110)     2715 2023-04-06 10:10:04.000000 umierrorcorrect-0.26/README.md
--rw-rw-r--   0 xsteto    (1208) unix       (110)       79 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/setup.cfg
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1447 2023-03-30 12:01:41.000000 umierrorcorrect-0.26/setup.py
--rw-rw-r--   0 xsteto    (1208) unix       (110)     3129 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/PKG-INFO
+drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-05-17 07:35:20.000000 umierrorcorrect-0.28/
+drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-05-17 07:35:20.000000 umierrorcorrect-0.28/umierrorcorrect/
+drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-05-17 07:35:20.000000 umierrorcorrect-0.28/umierrorcorrect/src/
+-rw-rw-r--   0 xsteto    (1208) unix       (110)        0 2021-11-24 14:09:37.000000 umierrorcorrect-0.28/umierrorcorrect/src/__init__.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     4943 2023-05-11 06:16:48.000000 umierrorcorrect-0.28/umierrorcorrect/src/check_args.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    12262 2022-03-16 12:25:44.000000 umierrorcorrect-0.28/umierrorcorrect/src/get_cons_info.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    18634 2023-05-12 07:21:46.000000 umierrorcorrect-0.28/umierrorcorrect/src/get_consensus3.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     3756 2022-03-22 07:54:18.000000 umierrorcorrect-0.28/umierrorcorrect/src/get_regions_from_bed.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     6566 2023-04-21 09:25:03.000000 umierrorcorrect-0.28/umierrorcorrect/src/group.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)      868 2023-05-10 14:11:39.000000 umierrorcorrect-0.28/umierrorcorrect/src/handle_sequences.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     7529 2023-03-30 12:01:41.000000 umierrorcorrect-0.28/umierrorcorrect/src/umi_cluster.py
+-rw-rw-r--   0 xsteto    (1208) unix       (110)        0 2021-11-24 14:09:37.000000 umierrorcorrect-0.28/umierrorcorrect/__init__.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     7853 2023-04-06 10:10:04.000000 umierrorcorrect-0.28/umierrorcorrect/call_variants.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     2889 2022-01-12 10:39:15.000000 umierrorcorrect-0.28/umierrorcorrect/downsampling_plots.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1165 2021-11-24 14:09:37.000000 umierrorcorrect-0.28/umierrorcorrect/filter_bam.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1895 2021-11-24 14:09:37.000000 umierrorcorrect-0.28/umierrorcorrect/filter_cons.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     2669 2021-11-24 14:09:37.000000 umierrorcorrect-0.28/umierrorcorrect/filter_cons2.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1806 2021-11-24 14:09:37.000000 umierrorcorrect-0.28/umierrorcorrect/filter_vcf.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     4254 2021-11-24 14:09:37.000000 umierrorcorrect-0.28/umierrorcorrect/fit_background_model.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    12378 2023-03-30 12:01:41.000000 umierrorcorrect-0.28/umierrorcorrect/get_consensus_statistics.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    12645 2022-02-01 13:00:49.000000 umierrorcorrect-0.28/umierrorcorrect/get_consensus_statistics2.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1798 2022-03-22 09:26:19.000000 umierrorcorrect-0.28/umierrorcorrect/get_umi_cluster_info.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    11999 2023-05-11 06:16:48.000000 umierrorcorrect-0.28/umierrorcorrect/preprocess.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     5643 2023-03-30 12:01:41.000000 umierrorcorrect-0.28/umierrorcorrect/run_mapping.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     9404 2023-05-12 13:35:31.000000 umierrorcorrect-0.28/umierrorcorrect/run_umierrorcorrect.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     3226 2021-11-24 14:09:38.000000 umierrorcorrect-0.28/umierrorcorrect/test_cons_info_indel.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    25529 2023-05-12 07:21:46.000000 umierrorcorrect-0.28/umierrorcorrect/umi_error_correct.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)       19 2023-05-17 07:33:13.000000 umierrorcorrect-0.28/umierrorcorrect/version.py
+drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-05-17 07:35:20.000000 umierrorcorrect-0.28/umierrorcorrect.egg-info/
+-rw-rw-r--   0 xsteto    (1208) unix       (110)     3127 2023-05-17 07:35:20.000000 umierrorcorrect-0.28/umierrorcorrect.egg-info/PKG-INFO
+-rw-rw-r--   0 xsteto    (1208) unix       (110)     1156 2023-05-17 07:35:20.000000 umierrorcorrect-0.28/umierrorcorrect.egg-info/SOURCES.txt
+-rw-rw-r--   0 xsteto    (1208) unix       (110)        1 2023-05-17 07:35:20.000000 umierrorcorrect-0.28/umierrorcorrect.egg-info/dependency_links.txt
+-rw-rw-r--   0 xsteto    (1208) unix       (110)        1 2022-01-24 15:00:25.000000 umierrorcorrect-0.28/umierrorcorrect.egg-info/not-zip-safe
+-rw-rw-r--   0 xsteto    (1208) unix       (110)       30 2023-05-17 07:35:20.000000 umierrorcorrect-0.28/umierrorcorrect.egg-info/requires.txt
+-rw-rw-r--   0 xsteto    (1208) unix       (110)       16 2023-05-17 07:35:20.000000 umierrorcorrect-0.28/umierrorcorrect.egg-info/top_level.txt
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1065 2021-11-29 10:11:37.000000 umierrorcorrect-0.28/LICENSE.txt
+-rw-rw-r--   0 xsteto    (1208) unix       (110)     2713 2023-05-17 07:33:25.000000 umierrorcorrect-0.28/README.md
+-rw-rw-r--   0 xsteto    (1208) unix       (110)       79 2023-05-17 07:35:20.000000 umierrorcorrect-0.28/setup.cfg
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1447 2023-03-30 12:01:41.000000 umierrorcorrect-0.28/setup.py
+-rw-rw-r--   0 xsteto    (1208) unix       (110)     3127 2023-05-17 07:35:20.000000 umierrorcorrect-0.28/PKG-INFO
```

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/check_args.py` & `umierrorcorrect-0.28/umierrorcorrect/src/check_args.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/get_cons_info.py` & `umierrorcorrect-0.28/umierrorcorrect/src/get_cons_info.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/get_consensus3.py` & `umierrorcorrect-0.28/umierrorcorrect/src/get_consensus3.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,14 +240,15 @@
                         if base not in consensus[refpos]:
                             consensus[refpos][base] = []
                         consensus[refpos][base].append(get_phred(qual[qpos]))
                     elif not refpos == ref + 1:
                         # deletion
                         dellength = refpos - (ref+1) #get the length of the deletion
                         delpos = refpos - dellength
+                        #print(consensus[delpos])
                         if delpos not in consensus:
                             consensus[delpos] = {}
                         if 'D' not in consensus[delpos]:
                             consensus[delpos]['D'] = {}
                         if dellength not in consensus[delpos]['D']:
                             consensus[delpos]['D'][dellength] = 0
                         consensus[delpos]['D'][dellength] += 1
@@ -266,15 +267,14 @@
                         if refpos not in consensus:
                             consensus[refpos] = {}
                         if base not in consensus[refpos]:
                             consensus[refpos][base] = []
                         consensus[refpos][base].append(get_phred(qual[qpos]))
                     q = qpos
                     ref = refpos
-    
     if len(consensus) > 0:
         #generate the consensus sequence
         consensus_sorted = sorted(consensus)
         consread = None
         add_consensus = True
         skippos = [] #if position is del
         prevpos = consensus_sorted[0] - 1
@@ -299,22 +299,24 @@
                         consread.add_insertion(sequence)
                     del(consensus[pos]['I'])
                     if poscov < 50:
                         cons_base, cons_qual = calc_consensus_probabilities(consensus[pos])
                     else:
                         cons_base, percent = get_most_common_allele(consensus[pos])
                         cons_qual = 60
-                    consread.add_base(cons_base, get_ascii(cons_qual))
+                    if not cons_base.startswith('D'):
+                        consread.add_base(cons_base, get_ascii(cons_qual))
 
                 elif 'D' in consensus[pos] and poscov >= 2:
                     # add the deletions
                     a, percent = get_most_common_allele(consensus[pos])
                     if a.startswith('D'):
                         if percent >= indel_freq_threshold:
                             dellength = int(a.lstrip('D'))
+                            #print(dellength)
                             consread.add_deletion(dellength)
                             if dellength > 1:
                                 for i in range(1,dellength):
                                     skippos.append(pos + i)
                         else:
                             consread.add_base('N', get_ascii(0))
                             add_consensus = False
```

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/get_regions_from_bed.py` & `umierrorcorrect-0.28/umierrorcorrect/src/get_regions_from_bed.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/group.py` & `umierrorcorrect-0.28/umierrorcorrect/src/group.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/handle_sequences.py` & `umierrorcorrect-0.28/umierrorcorrect/src/handle_sequences.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/src/umi_cluster.py` & `umierrorcorrect-0.28/umierrorcorrect/src/umi_cluster.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/call_variants.py` & `umierrorcorrect-0.28/umierrorcorrect/call_variants.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/downsampling_plots.py` & `umierrorcorrect-0.28/umierrorcorrect/downsampling_plots.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/filter_bam.py` & `umierrorcorrect-0.28/umierrorcorrect/filter_bam.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/filter_cons.py` & `umierrorcorrect-0.28/umierrorcorrect/filter_cons.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/filter_cons2.py` & `umierrorcorrect-0.28/umierrorcorrect/filter_cons2.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/filter_vcf.py` & `umierrorcorrect-0.28/umierrorcorrect/filter_vcf.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/fit_background_model.py` & `umierrorcorrect-0.28/umierrorcorrect/fit_background_model.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/get_consensus_statistics.py` & `umierrorcorrect-0.28/umierrorcorrect/get_consensus_statistics.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/get_consensus_statistics2.py` & `umierrorcorrect-0.28/umierrorcorrect/get_consensus_statistics2.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/get_umi_cluster_info.py` & `umierrorcorrect-0.28/umierrorcorrect/get_umi_cluster_info.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/preprocess.py` & `umierrorcorrect-0.28/umierrorcorrect/preprocess.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/run_mapping.py` & `umierrorcorrect-0.28/umierrorcorrect/run_mapping.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/run_umierrorcorrect.py` & `umierrorcorrect-0.28/umierrorcorrect/run_umierrorcorrect.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/test_cons_info_indel.py` & `umierrorcorrect-0.28/umierrorcorrect/test_cons_info_indel.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect/umi_error_correct.py` & `umierrorcorrect-0.28/umierrorcorrect/umi_error_correct.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/umierrorcorrect.egg-info/PKG-INFO` & `umierrorcorrect-0.28/umierrorcorrect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: umierrorcorrect
-Version: 0.26
+Version: 0.28
 Summary: UMI error correct
 Home-page: http://github.com/stahlberggroup/umierrorcorrect
 Author: Tobias Osterlund
 Author-email: tobias.osterlund@gu.se
 License: mit
-Download-URL: https://github.com/stahlberggroup/umierrorcorrect/archive/0.26.tar.gz
+Download-URL: https://github.com/stahlberggroup/umierrorcorrect/archive/0.28.tar.gz
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE.txt
 
 # umierrorcorrect
 
 Pipeline for analyzing barcoded amplicon sequencing data with Unique molecular identifiers (UMI)
@@ -19,15 +19,15 @@
 Reference
 ---------
 
 UMIErrorCorrect has been published in Clinical Chemistry.
 
 [Link to the Umierrorcorrect paper](https://doi.org/10.1093/clinchem/hvac136)
 
-Österlund T., Filges S., Johansson G., Ståhlberg A. UMIErrorCorrect and UMIAnalyzer: Software for Consensus Read Generation, Error Correction, and Visualization Using Unique Molecular Identifiers, Clinical Chemistry, 2022;, hvac136
+Osterlund T., Filges S., Johansson G., Stahlberg A. UMIErrorCorrect and UMIAnalyzer: Software for Consensus Read Generation, Error Correction, and Visualization Using Unique Molecular Identifiers, Clinical Chemistry, 2022;, hvac136
 
 Installation
 ------------
 
 To run Umierrorcorrect via Docker, see the [Docker documentation](doc/docker.md).
 
 To install the UMI-errorcorrect pipeline from source, open a terminal and type the following:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `umierrorcorrect-0.26/umierrorcorrect.egg-info/SOURCES.txt` & `umierrorcorrect-0.28/umierrorcorrect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/LICENSE.txt` & `umierrorcorrect-0.28/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/README.md` & `umierrorcorrect-0.28/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Reference
 ---------
 
 UMIErrorCorrect has been published in Clinical Chemistry.
 
 [Link to the Umierrorcorrect paper](https://doi.org/10.1093/clinchem/hvac136)
 
-Österlund T., Filges S., Johansson G., Ståhlberg A. UMIErrorCorrect and UMIAnalyzer: Software for Consensus Read Generation, Error Correction, and Visualization Using Unique Molecular Identifiers, Clinical Chemistry, 2022;, hvac136
+Osterlund T., Filges S., Johansson G., Stahlberg A. UMIErrorCorrect and UMIAnalyzer: Software for Consensus Read Generation, Error Correction, and Visualization Using Unique Molecular Identifiers, Clinical Chemistry, 2022;, hvac136
 
 Installation
 ------------
 
 To run Umierrorcorrect via Docker, see the [Docker documentation](doc/docker.md).
 
 To install the UMI-errorcorrect pipeline from source, open a terminal and type the following:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `umierrorcorrect-0.26/setup.py` & `umierrorcorrect-0.28/setup.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.26/PKG-INFO` & `umierrorcorrect-0.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: umierrorcorrect
-Version: 0.26
+Version: 0.28
 Summary: UMI error correct
 Home-page: http://github.com/stahlberggroup/umierrorcorrect
 Author: Tobias Osterlund
 Author-email: tobias.osterlund@gu.se
 License: mit
-Download-URL: https://github.com/stahlberggroup/umierrorcorrect/archive/0.26.tar.gz
+Download-URL: https://github.com/stahlberggroup/umierrorcorrect/archive/0.28.tar.gz
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE.txt
 
 # umierrorcorrect
 
 Pipeline for analyzing barcoded amplicon sequencing data with Unique molecular identifiers (UMI)
@@ -19,15 +19,15 @@
 Reference
 ---------
 
 UMIErrorCorrect has been published in Clinical Chemistry.
 
 [Link to the Umierrorcorrect paper](https://doi.org/10.1093/clinchem/hvac136)
 
-Österlund T., Filges S., Johansson G., Ståhlberg A. UMIErrorCorrect and UMIAnalyzer: Software for Consensus Read Generation, Error Correction, and Visualization Using Unique Molecular Identifiers, Clinical Chemistry, 2022;, hvac136
+Osterlund T., Filges S., Johansson G., Stahlberg A. UMIErrorCorrect and UMIAnalyzer: Software for Consensus Read Generation, Error Correction, and Visualization Using Unique Molecular Identifiers, Clinical Chemistry, 2022;, hvac136
 
 Installation
 ------------
 
 To run Umierrorcorrect via Docker, see the [Docker documentation](doc/docker.md).
 
 To install the UMI-errorcorrect pipeline from source, open a terminal and type the following:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

