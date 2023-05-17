# Comparing `tmp/ultra_bioinformatics-0.0.4.2.tar.gz` & `tmp/ultra_bioinformatics-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultra_bioinformatics-0.0.4.2.tar", last modified: Wed Oct 26 15:46:05 2022, max compression
+gzip compressed data, was "ultra_bioinformatics-0.1.tar", last modified: Wed May 17 12:24:59 2023, max compression
```

## Comparing `ultra_bioinformatics-0.0.4.2.tar` & `ultra_bioinformatics-0.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 ksahlin    (501) staff       (20)        0 2022-10-26 15:46:05.744391 ultra_bioinformatics-0.0.4.2/
--rw-r--r--   0 ksahlin    (501) staff       (20)    12502 2022-10-26 15:46:05.744115 ultra_bioinformatics-0.0.4.2/PKG-INFO
--rw-r--r--   0 ksahlin    (501) staff       (20)    11816 2022-10-23 15:41:39.000000 ultra_bioinformatics-0.0.4.2/README.md
-drwxr-xr-x   0 ksahlin    (501) staff       (20)        0 2022-10-26 15:46:05.742176 ultra_bioinformatics-0.0.4.2/modules/
--rw-r--r--   0 ksahlin    (501) staff       (20)        0 2020-02-11 11:07:56.000000 ultra_bioinformatics-0.0.4.2/modules/__init__.py
--rw-r--r--   0 ksahlin    (501) staff       (20)    36414 2022-10-23 15:41:39.000000 ultra_bioinformatics-0.0.4.2/modules/align.py
--rw-r--r--   0 ksahlin    (501) staff       (20)     3760 2021-02-23 17:39:05.000000 ultra_bioinformatics-0.0.4.2/modules/classify_alignment2.py
--rw-r--r--   0 ksahlin    (501) staff       (20)    31808 2021-02-23 17:39:05.000000 ultra_bioinformatics-0.0.4.2/modules/classify_read_with_mams.py
--rw-r--r--   0 ksahlin    (501) staff       (20)    19439 2021-02-23 17:39:05.000000 ultra_bioinformatics-0.0.4.2/modules/colinear_solver.py
--rw-r--r--   0 ksahlin    (501) staff       (20)    33838 2022-10-23 10:36:35.000000 ultra_bioinformatics-0.0.4.2/modules/create_augmented_gene.py
--rw-r--r--   0 ksahlin    (501) staff       (20)    10840 2022-10-21 12:23:49.000000 ultra_bioinformatics-0.0.4.2/modules/help_functions.py
--rw-r--r--   0 ksahlin    (501) staff       (20)     7954 2022-10-21 12:23:49.000000 ultra_bioinformatics-0.0.4.2/modules/mem_wrapper.py
--rw-r--r--   0 ksahlin    (501) staff       (20)     5802 2022-10-21 12:23:49.000000 ultra_bioinformatics-0.0.4.2/modules/prefilter_genomic_reads.py
--rw-r--r--   0 ksahlin    (501) staff       (20)    13132 2020-02-11 11:07:56.000000 ultra_bioinformatics-0.0.4.2/modules/range_query_max_search_tree.py
--rw-r--r--   0 ksahlin    (501) staff       (20)     8669 2022-10-23 15:30:17.000000 ultra_bioinformatics-0.0.4.2/modules/sam_output.py
--rw-r--r--   0 ksahlin    (501) staff       (20)       38 2022-10-26 15:46:05.744459 ultra_bioinformatics-0.0.4.2/setup.cfg
--rw-r--r--   0 ksahlin    (501) staff       (20)     4136 2022-10-23 15:41:39.000000 ultra_bioinformatics-0.0.4.2/setup.py
--rwxr-xr-x   0 ksahlin    (501) staff       (20)    45437 2022-10-23 15:41:39.000000 ultra_bioinformatics-0.0.4.2/uLTRA
-drwxr-xr-x   0 ksahlin    (501) staff       (20)        0 2022-10-26 15:46:05.743657 ultra_bioinformatics-0.0.4.2/ultra_bioinformatics.egg-info/
--rw-r--r--   0 ksahlin    (501) staff       (20)    12502 2022-10-26 15:46:05.000000 ultra_bioinformatics-0.0.4.2/ultra_bioinformatics.egg-info/PKG-INFO
--rw-r--r--   0 ksahlin    (501) staff       (20)      551 2022-10-26 15:46:05.000000 ultra_bioinformatics-0.0.4.2/ultra_bioinformatics.egg-info/SOURCES.txt
--rw-r--r--   0 ksahlin    (501) staff       (20)        1 2022-10-26 15:46:05.000000 ultra_bioinformatics-0.0.4.2/ultra_bioinformatics.egg-info/dependency_links.txt
--rw-r--r--   0 ksahlin    (501) staff       (20)       48 2022-10-26 15:46:05.000000 ultra_bioinformatics-0.0.4.2/ultra_bioinformatics.egg-info/requires.txt
--rw-r--r--   0 ksahlin    (501) staff       (20)        8 2022-10-26 15:46:05.000000 ultra_bioinformatics-0.0.4.2/ultra_bioinformatics.egg-info/top_level.txt
+drwxr-xr-x   0 ksahlin    (501) staff       (20)        0 2023-05-17 12:24:58.999412 ultra_bioinformatics-0.1/
+-rw-r--r--   0 ksahlin    (501) staff       (20)     6811 2023-05-17 12:24:58.999107 ultra_bioinformatics-0.1/PKG-INFO
+-rw-r--r--   0 ksahlin    (501) staff       (20)     6129 2023-05-17 12:18:23.000000 ultra_bioinformatics-0.1/README.md
+drwxr-xr-x   0 ksahlin    (501) staff       (20)        0 2023-05-17 12:24:58.996541 ultra_bioinformatics-0.1/modules/
+-rw-r--r--   0 ksahlin    (501) staff       (20)        0 2020-02-11 11:07:56.000000 ultra_bioinformatics-0.1/modules/__init__.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)    28224 2023-05-16 19:56:55.000000 ultra_bioinformatics-0.1/modules/align.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)     3760 2023-05-12 11:04:26.000000 ultra_bioinformatics-0.1/modules/classify_alignment2.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)    31757 2023-05-17 07:23:05.000000 ultra_bioinformatics-0.1/modules/classify_read_with_mams.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)    19513 2023-05-16 19:56:55.000000 ultra_bioinformatics-0.1/modules/colinear_solver.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)    33838 2022-10-23 10:36:35.000000 ultra_bioinformatics-0.1/modules/create_augmented_gene.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)    10848 2023-05-16 19:56:55.000000 ultra_bioinformatics-0.1/modules/help_functions.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)     3961 2023-05-16 19:56:55.000000 ultra_bioinformatics-0.1/modules/pc.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)     5372 2023-05-16 19:56:55.000000 ultra_bioinformatics-0.1/modules/prefilter_genomic_reads.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)    13132 2020-02-11 11:07:56.000000 ultra_bioinformatics-0.1/modules/range_query_max_search_tree.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)    10735 2023-05-16 19:56:55.000000 ultra_bioinformatics-0.1/modules/sam_output.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)     7343 2023-05-17 12:18:23.000000 ultra_bioinformatics-0.1/modules/seed_wrapper.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)     9094 2023-05-16 19:56:55.000000 ultra_bioinformatics-0.1/modules/test_pc_multiprocess.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)       38 2023-05-17 12:24:58.999517 ultra_bioinformatics-0.1/setup.cfg
+-rw-r--r--   0 ksahlin    (501) staff       (20)     4132 2023-05-16 19:56:55.000000 ultra_bioinformatics-0.1/setup.py
+-rwxr-xr-x   0 ksahlin    (501) staff       (20)    35547 2023-05-16 19:56:55.000000 ultra_bioinformatics-0.1/uLTRA
+drwxr-xr-x   0 ksahlin    (501) staff       (20)        0 2023-05-17 12:24:58.998581 ultra_bioinformatics-0.1/ultra_bioinformatics.egg-info/
+-rw-r--r--   0 ksahlin    (501) staff       (20)     6811 2023-05-17 12:24:58.000000 ultra_bioinformatics-0.1/ultra_bioinformatics.egg-info/PKG-INFO
+-rw-r--r--   0 ksahlin    (501) staff       (20)      598 2023-05-17 12:24:58.000000 ultra_bioinformatics-0.1/ultra_bioinformatics.egg-info/SOURCES.txt
+-rw-r--r--   0 ksahlin    (501) staff       (20)        1 2023-05-17 12:24:58.000000 ultra_bioinformatics-0.1/ultra_bioinformatics.egg-info/dependency_links.txt
+-rw-r--r--   0 ksahlin    (501) staff       (20)       48 2023-05-17 12:24:58.000000 ultra_bioinformatics-0.1/ultra_bioinformatics.egg-info/requires.txt
+-rw-r--r--   0 ksahlin    (501) staff       (20)        8 2023-05-17 12:24:58.000000 ultra_bioinformatics-0.1/ultra_bioinformatics.egg-info/top_level.txt
```

### Comparing `ultra_bioinformatics-0.0.4.2/modules/align.py` & `ultra_bioinformatics-0.1/modules/align.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import os
 import sys
 
+
 from collections import defaultdict
 from time import time
 from array import array
 import dill as pickle 
 import gffutils
 import pysam
 
-
 import signal
-from multiprocessing import Pool
-from operator import attrgetter
 
 from modules import colinear_solver 
 from modules import help_functions
 from modules import classify_read_with_mams
 from modules import classify_alignment2
 from modules import sam_output
-from modules import mem_wrapper
+from modules import seed_wrapper
 
+from collections import namedtuple
+mem = namedtuple('Mem', ['x', 'y', 'c', 'd', 'val', 'j', "exon_part_id"])
+globals()[mem.__name__] = mem # Global needed for multiprocessing
 
 ############### TMP #######
 from types import ModuleType, FunctionType
 from gc import get_referents
 
 # Custom objects know their class.
 # Function objects seem to know way too much, including modules.
@@ -318,15 +319,15 @@
                 covered += d - c + 1
             elif key in ref_flank_sequences:
                 seq = ref_flank_sequences[key] 
                 covered += d - c + 1
             else:
                 print("Bug encountered, {0} is not in {1}".format((x, y), mam_solution))
 
-        if prev_y_coord == x: #adjacent segments means its a flank and we should not add an new exon (i.e., intron split)
+        if prev_y_coord >= x: #adjacent segments means its a flank and we should not add an new exon (i.e., intron split)
             predicted_exons[-1] = (predicted_exons[-1][0], y)  # update the last exon
         else:
             predicted_exons.append( (x, y) )
 
         prev_y_coord = y
         chained_exon_seqs.append(seq)
     created_ref_seq = "".join([exon for exon in chained_exon_seqs])
@@ -349,359 +350,245 @@
         # print(read_acc)
         # print(read_aln)
         # print(ref_aln)
 
     return read_aln, ref_aln, alignment_score 
 
 
-# def run_tiling_solution(mem_solution, tiling_ref_segment_sequences, ref_flank_sequences, tiling_parts_to_segments, \
-#                         tiling_segment_to_gene, tiling_gene_to_small_segments, \
-#                         read_seq, warning_log_file, min_acc, \
-#                         chr_id, ref_exon_sequences, \
-#                         all_splice_pairs_annotations,
-#                         splices_to_transcripts, transcripts_to_splices, \
-#                         all_splice_sites_annotations, mam_sol_exons_length, \
-#                         alignment_score, read_aln, ref_aln, current_classification, non_covered_regions, covered,
-#                         predicted_exons, annotated_to_transcript_id):
-
-#     non_covered_regions_tiling, mam_value_tiling, mam_solution_tiling = classify_read_with_mams.main(mem_solution, tiling_ref_segment_sequences, ref_flank_sequences, tiling_parts_to_segments, \
-#                                                                                                             tiling_segment_to_gene, tiling_gene_to_small_segments, \
-#                                                                                                             read_seq, warning_log_file, min_acc, is_tiling_instance = True)
-
-#     # print("TILING finished Mam solution Tiling!!:",mam_value_tiling, mam_solution_tiling)
-#     # for zzz2 in mam_solution_tiling:
-#     #     print(zzz2)
-#     exons, tiling_created_ref_seq, tiling_predicted_exons, tiling_predicted_splices, tiling_covered = find_exons(chr_id, mam_solution_tiling, ref_exon_sequences, \
-#                                                                             tiling_ref_segment_sequences, ref_flank_sequences, all_splice_pairs_annotations)
-
-#     tiling_classification, tiling_annotated_to_transcript_id = classify_alignment2.main(chr_id, tiling_predicted_splices, splices_to_transcripts, transcripts_to_splices, all_splice_pairs_annotations, all_splice_sites_annotations)
-
-#     tiling_read_aln, tiling_ref_aln, tiling_alignment_score = get_exact_alignment(read_seq, tiling_created_ref_seq, mam_sol_exons_length)
-
-#     if tiling_alignment_score > alignment_score or tiling_classification == 'FSM':
-#         # print("TILING")        
-#         # print("old aln:", read_aln)
-#         # print("old aln:", ref_aln)
-#         # print(tiling_classification)            
-#         # print("BEFORE", non_covered_regions)
-#         # print("new aln:", tiling_read_aln)
-#         # print("new aln:", tiling_ref_aln)
-#         # print("NOW", non_covered_regions_tiling) 
-#         # print("read was", current_classification, "had aln score", alignment_score)
-#         # print("tiling read is ", tiling_classification, "has aln score", tiling_alignment_score)
-#         return  tiling_classification, tiling_alignment_score, non_covered_regions_tiling, \
-#                 tiling_read_aln, tiling_ref_aln, tiling_predicted_exons, tiling_annotated_to_transcript_id, tiling_covered
-#     else:
-#         return current_classification, alignment_score, non_covered_regions, \
-#                 read_aln, ref_aln, predicted_exons, annotated_to_transcript_id, covered
+def get_mems_from_input(hits):
+    # speed this parsing up by providing already sorted
+    # hits per ref_id and ref coord from namfinder
+
+    read_mems = defaultdict(list)
+    read_mems_rev = defaultdict(list)
+
+    for line in hits:
+        vals =  line.split() #11404_11606           1     11405       202
+        exon_part_id = vals[0]
+        chr_id, ref_coord_start, ref_coord_end = exon_part_id.split('^')
+        # chr_id, ref_coord_start, ref_coord_end = ['1', '1', '1'] # CURRENT DUMMY LINE FOR TESTING OUTSIDE ULTRA'S FORMAT
+        chr_id = int(chr_id)
+        mem_len = int(vals[3])
+
+        mem_ref_exon_part_start = int(vals[1]) - 1 # convert to 0-indexed reference as in python
+        mem_read_start = int(vals[2]) - 1
+        ref_coord_start = int(ref_coord_start) # has already been 0-indexed when constructing parts
+        mem_genome_start = ref_coord_start + mem_ref_exon_part_start
+        
+        info_tuple = ( mem_genome_start, mem_genome_start + mem_len - 1,
+                        mem_read_start, mem_read_start + mem_len - 1, 
+                        mem_len, exon_part_id) # however, for MEM length last coordinate is inclusive of the hit in MEM solvers, not as in python end-indexing
 
+        read_mems[chr_id].append(info_tuple)
 
-def align_single(reads, refs_lengths, args,  batch_number):
-    # print("reads:", getsize(reads)//1000000)
-    auxillary_data = import_data(args)
-    # import time
-    # time.sleep(10000)
-    mems_path =  os.path.join( args.outfolder, "seeds_batch_{0}.txt".format(batch_number) )
-    mems_path_rc =  os.path.join( args.outfolder, "seeds_batch_{0}_rc.txt".format(batch_number) )
+    for chr_id in list(read_mems.keys()):
+        coordinate_sorted_tuples = sorted(read_mems[chr_id], key = lambda x: x[1])
+        sorted_mems = [ mem(x,y,c,d,val,j,e_id) for j, (x, y, c, d, val, e_id) in enumerate(coordinate_sorted_tuples) ]
+        read_mems[chr_id] = sorted_mems
+
+    return read_mems
+
+
+
+def align_single(process_id, input_queue, output_sam_buffer, classification_and_aln_cov, args):
+
+    # set counters
     nlog_n_instance_counter = 0
     quadratic_instance_counter = 0
     max_global_intron = args.max_intron
     min_acc = args.min_acc
+    classifications = defaultdict(str)
+    processed_read_counter = 0
+
+    # read in index
+    auxillary_data = import_data(args)
     ref_segment_sequences, ref_flank_sequences, splices_to_transcripts, \
     transcripts_to_splices, all_splice_pairs_annotations, \
     all_splice_sites_annotations, parts_to_segments, \
     segment_to_gene, gene_to_small_segments, max_intron_chr, \
     ref_exon_sequences, chr_to_id, id_to_chr = auxillary_data
-    # ref_exon_sequences, chr_to_id, id_to_chr, tiling_structures = auxillary_data
-
-    if batch_number == -1:
-        alignment_outfile = pysam.AlignmentFile( os.path.join(args.outfolder, args.prefix+".sam"), "w", reference_names=list(refs_lengths.keys()), reference_lengths=list(refs_lengths.values()) ) #, template=samfile)
-        warning_log_file = open(os.path.join(args.outfolder, "uLTRA.stderr"), "w")
-
-    else:
-        alignment_outfile = pysam.AlignmentFile( os.path.join(args.outfolder, "reads_batch_{0}.sam".format(batch_number)), "w", reference_names=list(refs_lengths.keys()), reference_lengths=list(refs_lengths.values()) ) #, template=samfile)
-        warning_log_file = open(os.path.join(args.outfolder, "uLTRA_batch_{0}.stderr".format(batch_number)), "w")
-
 
+    warning_log_file = open(os.path.join(args.outfolder, "uLTRA_batch_{0}.stderr".format(process_id)), "w")
+    
+    classification_list = [0, 0, 0, 0, 0, 0, 0, 0] # entries: [aln_cov, 'FSM', 'unaligned', 'NO_SPLICE', 'Insufficient_junction_coverage_unclassified', 'ISM/NIC_known', 'NIC_novel', 'NNC']
+    # code: aln_cov (0), 'FSM' (1), 'unaligned' (2), 'NO_SPLICE' (3), 'Insufficient_junction_coverage_unclassified' (4), 'ISM/NIC_known' (5), 'NIC_novel' (6), 'NNC' (7)
+    class_to_offset = {'FSM' : 1, 'unaligned' : 2, 'NO_SPLICE' : 3, 'Insufficient_junction_coverage_unclassified' : 4, 'ISM/NIC_known' : 5, 'NIC_novel' : 6 , 'NNC': 7}
+
+    while True:
+        batch = input_queue.get()
+        # check for stop
+        if batch is None:
+            # add the signal back for other consumers
+            input_queue.put(batch)
+            # stop running
+            break
+
+        alignments_output = []
+
+        for b in batch[1]:
+            (read_acc, seq, hits, hits_rc) = b
+            mems = get_mems_from_input(hits)
+            mems_rc = get_mems_from_input(hits_rc)
+            read_seq_mod = help_functions.remove_read_polyA_ends(seq, args.reduce_read_ployA, 1)
 
-    # tiling_segment_to_gene, \
-    # tiling_parts_to_segments, tiling_gene_to_small_segments, \
-    # tiling_ref_segment_sequences = tiling_structures # unpacking tiling structures
+            upper_bound = annotate_guaranteed_optimal_bound(mems, False, max_intron_chr, max_global_intron)
+            upper_bound_rc = annotate_guaranteed_optimal_bound(mems_rc, True, max_intron_chr, max_global_intron)
+            # print()
+            processed_read_counter += 1
+            if processed_read_counter % 5000 == 0:
+                print('Processed {0} reads in consumer process {1}. Queue size: {2}'.format(processed_read_counter, process_id, input_queue.qsize()))
+            # do the chaining here immediately!
+            all_chainings = []
+            best_solution_value = 0
+            for (chr_id, chr_instance_index) , (upper_bound_cov, is_rc, all_mems_to_chromosome) in sorted(list(upper_bound.items()) + list(upper_bound_rc.items()), key = lambda x: x[1][0], reverse = True ): # mems.items():
+                if upper_bound_cov < best_solution_value*args.dropoff:
+                    break
+
+                max_allowed_intron = min(max_intron_chr[chr_id] + 20000, max_global_intron)
+
+                if len(all_mems_to_chromosome) < 90:
+                    solutions, mem_solution_value = colinear_solver.read_coverage(all_mems_to_chromosome, max_allowed_intron)
+                    quadratic_instance_counter += 1 
+                else:
+                    solutions, mem_solution_value = colinear_solver.n_logn_read_coverage(all_mems_to_chromosome)
+                    nlog_n_instance_counter += 1
 
-    classifications = defaultdict(str)
-    read_accessions_with_mappings = set()
-    processed_read_counter = 0
+                if mem_solution_value > best_solution_value:
+                    best_solution_value = mem_solution_value
 
-    for (read_acc, mems), (_, mems_rc) in zip(mem_wrapper.get_mem_records(mems_path,reads), mem_wrapper.get_mem_records(mems_path_rc, reads)):
-        # multiple = False
-        if read_acc not in reads: # if parallelization not all reads in mummer file are in read batches
-            continue
-        else:
-            read_seq_mod = help_functions.remove_read_polyA_ends(reads[read_acc], args.reduce_read_ployA, 1)
-        # print("instance sizes fw:", [ (chr_id, len(mm)) for chr_id, mm in mems.items()])
-        # print("instance sizes rc:", [ (chr_id, len(mm)) for chr_id, mm in mems_rc.items()])
-        # print()
-        # print()
-        # print(read_acc)
-        upper_bound = annotate_guaranteed_optimal_bound(mems, False, max_intron_chr, max_global_intron)
-        upper_bound_rc = annotate_guaranteed_optimal_bound(mems_rc, True, max_intron_chr, max_global_intron)
-        # print()
-        processed_read_counter += 1
-        if processed_read_counter % 5000 == 0:
-            print('Processed {0} reads in batch {1}'.format(processed_read_counter, batch_number))
-        # do the chaining here immediately!
-        all_chainings = []
-        best_solution_value = 0
-        for (chr_id, chr_instance_index) , (upper_bound_cov, is_rc, all_mems_to_chromosome) in sorted(list(upper_bound.items()) + list(upper_bound_rc.items()), key = lambda x: x[1][0], reverse = True ): # mems.items():
-            # print(read_acc, id_to_chr[chr_id], upper_bound_cov)
-            if upper_bound_cov < best_solution_value*args.dropoff:
-                # print("Breaking for", chr_id, is_rc, upper_bound_cov, "best:", best_solution_value, "read length:", len(read_seq_mod))
-                break
-            
-            # print("Processing", chr_id, is_rc, upper_bound_cov, "best:", best_solution_value, "read length:", len(read_seq_mod))
-            # for mem in all_mems_to_chromosome:
-            #     print(mem.exon_part_id, mem.x, mem.y, mem.c, mem.d, '\t', mem.val)
-            # print(len(all_mems_to_chromosome))
-
-
-            max_allowed_intron = min(max_intron_chr[chr_id] + 20000, max_global_intron)
-            # print("max_allowed_intron", max_allowed_intron, max_intron_chr[chr_id])
-            # print("LEM MEMS", len(all_mems_to_chromosome))
-            if len(all_mems_to_chromosome) < 90:
-                solutions, mem_solution_value = colinear_solver.read_coverage(all_mems_to_chromosome, max_allowed_intron)
-                quadratic_instance_counter += 1 
-            else:
-                solutions, mem_solution_value = colinear_solver.n_logn_read_coverage(all_mems_to_chromosome)
-                nlog_n_instance_counter += 1
+                for sol in solutions:
+                    all_chainings.append( (chr_id, sol, mem_solution_value, is_rc) )
 
-            if mem_solution_value > best_solution_value:
-                best_solution_value = mem_solution_value
-                # print("best now:", mem_solution_value)
-
-            # if len(solutions) > 1:
-            #     # print("More than 1 solution on chromosome")
-            #     # for sol in solutions:
-            #     #     print(mem_solution_value, [ (m.x, m.y) for m in sol])
-            #     # multiple = True
-
-            for sol in solutions:
-                all_chainings.append( (chr_id, sol, mem_solution_value, is_rc) )
-                # for mem in sol:
-                #     print(mem.exon_part_id, mem.x, mem.y, mem.c, mem.d, '\t', mem.val, "(sol)")
-            # print(all_chainings)
-        is_secondary =  False
-        is_rc =  False
-        if not all_chainings:
-            sam_output.main(read_acc, read_seq_mod, '*', 'unaligned', [], '*', '*', '*', alignment_outfile, is_rc, is_secondary, 0)
-            continue
-
-        # all_chainings = sorted(all_chainings, key=lambda x: x[2], reverse=True) 
-        all_chainings = sorted(all_chainings, key=lambda x:(-x[2],(x[1][-1].y - x[1][0].x))) 
-        # if multiple:
-        #     print(all_chainings)
-        best_chaining_score = all_chainings[0][2]
-        read_alignments = []
-        mam_solutions = set()
-        for i_nr_sol, (chr_id, mem_solution, chaining_score, is_rc) in enumerate(all_chainings):
-            # print(i_nr_sol, chr_id, chaining_score)
-            # if read_acc == "100:823|c8740d7a-53bd-4690-aa53-de3ebd003d20": #len(all_chainings) > 20: 
-            #     print(read_acc, len(all_chainings), chaining_score)
-            #     print(all_chainings)
-            # for c in all_chainings:
-            #     print(c[1][-1].y - c[1][0].x, c[1][0].x, c[1][-1].y)
-            #     sys.exit()
-            if chaining_score/float(best_chaining_score) < args.dropoff or i_nr_sol >= args.max_loc:
-                # print(chr_id, chaining_score, best_chaining_score, "NOT CONSIDERED")
-                # print(i_nr_sol, "lol")
-                break
-            # print(chr_id, chaining_score, best_chaining_score)
+            is_secondary =  False
+            is_rc =  False
+            if not all_chainings:
+                sam_aln_entry = sam_output.main(read_acc, read_seq_mod, '*', 'unaligned', [], '*', '*', '*', is_rc, is_secondary, 0)
+                alignments_output.append(sam_aln_entry)
 
-            if is_rc:
-                read_seq = help_functions.reverse_complement(read_seq_mod)
-            else:
-                read_seq = read_seq_mod
-            # print("mem solution:", is_rc, chaining_score, mem_solution)
-            # print()
-            # print()
-            # print(is_rc, mem_solution[0].x)
-            # print(mem_solution)
-            # print(read_seq)
-            non_covered_regions, mam_value, mam_solution = classify_read_with_mams.main(mem_solution, ref_segment_sequences, ref_flank_sequences, parts_to_segments, \
-                                                                                                                    segment_to_gene, gene_to_small_segments, \
-                                                                                                                    read_seq, warning_log_file, min_acc)
-            
-            # We can enter the if statement below because sometimes the MEM chaining finder will 
-            # return multiple optimal chainings that lead to the same mam_solution
-            if mam_solution in mam_solutions:
                 continue
 
-            mam_solutions.add(mam_solution)
-            # print("finished Mam solution:",mam_value, mam_solution)
-            # for zzz2 in mam_solution:
-            #     print(zzz2)
-            # print(non_covered_regions)
-            mam_sol_exons_length = sum([ mam.y - mam.x for mam in mam_solution])
-            # print(max_intron_size)
-            if mam_value > 0:
-                exons, created_ref_seq, predicted_exons, predicted_splices, covered = find_exons(chr_id, mam_solution, ref_exon_sequences, \
-                                                                                            ref_segment_sequences, ref_flank_sequences, all_splice_pairs_annotations)
-
-
-                classification, annotated_to_transcript_id = classify_alignment2.main(chr_id, predicted_splices, splices_to_transcripts, transcripts_to_splices, all_splice_pairs_annotations, all_splice_sites_annotations)
-                largest_intron_size = max([m2.x - m1.y for m1,m2 in zip(mam_solution[:-1], mam_solution[1:]) ]) if len(mam_solution) > 1 else 0
-                if largest_intron_size > max_allowed_intron and classification != 'FSM':
-                    # print(i_nr_sol, mem_solution[0].x, "HERE", largest_intron_size)
-                    # print()
-                    # print(read_acc)
-                    # print(classification, alignment_score/len(read_seq), "Score: {0}, old T: {1}, new T: {2}".format(alignment_score, 2*args.alignment_threshold*len(read_seq), len(read_seq)*8*args.alignment_threshold))
-                    continue
-
-                read_aln, ref_aln, alignment_score = get_exact_alignment(read_seq, created_ref_seq, mam_sol_exons_length)
-
-                # if classification != 'FSM' and len(non_covered_regions) >= 3 and (max(non_covered_regions[1:-1]) > args.non_covered_cutoff):
-                #     classification, alignment_score, non_covered_regions, \
-                #     read_aln, ref_aln, predicted_exons, annotated_to_transcript_id, covered = run_tiling_solution(mem_solution, tiling_ref_segment_sequences, ref_flank_sequences, tiling_parts_to_segments, \
-                #                         tiling_segment_to_gene, tiling_gene_to_small_segments, \
-                #                         read_seq, warning_log_file, min_acc, chr_id, ref_exon_sequences, \
-                #                         all_splice_pairs_annotations,
-                #                         splices_to_transcripts, transcripts_to_splices, \
-                #                         all_splice_sites_annotations, mam_sol_exons_length, alignment_score, \
-                #                         read_aln, ref_aln, classification, non_covered_regions, covered, predicted_exons, annotated_to_transcript_id)
-
+            all_chainings = sorted(all_chainings, key=lambda x:(-x[2],(x[1][-1].y - x[1][0].x))) 
+            best_chaining_score = all_chainings[0][2]
+            read_alignments = []
+            mam_solutions = set()
+            for i_nr_sol, (chr_id, mem_solution, chaining_score, is_rc) in enumerate(all_chainings):
+                if chaining_score/float(best_chaining_score) < args.dropoff or i_nr_sol >= args.max_loc:
+                    break
 
+                if is_rc:
+                    read_seq = help_functions.reverse_complement(read_seq_mod)
+                else:
+                    read_seq = read_seq_mod
 
-                if alignment_score < 2*args.alignment_threshold*len(read_seq) and classification != 'FSM': # match score * aln_threshold
-                    # print(i_nr_sol, mem_solution[0].x, "HERE2", chaining_score, alignment_score, 2*args.alignment_threshold*len(read_seq))
-                    # print()
-                    # print(read_acc)
-                    # print(read_aln)
-                    # print(ref_aln)
-                    # print(classification, alignment_score/len(read_seq), "Score: {0}, T: {1}".format(alignment_score, 2*args.alignment_threshold*len(read_seq)))
+                non_covered_regions, mam_value, mam_solution = classify_read_with_mams.main(mem_solution, ref_segment_sequences, ref_flank_sequences, parts_to_segments, \
+                                                                                                                        segment_to_gene, gene_to_small_segments, \
+                                                                                                                        read_seq, warning_log_file, min_acc)
+                
+                # We can enter the if statement below because sometimes the MEM chaining finder will 
+                # return multiple optimal chainings that lead to the same mam_solution
+                if mam_solution in mam_solutions:
                     continue
-                # print(classification)
-                # checing for internal (splice site) non covered regions
-                if len(non_covered_regions) >= 3 and (max(non_covered_regions[1:-1]) > args.non_covered_cutoff):
-                    classification = 'Insufficient_junction_coverage_unclassified'
-                coverage = covered / float(len(read_seq)) 
-                # print(len(read_alignments), read_alignments)
-                genome_start = mam_solution[0].x
-                genome_stop = mam_solution[-1].y
-                read_alignments.append( (alignment_score, genome_start, genome_stop, read_acc, chr_id, classification, predicted_exons, read_aln, ref_aln, annotated_to_transcript_id, is_rc, coverage) )
-
-            # else:
-            #     print(i_nr_sol, mem_solution[0].x, "OK", chaining_score, mam_value, mem_solution[-1].y - mem_solution[0].x, mem_solution[0].x)    
-        # if read_acc == "100:823|c8740d7a-53bd-4690-aa53-de3ebd003d20": #len(all_chainings) > 20: 
-        #     print(read_acc, len(all_chainings), chaining_score, chr_id, max_allowed_intron)
-        #     print(read_seq)
-        #     # print(all_chainings)
-        #     for c in all_chainings:
-        #         print(is_rc, c[2], c[1][-1].y - c[1][0].x, c[1][0].x, c[1][-1].y)
-        #     print("Nr alignments:", len(read_alignments))
-        #     for r in read_alignments:
-        #         print(r[0],r[1], r[2], r[3],r[4])
-        #     # sys.exit()
-
-            # elif 10*len(read_seq) < mam_sol_exons_length:
-            #     print("length ref: {0}, length query:{1}".format(mam_sol_exons_length, len(read_seq)))
-            #     print(read_acc, "to chr", chr_id)
-            #     print(read_seq)
-
-        ##################  Process alignments and decide primary
-        if len(read_alignments) == 0:
-            sam_output.main(read_acc, read_seq, '*', 'unaligned', [], '*', '*', '*', alignment_outfile, is_rc, is_secondary, 0)
-        else:
-            # sorted_wrt_alignement_score = sorted(read_alignments, key = lambda x: x[0], reverse = True)
-            sorted_wrt_alignement_score = sorted(read_alignments, key = lambda x: (-x[0], (x[2] - x[1]), x[5]))
-            # sorted_wrt_alignement_score = sorted(read_alignments, key = lambda x: (-(x[0] - 0.002*(x[2] - x[1])), len(x[5]) ))
-            # if len(read_alignments) > 1 and "FSM" in set( [r[5] for r in read_alignments]):
-            #     print(read_acc)
-            #     for r in sorted_wrt_alignement_score:
-            #         print(r[0], r[5], r[1], (r[2] - r[1]))
-            #         print(r[7])
-            #         print(r[8])
-            #     for c in all_chainings:
-            #         print(c[0], c[2], c[1][0].x, c[1][-1].y)
-            # sorted_wrt_alignement_score = sorted(read_alignments, key = lambda x: (x[5] != "FSM", -x[0], (x[2] - x[1])))
-            best_aln_sw_score = sorted_wrt_alignement_score[0][0]
-            more_than_one_alignment = True if len(sorted_wrt_alignement_score) > 1 else False
-
-            # if read_acc == "100:823|c8740d7a-53bd-4690-aa53-de3ebd003d20": #len(all_chainings) > 20: 
-            #     print()
-            #     print( "SORTED", best_aln_sw_score)
-            #     for r in sorted_wrt_alignement_score:
-            #         print(r[0],r[1], (r[2]-r[1]), r[5],r[6])
-            #     sys.exit()
-
-
-            for i, (alignment_score, genome_start, genome_stop, read_acc, chr_id, classification, predicted_exons, read_aln, ref_aln, annotated_to_transcript_id, is_rc, coverage) in enumerate(sorted_wrt_alignement_score):
-                if i == 0:
-                    is_secondary =  False
-                    assert alignment_score == best_aln_sw_score
-                    if more_than_one_alignment:
-                        if alignment_score == sorted_wrt_alignement_score[1][0]:
-                            map_score = 0
+
+                mam_solutions.add(mam_solution)
+                mam_sol_exons_length = sum([ mam.y - mam.x for mam in mam_solution])
+                if mam_value > 0:
+                    exons, created_ref_seq, predicted_exons, predicted_splices, covered = find_exons(chr_id, mam_solution, ref_exon_sequences, \
+                                                                                                ref_segment_sequences, ref_flank_sequences, all_splice_pairs_annotations)
+
+
+                    classification, annotated_to_transcript_id = classify_alignment2.main(chr_id, predicted_splices, splices_to_transcripts, transcripts_to_splices, all_splice_pairs_annotations, all_splice_sites_annotations)
+                    largest_intron_size = max([m2.x - m1.y for m1,m2 in zip(mam_solution[:-1], mam_solution[1:]) ]) if len(mam_solution) > 1 else 0
+                    if largest_intron_size > max_allowed_intron and classification != 'FSM':
+                        continue
+
+                    read_aln, ref_aln, alignment_score = get_exact_alignment(read_seq, created_ref_seq, mam_sol_exons_length)
+
+                    if alignment_score < 2*args.alignment_threshold*len(read_seq) and classification != 'FSM': # match score * aln_threshold
+                        continue
+
+                    # checing for internal (splice site) non covered regions
+                    if len(non_covered_regions) >= 3 and (max(non_covered_regions[1:-1]) > args.non_covered_cutoff):
+                        classification = 'Insufficient_junction_coverage_unclassified'
+                    coverage = covered / float(len(read_seq)) 
+                    genome_start = mam_solution[0].x
+                    genome_stop = mam_solution[-1].y
+                    read_alignments.append( (alignment_score, genome_start, genome_stop, read_acc, chr_id, classification, predicted_exons, read_aln, ref_aln, annotated_to_transcript_id, is_rc, coverage) )
+
+
+            ##################  Process alignments and decide primary
+            if len(read_alignments) == 0:
+                sam_aln_entry = sam_output.main(read_acc, read_seq, '*', 'unaligned', [], '*', '*', '*', is_rc, is_secondary, 0)
+                alignments_output.append(sam_aln_entry)
+            else:
+                sorted_wrt_alignement_score = sorted(read_alignments, key = lambda x: (-x[0], (x[2] - x[1]), x[5]))
+                best_aln_sw_score = sorted_wrt_alignement_score[0][0]
+                more_than_one_alignment = True if len(sorted_wrt_alignement_score) > 1 else False
+
+                for i, (alignment_score, genome_start, genome_stop, read_acc, chr_id, classification, predicted_exons, read_aln, ref_aln, annotated_to_transcript_id, is_rc, coverage) in enumerate(sorted_wrt_alignement_score):
+                    if i == 0:
+                        is_secondary =  False
+                        assert alignment_score == best_aln_sw_score
+                        if more_than_one_alignment:
+                            if alignment_score == sorted_wrt_alignement_score[1][0]:
+                                map_score = 0
+                            else:
+                                map_score = 60  # TODO: predict this value with formula instead.                           
                         else:
-                            map_score = 60  # TODO: predict this value with formula instead.                           
+                            map_score = 60
+                        # classifications[read_acc] = (classification, coverage )
+                        classification_list[0] += coverage
+                        classification_list[class_to_offset[classification]] += 1
                     else:
-                        map_score = 60
-                    classifications[read_acc] = (classification, coverage )
-                else:
-                    is_secondary =  True
-                    map_score = 0
+                        is_secondary =  True
+                        map_score = 0
 
 
-                sam_output.main(read_acc, read_seq, id_to_chr[chr_id], classification, predicted_exons, read_aln, ref_aln, annotated_to_transcript_id, alignment_outfile, is_rc, is_secondary, map_score, aln_score = alignment_score)
-                read_accessions_with_mappings.add(read_acc)
+                    sam_aln_entry = sam_output.main(read_acc, read_seq, id_to_chr[chr_id], classification, predicted_exons, read_aln, ref_aln, annotated_to_transcript_id, is_rc, is_secondary, map_score, aln_score = alignment_score)
+                    alignments_output.append(sam_aln_entry)
+        
+        output_sam_buffer.put(alignments_output)
 
+    classification_and_aln_cov.put(classification_list)
+    print('Process:', classification_list)
 
-    alignment_outfile.close()
     warning_log_file.close()
     print("Number of instances solved with quadratic collinear chainer solution:", quadratic_instance_counter)
     print("Number of instances solved with n*log n collinear chainer solution:", nlog_n_instance_counter)
-    # print(alignment_outfile.filename, dir(alignment_outfile))
-    return classifications, alignment_outfile.filename
+    # return classifications
 
 
 
 
-def align_single_helper(arguments):
-    # for v in arguments:
-    #     args = v
-    # print(len(arguments))
-    return align_single(*arguments)
-    # print(len(args))
-    # read_data, auxillary_data = args[0], args[1]
-    # align_single()
-    # return 1
+# def align_single_helper(arguments):
+#     return align_single(*arguments)
 
 
 
-def align_parallel(read_data, refs_lengths, args):
-    ####### parallelize alignment #########
-    # pool = Pool(processes=mp.cpu_count())
-    original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
-    signal.signal(signal.SIGINT, original_sigint_handler)
-
-    start_multi = time()
-    pool = Pool(processes=int(args.nr_cores))
-    try:
-        res = pool.map_async(align_single_helper, [ (d, refs_lengths, args, i) for i,d in enumerate(read_data)] )
-        results =res.get(999999999) # Without the timeout this blocking call ignores all signals.
-    except KeyboardInterrupt:
-        print("Caught KeyboardInterrupt, terminating workers")
-        pool.terminate()
-        sys.exit()
-    else:
-        pool.close()
-    pool.join()
 
-    classifications = defaultdict(str)
-    alignment_outfiles = []
-    for r, alignment_outfile_name in results:
-        alignment_outfiles.append(alignment_outfile_name)
-        for acc in r:
-            classifications[acc] = r[acc]
-        # print(r)
-    print("Time elapesd multiprocessing:", time() - start_multi)  
-    return classifications, alignment_outfiles
+# def align_parallel(read_data, args):
+#     ####### parallelize alignment #########
+#     # pool = Pool(processes=mp.cpu_count())
+#     original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
+#     signal.signal(signal.SIGINT, original_sigint_handler)
+
+#     start_multi = time()
+#     pool = Pool(processes=int(args.nr_cores))
+#     try:
+#         res = pool.map_async(align_single_helper, [ (d, args, i) for i,d in enumerate(read_data)] )
+#         results =res.get(999999999) # Without the timeout this blocking call ignores all signals.
+#     except KeyboardInterrupt:
+#         print("Caught KeyboardInterrupt, terminating workers")
+#         pool.terminate()
+#         sys.exit()
+#     else:
+#         pool.close()
+#     pool.join()
+
+#     # classifications = defaultdict(str)
+#     # for r in results:
+#     #     for acc in r:
+#     #         classifications[acc] = r[acc]
+#     #     # print(r)
+#     # print("Time elapesd multiprocessing:", time() - start_multi)  
+#     # return classifications
```

### Comparing `ultra_bioinformatics-0.0.4.2/modules/classify_alignment2.py` & `ultra_bioinformatics-0.1/modules/classify_alignment2.py`

 * *Files identical despite different names*

### Comparing `ultra_bioinformatics-0.0.4.2/modules/classify_read_with_mams.py` & `ultra_bioinformatics-0.1/modules/classify_read_with_mams.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,15 @@
                 # segm_id = all_exon_ids.pop()
                 mam_tuple = mam(e_start, e_stop, start, stop, 
                         score, 0, min_segment_length, str(segm_id) + annot_label, ref_chr_id)
                 mam_instance.append(mam_tuple)
     
 
 
-def main(solution, ref_segment_sequences, ref_flank_sequences, parts_to_segments, segment_to_gene, gene_to_small_segments, read_seq, warning_log_file, min_acc, is_tiling_instance = False):
+def main(solution, ref_segment_sequences, ref_flank_sequences, parts_to_segments, segment_to_gene, gene_to_small_segments, read_seq, warning_log_file, min_acc):
     """
         NOTE: if paramerer task = 'path' is given to edlib_alignment function calls below, it will give exact accuracy of the aligmnent but the program will be ~40% slower to calling task = 'locations'
             Now we are approxmating accuracy by dividing by start and end of the reference coordinates of the alignment. This is not good approw if there is a large instertion
             in the exon w.r.t. the read.
     """
     # chained_parts_seq = []
     # chained_parts_ids = []
@@ -554,15 +554,15 @@
     #  sorted_mems = [ mem(x,y,c,d,val,j,e_id) for j, (x, y, c, d, val, e_id) in enumerate(coordinate_sorted_tuples) ]
     mam_instance  = [mam(m.x, m.y, m.c, m.d, m.val, j, m.min_segment_length, m.mam_id, m.ref_chr_id) for j, m in enumerate(mam_instance) ]  # assingn an index j based on the hit choordinate
     ###################################################################################################
     ###################################################################################################
     ###################################################################################################
     # print("MAM INSTANCE", mam_instance)
     if mam_instance:
-        if is_tiling_instance and len(mam_instance) > 100:
+        if len(mam_instance) > 200:
             # mam_solution_old, value_old, unique_old = colinear_solver.read_coverage_mam_score(mam_instance, overlap_threshold = 5)
             mam_solution, value, unique = colinear_solver.n_logn_read_coverage_mams(mam_instance, overlap_threshold = 5)
             # if mam_solution != mam_solution2:
             #     print("OLD")
             #     for zzz2 in mam_solution:
             #         print(zzz2)
             #     print()
```

### Comparing `ultra_bioinformatics-0.0.4.2/modules/colinear_solver.py` & `ultra_bioinformatics-0.1/modules/colinear_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,16 +174,16 @@
         so n^2 time complexity instead of O(n log n).
 
         each mem is an Namedtuple. python object
 
     """
     # assert mems == sorted(mems, key = lambda x: x.y )
 
-    if len(mems) > 1000:
-        print('MEM',len(mems))
+    # if len(mems) > 1000:
+    #     print('MEM',len(mems))
 
     # print("Going in to mem chaining:", mems)
     T = [ (v.d, v.val)  for v in mems]
     I = [ (v.d, v.val)  for v in mems]
     
     # T_dict = {mems[i][3] : -10000 for i in range(len(mems))}
     # T_dict[0] = -10000
@@ -286,16 +286,16 @@
 
     # assert mams == sorted(mams, key=lambda x: x.y)
     # mams = sorted(mams, key = lambda x: x.y )
 
     # print("MAM INSTANCE", mams)
     # for mam in mams:
     #     print(mam.mam_id, mam.x, mam.y, mam.c, mam.d, '\t', mam.val, mam.min_segment_length)
-    if len(mams) > 1000:
-        print('MAM',len(mams))
+    # if len(mams) > 1000:
+    #     print('MAM',len(mams))
     T = [ (v.d, v.val)  for v in mams]
     I = [ (v.d, v.val)  for v in mams]
     
     # T_dict = {mams[i][3] : -10000 for i in range(len(mams))}
     # T_dict[0] = -10000
     # I_dict = {mams[i][3] : -10000 for i in range(len(mams))}
     # I_dict[0] = -10000
@@ -395,14 +395,18 @@
     """
         Algorithm 15.1 in Genome scale algorithmic design, Makinen et al.
 
         Using Binary search trees for range max queries,
         so n log n time complexity. Each mem is an Namedtuple. python object
 
     """
+    
+    # if len(mams) > 1000:
+    #     print('MAM',len(mams))
+
     # assert mams == sorted(mams, key=lambda x: x.y)
     # for mam in mams:
     #     print(mam.mam_id, mam.x, mam.y, mam.c, mam.d, '\t', mam.val, mam.min_segment_length)
     # overlap_threshold = 20
     T_leafs = make_leafs_power_of_2(mams)
     I_leafs = make_leafs_power_of_2(mams)
     n = len(T_leafs)
```

### Comparing `ultra_bioinformatics-0.0.4.2/modules/create_augmented_gene.py` & `ultra_bioinformatics-0.1/modules/create_augmented_gene.py`

 * *Files identical despite different names*

### Comparing `ultra_bioinformatics-0.0.4.2/modules/help_functions.py` & `ultra_bioinformatics-0.1/modules/help_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,17 +182,17 @@
         else:
             raise
 
 def parasail_alignment(s1, s2, match_score = 2, mismatch_penalty = -2, opening_penalty = 3, gap_ext = 1):
     user_matrix = parasail.matrix_create("ACGT", match_score, mismatch_penalty)
     result = parasail.sg_trace_scan_16(s1, s2, opening_penalty, gap_ext, user_matrix)
     if result.saturated:
-        print("SATURATED!",len(s1), len(s2))
+        # print("SATURATED!",len(s1), len(s2))
         result = parasail.sg_trace_scan_32(s1, s2, opening_penalty, gap_ext, user_matrix)
-        print("computed 32 bit instead")
+        # print("computed 32 bit instead")
 
     # difference in how to obtain string from parasail between python v2 and v3... 
     if sys.version_info[0] < 3:
         cigar_string = str(result.cigar.decode).decode('utf-8')
     else:
         cigar_string = str(result.cigar.decode, 'utf-8')
     s1_alignment, s2_alignment, cigar_tuples = cigar_to_seq(cigar_string, s1, s2)
@@ -243,17 +243,17 @@
     # print()
     return s1_alignment, s2_alignment, cigar_string, cigar_tuples, result.score
 
 def parasail_local(s1, s2, match_score = 2, mismatch_penalty = -2, opening_penalty = 3, gap_ext = 1):
     user_matrix = parasail.matrix_create("ACGT", match_score, mismatch_penalty)
     result = parasail.sw_trace_scan_16(s1, s2, opening_penalty, gap_ext, user_matrix)
     if result.saturated:
-        print("SATURATED!",len(s1), len(s2))
+        # print("SATURATED!",len(s1), len(s2))
         result = parasail.sg_trace_scan_32(s1, s2, opening_penalty, gap_ext, user_matrix)
-        print("computed 32 bit instead")
+        # print("computed 32 bit instead")
 
     # difference in how to obtain string from parasail between python v2 and v3... 
     if sys.version_info[0] < 3:
         cigar_string = str(result.cigar.decode).decode('utf-8')
     else:
         cigar_string = str(result.cigar.decode, 'utf-8')
     s1_alignment, s2_alignment, cigar_tuples = cigar_to_seq(cigar_string, s1[result.cigar.beg_query:result.end_query], s2[result.cigar.beg_ref: result.end_ref])
```

### Comparing `ultra_bioinformatics-0.0.4.2/modules/mem_wrapper.py` & `ultra_bioinformatics-0.1/modules/seed_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,86 @@
 import os
 import subprocess
-from sys import stdout, exit
+import sys
+import gzip
 
 from collections import defaultdict
 from collections import namedtuple
 
-mem = namedtuple('Mem', ['x', 'y', 'c', 'd', 'val', 'j', "exon_part_id"])
-globals()[mem.__name__] = mem # Global needed for multiprocessing
+# mem = namedtuple('Mem', ['x', 'y', 'c', 'd', 'val', 'j', "exon_part_id"])
+# globals()[mem.__name__] = mem # Global needed for multiprocessing
 
 def find_mems_mummer(outfolder, read_path, refs_path, mummer_out_path, min_mem):
     with open(mummer_out_path, "w") as output_file:
         # print('Running spoa...', end=' ')
-        stdout.flush()
+        sys.stdout.flush()
         null = open(os.path.join(outfolder, "mummer_errors.1") , "w")
         subprocess.check_call([ 'mummer',   '-maxmatch', '-l' , str(min_mem),  refs_path, read_path], stdout=output_file, stderr=null)
         # print('Done.')
-        stdout.flush()
+        sys.stdout.flush()
     output_file.close()
 
 
 def find_mems_slamem(outfolder, read_path, refs_path, out_path, min_mem):
     # time slaMEM -l 14 /Users/kxs624/tmp/ULTRA/human_test/refs_sequences.fa /Users/kxs624/tmp/ULTRA/human_test_new_flanking_strat/reads_tmp.fq -o /Users/kxs624/tmp/ULTRA/human_test/slamem_test.tx
     # with open(out_path, "w") as output_file:
     tmp = out_path.split("seeds_batch_")[1]
     batch_id =  tmp.split('.')[0]
-    stdout.flush()
+    sys.stdout.flush()
     stderr_file = open(os.path.join(outfolder, "slamem_stderr_{0}.1".format(batch_id)) , "w")
     stdout_file = open(os.path.join(outfolder, "slamem_stdout_{0}.1".format(batch_id)) , "w")
     try: # slaMEM throws error if no MEMs are found in any of the sequences
         subprocess.check_call([ 'slaMEM', '-l' , str(min_mem),  refs_path, read_path, '-o', out_path ], stdout=stdout_file, stderr=stderr_file)
         print("Using SLAMEM")
     except:
         find_mems_mummer(outfolder, read_path, refs_path, out_path, min_mem)
         print("Using MUMMER")
 
     # print('Done.')
-    stdout.flush()
+    sys.stdout.flush()
     # output_file.close()
 
 
-def find_nams_strobemap(outfolder, read_path, refs_path, out_path, nr_cores, min_mem):
-    # /usr/bin/time -l ./StrobeMap -n 2 -k 9 -w 30 -t 3 -s  -o /Users/kxs624/tmp/ULTRA/human_test/refs_sequences.fa /Users/kxs624/tmp/ULTRA/human_test_new_flanking_strat/reads_tmp.fq
-    # StrobeMap -n 2 -k 9 -w 30 -t 3 -s  -o ~/tmp/STROBEMERS/multithreading/ /Users/kxs624/tmp/ULTRA/dros_tmp/refs_sequences.fa /Users/kxs624/tmp/ULTRA/dros_test/reads_16xrep.fa
-    # with open(out_path, "w") as output_file:
-    stdout.flush()
-    stderr_file = open(os.path.join(outfolder, "strobemap_stderr.1") , "w")
-    stdout_file = open(os.path.join(outfolder, "strobemap_stdout.1") , "w")
-    try: # slaMEM throws error if no MEMs are found in any of the sequences
-        subprocess.check_call([ 'StrobeMap', '-n' , "2", '-k' , '10', '-v' , "11", '-w' , "35", '-C' , '500', '-L' , '1000', '-S', '-t', str(nr_cores), '-s', '-o', outfolder, refs_path, read_path ], stdout=stdout_file, stderr=stderr_file)
-        print("Using StrobeMap")
-        print([ 'StrobeMap', '-n' , "2", '-k' , '10', '-v' , "11", '-w' , "35", '-C' , '500', '-L' , '1000', '-S', '-t', str(nr_cores), '-s', '-o', outfolder, refs_path, read_path ])
+def find_nams_namfinder(outfolder, read_path, refs_path, out_path, nr_cores, strobe_size, thinning_level):
+    sys.stdout.flush()
+    outfile = os.path.join(outfolder, "seeds.txt")
+    if thinning_level == 0:
+        s = strobe_size
+        l = strobe_size
+        u = strobe_size + 1 # seems to be ok value based on some tests
+    elif thinning_level == 1: # expected seed distance: 3
+        s = strobe_size - 2
+        l = (strobe_size + 1)//3 # Need to scale down offsets since seeds subsampled
+        u = (strobe_size + 1)//3 + 1 # seems to be ok value based on some tests
+    elif thinning_level == 2: # expected seed distance: 5
+        s = strobe_size - 4 
+        l = (strobe_size + 1)//5 # Need to scale down offsets since seeds subsampled
+        u = (strobe_size + 1)//5 +1 # seems to be ok value based on some tests
+
+    stderr = open('/dev/null', 'r')
+    stdout = open('/dev/null', 'r')
+    try:
+        res = subprocess.run(['namfinder', '--help'], check = True, stdout = stdout, stderr = stderr)
     except:
-        find_mems_slamem(outfolder, read_path, refs_path, out_path, min_mem)
-        print("An unexpected error happend in StrobeMap, check error log at:", stderr_file)
-        print("If you beileive this is a bug in StrobeMap, report an issue at: https://github.com/ksahlin/strobemers")
-        print("You can always sidestep this issue by providing another seed finder to uLTRA, i.e., remove option --use_NAM_seeds.")
+        print ('Command "namfinder --help" returned an error. Check your installation of namfinder')
         sys.exit()
-    stdout.flush()
-
-# def parse_results(mems_path):
-#     # file = open(os.path.join(mems_folder, "mummer_mems.txt"), 'r')
-#     mems_db = {}
-#     # read_mems_tmp = {}
-
-#     for i, line in enumerate(open(mems_path, 'r')):
-#         if line[0] == '>':
-#             if i == 0:
-#                 read_acc = line.split()[1].strip()  # mems_db[line.split()[1].strip)()] = [] 
-#             else:
-#                 mems_db[read_acc] = read_mems_tmp 
-#                 read_acc = line.split()[1].strip() 
-            
-#             read_mems_tmp = defaultdict(list)
-
-#         else:
-#             vals =  line.split() #11404_11606           1     11405       202
-#             exon_part_id = vals[0]
-#             chr_id, ref_coord_start, ref_coord_end = exon_part_id.split('^')
-#             mem_len = int(vals[3])
-#             mem_ref_exon_part_start = int(vals[1])
-#             mem_read_start = int(vals[2])
-#             # convert to 0-indexed as python, however last coordinate is inclusive of the hit, not as in python end-indexing
-#             mem_tuple = mem(int(ref_coord_start) + mem_ref_exon_part_start - 1, int(ref_coord_start) + mem_ref_exon_part_start -1 + mem_len - 1,
-#                             mem_read_start-1, mem_read_start-1 + mem_len - 1, 
-#                             mem_len, None, exon_part_id)
-            
-#             read_mems_tmp[chr_id].append( mem_tuple )
-#         # print(line)
-#     # add last read
-#     mems_db[read_acc] = read_mems_tmp 
-
-
-#     return mems_db
 
+    stderr_file = os.path.join(outfolder, "namfinder_stderr.1")
+    stdout_file = os.path.join(outfolder, "seeds.txt.gz") 
+    cmd = " ".join(c for c in [ 'namfinder', '-k' , str(strobe_size), '-s' , str(s), '-l' , str(l), '-u' , str(u), '-C' , '500', '-L' , '1000', '-t', str(nr_cores), '-S', refs_path, read_path, "2>", stderr_file, "|", "gzip", "-1", "--stdout", ">", stdout_file ])
+
+    print('RUNNING NAMFINDER USING COMMAND:')
+    print(cmd)
+
+    returncode = os.system(cmd)
+    if returncode != 0:
+        print("An unexpected error happend in namfinder, check error log at:", stderr_file)
+        print("If you beileive this is a bug in namfinder, report an issue at: https://github.com/ksahlin/namfinder or report in the uLTRA repository")
+        sys.exit()
+    return stdout_file
 
 def get_mem_records(mems_path, reads):
     '''
         Reads contains all the relevant reads in the batch to read mems from 
     '''
     relevant = False
     relevant_read_cnt = 0
@@ -132,32 +116,65 @@
                 mem_len = int(vals[3])
                 # convert to 0-indexed reference as in python
                 # however, for MEM length last coordinate is inclusive of the hit in MEM solvers, not as in python end-indexing
                 mem_ref_exon_part_start = int(vals[1]) - 1
                 mem_read_start = int(vals[2]) - 1
                 ref_coord_start = int(ref_coord_start) # has already been 0-indexed when constructing parts
                 mem_genome_start = ref_coord_start + mem_ref_exon_part_start
-                
-                
-                # mem_tuple = mem(int(ref_coord_start) - 1 + mem_ref_exon_part_start - 1, int(ref_coord_start) - 1 + mem_ref_exon_part_start -1 + mem_len - 1,
-                #                 mem_read_start-1, mem_read_start-1 + mem_len - 1, 
-                #                 mem_len, None, exon_part_id)
-                # read_mems_tmp[chr_id].append( mem_tuple )
+                                
                 info_tuple = ( mem_genome_start, mem_genome_start + mem_len - 1,
                                 mem_read_start, mem_read_start + mem_len - 1, 
                                 mem_len, exon_part_id)
                 read_mems_tmp[chr_id].append( info_tuple )
 
 
     for chr_id in list(read_mems_tmp.keys()):
         coordinate_sorted_tuples = sorted(read_mems_tmp[chr_id], key = lambda x: x[1])
         sorted_mems = [ mem(x,y,c,d,val,j,e_id) for j, (x, y, c, d, val, e_id) in enumerate(coordinate_sorted_tuples) ]
         read_mems_tmp[chr_id] = sorted_mems
     print("READ {0} RECORDS.".format(relevant_read_cnt))
     yield read_acc, read_mems_tmp
 
 
-# def find_file_positions(read_pos_list, mummer_out_path, mummer_out_path_rc):
-#     print(read_pos_list)
 
+def read_seeds(seeds):
+    curr_acc = ''
+    curr_acc_rev = ''
+    is_rc = False
+    nr_reads = 0
+    hits = []
+    hits_rc = []
+
+    for i, encoded_line in enumerate(gzip.open(seeds, 'rb')):
+        line = encoded_line.decode('utf-8')
+        if line[0] == '>':
+            if curr_acc and curr_acc_rev:
+                yield curr_acc, hits, curr_acc_rev, hits_rc
+
+                # Reset
+                curr_acc = ''
+                curr_acc_rev = ''
+                is_rc = False
+                hits = []
+                hits_rc = []
+
+            if 'Reverse' in line:
+                curr_acc_rev = line[1:].strip()
+                is_rc = True
+            else:
+                curr_acc = line[1:].strip()
+                is_rc = False
+
+            nr_reads += 1
+
+        elif is_rc:
+            hits_rc.append(line)
+        else:
+            hits.append(line)
+
+
+    # Last record
+    if curr_acc and curr_acc_rev:        
+        yield curr_acc, hits, curr_acc_rev, hits_rc
 
+    print("READ {0} RECORDS (FW and RC counted as 2 records).".format(nr_reads))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ultra_bioinformatics-0.0.4.2/modules/prefilter_genomic_reads.py` & `ultra_bioinformatics-0.1/modules/prefilter_genomic_reads.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     minimap2_samfile_path = os.path.join(outfolder, "minimap2.sam")
     with open(minimap2_samfile_path, "w") as output_file:
         # print('Running spoa...', end=' ')
         sys.stdout.flush()
         stderr_file = open(os.path.join(outfolder, "minimap2_errors.1") , 'w')
         # minimap2 --eqx -t 62 -ax splice -k13 -w 5 -G 500k {input.index} {input.fastq}
         subprocess.check_call([ 'minimap2',  '-ax', 'splice', '--eqx' , '-k', str(k_size), '-t', str(nr_cores), refs_path, read_path], stdout=output_file, stderr=stderr_file)
-        # print('Done.')
         sys.stdout.flush()
     output_file.close()
     return minimap2_samfile_path
 
 def get_exons_from_cigar(read):
     # https://pysam.readthedocs.io/en/latest/api.html
     # M   BAM_CMATCH  0
@@ -79,72 +78,64 @@
     min_stop = min(b, d)
     return min_stop - max_start
 
 def is_overlapping(a_start,a_stop, b_start,b_stop):
     return (int(a_start) <= int(b_start) <= int(a_stop) )  or (int(a_start) <= int(b_stop) <= int(a_stop)) or (int(b_start) <= int(a_start) <= int(a_stop) <= int(b_stop) )
 
 
-def parse_alignments_and_mask(minimap2_samfile_path, indexed_regions, genomic_frac_cutoff):
+def filter_reads_to_align(minimap2_samfile_path, indexed_regions, outfolder, genomic_frac_cutoff):
     SAM_file = pysam.AlignmentFile(minimap2_samfile_path, "r", check_sq=False)
-    reads_unindexed = {}
-    reads_indexed = {}
+
+    reads_to_align = open(os.path.join(outfolder, "reads_after_genomic_filtering.fasta"), "w")
+    unindexed_aligned = pysam.AlignmentFile(os.path.join(outfolder, "unindexed.sam"), "w", template=SAM_file)
+    indexed_aligned = pysam.AlignmentFile(os.path.join(outfolder, "indexed.sam"), "w", template=SAM_file)
+
+    # reads_unindexed = {}
+    # reads_indexed = {}
+    nr_reads_unindexed = 0 
+
     for read in SAM_file.fetch(until_eof=True):
         if read.flag == 0 or read.flag == 16:
 
             aligned_choordinates = get_exons_from_cigar(read)
             total_overlap = 0
             total_aligned_length = 0
             for (a_start, a_stop) in aligned_choordinates:
                 overlaps = indexed_regions[read.reference_name].overlap(a_start, a_stop)
                 for ovl in overlaps: #continue here to get sizxe of overlap
-                    # print(ovl.begin, ovl.end)
                     total_overlap += overlap_size(a_start, a_stop, ovl.begin, ovl.end)
-                # print("overlaps", overlaps)
-                # total_overlap += overlaps
                 total_aligned_length += a_stop - a_start
 
-            # is_exonic = 1 if indexed_regions[reference_name].overlaps(reference_start, reference_end) else 0
-            # print(read.query_name, "unindexed portion:", 1 - (total_overlap/total_aligned_length))
             if 1 - (total_overlap/total_aligned_length) > genomic_frac_cutoff:
-                reads_unindexed[read.query_name] = read
+                read.set_tag('XA', "")
+                read.set_tag('XC', "uLTRA_unindexed")
+                unindexed_aligned.write(read)
+                # reads_unindexed[read.query_name] = read
+                nr_reads_unindexed += 1
             else:
-                reads_indexed[read.query_name] = read
-
-    return reads_unindexed, reads_indexed, SAM_file
-
-
-def print_read_categories(reads_unindexed, reads_indexed, reads, outfolder, SAM_file):
-    reads_to_align = open(os.path.join(outfolder, "reads_after_genomic_filtering.fasta"), "w")
-    unindexed_aligned = pysam.AlignmentFile(os.path.join(outfolder, "unindexed.sam"), "w", template=SAM_file)
-    indexed_aligned = pysam.AlignmentFile(os.path.join(outfolder, "indexed.sam"), "w", template=SAM_file)
-
-    for acc, (seq, _) in help_functions.readfq(open(reads,"r")):
-        if acc in reads_unindexed:
-            read = reads_unindexed[acc]
-            read.set_tag('XA', "")
-            read.set_tag('XC', "uLTRA_unindexed")
-            unindexed_aligned.write(read)
-        else:
-            reads_to_align.write(">{0}\n{1}\n".format(acc, seq))
-            if acc in reads_indexed:
-                read = reads_indexed[acc]
+                seq = help_functions.reverse_complement(read.query_sequence) if read.is_reverse else read.query_sequence
+                reads_to_align.write(">{0}\n{1}\n".format(read.query_name, seq))
                 indexed_aligned.write(read)
+                # reads_indexed[read.query_name] = read
+        
+        elif read.flag == 4: # unmapped
+            reads_to_align.write(">{0}\n{1}\n".format(read.query_name, read.query_sequence))
+
 
     unindexed_aligned.close()
     indexed_aligned.close()
     reads_to_align.close()
-    return reads_to_align.name
 
+    return nr_reads_unindexed, reads_to_align.name
 
 
 def main(ref_part_sequences, ref, reads, outfolder, indexfolder, nr_cores, genomic_frac_cutoff, k_size):
     indexed_regions = get_ultra_indexed_choordinates(ref_part_sequences, indexfolder, outfolder)
     minimap2_samfile_path = align_with_minimap2(ref, reads, outfolder, nr_cores, k_size)
-    reads_unindexed, reads_indexed, SAM_file = parse_alignments_and_mask(minimap2_samfile_path, indexed_regions, genomic_frac_cutoff)
-    path_reads_to_align = print_read_categories(reads_unindexed, reads_indexed, reads, outfolder, SAM_file)
-    return len(reads_unindexed), path_reads_to_align
-
+    print('minimap2 done.')
+    nr_reads_unindexed, path_reads_to_align = filter_reads_to_align(minimap2_samfile_path, indexed_regions, outfolder, genomic_frac_cutoff)
+    return nr_reads_unindexed, path_reads_to_align
```

### Comparing `ultra_bioinformatics-0.0.4.2/modules/range_query_max_search_tree.py` & `ultra_bioinformatics-0.1/modules/range_query_max_search_tree.py`

 * *Files identical despite different names*

### Comparing `ultra_bioinformatics-0.0.4.2/modules/sam_output.py` & `ultra_bioinformatics-0.1/modules/sam_output.py`

 * *Files 22% similar despite different names*

```diff
@@ -124,19 +124,21 @@
 #         m = m_rev[::-1]
 #         add_N_end  = int(m[:-1])
 #         c = c[:-len(m)]
 #     return c, add_N_end
 
 
 def get_genomic_cigar(read_aln, ref_aln, predicted_exons):
-    # print('here', read_aln)
-    # print('here', ref_aln)
+    # print('read_aln', read_aln)
+    # print('ref_aln', ref_aln)
+    # print('predicted_exons', predicted_exons)
     segments = get_segments(read_aln, ref_aln, predicted_exons)
+    # print('segments', segments)
     cigars, start_offset = get_cigars(segments)
-    # print('cigar segments', cigars)
+    # print('cigar segments', cigars, start_offset)
 
     # ######## ORIGINAL  ###########################
     # for c in cigars:
     #     print(c)
     genomic_cigar = []
     intron_lengths = [e2[0] - e1[1] for e1, e2 in zip(predicted_exons[:-1], predicted_exons[1:])]
     # print(intron_lengths)
@@ -206,53 +208,108 @@
     ed_types = {"X", "I", "D"}
     for length_, type_ in cigar_tuples:
         if type_ in ed_types:
             ed += length_
     return ed 
 
 
-def main(read_id, read_seq, ref_id, classification, predicted_exons, read_aln, ref_aln, annotated_to_transcript_id, alignment_outfile, is_rc, is_secondary, map_score, aln_score = 0):
-    # print(ref_id, classification, predicted_exons, read_aln, ref_aln, alignment_outfile)
-    read_sam_entry = pysam.AlignedSegment(alignment_outfile.header)
+# def main(read_id, read_seq, ref_id, classification, predicted_exons, read_aln, ref_aln, annotated_to_transcript_id, alignment_outfile, is_rc, is_secondary, map_score, aln_score = 0):
+#     # print(ref_id, classification, predicted_exons, read_aln, ref_aln, alignment_outfile)
+#     read_sam_entry = pysam.AlignedSegment(alignment_outfile.header)
+#     if classification != 'unaligned':
+#         genomic_cigar, start_offset = get_genomic_cigar(read_aln, ref_aln, predicted_exons)
+#         # if genomic_cigar == "":
+#         #     print(classification, is_rc, is_secondary, aln_score)
+#         #     print('genomic cigar:', genomic_cigar, read_id)
+#         #     print(read_aln)
+#         #     print(ref_aln)
+#         #     print(predicted_exons)
+#         if is_secondary and is_rc:
+#             read_sam_entry.flag = 256 + 16 
+#         elif is_secondary:
+#             read_sam_entry.flag = 256
+#         elif is_rc:
+#             read_sam_entry.flag = 16 
+#         else:
+#             read_sam_entry.flag = 0 
+
+#         read_sam_entry.reference_name = ref_id
+#         read_sam_entry.mapping_quality = 60 # TODO: calculate mapping quality 
+
+#         read_sam_entry.cigarstring = genomic_cigar 
+#         read_sam_entry.reference_start = predicted_exons[0][0] + start_offset
+#         read_sam_entry.mapping_quality = map_score 
+#         # print(predicted_exons[0][0], start_offset)
+#         read_sam_entry.set_tag('XA', annotated_to_transcript_id)
+#         read_sam_entry.set_tag('XC', classification)
+#         read_sam_entry.set_tag('NM', edit_distance(genomic_cigar))
+#     else:
+#         read_sam_entry.cigarstring = '*'
+#         read_sam_entry.reference_start = -1
+#         read_sam_entry.flag = 4
+
+
+#     read_sam_entry.query_sequence  = read_seq
+#     read_sam_entry.query_name = read_id
+
+#     return read_sam_entry.to_string()
+#     #alignment_outfile.write(read_sam_entry)
+
+
+def main(read_id, read_seq, ref_id, classification, predicted_exons, read_aln, ref_aln, annotated_to_transcript_id, is_rc, is_secondary, map_score, aln_score = 0):
+    sam_entry = []
+    sam_entry.append(read_id)
+    sam_entry.append("\t")
+    reference_name = ref_id
+
     if classification != 'unaligned':
         genomic_cigar, start_offset = get_genomic_cigar(read_aln, ref_aln, predicted_exons)
-        # if genomic_cigar == "":
-        #     print(classification, is_rc, is_secondary, aln_score)
-        #     print('genomic cigar:', genomic_cigar, read_id)
-        #     print(read_aln)
-        #     print(ref_aln)
-        #     print(predicted_exons)
         if is_secondary and is_rc:
-            read_sam_entry.flag = 256 + 16 
+            flag = 256 + 16 
         elif is_secondary:
-            read_sam_entry.flag = 256
+            flag = 256
         elif is_rc:
-            read_sam_entry.flag = 16 
+            flag = 16 
         else:
-            read_sam_entry.flag = 0 
-
-        read_sam_entry.reference_name = ref_id
-        read_sam_entry.mapping_quality = 60 # TODO: calculate mapping quality 
+            flag = 0 
 
-        read_sam_entry.cigarstring = genomic_cigar 
-        read_sam_entry.reference_start = predicted_exons[0][0] + start_offset
-        read_sam_entry.mapping_quality = map_score 
-        # print(predicted_exons[0][0], start_offset)
-        read_sam_entry.set_tag('XA', annotated_to_transcript_id)
-        read_sam_entry.set_tag('XC', classification)
-        read_sam_entry.set_tag('NM', edit_distance(genomic_cigar))
+        cigarstring = genomic_cigar 
+        reference_start = predicted_exons[0][0] + start_offset + 1 # SAM file used 1-based coordinate system, hence +1
+        mapping_quality = map_score 
     else:
-        read_sam_entry.cigarstring = '*'
-        read_sam_entry.reference_start = -1
-        read_sam_entry.flag = 4
-
-
-    read_sam_entry.query_sequence  = read_seq
-    read_sam_entry.query_name = read_id
-
-
-
-
-    alignment_outfile.write(read_sam_entry)
-    # sys.exit()
+        cigarstring = '*'
+        reference_start = 0
+        flag = 4
+        mapping_quality = 0 
+
+    sam_entry.append(str(flag))
+    sam_entry.append("\t")
+    sam_entry.append(reference_name)
+    sam_entry.append("\t")
+    sam_entry.append(str(reference_start))
+    sam_entry.append("\t")
+    sam_entry.append(str(mapping_quality))
+    sam_entry.append("\t")
+    sam_entry.append(cigarstring)
+    sam_entry.append("\t")
+
+    sam_entry.append('*')
+    sam_entry.append("\t")
+    sam_entry.append('0')
+    sam_entry.append("\t")
+    sam_entry.append('0')
+    sam_entry.append("\t")
+
+    sam_entry.append(read_seq)
+    sam_entry.append("\t")
+    sam_entry.append('*')
+    sam_entry.append("\t")
 
+    if classification != 'unaligned':
+        sam_entry.append('XA:Z:{0}'.format(annotated_to_transcript_id))
+        sam_entry.append("\t")
+        sam_entry.append('XC:Z:{0}'.format(classification))
+        sam_entry.append("\t")
+        sam_entry.append('NM:i:{0}'.format(edit_distance(genomic_cigar)))
+    sam_entry.append('\n')
 
+    return ''.join( [e for e in sam_entry])
```

### Comparing `ultra_bioinformatics-0.0.4.2/setup.py` & `ultra_bioinformatics-0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
 
     name='ultra_bioinformatics',  # Required
-    version='0.0.4.2',  # Required
+    version='0.1',  # Required
     description='Splice aligner of long transcriptomic reads to genome.',  # Required
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',
     url='https://github.com/ksahlin/uLTRA',  # Optional
     author='Kristoffer Sahlin',  # Optional
     author_email='ksahlin@math.su.se',  # Optional
```

### Comparing `ultra_bioinformatics-0.0.4.2/uLTRA` & `ultra_bioinformatics-0.1/uLTRA`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import sys
 import glob
 from time import time
 import itertools
 from itertools import islice, chain
 from struct import *
 import shutil
+import gzip
 
 import argparse
 import errno
 import math
 
 # import pickle
 import dill as pickle 
@@ -24,21 +25,21 @@
 from collections import defaultdict
 # from collections import OrderedDict
 
 # from modules import create_splice_graph as splice_graph
 # from modules import graph_chainer 
 
 from modules import create_augmented_gene as augmented_gene 
-from modules import mem_wrapper 
+from modules import seed_wrapper 
 from modules import colinear_solver 
 from modules import help_functions
 from modules import classify_read_with_mams
 from modules import classify_alignment2
 from modules import sam_output
-from modules import align
+from modules import pc
 from modules import prefilter_genomic_reads
 
 
 def load_reference(args):
     refs = {acc : seq for acc, (seq, _) in help_functions.readfq(open(args.ref,"r"))}
     refs_lengths = { acc : len(seq) for acc, seq in refs.items()} 
     return refs, refs_lengths
@@ -154,17 +155,14 @@
         print("Warning: Detected {0} sequences in reference fasta that are not in annotation:\n".format(len(not_in_annot)))
         for s in not_in_annot:
             print(s, "with length:{0}".format(len(refs[s])))
     # ref_part_sequences, ref_flank_sequences = augmented_gene.get_part_sequences_from_choordinates(parts_to_segments, flank_choordinates, refs_id)
     ref_part_sequences = augmented_gene.get_sequences_from_choordinates(parts_to_segments, refs_id)
     ref_flank_sequences = augmented_gene.get_sequences_from_choordinates(flank_choordinates, refs_id)
 
-    if not args.use_NAM_seeds: # not using NAM seeds
-        augmented_gene.mask_abundant_kmers(ref_part_sequences, args.min_mem, args.mask_threshold)
-        augmented_gene.mask_abundant_kmers(ref_flank_sequences, args.min_mem, args.mask_threshold)
 
     # print([unpack('LLL',t) for t in ref_flank_sequences.keys()])
     ref_part_sequences = help_functions.update_nested(ref_part_sequences, ref_flank_sequences)
     ref_segment_sequences = augmented_gene.get_sequences_from_choordinates(segment_id_to_choordinates, refs_id)
     # ref_flank_sequences = augmented_gene.get_sequences_from_choordinates(flank_choordinates, refs_id)
     ref_exon_sequences = augmented_gene.get_sequences_from_choordinates(exon_choordinates_to_id, refs_id)
     help_functions.pickle_dump(index_folder, segment_id_to_choordinates, 'segment_id_to_choordinates.pickle')
@@ -197,362 +195,210 @@
     if curr_nt_count/size != 0:
         sub_dict[acc] = seq
         batches.append(sub_dict)
     
     return batches
 
 
-def strobemap_batching(reads, STROBEMAP_BATCH_SIZE, nr_cores):
-    batches = []
-    for j in range(nr_cores):
-        batches.append({})
-
-    # read_idx_to_thread_map = {}
-    # for i in range(len(reads)):
-    #     if i % STROBEMAP_BATCH_SIZE == 0:
-    #         if i > 0: # remove already parsed reads
-    #             remaining_reads -= min(STROBEMAP_BATCH_SIZE, remaining_reads)
-    #     for j in range(remaining_reads):
-
-    remaining_reads = len(reads)
-    for i, (acc, seq) in enumerate(reads.items()):
-        if i % STROBEMAP_BATCH_SIZE == 0:
-            if i > 0: # remove already parsed reads
-                remaining_reads -= min(STROBEMAP_BATCH_SIZE, remaining_reads)
-            min_strobemap_thread_split_size = min(STROBEMAP_BATCH_SIZE, remaining_reads) // nr_cores
-            max_strobemap_thread_split_size = math.ceil((min(STROBEMAP_BATCH_SIZE, remaining_reads) / nr_cores))
-            idx_cutoff = min(STROBEMAP_BATCH_SIZE, remaining_reads) % nr_cores
-            # print(min_strobemap_thread_split_size,max_strobemap_thread_split_size)
-
-        idx_in_curr_batch = (i % STROBEMAP_BATCH_SIZE)
-        if idx_in_curr_batch < idx_cutoff * max_strobemap_thread_split_size:
-            thread_id = idx_in_curr_batch // max_strobemap_thread_split_size
-        else:
-            tmp = idx_in_curr_batch - idx_cutoff * max_strobemap_thread_split_size
-            thread_id = idx_cutoff + tmp // min_strobemap_thread_split_size
-
-        # print(acc, thread_id, idx_in_curr_batch)
-        batches[thread_id][acc] = seq
-    return batches  
+def score(cigartuples):
+    diffs = {1,2,8} # cigar IDs for INS, DEL, SUBS
+    matches = sum([length for type_, length in cigartuples if type_ == 7])
+    diffs = sum([length for type_, length in cigartuples if type_ in diffs]) 
+    return (matches - diffs)
 
 
-def check_alignment_fit(aln_ultra, aln_other):
+def output_final_alignments( ultra_alignments_path, path_indexed_aligned, path_unindexed_aligned):
     """
-        returns: 
-        1. the differnce in scoring is positive if uLTRA better
-        2. the classification obtained by uLTRA
+        This function have been improved in memory usage at the cost of speed. 
+        As opposed ot previous solution, we now never keep a full set of SAM records 
+        in memory for comparison as in previous functions. Steps:
+
+        1. Read in dictionary  {read_acc : score} from uLTRA's alignments
+        2. Steam over alternative aligner's (only mm2 impl currently) reads and log in a set {read_acc} where uLtra's alignments are better. 
+        3. Delete dictionary {read_acc : score} from step 1.
+        4. Stream over uLTRA's reads and save {read_acc : read (full SAM record)} for uLTRA's primary alignments with better score
+        5. Steam over alternative aligners records and replace the records from step 4 with uLTRA's
+    
+        Instead of parsing two SAM files (keeping one in RAM for coparison) as previous solution, 
+        this approach contains four parses at but is only keeping either all the read accessions plus an integer (cores)
+        or all uLTRA alignments and therir full sam record as max memory. 
     """
-    diffs = {1,2,8} # cigar IDs for INS, DEL, SUBS
-    matches_ultra = sum([length for type_, length in aln_ultra.cigartuples if type_ == 7])
-    diffs_ultra = sum([length for type_, length in aln_ultra.cigartuples if type_ in diffs]) 
-    matches_other = sum([length for type_, length in aln_other.cigartuples if type_ == 7])
-    diffs_other = sum([length for type_, length in aln_other.cigartuples if type_ in diffs]) 
-    # print(matches_ultra, diffs_ultra, matches_other, diffs_other, matches_other - diffs_other <= matches_ultra - diffs_ultra)
-    # return matches_other - diffs_other <= matches_ultra - diffs_ultra
-    return (matches_ultra - diffs_ultra) - (matches_other - diffs_other), aln_ultra.get_tag('XC')
+    replaced_unaligned_cntr = 0
+    equal_score = 0
+    slightly_worse_score = 0
+    worse_score = 0
+    ultra_unmapped = 0
+    # Step 1
+    ultra_SAM = pysam.AlignmentFile( ultra_alignments_path, "r" )
+    # take only primary alignments
+    ultra_scores = { read.query_name : score(read.cigartuples) for read in ultra_SAM.fetch() if (not read.is_secondary) and (not read.is_unmapped) }
+    ultra_SAM.close()
+
+    # Step 2
+    mm2_SAM = pysam.AlignmentFile(path_indexed_aligned, "r", check_sq=False)
+    ultra_better = set()
+    for read in mm2_SAM.fetch(until_eof=True):
+        if read.query_name not in ultra_scores:
+            ultra_unmapped += 1
+            continue
+
+        if read.is_unmapped:
+            if read.query_name in ultra_scores: # uLTRA aligned the read
+                ultra_better.add(read.query_name)
+                replaced_unaligned_cntr += 1
+            else:
+                pass
 
+        if (not read.is_secondary): # primary alignment in both files
+            mm2_score = score(read.cigartuples)
 
-def output_final_alignments( ultra_alignments_path, path_indexed_aligned, path_unindexed_aligned):
-    # read in all reads from alternative aligner that was also mapped by uLTRA
-    
-    alt_alignments_file = pysam.AlignmentFile(path_indexed_aligned, "r", check_sq=False)
-    alt_alignments = { read.query_name : read for read in alt_alignments_file.fetch(until_eof=True) if not read.is_secondary }
+            if mm2_score < ultra_scores[read.query_name]: 
+                ultra_better.add(read.query_name)
+            elif mm2_score == ultra_scores[read.query_name]:
+                equal_score += 1
+            elif mm2_score <= ultra_scores[read.query_name] + 10:
+                slightly_worse_score += 1
+            else:
+                worse_score += 1
+                
+        if (not read.is_secondary):
+            del ultra_scores[read.query_name]
 
+    mm2_SAM.close()
+
+    print("Total mm2's primary alignments replaced with uLTRA:", len(ultra_better))
+    print("Total mm2's alignments unmapped but mapped with uLTRA:", replaced_unaligned_cntr)
+
+    # Step 3
+    del ultra_scores
+
+    # Step 4
+    ultra_SAM = pysam.AlignmentFile( ultra_alignments_path, "r" )
+    ultra_better_records = { read.query_name: read for read in ultra_SAM.fetch() if (not read.is_secondary) and (read.query_name in ultra_better) }
+    tmp_merged_sam = pysam.AlignmentFile( ultra_alignments_path.decode()+ 'tmp', "w", template= ultra_SAM)
+    ultra_SAM.close()
+
+    # Step 5
+    mm2_SAM = pysam.AlignmentFile(path_indexed_aligned, "r", check_sq=False)
+    for read in mm2_SAM.fetch(until_eof=True):
+        if not read.is_secondary: # replacing primary alignments
+            if read.query_name in ultra_better_records:
+                read = ultra_better_records[read.query_name]
+
+        tmp_merged_sam.write(read)
+
+    mm2_SAM.close()
 
-    alignment_infile = pysam.AlignmentFile( ultra_alignments_path, "r" )
-    tmp_merged_outfile = pysam.AlignmentFile( ultra_alignments_path.decode()+ 'tmp', "w", template= alignment_infile)
-    replaced_unaligned_cntr = 0
-    tot_counter = 0
-    scoring_dict = defaultdict(int)
-    for read in alignment_infile.fetch():
-        if not read.is_secondary:
-            tot_counter += 1
-
-        if read.query_name in alt_alignments:
-            if read.flag == 4:
-               read = alt_alignments[ read.query_name ] # replace unmapped uLTRA read with alternative alignment if mapped
-               replaced_unaligned_cntr += 1
-            elif not read.is_secondary: 
-                ultra_scoring_diff, classification = check_alignment_fit(read,  alt_alignments[ read.query_name ])
-                scoring_dict[ultra_scoring_diff] += 1
-                if ultra_scoring_diff < 0:
-                    read = alt_alignments[ read.query_name ] # replace uLTRA read with alternative alignment if better fit
-
-        tmp_merged_outfile.write(read)
-    alignment_infile.close()
-    # path_genomic_aligned = os.path.join(args.outfolder, "unindexed.sam")
 
     # add all reads that we did not attempt to align with uLTRA
     # these reads had a primary alignment to unindexed regions by other pre-processing aligner (minimap2 as of now)
     not_attempted_cntr = 0
     unindexed = pysam.AlignmentFile(path_unindexed_aligned, "r")
     for read in unindexed.fetch():
-        tmp_merged_outfile.write(read)
+        tmp_merged_sam.write(read)
         if not read.is_secondary: 
             not_attempted_cntr += 1
     unindexed.close()
-    tmp_merged_outfile.close()
-    print("{0} reads were not attempted to be aligned with ultra, instead alternative aligner was used.".format(not_attempted_cntr))
-    print("{0} reads with primary alignments were replaced with alternative aligner because they were unaligned with uLTRA.".format(replaced_unaligned_cntr))
-    print("{0} primary alignments had best fit with uLTRA.".format(sum([v for k,v in scoring_dict.items() if k > 0])))
-    print("{0} primary alignments had equal fit.".format(scoring_dict[0]))
-    print("{0} primary alignments had best fit with alternative aligner.".format(sum([v for k,v in scoring_dict.items() if k < 0])))
-
-    bin_boundaries = [-2**32, -100,-50,-20,-10,-5,-4,-3,-2,-1, 0, 1, 2, 3, 4, 5, 10, 20, 50, 100, 2**32]
-    n = len(bin_boundaries)
-    counts = [0]*n #{ (b_l, b_u) : 0 for b_l, b_u in zip(bin_boundaries[:-1], bin_boundaries[1:])}
-    start_next = 0
-    for k in sorted(scoring_dict.keys()):
-        for i in range(start_next, n):
-            b = bin_boundaries[i]
-        # for i, b in enumerate(bin_boundaries):
-            if k < b:
-                counts[i] += scoring_dict[k]
-            else:
-                start_next = i
+    tmp_merged_sam.close()
+    print("{0} primary alignments had better score with uLTRA.".format(len(ultra_better_records)))
+    print("{0} primary alignments had equal score with alternative aligner.".format(equal_score))
+    print("{0} primary alignments had slightly better score with alternative aligner (typically ends bonus giving better scoring in ends, which needs to be implemented in uLTRA).".format(slightly_worse_score))
+    print("{0} primary alignments had significantly better score with alternative aligner.".format(worse_score))
+    print("{0} reads were unmapped with ultra but not by alternative aligner.".format(ultra_unmapped))
+    print("{0} reads were not attempted to be aligned with ultra (unindexed regions), instead alternative aligner was used.".format(not_attempted_cntr))
 
+    shutil.move(ultra_alignments_path.decode()+ 'tmp', ultra_alignments_path)
 
-    print("Table of score-difference between alignment methods (negative number: alternative aligner better fit, positive number is uLTRA better fit)")
-    print("Score is calculated as sum(identities) - sum(ins, del, subs)")
-    print("Format: Score difference: Number of primary alignments ")
-    for i in range(len(counts)-1):
-        print("[{0} - {1}): {2}".format(bin_boundaries[i],bin_boundaries[i+1], counts[i+1] - counts[i]))
-    # print("{0} read with primary alignments aligned with uLTRA.".format(tot_counter - replaced_unaligned_cntr - replaced_fit_cntr))
+    #########################
 
-    shutil.move(ultra_alignments_path.decode()+ 'tmp', ultra_alignments_path)
 
 
 def align_reads(args):
-    if args.nr_cores > 1:
-        mp.set_start_method('spawn')
-        print(mp.get_context())
-        print("Environment set:", mp.get_context())
-        print("Using {0} cores.".format(args.nr_cores))
-
     if args.index:
         if os.path.isdir(args.index):
             index_folder = args.index
         else:
             print("The index folder specified for alignment is not found. You specified: ", args.index )
             print("Build  the index to this folder, or specify another forder where the index has been built." )
             sys.exit()
     else:
         index_folder = args.outfolder
 
-    # topological_sorts = help_functions.pickle_load( os.path.join(args.outfolder, 'top_sorts.pickle') )
-    # path_covers = help_functions.pickle_load( os.path.join(args.outfolder, 'paths.pickle') )
-
     ref_part_sequences = help_functions.pickle_load( os.path.join(index_folder, 'ref_part_sequences.pickle') )
     refs_id_lengths = help_functions.pickle_load( os.path.join(index_folder, 'refs_id_lengths.pickle') )
     refs_lengths = help_functions.pickle_load( os.path.join(index_folder, 'refs_lengths.pickle') )
 
     if not args.disable_mm2:
         print("Filtering reads aligned to unindexed regions with minimap2 ")
+        print("Running minimap2...")
+        mm2_start = time()
         nr_reads_to_ignore, path_reads_to_align = prefilter_genomic_reads.main(ref_part_sequences, args.ref, args.reads, args.outfolder, index_folder, args.nr_cores, args.genomic_frac, args.mm2_ksize)
         args.reads = path_reads_to_align
         print("Done filtering. Reads filtered:{0}".format(nr_reads_to_ignore))
+        print("Time for minimap2:{0} seconds.".format(time() - mm2_start))
 
-    # print(ref_part_sequences)
     ref_path = os.path.join(args.outfolder, "refs_sequences.fa")
-    refs_file = open(ref_path, 'w') #open(os.path.join(outfolder, "refs_sequences_tmp.fa"), "w")
+    refs_file = open(ref_path, 'w')
     for sequence_id, seq  in ref_part_sequences.items():
         chr_id, start, stop = unpack('LLL',sequence_id)
-        # for (start,stop), seq  in ref_part_sequences[chr_id].items():
         refs_file.write(">{0}\n{1}\n".format(str(chr_id) + str("^") + str(start) + "^" + str(stop), seq))
     refs_file.close()
 
     del ref_part_sequences
 
-    ######### FIND MEMS WITH MUMMER #############
+    ######### FIND MEMS WITH NAMFINDER ##########
     #############################################
     #############################################
 
-    mummer_start = time()
-    if args.use_NAM_seeds:
-        print("Processing reads for MEM finding")
-        reads_tmp = open(os.path.join(args.outfolder, 'reads_tmp.fq'), 'w')
-        for acc, (seq, qual) in help_functions.readfq(open(args.reads, 'r')):
-            # print(seq)
-            # print(help_functions.remove_read_polyA_ends(seq, args.reduce_read_ployA))
-            reads_tmp.write('>{0}\n{1}\n'.format(acc, help_functions.remove_read_polyA_ends(seq, args.reduce_read_ployA, 5)))
-        reads_tmp.close()
-        args.reads_tmp = reads_tmp.name
-        mem_wrapper.find_nams_strobemap(args.outfolder, args.reads_tmp, ref_path, args.outfolder, args.nr_cores, args.min_mem)
-        print("Time for StrobeMap to find NAMs:{0} seconds.".format(time()-mummer_start))
-    else: # Use slaMEM
-        if args.nr_cores == 1:
-            print("Processing reads for MEM finding")
-            reads_tmp = open(os.path.join(args.outfolder, 'reads_tmp.fq'), 'w')
-            for acc, (seq, qual) in help_functions.readfq(open(args.reads, 'r')):
-                # print(seq)
-                # print(help_functions.remove_read_polyA_ends(seq, args.reduce_read_ployA))
-                reads_tmp.write('>{0}\n{1}\n'.format(acc, help_functions.remove_read_polyA_ends(seq, args.reduce_read_ployA, 5)))
-            reads_tmp.close()
-            args.reads_tmp = reads_tmp.name
-            print("Finished processing reads for MEM finding ")
-
-            mummer_out_path =  os.path.join( args.outfolder, "seeds_batch_-1.txt" )
-            print("Running MEM finding forward") 
-            mem_wrapper.find_mems_slamem(args.outfolder, args.reads_tmp, ref_path, mummer_out_path, args.min_mem)
-            print("Completed MEM finding forward")
-
-            print("Processing reverse complement reads for MEM finding")
-            reads_rc = open(os.path.join(args.outfolder, 'reads_rc.fq'), 'w')
-            for acc, (seq, qual) in help_functions.readfq(open(args.reads, 'r')):
-                # print(help_functions.reverse_complement(seq))
-                # print(help_functions.remove_read_polyA_ends(help_functions.reverse_complement(seq), args.reduce_read_ployA))
-                reads_rc.write('>{0}\n{1}\n'.format(acc, help_functions.reverse_complement(help_functions.remove_read_polyA_ends(seq, args.reduce_read_ployA, 5))))
-            reads_rc.close()
-            args.reads_rc = reads_rc.name
-            print("Finished processing reverse complement reads for MEM finding")
-
-            mummer_out_path =  os.path.join(args.outfolder, "seeds_batch_-1_rc.txt" )
-            print("Running MEM finding reverse")
-            mem_wrapper.find_mems_slamem(args.outfolder, args.reads_rc, ref_path, mummer_out_path, args.min_mem)
-            print("Completed MEM finding reverse")
-        
-        else: # multiprocess with slaMEM
-            reads = { acc : seq for acc, (seq, qual) in help_functions.readfq(open(args.reads, 'r'))}
-            total_nt = sum([len(seq) for seq in reads.values() ])
-            batch_size = int(total_nt/int(args.nr_cores) + 1)
-            print("batch nt:", batch_size, "total_nt:", total_nt)
-            read_batches = batch(reads, batch_size, 'nt')
-            
-            #### TMP remove not to call mummer repeatedly when bugfixing #### 
-            
-            batch_args = []
-            for i, read_batch_dict in enumerate(read_batches):
-                print(len(read_batch_dict))
-                read_batch_temp_file = open(os.path.join(args.outfolder, "reads_batch_{0}.fa".format(i)), "w")
-                read_batch_temp_file_rc = open(os.path.join(args.outfolder, "reads_batch_{0}_rc.fa".format(i) ), "w")
-                for acc, seq in read_batch_dict.items():
-                    read_batch_temp_file.write('>{0}\n{1}\n'.format(acc, help_functions.remove_read_polyA_ends(seq, args.reduce_read_ployA, 5)))
-                read_batch_temp_file.close()
-
-                for acc, seq in read_batch_dict.items():
-                    read_batch_temp_file_rc.write('>{0}\n{1}\n'.format(acc, help_functions.reverse_complement(help_functions.remove_read_polyA_ends(seq, args.reduce_read_ployA, 5))))
-                read_batch_temp_file_rc.close()
-                
-                read_batch = read_batch_temp_file.name
-                read_batch_rc = read_batch_temp_file_rc.name
-                mummer_batch_out_path =  os.path.join( args.outfolder, "seeds_batch_{0}.txt".format(i) )
-                mummer_batch_out_path_rc =  os.path.join(args.outfolder, "seeds_batch_{0}_rc.txt".format(i) )
-                batch_args.append( (args.outfolder, read_batch, ref_path, mummer_batch_out_path, args.min_mem ) )
-                batch_args.append( (args.outfolder, read_batch_rc, ref_path, mummer_batch_out_path_rc, args.min_mem ) )
-
-            pool = Pool(processes=int(args.nr_cores))
-            results = pool.starmap(mem_wrapper.find_mems_slamem, batch_args)
-            pool.close()
-            pool.join() 
-            
-            ####################################################################
-
-
-        print("Time for slaMEM to find mems:{0} seconds.".format(time()-mummer_start))
+    print("Processing reads for NAM finding")
+    processing_start = time()
+    reads_tmp = gzip.open(os.path.join(args.outfolder, 'reads_tmp.fa.gz'), 'wb', compresslevel=1)
+    for acc, (seq, qual) in help_functions.readfq(open(args.reads, 'r')):
+        record = '>{0}\n{1}\n'.format(acc, help_functions.remove_read_polyA_ends(seq, args.reduce_read_ployA, 5))
+        reads_tmp.write(record.encode('utf-8'))
+    reads_tmp.close()
+    print("Completed processing poly-A tails")
+    print("Time for processing reads:{0} seconds.".format(time() - processing_start))
+    args.reads_tmp = reads_tmp.name
+    namfinder_start = time()
+    seed_file_name = seed_wrapper.find_nams_namfinder(args.outfolder, args.reads_tmp, ref_path, args.outfolder, args.nr_cores, args.s, args.thinning)
+    print("Time for namfinder to find seeds:{0} seconds.".format(time() - namfinder_start))
     #############################################
     #############################################
     #############################################
 
+    
+    # ## For development omitting prefilter and namfinder steps.
+    # seed_file_name = os.path.join(args.outfolder, "seeds.txt.gz") 
+    # args.reads = os.path.join(args.outfolder, "reads_after_genomic_filtering.fasta")
+    # ############################################################
 
-    print("Starting aligning reads.")
-    if args.use_NAM_seeds:
-        if args.nr_cores == 1:
-            reads = { acc : seq for acc, (seq, qual) in help_functions.readfq(open(args.reads, 'r'))}
-            classifications, alignment_outfile_name = align.align_single(reads, refs_lengths, args, -1)
-        else:
-            # OrderedDict # dicts are ordered from python v3.6 and above. 
-            # One can use OrderedDict for compatibility with python v 3.4-3.5
-            reads = {acc : seq for acc, (seq, qual) in help_functions.readfq(open(args.reads, 'r'))}
-            # batch reads and mems up: divide reads by  nr_cores to get batch size
-            # then write to separate SAM-files with a batch index, 
-            # finally merge sam file by simple cat in terminal 
-            aligning_start = time()
-            # batch_size = int(len(reads)/int(args.nr_cores) + 1)
-            STROBEMAP_BATCH_SIZE=500000
-            read_batches = strobemap_batching(reads, STROBEMAP_BATCH_SIZE, int(args.nr_cores))
-            print('Nr reads:', len(reads), "nr batches:", len(read_batches), [len(b) for b in read_batches])
-            classifications, alignment_outfiles = align.align_parallel(read_batches, refs_lengths, args)
-        
-            print("Time to align reads:{0} seconds.".format(time()-aligning_start))
-
-            # Combine samfiles produced from each batch
-            combine_start = time()
-            # print(refs_lengths)
-            alignment_outfile = pysam.AlignmentFile( os.path.join(args.outfolder, args.prefix+".sam"), "w", reference_names=list(refs_lengths.keys()), reference_lengths=list(refs_lengths.values()) ) #, template=samfile)
-
-            for f in alignment_outfiles:
-                samfile = pysam.AlignmentFile(f, "r")
-                for read in samfile.fetch():
-                    alignment_outfile.write(read)
-                samfile.close()
-
-            alignment_outfile.close()
-            alignment_outfile_name = alignment_outfile.filename
-            print("Time to merge SAM-files:{0} seconds.".format(time() - combine_start))
-
-    else: # Use slaMEM
-        if args.nr_cores == 1:
-            reads = { acc : seq for acc, (seq, qual) in help_functions.readfq(open(args.reads, 'r'))}
-            classifications, alignment_outfile_name = align.align_single(reads, refs_lengths, args, -1)
-        else:
-            # batch reads and mems up: divide reads by  nr_cores to get batch size
-            # then write to separate SAM-files with a batch index, 
-            # finally merge sam file by simple cat in terminal 
-            aligning_start = time()
-            batch_size = int(len(reads)/int(args.nr_cores) + 1)
-            # read_batches = batch(reads, batch_size)
-            print('Nr reads:', len(reads), "nr batches:", len(read_batches), [len(b) for b in read_batches])
-            classifications, alignment_outfiles = align.align_parallel(read_batches, refs_lengths, args)
-        
-            print("Time to align reads:{0} seconds.".format(time()-aligning_start))
 
-            # Combine samfiles produced from each batch
-            combine_start = time()
-            # print(refs_lengths)
-            alignment_outfile = pysam.AlignmentFile( os.path.join(args.outfolder, args.prefix+".sam"), "w", reference_names=list(refs_lengths.keys()), reference_lengths=list(refs_lengths.values()) ) #, template=samfile)
-
-            for f in alignment_outfiles:
-                samfile = pysam.AlignmentFile(f, "r")
-                for read in samfile.fetch():
-                    alignment_outfile.write(read)
-                samfile.close()
-
-            alignment_outfile.close()
-            alignment_outfile_name = alignment_outfile.filename
-            print("Time to merge SAM-files:{0} seconds.".format(time() - combine_start))
+    print("Starting aligning reads.")
+    aln_file_name = os.path.join(args.outfolder, args.prefix+".sam")
+    alignment_outfile = pysam.AlignmentFile(aln_file_name , "w", reference_names=list(refs_lengths.keys()), reference_lengths=list(refs_lengths.values()) ) #, template=samfile)
+    alignment_outfile.close()
+    aligning_start = time()
+    tot_counts = pc.main(args.reads, seed_file_name, aln_file_name, args)
+    print("Time to align reads:{0} seconds.".format(time()-aligning_start))
+    alignment_outfile.close()
+    alignment_outfile_name = alignment_outfile.filename
 
 
 
     # need to merge genomic/unindexed alignments with the uLTRA-aligned alignments
     if not args.disable_mm2:
+        output_start = time()
         path_indexed_aligned = os.path.join(args.outfolder, "indexed.sam")
         path_unindexed_aligned = os.path.join(args.outfolder, "unindexed.sam")
         output_final_alignments(alignment_outfile_name, path_indexed_aligned, path_unindexed_aligned)
+        print("Time for selecting final best alignments (selecting the best of mm2's vs uLTRA's alignments):{0} seconds.".format(time() - output_start))
 
-    counts = defaultdict(int)
-    alignment_coverage = 0
-    for read_acc in reads:
-        if read_acc not in classifications:
-            # print(read_acc, "did not meet the threshold")
-            pass
-        elif classifications[read_acc][0] != 'FSM':
-            # print(read_acc, classifications[read_acc]) 
-            pass
-        if read_acc in classifications:
-            alignment_coverage += classifications[read_acc][1]
-            if classifications[read_acc][1] < 1.0:
-                # print(read_acc, 'alignemnt coverage:', classifications[read_acc][1])
-                pass
-            counts[classifications[read_acc][0]] += 1
-        else:
-            counts['unaligned'] += 1
-
-
-    print(counts)
-    print("total alignment coverage:", alignment_coverage)
+    print("FSM : {0}, NO_SPLICE : {1}, Insufficient_junction_coverage_unclassified : {2}, ISM/NIC_known : {3}, NIC_novel : {4}, NNC : {5}".format(tot_counts[1], *tot_counts[3:]))
+    print("total alignment coverage:", tot_counts[0])
 
     if not args.keep_temporary_files:
         print("Deleting temporary files...")
         seeds = glob.glob(os.path.join(args.outfolder, "seeds_*"))
         mum = glob.glob(os.path.join(args.outfolder, "mummer*"))
         sla = glob.glob(os.path.join(args.outfolder, "slamem*"))
         reads_tmp = glob.glob(os.path.join(args.outfolder, "reads_batch*"))
@@ -561,54 +407,49 @@
         
         f1 = os.path.join(args.outfolder, "reads_after_genomic_filtering.fasta")
         f2 = os.path.join(args.outfolder, "indexed.sam")
         f3 = os.path.join(args.outfolder, "unindexed.sam")
         f4 = os.path.join(args.outfolder, "refs_sequences.fa")
         f5 = os.path.join(args.outfolder, "refs_sequences.fa")
         f6 = os.path.join(args.outfolder, "reads_rc.fq")
-        f7 = os.path.join(args.outfolder, "reads_tmp.fq")
+        f7 = os.path.join(args.outfolder, "reads_tmp.fa")
         misc_files = [f1,f2,f3,f4,f5,f6,f7]
         for f in seeds + mum + sla + reads_tmp + minimap_tmp + ultra_tmp+ misc_files:
             if os.path.isfile(f):
                 os.remove(f)
                 print("removed:", f)
     print("Done.")
 
 
-
 if __name__ == '__main__':
 
     parser = argparse.ArgumentParser(description="uLTRA -- Align and classify long transcriptomic reads based on colinear chaining algorithms to gene regions")
-    parser.add_argument('--version', action='version', version='%(prog)s 0.0.4.2')
+    parser.add_argument('--version', action='version', version='%(prog)s 0.1')
 
     subparsers = parser.add_subparsers(help='Subcommands for eaither constructing a graph, or align reads')
     # parser.add_argument("-v", help='Different subcommands for eaither constructing a graph, or align reads')
 
     pipeline_parser = subparsers.add_parser('pipeline', help= "Perform all in one: prepare splicing database and reference sequences and align reads.")
     indexing_parser = subparsers.add_parser('index', help= "Construct data structures used for alignment.")
     align_reads_parser = subparsers.add_parser('align', help="Classify and align reads with colinear chaining to DAGs")
 
     pipeline_parser.add_argument('ref', type=str, help='Reference genome (fasta)')
     pipeline_parser.add_argument('gtf', type=str, help='Path to gtf file with gene models.')
     pipeline_parser.add_argument('reads', type=str, help='Path to fasta/fastq file with reads.')
     pipeline_parser.add_argument('outfolder', type=str, help='Path to output folder.')
     group = pipeline_parser.add_mutually_exclusive_group()
-    group.add_argument('--ont', action="store_true", help='Set parameters suitable for ONT (Currently sets: --min_mem 17, --min_acc 0.6 --alignment_threshold 0.5).')
-    group.add_argument('--isoseq', action="store_true", help='Set parameters suitable for IsoSeq (Currently sets: --min_mem 20, --min_acc 0.8 --alignment_threshold 0.5).')
-    # group2 = pipeline_parser.add_mutually_exclusive_group()
-    # group2.add_argument('--mummer', action="store_true", help='Use mummer to find mems. About 1.5-2x faster than slamem but consumes  >4x more memory (slamem is recommended for human and larger)')
-    # group2.add_argument('--slamem', action="store_true", help='Use slaMEM to find mems. About 1.5-2x slower than mumer but consumes less than 25% of the memory compared to mummer')
+    group.add_argument('--ont', action="store_true", help='Set parameters suitable for ONT (Sets: --min_seed 18 --s 9 --min_acc 0.6 --alignment_threshold 0.5).')
+    group.add_argument('--isoseq', action="store_true", help='Set parameters suitable for IsoSeq (Sets: --min_seed 20 --s 10 --min_acc 0.8 --alignment_threshold 0.5).')
 
-    pipeline_parser.add_argument('--min_mem', type=int, default=17, help='Threshold for minimum mem size considered.')
     pipeline_parser.add_argument('--min_segm', type=int, default=25, help='Threshold for minimum segment size considered.')
     pipeline_parser.add_argument('--min_acc', type=float, default=0.5, help='Minimum accuracy of MAM to be considered in mam chaining.')
     pipeline_parser.add_argument('--flank_size', type=int, default=1000, help='Size of genomic regions surrounding genes.')
     pipeline_parser.add_argument('--max_intron', type=int, default=1200000, help='Set global maximum size between mems considered in chaining solution. This is otherwise inferred from GTF file per chromosome.')
     pipeline_parser.add_argument('--small_exon_threshold', type=int, default=200, help='Considered in MAM solution even if they cont contain MEMs.')
-    pipeline_parser.add_argument('--reduce_read_ployA', type=int, default=8, help='Reduces polyA tails longer than X bases (default 10) in reads to 5bp before MEM finding. This helps MEM matching to spurios regions but does not affect final read alignments.')
+    pipeline_parser.add_argument('--reduce_read_ployA', type=int, default=8, help='Reduces polyA tails longer than X bases (default 8) in reads to 5bp before MEM finding. This helps MEM matching to spurios regions but does not affect final read alignments.')
     pipeline_parser.add_argument('--alignment_threshold', type=int, default=0.5, help='Lower threshold for considering an alignment. \
                                                                                         Counted as the difference between total match score and total mismatch penalty. \
                                                                                         If a read has 25%% errors (under edit distance scoring), the difference between \
                                                                                         matches and mismatches would be (very roughly) 0.75 - 0.25 = 0.5 with default alignment parameters \
                                                                                         match =2, subs=-2, gap open 3, gap ext=1. Default val (0.5) sets that a score\
                                                                                         higher than 2*0.5*read_length would be considered an alignment, otherwise unaligned.')
     pipeline_parser.add_argument('--t', dest = 'nr_cores', type=int, default=3, help='Number of cores.')
@@ -617,99 +458,99 @@
     pipeline_parser.add_argument('--non_covered_cutoff', type=int, default=15, help='Threshold for what is counted as varation/intron in alignment as opposed to deletion.')
     pipeline_parser.add_argument('--dropoff', type=float, default=0.95, help='Ignore alignment to hits with read coverage of this fraction less than the best hit.')
     pipeline_parser.add_argument('--max_loc', type=float, default=5, help='Limit read to be aligned to at most max_loc places (default 5).\
                                                                             This prevents time blowup for reads from highly repetitive regions (e.g. some genomic intra-priming reads)\
                                                                             but may limit all posible alignments to annotated gene families with many highly similar copies.')
     pipeline_parser.add_argument('--ignore_rc', action='store_true', help='Ignore to map to reverse complement.')
     pipeline_parser.add_argument('--disable_infer', action='store_true', help='Makes splice creation step much faster. This parameter can be set if gene and transcript name fields are provided in gtf file, which is standard for the ones provided by GENCODE and Ensemble.')
-    pipeline_parser.add_argument('--mask_threshold', type=int, default=200, help='Abundance occurance threshold. Masks more abundant k-mers than this threshold before MEM finding.')
     pipeline_parser.add_argument('--disable_mm2', action='store_true', help='Disables utilizing minimap2 to detect genomic primary alignments and to quality check uLTRAs primary alignments.\
                                                                                 An alignment is classified as genomic if more than --genomic_frac (default 10%%) of its aligned length is outside\
                                                                                 regions indexed by uLTRA. Note that uLTRA indexes flank regions such as 3 prime, 5 prime and (parts of) introns.')
     pipeline_parser.add_argument('--genomic_frac', type=float, default=0.1, help='If parameter prefilter_genomic is set, this is the threshild for fraction of aligned portion of read that is outside uLTRA indexed regions to be considered genomic (default 0.1).')
     pipeline_parser.add_argument('--keep_temporary_files', action='store_true', help='Keeps all intermediate files used for the alignment. This parameter is manily good for bugfixing and development.')
-    pipeline_parser.add_argument('--use_NAM_seeds', action='store_true', help='Uses StrobeMap to generate NAM seeds instead of MEMs. Uses StrobeMap parameters ./StrobeMap -n 2 -k 15 -v 16 -w 45 -t [nr_cores] -s.')
+    pipeline_parser.add_argument('--thinning', type=int, default=0, help='Seed thinning level 0-2: 0 (deactivated, default) 1 (in expectation every third base) or 2 (in expectation every fifth base). Thinning makes seedins step much faster and less memory consuming at cost of accuracy.')
+    pipeline_parser.add_argument('--s', type=int, default=10, help='Strobe size (default s=10). Uses strobemers of (2, s, s+1, 35).')
     pipeline_parser.set_defaults(which='pipeline')
 
     indexing_parser.add_argument('ref', type=str, help='Reference genome (fasta)')
     indexing_parser.add_argument('gtf', type=str, help='Path to gtf or gtf file with gene models.')
     indexing_parser.add_argument('outfolder', type=str, help='Path to output folder.')
     indexing_parser.add_argument('--min_segm', type=int, default=25, help='Threshold for minimum segment size considered.')
     indexing_parser.add_argument('--flank_size', type=int, default=1000, help='Size of genomic regions surrounding genes.')
     indexing_parser.add_argument('--small_exon_threshold', type=int, default=200, help='Considered in MAM solution even if they cont contain MEMs.')
     indexing_parser.add_argument('--disable_infer', action='store_true', help='Makes splice creation step much faster. Thes parameter can be set if gene and transcript name fields are provided in gtf file.')
-    indexing_parser.add_argument('--min_mem', type=int, default=17, help='Threshold for minimum mem size considered.')
-    indexing_parser.add_argument('--mask_threshold', type=int, default=200, help='Abundance occurance threshold. Masks more abundant k-mers than this threshold before MEM finding.')
-    indexing_parser.add_argument('--use_NAM_seeds', action='store_true', help='Activate this is you plan to align with parameter --use_NAM_seeds. Will inactivate masking in the indexing step.')
+    indexing_parser.add_argument('--thinning', type=int, default=0, help='Seed thinning level 0-2: 0 (deactivated, default) 1 (in expectation every third base) or 2 (in expectation every fifth base). Thinning makes seedins step much faster and less memory consuming at cost of accuracy.')
+    indexing_parser.add_argument('--s', type=int, default=10, help='Strobe size (default s=10). Uses strobemers of (2, s, s+1, 35).')
 
     indexing_parser.set_defaults(which='index')
 
 
     align_reads_parser.add_argument('ref', type=str, help='Reference genome (fasta).')    
     align_reads_parser.add_argument('reads', type=str, help='Path to fasta/fastq file with reads.')
     align_reads_parser.add_argument('outfolder', type=str, help='Path to output folder.')   
     align_reads_parser.add_argument('--t', dest = 'nr_cores', type=int, default=3, help='Number of cores.')
     align_reads_parser.add_argument('--index', type=str, default="", help='Path to where index files will be read from [default is the outfolder path].')
     align_reads_parser.add_argument('--prefix', default="reads", type=str, help='Outfile prefix [default=reads]. "--prefix sample_X" will output a file sample_X.sam.')
     align_reads_parser.add_argument('--max_intron', type=int, default=1200000, help='Set global maximum size between mems considered in chaining solution. This is otherwise inferred from GTF file per chromosome.')
-    align_reads_parser.add_argument('--reduce_read_ployA', type=int, default=8, help='Reduces polyA tails longer than X bases (default 10) in reads to 5bp before MEM finding. This helps MEM matching to spurios regions but does not affect final read alignments.')
+    align_reads_parser.add_argument('--reduce_read_ployA', type=int, default=8, help='Reduces polyA tails longer than X bases (default 8) in reads to 5bp before MEM finding. This helps MEM matching to spurios regions but does not affect final read alignments.')
     align_reads_parser.add_argument('--alignment_threshold', type=int, default=0.5, help='Lower threshold for considering an alignment. \
                                                                                         Counted as the difference between total match score and total mismatch penalty. \
                                                                                         If a read has 25%% errors (under edit distance scoring), the difference between \
                                                                                         matches and mismatches would be (very roughly) 0.75 - 0.25 = 0.5 with default alignment parameters \
                                                                                         match =2, subs=-2, gap open 3, gap ext=1. Default val (0.5) sets that a score\
                                                                                         higher than 2*0.5*read_length would be considered an alignment, otherwise unaligned.')
     align_reads_parser.add_argument('--non_covered_cutoff', type=int, default=15, help='Threshold for what is counted as varation/intron in alignment as opposed to deletion.')
     align_reads_parser.add_argument('--dropoff', type=float, default=0.95, help='Ignore alignment to hits with read coverage of this fraction less than the best hit.')
     align_reads_parser.add_argument('--max_loc', type=float, default=5, help='Limit read to be aligned to at most max_loc places (default 5).\
                                                                             This prevents time blowup for reads from highly repetitive regions (e.g. some genomic intra-priming reads)\
                                                                             but may limit all posible alignments to annotated gene families with many highly similar copies.')
 
     align_reads_parser.add_argument('--ignore_rc', action='store_true', help='Ignore to map to reverse complement.')
-    align_reads_parser.add_argument('--min_mem', type=int, default=17, help='Threshold for minimum mem size considered.')
     align_reads_parser.add_argument('--min_acc', type=float, default=0.5, help='Minimum accuracy of MAM to be considered in mam chaining.')
 
     align_reads_parser.add_argument('--disable_mm2', action='store_true', help='Disables utilizing minimap2 to detect genomic primary alignments and to quality check uLTRAs primary alignments.\
                                                                                 An alignment is classified as genomic if more than --genomic_frac (default 10%%) of its aligned length is outside\
                                                                                 regions indexed by uLTRA. Note that uLTRA indexes flank regions such as 3 prime, 5 prime and (parts of) introns.')
 
     align_reads_parser.add_argument('--genomic_frac', type=float, default=0.1, help='If parameter prefilter_genomic is set, this is the threshild for fraction of aligned portion of read that is outside uLTRA indexed regions to be considered genomic (default 0.1).')
     align_reads_parser.add_argument('--keep_temporary_files', action='store_true', help='Keeps all intermediate files used for the alignment. This parameter is manily good for bugfixing and development.')
-    align_reads_parser.add_argument('--use_NAM_seeds', action='store_true', help='Uses StrobeMap to generate NAM seeds instead of MEMs. Uses StrobeMap parameters ./StrobeMap -n 2 -k 15 -v 16 -w 45 -t [nr_cores] -s.')
+    align_reads_parser.add_argument('--thinning', type=int, default=0, help='Seed thinning level (0-2): 0 (deactivated, default) 1 (in expectation every third base) or 2 (in expectation every fifth base). Thinning makes seedins step much faster and less memory consuming at cost of accuracy.')
+    align_reads_parser.add_argument('--s', type=int, default=10, help='Strobe size (default s=10). Uses strobemers of (2, s, s+1, 35).')
 
 
     group2 = align_reads_parser.add_mutually_exclusive_group()
-    group2.add_argument('--ont', action="store_true", help='Set parameters suitable for ONT (Currently sets: --min_mem 17, --min_acc 0.6 --alignment_threshold 0.5).')
-    group2.add_argument('--isoseq', action="store_true", help='Set parameters suitable for IsoSeq (Currently sets: --min_mem 20, --min_acc 0.8 --alignment_threshold 0.5).')
+    group2.add_argument('--ont', action="store_true", help='Set parameters suitable for ONT (Sets: --s 9 --min_acc 0.6).')
+    group2.add_argument('--isoseq', action="store_true", help='Set parameters suitable for IsoSeq (Sets: --s 10 --min_acc 0.8).')
 
 
     align_reads_parser.set_defaults(which='align_reads')
 
     args = parser.parse_args()
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit()
 
     help_functions.mkdir_p(args.outfolder)
     if len(sys.argv)==1:
         parser.print_help()
         sys.exit()
 
+    if args.thinning < 0 or args.thinning > 2:
+        print("Invalid thinning level. Choose 0, 1 or 2.")
+        sys.exit()
 
     if args.which == 'align_reads' or args.which == 'pipeline':
         args.mm2_ksize = 15
         if args.ont:
-            args.min_mem = 17
             args.min_acc = 0.6
             args.mm2_ksize = 14
-            # args.alignment_threshold = 0.5
+            args.s = 9
         if args.isoseq:
-            args.min_mem = 20
             args.min_acc = 0.8
-            # args.alignment_threshold = 0.5
+            args.s = 10
 
 
     if args.which == 'index':
         args.index = args.outfolder
         refs, refs_lengths = load_reference(args)
         prep_splicing(args, refs_lengths)
         prep_seqs(args, refs, refs_lengths)
```

### Comparing `ultra_bioinformatics-0.0.4.2/ultra_bioinformatics.egg-info/SOURCES.txt` & `ultra_bioinformatics-0.1/ultra_bioinformatics.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 modules/__init__.py
 modules/align.py
 modules/classify_alignment2.py
 modules/classify_read_with_mams.py
 modules/colinear_solver.py
 modules/create_augmented_gene.py
 modules/help_functions.py
-modules/mem_wrapper.py
+modules/pc.py
 modules/prefilter_genomic_reads.py
 modules/range_query_max_search_tree.py
 modules/sam_output.py
+modules/seed_wrapper.py
+modules/test_pc_multiprocess.py
 ultra_bioinformatics.egg-info/PKG-INFO
 ultra_bioinformatics.egg-info/SOURCES.txt
 ultra_bioinformatics.egg-info/dependency_links.txt
 ultra_bioinformatics.egg-info/requires.txt
 ultra_bioinformatics.egg-info/top_level.txt
```

