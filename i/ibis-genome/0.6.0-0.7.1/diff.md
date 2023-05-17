# Comparing `tmp/ibis-genome-0.6.0.tar.gz` & `tmp/ibis-genome-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibis-genome-0.6.0.tar", last modified: Thu Apr  6 03:47:35 2023, max compression
+gzip compressed data, was "ibis-genome-0.7.1.tar", last modified: Wed May 17 03:49:33 2023, max compression
```

## Comparing `ibis-genome-0.6.0.tar` & `ibis-genome-0.7.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:47:35.581355 ibis-genome-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    44009 2023-04-06 03:47:35.581355 ibis-genome-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:47:35.577355 ibis-genome-0.6.0/ibis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:47:35.577355 ibis-genome-0.6.0/ibis/config/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/config/template_coassemble.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/config/template_evaluate.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    37778 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/ibis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:47:35.577355 ibis-genome-0.6.0/ibis/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/coassemble.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:47:35.577355 ibis-genome-0.6.0/ibis/workflow/env/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/env/aviary.yml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/env/coverm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/env/kingfisher.yml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/env/prodigal.yml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/env/r.yml
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/env/singlem.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/evaluate.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:47:35.577355 ibis-genome-0.6.0/ibis/workflow/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2548 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/scripts/aviary_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/scripts/cluster_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2985 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/scripts/collect_reference_bins.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8667 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/scripts/evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      429 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/scripts/no_genomes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3173 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/scripts/query_processing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/scripts/separate_SingleM_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/scripts/summarise_coassemblies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3541 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/ibis/workflow/scripts/target_elusive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:47:35.581355 ibis-genome-0.6.0/ibis_genome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44009 2023-04-06 03:47:35.000000 ibis-genome-0.6.0/ibis_genome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-06 03:47:35.000000 ibis-genome-0.6.0/ibis_genome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 03:47:35.000000 ibis-genome-0.6.0/ibis_genome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-06 03:47:35.000000 ibis-genome-0.6.0/ibis_genome.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-06 03:47:35.000000 ibis-genome-0.6.0/ibis_genome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-06 03:47:35.000000 ibis-genome-0.6.0/ibis_genome.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 03:47:35.581355 ibis-genome-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:47:35.581355 ibis-genome-0.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/test/test_cluster_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    36484 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/test/test_coassemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/test/test_collect_reference_bins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    26417 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/test/test_evaluate_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/test/test_iterate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/test/test_query_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/test/test_target_elusive.py
--rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-04-06 03:47:24.000000 ibis-genome-0.6.0/test/test_unmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.678264 ibis-genome-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    44009 2023-05-17 03:49:33.678264 ibis-genome-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.670264 ibis-genome-0.7.1/ibis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.670264 ibis-genome-0.7.1/ibis/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/config/template_coassemble.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/config/template_evaluate.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37806 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/ibis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.670264 ibis-genome-0.7.1/ibis/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    16160 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/coassemble.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.670264 ibis-genome-0.7.1/ibis/workflow/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/env/aviary.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/env/coverm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/env/kingfisher.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/env/prodigal.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/env/r.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/env/singlem.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/evaluate.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.674264 ibis-genome-0.7.1/ibis/workflow/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2548 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/aviary_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/cluster_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3020 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/collect_reference_bins.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10121 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/evaluate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/no_genomes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3351 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/query_processing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/separate_SingleM_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/summarise_coassemblies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3524 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/ibis/workflow/scripts/target_elusive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.674264 ibis-genome-0.7.1/ibis_genome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44009 2023-05-17 03:49:33.000000 ibis-genome-0.7.1/ibis_genome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-17 03:49:33.000000 ibis-genome-0.7.1/ibis_genome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 03:49:33.000000 ibis-genome-0.7.1/ibis_genome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 03:49:33.000000 ibis-genome-0.7.1/ibis_genome.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 03:49:33.000000 ibis-genome-0.7.1/ibis_genome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 03:49:33.000000 ibis-genome-0.7.1/ibis_genome.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-17 03:49:20.000000 ibis-genome-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:49:33.678264 ibis-genome-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:49:33.678264 ibis-genome-0.7.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_cluster_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40641 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_coassemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_collect_reference_bins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_evaluate_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_iterate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_no_genomes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_query_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_target_elusive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-05-17 03:49:21.000000 ibis-genome-0.7.1/test/test_unmap.py
```

### Comparing `ibis-genome-0.6.0/LICENSE` & `ibis-genome-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.6.0/PKG-INFO` & `ibis-genome-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibis-genome
-Version: 0.6.0
+Version: 0.7.1
 Summary: Ibis (Australian bin chicken) - targeted recovery of low abundance genomes through intelligent coassembly
 Author-email: Samuel Aroney <samuel.aroney@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ibis-genome-0.6.0/README.md` & `ibis-genome-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.6.0/ibis/ibis.py` & `ibis-genome-0.7.1/ibis/ibis.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         completeness_col = "Completeness (CheckM2)"
         contamination_col = "Contamination (CheckM2)"
     else:
         raise ValueError("Invalid CheckM version")
 
     coassembly_bins = {}
     for coassembly in checkm_out_dict:
-        checkm_out = pl.read_csv(checkm_out_dict[coassembly], sep = "\t")
+        checkm_out = pl.read_csv(checkm_out_dict[coassembly], separator="\t")
         passed_bins = checkm_out.filter(
             (pl.col(completeness_col) >= min_completeness) & (pl.col(contamination_col) <= max_contamination),
         ).get_column("Bin Id"
         ).to_list()
         coassembly_bins[coassembly] = passed_bins
 
     if iteration:
@@ -373,19 +373,19 @@
         args.appraise_unbinned = os.path.join(args.coassemble_output, "appraise", "unbinned.otu_table.tsv")
     if args.elusive_clusters and not args.coassemblies:
         copy_input(
             os.path.abspath(args.elusive_clusters),
             os.path.join(args.output, "coassemble", "target", "elusive_clusters.tsv")
         )
     elif args.elusive_clusters and args.coassemblies:
-        elusive_clusters = pl.read_csv(os.path.abspath(args.elusive_clusters), sep="\t")
+        elusive_clusters = pl.read_csv(os.path.abspath(args.elusive_clusters), separator="\t")
         elusive_clusters = elusive_clusters.filter(pl.col("coassembly").is_in(args.coassemblies))
 
         os.makedirs(os.path.join(args.output, "coassemble", "target"), exist_ok=True)
-        elusive_clusters.write_csv(os.path.join(args.output, "coassemble", "target", "elusive_clusters.tsv"), sep="\t")
+        elusive_clusters.write_csv(os.path.join(args.output, "coassemble", "target", "elusive_clusters.tsv"), separator="\t")
 
     if args.appraise_binned:
         copy_input(
             os.path.abspath(args.appraise_binned),
             os.path.join(args.output, "coassemble", "appraise", "binned.otu_table.tsv")
         )
     if args.appraise_unbinned:
@@ -445,17 +445,17 @@
 
     if args.genome_singlem:
         args.genome_singlem = generate_genome_singlem(args, new_genomes)
 
     coassemble(args)
 
     if args.elusive_clusters:
-        new_cluster = pl.read_csv(os.path.join(args.output, "coassemble", "target", "elusive_clusters.tsv"), sep="\t")
+        new_cluster = pl.read_csv(os.path.join(args.output, "coassemble", "target", "elusive_clusters.tsv"), separator="\t")
         for cluster in args.elusive_clusters:
-            old_cluster = pl.read_csv(cluster, sep="\t")
+            old_cluster = pl.read_csv(cluster, separator="\t")
             comb_cluster = new_cluster.join(old_cluster, on="samples", how="inner")
 
             if comb_cluster.height > 0:
                 _ = comb_cluster.select(
                     pl.col("coassembly").apply(lambda x: logging.warn(f"{x} has been previously suggested"))
                     )
     else:
@@ -567,15 +567,15 @@
         coassemble_clustering.add_argument("--max-coassembly-size", type=int, help="Maximum size (Gbp) of coassembly cluster [default: None]", default=None)
         coassemble_clustering.add_argument("--max-recovery-samples", type=int, help="Upper bound for number of related samples to use for differential abundance binning [default: 20]", default=20)
         coassemble_clustering.add_argument("--prodigal-meta", action="store_true", help="Use prodigal \"-p meta\" argument (for testing)")
         # Coassembly options
         coassemble_coassembly = parser.add_argument_group("Coassembly options")
         coassemble_coassembly.add_argument("--assemble-unmapped", action="store_true", help="Only assemble reads that do not map to reference genomes")
         coassemble_coassembly.add_argument("--unmapping-min-appraised", type=int, help="Minimum fraction of sequences binned to justify unmapping [default: 0.1]", default=0.1)
-        coassemble_coassembly.add_argument("--unmapping-max-identity", type=float, help="Maximum sequence identity of mapped sequences kept for coassembly [default: 95%]", default=95)
+        coassemble_coassembly.add_argument("--unmapping-max-identity", type=float, help="Maximum sequence identity of mapped sequences kept for coassembly [default: 99%]", default=99)
         add_aviary_options(coassemble_coassembly)
         # General options
         coassemble_general = parser.add_argument_group("General options")
         add_general_snakemake_options(coassemble_general)
 
     add_coassemble_arguments(coassemble_parser)
```

### Comparing `ibis-genome-0.6.0/ibis/workflow/coassemble.smk` & `ibis-genome-0.7.1/ibis/workflow/coassemble.smk`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #############
 ### Setup ###
 #############
-ruleorder: no_genomes > query_processing > singlem_appraise
+ruleorder: no_genomes > query_processing > singlem_appraise_filtered
 
 import os
 import pandas as pd
 
 output_dir = os.path.abspath("coassemble")
 logs_dir = output_dir + "/logs"
 
@@ -158,16 +158,16 @@
 ### SingleM appraise ###
 ########################
 rule singlem_appraise:
     input:
         reads=expand(output_dir + "/pipe/{read}_read.otu_table.tsv", read=config["reads_1"]),
         bins=output_dir + "/summarise/bins_summarised.otu_table.tsv",
     output:
-        unbinned=output_dir + "/appraise/unbinned.otu_table.tsv",
-        binned=output_dir + "/appraise/binned.otu_table.tsv",
+        unbinned=output_dir + "/appraise/unbinned_raw.otu_table.tsv",
+        binned=output_dir + "/appraise/binned_raw.otu_table.tsv",
     log:
         logs_dir + "/appraise/appraise.log"
     params:
         sequence_identity=config["appraise_sequence_identity"],
         singlem_metapackage=config["singlem_metapackage"],
     conda:
         "env/singlem.yml"
@@ -179,14 +179,27 @@
         "--output-unaccounted-for-otu-table {output.unbinned} "
         "--output-binned-otu-table {output.binned} "
         "--imperfect "
         "--sequence-identity {params.sequence_identity} "
         "--output-found-in "
         "&> {log}"
 
+rule singlem_appraise_filtered:
+    input:
+        unbinned=output_dir + "/appraise/unbinned_raw.otu_table.tsv",
+        binned=output_dir + "/appraise/binned_raw.otu_table.tsv",
+    output:
+        unbinned=output_dir + "/appraise/unbinned.otu_table.tsv",
+        binned=output_dir + "/appraise/binned.otu_table.tsv",
+    params:
+        bad_package="S3.18.EIF_2_alpha",
+    shell:
+        "grep -v {params.bad_package} {input.unbinned} > {output.unbinned} && "
+        "grep -v {params.bad_package} {input.binned} > {output.binned}"
+
 ###################################
 ### SingleM query (alternative) ###
 ###################################
 rule query_processing:
     input:
         pipe_reads=expand(output_dir + "/pipe/{read}_read.otu_table.tsv", read=config["reads_1"]),
         query_reads=expand(output_dir + "/query/{read}_query.otu_table.tsv", read=config["reads_1"]),
```

### Comparing `ibis-genome-0.6.0/ibis/workflow/env/singlem.yml` & `ibis-genome-0.7.1/ibis/workflow/env/singlem.yml`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.6.0/ibis/workflow/evaluate.smk` & `ibis-genome-0.7.1/ibis/workflow/evaluate.smk`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     input:
         recovered_otu_table = output_dir + "/summarise/bins_summarised.otu_table.tsv"
     output:
         matched_hits = output_dir + "/evaluate/matched_hits.tsv",
         novel_hits = output_dir + "/evaluate/novel_hits.tsv",
         summary_stats = output_dir + "/evaluate/summary_stats.tsv",
     params:
-        unbinned_otu_table=config["targets"],
+        target_otu_table=config["targets"],
         binned_otu_table=config["binned"],
         elusive_edges=config["elusive_edges"],
         elusive_clusters=config["elusive_clusters"],
         recovered_bins=config["recovered_bins"],
     threads:
         64
     script:
```

### Comparing `ibis-genome-0.6.0/ibis/workflow/scripts/aviary_commands.py` & `ibis-genome-0.7.1/ibis/workflow/scripts/aviary_commands.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.6.0/ibis/workflow/scripts/cluster_graph.py` & `ibis-genome-0.7.1/ibis/workflow/scripts/cluster_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,17 +136,17 @@
                 ).filter(pl.col("sample1_bool") & pl.col("sample2_bool")
                 ).select(
                     pl.col("target_ids").str.split(",").flatten().alias("target_ids"),
                 ).get_column("target_ids")
             ).alias("relevant_targets"),
     ).with_columns(
         pl.when(
-            (pl.col("recover_samples_list").arr.lengths().first() >= MAX_RECOVERY_SAMPLES) | (pl.col("relevant_edges").apply(lambda x: x.height) == 0)
+            (pl.col("recover_samples_list").arr.lengths() >= MAX_RECOVERY_SAMPLES) | (pl.col("relevant_edges").apply(lambda x: x.height) == 0)
         ).then(
-            pl.Series("other_samples", [[]])
+            pl.Series("other_samples", [[]], dtype = pl.List(pl.Utf8))
         ).otherwise(
             pl.col("relevant_edges").apply(
                 lambda x: x.with_columns(pl.col("target_ids").str.split(","))
                     .explode("target_ids")
                     .groupby("other_sample")
                     .agg(pl.count())
                     .sort(["count", "other_sample"], descending=True)
@@ -181,19 +181,19 @@
     MAX_COASSEMBLY_SAMPLES = snakemake.params.max_coassembly_samples
     MIN_COASSEMBLY_SAMPLES = snakemake.params.num_coassembly_samples
     MAX_RECOVERY_SAMPLES = snakemake.params.max_recovery_samples
     elusive_edges_path = snakemake.input.elusive_edges
     read_size_path = snakemake.input.read_size
     elusive_clusters_path = snakemake.output.elusive_clusters
 
-    elusive_edges = pl.read_csv(elusive_edges_path, sep="\t", dtypes={"target_ids": str})
+    elusive_edges = pl.read_csv(elusive_edges_path, separator="\t", dtypes={"target_ids": str})
     read_size = pl.read_csv(read_size_path, has_header=False, new_columns=["sample", "read_size"])
 
     clusters = pipeline(
         elusive_edges,
         read_size,
         MAX_COASSEMBLY_SIZE=MAX_COASSEMBLY_SIZE,
         MAX_COASSEMBLY_SAMPLES=MAX_COASSEMBLY_SAMPLES,
         MIN_COASSEMBLY_SAMPLES=MIN_COASSEMBLY_SAMPLES,
         MAX_RECOVERY_SAMPLES=MAX_RECOVERY_SAMPLES
         )
-    clusters.write_csv(elusive_clusters_path, sep="\t")
+    clusters.write_csv(elusive_clusters_path, separator="\t")
```

### Comparing `ibis-genome-0.6.0/ibis/workflow/scripts/collect_reference_bins.py` & `ibis-genome-0.7.1/ibis/workflow/scripts/collect_reference_bins.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     ).with_columns(
         pl.col("found_in").str.replace("_protein$", "")
     ).groupby(
         ["gene", "found_in"]
     ).agg(
         pl.col("coverage").sum()
     ).pivot(
-        values="coverage", index="gene", columns="found_in", 
+        values="coverage", index="gene", columns="found_in", aggregate_function=None
     ).melt(
         id_vars="gene", variable_name="found_in", value_name="coverage"
     ).fill_null(0
     ).groupby(
         "found_in"
     ).agg(
         (pl.col("coverage").len() * TRIM_FRACTION).floor().cast(int).alias("cut"),
@@ -77,16 +77,16 @@
     unbinned_path = snakemake.input.appraise_unbinned
     genomes = snakemake.params.genomes
     sample = snakemake.params.sample
     MIN_APPRAISED = snakemake.params.min_appraised
     sample_read = snakemake.wildcards.read
     output_path = snakemake.output
 
-    appraise_binned = pl.read_csv(binned_path, sep="\t")
-    appraise_unbinned = pl.read_csv(unbinned_path, sep="\t")
+    appraise_binned = pl.read_csv(binned_path, separator="\t")
+    appraise_unbinned = pl.read_csv(unbinned_path, separator="\t")
 
     reference_bins = pipeline(appraise_binned, appraise_unbinned, sample, MIN_APPRAISED=MIN_APPRAISED)
 
     if len(reference_bins) == 0:
         print(f"Warning: No reference bins found for {sample_read}")
         cmd = f"touch {output_path}"
         extern.run(cmd)
```

### Comparing `ibis-genome-0.6.0/ibis/workflow/scripts/evaluate.py` & `ibis-genome-0.7.1/ibis/workflow/scripts/evaluate.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,112 +9,136 @@
 OUTPUT_COLUMNS={
     "coassembly": str,
     "gene": str,
     "sequence": str,
     "genome": str,
     "target": str,
     "found_in": str,
+    "source_samples": str,
     "taxonomy": str,
     }
 SUMMARY_COLUMNS = {
     "coassembly": str,
     "statistic": str,
     "within": str,
     "match": int,
     "nonmatch": int,
     "total": int,
     "match_percent": float,
     }
 
-def evaluate(unbinned_otu_table, binned_otu_table, elusive_clusters, elusive_edges, recovered_otu_table, recovered_bins):
+def evaluate(target_otu_table, binned_otu_table, elusive_clusters, elusive_edges, recovered_otu_table, recovered_bins):
 
     print(f"Polars using {str(pl.threadpool_size())} threads")
 
     if len(recovered_otu_table) == 0:
         empty_output = pl.DataFrame(schema=OUTPUT_COLUMNS)
         return empty_output, empty_output, pl.DataFrame(schema=SUMMARY_COLUMNS)
 
-    # Load otu table of unbinned sequences and get unique id for each sequence (to match sequences to target id)
-    unbinned_otu_table = unbinned_otu_table.select([
+    # Load otu table of target sequences and get unique id for each sequence (to match sequences to target id)
+    relevant_target_otu_table = target_otu_table.select([
         "gene", "sequence",
         pl.first("target").over(["gene", "sequence"]).cast(str),
         pl.first("taxonomy").over(["gene", "sequence"]),
     ]).unique().drop_nulls()
 
     # Load elusive clusters and edges (to match targets to coassemblies, with duplicates)
     sample_coassemblies = elusive_clusters.select(
         pl.col("samples").str.split(","),
         "coassembly"
     ).explode("samples")
 
-    coassembly_edges = elusive_edges.with_columns(
+    elusive_edges = elusive_edges.with_columns(
         pl.col("sample1").str.replace(r"\.1$", ""),
         pl.col("sample2").str.replace(r"\.1$", ""),
     ).join(
         sample_coassemblies, left_on="sample1", right_on="samples", how="left"
     ).join(
         sample_coassemblies, left_on="sample2", right_on="samples", how="left", suffix="2"
     ).filter(
         pl.col("coassembly") == pl.col("coassembly2")
     ).with_columns(
         pl.col("target_ids").str.split(",").alias("target")
     ).explode("target"
-    ).select(["target", "coassembly"]
+    )
+
+    coassembly_edges = elusive_edges.select(["target", "coassembly"]
     ).unique()
 
-    # Create otu table with original sequence, cluster id, target id and associated coassemblies
+    # Create otu table with original sequence, samples present, cluster id, target id and associated coassemblies
+    sample_edges = elusive_edges.melt(
+        id_vars=["coassembly", "target"],
+        value_vars=["sample1", "sample2"],
+        value_name="sample"
+    ).groupby([
+        "coassembly", "target"
+    ]).agg([
+        pl.col("sample").unique().sort().str.concat(",").alias("source_samples")
+    ])
+
     elusive_otu_table = coassembly_edges.join(
-        unbinned_otu_table, on="target", how="left"
+        relevant_target_otu_table, on="target", how="left"
     ).select(
-        "gene", "sequence", "taxonomy",
+        "gene", "sequence", "coassembly", "taxonomy",
         pl.lit(None).cast(str).alias("found_in"),
-        "coassembly", "target",
+        "target",
+    ).join(
+        sample_edges, on=["coassembly", "target"], how="left"
     )
 
     # Add binned otu table to above with target NA
-    nontarget_otu_table = binned_otu_table.select([
+    nontarget_otu_table = pl.concat([
+        binned_otu_table,
+        target_otu_table
+            .join(elusive_otu_table, on=["gene", "sequence"], how="anti")
+            .drop("target")
+            .with_columns(pl.lit(None).cast(str).alias("found_in"))
+    ]).select([
         pl.col("sample").str.replace(r"\.1$", ""),
         "gene", "sequence", "taxonomy", "found_in"
     ]).join(
         sample_coassemblies, left_on="sample", right_on="samples", how="left"
-    ).drop("sample"
     ).drop_nulls("coassembly"
-    ).unique(
-    ).with_columns(
-        pl.lit(None).cast(str).alias("target")
+    ).groupby(["gene", "sequence", "coassembly"]
+    ).agg([
+        pl.first("taxonomy"),
+        pl.first("found_in"),
+        pl.lit(None).cast(str).alias("target"),
+        pl.col("sample").unique().sort().str.concat(",").alias("source_samples")
+    ]).unique(
     )
 
     haystack_otu_table = pl.concat([elusive_otu_table, nontarget_otu_table])
 
     # Load recovered otu table and join elusive and nontarget sequences
     recovered_otu_table = recovered_otu_table.with_columns(
-        pl.col("sample").str.split("-").arr.to_struct(upper_bound=2, name_generator=lambda id: ["coassembly", "genome"][id])
+        pl.col("sample").str.split("-").arr.to_struct(upper_bound=2, fields=["coassembly", "genome"])
     ).unnest("sample"
     )
 
     combined_otu_table = recovered_otu_table.join(
         haystack_otu_table, on=["coassembly", "gene", "sequence"], how="outer", suffix="old"
     ).select(
-        "coassembly", "gene", "sequence", "genome", "target", "found_in",
+        "coassembly", "gene", "sequence", "genome", "target", "found_in", "source_samples",
         pl.when(pl.col("taxonomy").is_null())
         .then(pl.col("taxonomyold"))
         .otherwise(pl.col("taxonomy"))
         .alias("taxonomy"),
     ).filter(
         (pl.col("coassembly").is_in(pl.lit(recovered_otu_table["coassembly"]))) &
         # Choose sequences where genome is present (from recovered) and/or target is present (from unbinned targets)
         ((pl.col("genome").is_not_null()) | (pl.col("target").is_not_null()))
     )
 
     matches = combined_otu_table.filter(
-        ~pl.all(pl.col(["target", "found_in"]).is_null())
+        ~pl.all(pl.col(["target", "found_in", "source_samples"]).is_null())
     )
 
     unmatched = combined_otu_table.filter(
-        (pl.col("target").is_null()) & (pl.col("found_in").is_null())
+        pl.all(pl.col(["target", "found_in", "source_samples"]).is_null())
     )
 
     # Summarise recovery stats
     summary = summarise_stats(matches, combined_otu_table, recovered_bins)
 
     return matches, unmatched, summary
 
@@ -141,22 +165,34 @@
         recovered_hits.with_columns(
             pl.when(
                 pl.col("found_in").is_not_null()
             ).then("match").otherwise("nonmatch").alias("status")
         ).groupby([
             "coassembly", "status"
         ]).agg(
-            pl.col("sequence").len().alias("nontarget_sequences")
+            pl.col("sequence").len().alias("nontarget_bin_sequences")
+        ),
+        on=["coassembly", "status"], how="outer"
+    ).join(
+        # Duplicate sequences are counted multiple times to give a proportion at bin level
+        recovered_hits.with_columns(
+            pl.when(
+                pl.all(pl.col(["target", "found_in"]).is_null()) & (pl.col("source_samples").is_not_null())
+            ).then("match").otherwise("nonmatch").alias("status")
+        ).groupby([
+            "coassembly", "status"
+        ]).agg(
+            pl.col("sequence").len().alias("nontarget_unbin_sequences")
         ),
         on=["coassembly", "status"], how="outer"
     ).join(
         # Duplicate sequences are counted multiple times to give a proportion at bin level
         recovered_hits.with_columns(
             pl.when(
-                (pl.col("found_in").is_null()) & (pl.col("target").is_null())
+                pl.all(pl.col(["target", "found_in", "source_samples"]).is_null())
             ).then("match").otherwise("nonmatch").alias("status")
         ).groupby([
             "coassembly", "status"
         ]).agg(
             pl.col("sequence").len().alias("novel_sequences")
         ),
         on=["coassembly", "status"], how="outer"
@@ -165,15 +201,15 @@
     ).fill_null(
         0
     )
 
     recovered_counts = pl.from_dict(recovered_bins
     ).melt(variable_name="name"
     ).with_columns(
-        pl.col("name").str.split("-").arr.to_struct(upper_bound=2, name_generator=lambda id: ["coassembly", "genome"][id])
+        pl.col("name").str.split("-").arr.to_struct(upper_bound=2, fields=["coassembly", "genome"])
     ).unnest("name"
     ).groupby("coassembly"
     ).agg(
         pl.count().alias("n")
     ).with_columns(
         pl.lit("match").alias("status"),
         pl.lit("bins").alias("statistic"),
@@ -185,15 +221,15 @@
         pl.col("n").alias("value") - pl.col("match")
     )
 
     summary = pl.concat([
         summary.filter((pl.col("statistic") != "bins") | (pl.col("status") != "nonmatch")),
         recovered_counts
     ]).pivot(
-        index=["coassembly", "statistic"], values="value", columns="status"
+        index=["coassembly", "statistic"], values="value", columns="status", aggregate_function=None
     ).select(
         "coassembly", "statistic",
         pl.when(pl.col("statistic").is_in(["sequences", "taxonomy"])).then("targets").otherwise("recovery").alias("within"),
         "match", "nonmatch",
         pl.col("match").alias("total") + pl.col("nonmatch"),
         (pl.col("match") / (pl.col("match") + pl.col("nonmatch")) * 100).round(2).alias("match_percent"),
     ).sort(
@@ -202,30 +238,30 @@
 
     return summary
 
 if __name__ == "__main__":
     os.environ["POLARS_MAX_THREADS"] = str(snakemake.threads)
     import polars as pl
 
-    unbinned_path = snakemake.params.unbinned_otu_table
+    target_path = snakemake.params.target_otu_table
     binned_path = snakemake.params.binned_otu_table
     elusive_clusters_path = snakemake.params.elusive_clusters
     elusive_edges_path = snakemake.params.elusive_edges
     recovered_otu_table_path = snakemake.input.recovered_otu_table
     recovered_bins = snakemake.params.recovered_bins
     matched_hits_path = snakemake.output.matched_hits
     novel_hits_path = snakemake.output.novel_hits
     summary_stats_path = snakemake.output.summary_stats
 
-    unbinned_otu_table = pl.read_csv(unbinned_path, sep="\t")
-    binned_otu_table = pl.read_csv(binned_path, sep="\t")
-    elusive_clusters = pl.read_csv(elusive_clusters_path, sep="\t")
-    elusive_edges = pl.read_csv(elusive_edges_path, sep="\t")
-    recovered_otu_table = pl.read_csv(recovered_otu_table_path, sep="\t")
+    target_otu_table = pl.read_csv(target_path, separator="\t")
+    binned_otu_table = pl.read_csv(binned_path, separator="\t")
+    elusive_clusters = pl.read_csv(elusive_clusters_path, separator="\t")
+    elusive_edges = pl.read_csv(elusive_edges_path, separator="\t")
+    recovered_otu_table = pl.read_csv(recovered_otu_table_path, separator="\t")
 
-    matches, unmatched, summary = evaluate(unbinned_otu_table, binned_otu_table, elusive_clusters, elusive_edges, recovered_otu_table, recovered_bins)
+    matches, unmatched, summary = evaluate(target_otu_table, binned_otu_table, elusive_clusters, elusive_edges, recovered_otu_table, recovered_bins)
     # Export hits matching elusive targets
-    matches.write_csv(matched_hits_path, sep="\t")
+    matches.write_csv(matched_hits_path, separator="\t")
     # Export non-elusive sequence hits
-    unmatched.write_csv(novel_hits_path, sep="\t")
+    unmatched.write_csv(novel_hits_path, separator="\t")
     # Export summary stats
-    summary.write_csv(summary_stats_path, sep="\t")
+    summary.write_csv(summary_stats_path, separator="\t")
```

### Comparing `ibis-genome-0.6.0/ibis/workflow/scripts/query_processing.py` & `ibis-genome-0.7.1/ibis/workflow/scripts/query_processing.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,28 +50,32 @@
         appraised, on=["gene", "sample", "sequence", "num_hits", "coverage", "taxonomy"], how="left"
     ).filter(~pl.col("binned").fill_null(False)
     ).drop(["divergence", "binned"]
     ).with_columns(
         pl.lit(None).cast(str).alias("found_in")
     )
 
+    # Filter out EIF
+    binned = binned.filter(pl.col("gene") != "S3.18.EIF_2_alpha")
+    unbinned = unbinned.filter(pl.col("gene") != "S3.18.EIF_2_alpha")
+
     return binned, unbinned
 
 def pipeline(
     query_reads,
     pipe_reads,
     SEQUENCE_IDENTITY=0.86,
     WINDOW_SIZE=60):
 
     print(f"Polars using {str(pl.threadpool_size())} threads")
 
     for query, pipe in zip(query_reads, pipe_reads):
         binned, unbinned = processing(
-            pl.read_csv(query, sep = "\t"),
-            pl.read_csv(pipe, sep = "\t"),
+            pl.read_csv(query, separator="\t"),
+            pl.read_csv(pipe, separator="\t"),
             SEQUENCE_IDENTITY,
             WINDOW_SIZE)
         yield binned, unbinned
 
 if __name__ == "__main__":
     os.environ["POLARS_MAX_THREADS"] = str(snakemake.threads)
     import polars as pl
@@ -89,10 +93,10 @@
         SEQUENCE_IDENTITY=SEQUENCE_IDENTITY,
         WINDOW_SIZE=WINDOW_SIZE
         )
 
     with open(binned_path, "ab") as binned_file, open(unbinned_path, "ab") as unbinned_file:
         first = True
         for binned, unbinned in outputs:
-            binned.write_csv(binned_file, sep="\t", has_header=first)
-            unbinned.write_csv(unbinned_file, sep="\t", has_header=first)
+            binned.write_csv(binned_file, separator="\t", has_header=first)
+            unbinned.write_csv(unbinned_file, separator="\t", has_header=first)
             first = False
```

### Comparing `ibis-genome-0.6.0/ibis/workflow/scripts/separate_SingleM_seq.py` & `ibis-genome-0.7.1/ibis/workflow/scripts/separate_SingleM_seq.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.6.0/ibis/workflow/scripts/summarise_coassemblies.py` & `ibis-genome-0.7.1/ibis/workflow/scripts/summarise_coassemblies.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.6.0/ibis/workflow/scripts/target_elusive.py` & `ibis-genome-0.7.1/ibis/workflow/scripts/target_elusive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #########################
 ### target_elusive.py ###
 #########################
 # Author: Samuel Aroney
 
 import polars as pl
 import os
-from itertools import combinations
 
 EDGES_COLUMNS={
     "taxa_group": str,
     "weight": int,
     "target_ids": str,
     "sample1": str,
     "sample2": str
@@ -87,16 +86,16 @@
 
     MIN_COASSEMBLY_COVERAGE = snakemake.params.min_coassembly_coverage
     TAXA_OF_INTEREST = snakemake.params.taxa_of_interest
     unbinned_path = snakemake.input.unbinned
     targets_path = snakemake.output.output_targets
     edges_path = snakemake.output.output_edges
 
-    unbinned = pl.read_csv(unbinned_path, sep="\t")
+    unbinned = pl.read_csv(unbinned_path, separator="\t")
 
     targets, edges = pipeline(
         unbinned,
         MIN_COASSEMBLY_COVERAGE=MIN_COASSEMBLY_COVERAGE,
         TAXA_OF_INTEREST=TAXA_OF_INTEREST
         )
-    targets.write_csv(targets_path, sep="\t")
-    edges.write_csv(edges_path, sep="\t")
+    targets.write_csv(targets_path, separator="\t")
+    edges.write_csv(edges_path, separator="\t")
```

### Comparing `ibis-genome-0.6.0/ibis_genome.egg-info/PKG-INFO` & `ibis-genome-0.7.1/ibis_genome.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibis-genome
-Version: 0.6.0
+Version: 0.7.1
 Summary: Ibis (Australian bin chicken) - targeted recovery of low abundance genomes through intelligent coassembly
 Author-email: Samuel Aroney <samuel.aroney@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ibis-genome-0.6.0/ibis_genome.egg-info/SOURCES.txt` & `ibis-genome-0.7.1/ibis_genome.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,10 +31,11 @@
 ibis_genome.egg-info/top_level.txt
 test/test_cluster_graph.py
 test/test_coassemble.py
 test/test_collect_reference_bins.py
 test/test_evaluate.py
 test/test_evaluate_script.py
 test/test_iterate.py
+test/test_no_genomes.py
 test/test_query_processing.py
 test/test_target_elusive.py
 test/test_unmap.py
```

### Comparing `ibis-genome-0.6.0/pyproject.toml` & `ibis-genome-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.6.0/test/test_cluster_graph.py` & `ibis-genome-0.7.1/test/test_cluster_graph.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.6.0/test/test_coassemble.py` & `ibis-genome-0.7.1/test/test_coassemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,25 +22,33 @@
 ])
 GENOMES = " ".join([os.path.join(path_to_data, "GB_GCA_013286235.1.fna")])
 TWO_GENOMES = " ".join([
     os.path.join(path_to_data, "GB_GCA_013286235.1.fna"),
     os.path.join(path_to_data, "GB_GCA_013286235.2.fna"),
     ])
 METAPACKAGE = os.path.join(path_to_data, "singlem_metapackage.smpkg")
+METAPACKAGE_EIF = os.path.join(path_to_data, "singlem_metapackage_EIF.smpkg")
 
 MOCK_COASSEMBLE = os.path.join(path_to_data, "mock_coassemble")
 
 SAMPLE_READ_SIZE = os.path.join(MOCK_COASSEMBLE, "read_size2.csv")
 SAMPLE_SINGLEM = ' '.join([
     os.path.join(MOCK_COASSEMBLE, "pipe", "sample_1_read.otu_table.tsv"),
     os.path.join(MOCK_COASSEMBLE, "pipe", "sample_2_read.otu_table.tsv"),
     os.path.join(MOCK_COASSEMBLE, "pipe", "sample_3_read.otu_table.tsv"),
     ])
+SAMPLE_SINGLEM_EIF = ' '.join([
+    os.path.join(MOCK_COASSEMBLE, "pipe_EIF", "sample_1_read.otu_table.tsv"),
+    os.path.join(MOCK_COASSEMBLE, "pipe_EIF", "sample_2_read.otu_table.tsv"),
+    os.path.join(MOCK_COASSEMBLE, "pipe_EIF", "sample_3_read.otu_table.tsv"),
+    ])
+
 GENOME_TRANSCRIPTS = ' '.join([os.path.join(path_to_data, "GB_GCA_013286235.1_protein.fna")])
 GENOME_SINGLEM = os.path.join(MOCK_COASSEMBLE, "summarise", "bins_summarised.otu_table2.tsv")
+GENOME_SINGLEM_EIF = os.path.join(MOCK_COASSEMBLE, "summarise", "bins_summarised_EIF.otu_table.tsv")
 
 SAMPLE_QUERY_DIR = os.path.join(path_to_data, "query")
 SAMPLE_QUERY = ' '.join([
     os.path.join(path_to_data, "query", "sample_1_query.otu_table.tsv"),
     os.path.join(path_to_data, "query", "sample_2_query.otu_table.tsv"),
     os.path.join(path_to_data, "query", "sample_3_query.otu_table.tsv"),
     ])
@@ -60,14 +68,15 @@
             cmd = (
                 f"ibis coassemble "
                 f"--forward {SAMPLE_READS_FORWARD} "
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
                 f"--singlem-metapackage {METAPACKAGE} "
                 f"--assemble-unmapped "
+                f"--unmapping-max-identity 95 "
                 f"--prodigal-meta "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
             )
             extern.run(cmd)
 
             config_path = os.path.join("test", "config.yaml")
@@ -798,15 +807,15 @@
                 f"ibis coassemble "
                 f"--forward {SAMPLE_READS_FORWARD} "
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
                 f"--genome-transcripts {GENOME_TRANSCRIPTS} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
-                f"--snakemake-args \"singlem_appraise\" "
+                f"--snakemake-args \"singlem_appraise_filtered\" "
             )
             import subprocess
             _ = subprocess.run(cmd, shell=True, check=True, capture_output=True, env=os.environ)
 
             appraise_path = os.path.join("test", "coassemble", "appraise", "binned.otu_table.tsv")
             self.assertTrue(os.path.exists(appraise_path))
             expected = "\n".join(
@@ -817,10 +826,47 @@
                     "\t".join(["S3.7.ribosomal_protein_S7", "sample_3.1", "TTCCAGGTGCCTACCGAAGTTCGTCCCGAGCGTAAAATTGCATTGGGTATGAAATGGCTC", "1", "1.64", "Root; d__Bacteria; p__Bacteroidota; c__Bacteroidia; o__Sphingobacteriales; f__Sphingobacteriaceae; g__Mucilaginibacter; s__Mucilaginibacter_sp013286235", "GB_GCA_013286235.1_protein"]),
                     ""
                 ]
             )
             with open(appraise_path) as f:
                 self.assertEqual(expected, f.read())
 
+    def test_coassemble_remove_EIF(self):
+        with in_tempdir():
+            cmd = (
+                f"ibis coassemble "
+                f"--forward {SAMPLE_READS_FORWARD} "
+                f"--reverse {SAMPLE_READS_REVERSE} "
+                f"--genomes {GENOMES} "
+                f"--genome-transcripts {GENOME_TRANSCRIPTS} "
+                f"--sample-singlem {SAMPLE_SINGLEM_EIF} "
+                f"--sample-read-size {SAMPLE_READ_SIZE} "
+                f"--genome-singlem {GENOME_SINGLEM_EIF} "
+                f"--singlem-metapackage {METAPACKAGE_EIF} "
+                f"--output test "
+                f"--conda-prefix {path_to_conda} "
+                f"--snakemake-args \"target_elusive\" "
+            )
+            output = extern.run(cmd)
+
+            unbinned_path = os.path.join("test", "coassemble", "appraise", "unbinned.otu_table.tsv")
+            self.assertTrue(os.path.exists(unbinned_path))
+            expected = "\n".join(
+                [
+                    "\t".join(["gene", "sample", "sequence", "num_hits", "coverage", "taxonomy", "found_in"]),
+                    "\t".join(["S3.7.ribosomal_protein_S7", "sample_1.1", "TATCAAGTTCCACAAGAAGTTAGAGGAGAAAGAAGAATCTCGTTAGCTATTAGATGGATT", "3", "4.92", "Root; d__Bacteria; p__Proteobacteria; c__Gammaproteobacteria; o__Burkholderiales; f__Burkholderiaceae; g__Polynucleobacter; s__Polynucleobacter sp018688335", ""]),
+                    "\t".join(["S3.7.ribosomal_protein_S7", "sample_1.1", "TACCAGGTCCCGGTCGAGGTCCGTCCGATCCGCCAGACGACGCTCGCCCTGCGCTGGCTC", "5", "8.21", "Root; d__Bacteria; p__Actinobacteriota; c__Actinomycetia; o__Mycobacteriales; f__Mycobacteriaceae; g__Nocardia; s__Nocardia grenadensis", ""]),
+                    "\t".join(["S3.7.ribosomal_protein_S7", "sample_1.1", "TATCAGGTGCCTATTGAGGTAAGACCTGAAAGAAGACAGACTTTAGCGCTTCGCTGGATA", "1", "1.64", "Root; d__Bacteria; p__Actinobacteriota; c__Actinomycetia; o__Mycobacteriales; f__Mycobacteriaceae; g__Nocardia; s__Nocardia grenadensis2", ""]),
+                    "\t".join(["S3.7.ribosomal_protein_S7", "sample_1.1", "TATCAGGTGCCTATTGAGGTAAGACCTGAAAGAAGACAGACTTTAGCGCTTCGCTGGATC", "5", "8.21", "Root; d__Bacteria; p__Actinobacteriota; c__Actinomycetia; o__Mycobacteriales; f__Mycobacteriaceae; g__Nocardia; s__Nocardia grenadensis3", ""]),
+                    "\t".join(["S3.7.ribosomal_protein_S7", "sample_2.1", "TATCAAGTTCCACAAGAAGTTAGAGGAGAAAGAAGAATCTCGTTAGCTATTAGATGGATT", "4", "6.57", "Root; d__Bacteria; p__Proteobacteria; c__Gammaproteobacteria; o__Burkholderiales; f__Burkholderiaceae; g__Polynucleobacter; s__Polynucleobacter sp018688335", ""]),
+                    "\t".join(["S3.7.ribosomal_protein_S7", "sample_2.1", "TACCAGGTCCCGGTCGAGGTCCGTCCGATCCGCCAGACGACGCTCGCCCTGCGCTGGCTC", "3", "4.92", "Root; d__Bacteria; p__Actinobacteriota; c__Actinomycetia; o__Mycobacteriales; f__Mycobacteriaceae; g__Nocardia; s__Nocardia grenadensis", ""]),
+                    "\t".join(["S3.7.ribosomal_protein_S7", "sample_3.1", "TATCAGGTGCCTATTGAGGTAAGACCTGAAAGAAGACAGACTTTAGCGCTTCGCTGGATA", "6", "9.85", "Root; d__Bacteria; p__Actinobacteriota; c__Actinomycetia; o__Mycobacteriales; f__Mycobacteriaceae; g__Nocardia; s__Nocardia grenadensis2", ""]),
+                    "\t".join(["S3.7.ribosomal_protein_S7", "sample_3.1", "TATCAGGTGCCTATTGAGGTAAGACCTGAAAGAAGACAGACTTTAGCGCTTCGCTGGATC", "5", "8.21", "Root; d__Bacteria; p__Actinobacteriota; c__Actinomycetia; o__Mycobacteriales; f__Mycobacteriaceae; g__Nocardia; s__Nocardia grenadensis3", ""]),
+                    ""
+                ]
+            )
+            with open(unbinned_path) as f:
+                self.assertEqual(expected, f.read())
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ibis-genome-0.6.0/test/test_collect_reference_bins.py` & `ibis-genome-0.7.1/test/test_collect_reference_bins.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.6.0/test/test_evaluate.py` & `ibis-genome-0.7.1/test/test_evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,23 +74,32 @@
                         "1",
                         "1",
                         "2",
                         "50.0",
                     ]),
                     "\t".join([
                         "coassembly_0",
-                        "nontarget_sequences",
+                        "nontarget_bin_sequences",
                         "recovery",
                         "1",
                         "2",
                         "3",
                         "33.33",
                     ]),
                     "\t".join([
                         "coassembly_0",
+                        "nontarget_unbin_sequences",
+                        "recovery",
+                        "0",
+                        "3",
+                        "3",
+                        "0.0",
+                    ]),
+                    "\t".join([
+                        "coassembly_0",
                         "novel_sequences",
                         "recovery",
                         "1",
                         "2",
                         "3",
                         "33.33",
                     ]),
```

### Comparing `ibis-genome-0.6.0/test/test_evaluate_script.py` & `ibis-genome-0.7.1/test/test_evaluate_script.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 OUTPUT_COLUMNS={
     "coassembly": str,
     "gene": str,
     "sequence": str,
     "genome": str,
     "target": str,
     "found_in": str,
+    "source_samples": str,
     "taxonomy": str,
     }
 SUMMARY_COLUMNS = {
     "coassembly": str,
     "statistic": str,
     "within": str,
     "match": int,
@@ -36,60 +37,68 @@
     def assertDataFrameEqual(self, a, b):
         assert_frame_equal(a, b, check_dtype=False, check_row_order=False)
 
     def test_evaluate_script(self):
         targets = pl.DataFrame([
             ["S3.1", "sample_1.1", "AAA", 5, 10.0, "Root; old", 10],
             ["S3.1", "sample_2.1", "AAA", 5, 10.0, "Root; old", 10],
+            ["S3.1", "sample_1.1", "CCC", 1, 2.0, "Root; old", 11],
+            ["S3.1", "sample_2.1", "CCC", 1, 2.0, "Root; old", 11],
+            ["S3.1", "sample_1.1", "DDD", 1, 2.0, "Root; old", 12],
         ], schema=TARGET_COLUMNS)
-        nontargets = pl.DataFrame([
+        binned = pl.DataFrame([
             ["S3.1", "sample_1.1", "BBB", 5, 10.0, "Root; old", "oldgenome_1"],
         ], schema=APPRAISE_COLUMNS)
         clusters = pl.DataFrame([
             ["sample_1,sample_2", 2, 1, 1, 100, "sample_1,sample_2,sample_3", "coassembly_0"],
         ], schema=CLUSTER_COLUMNS)
         edges = pl.DataFrame([
             ["Root", 1, "10", "sample_1.1", "sample_2.1"],
         ], schema=EDGE_COLUMNS)
         recovered = pl.DataFrame([
             ["S3.1", "coassembly_0-genome_1_transcripts", "AAA", 1, 2.0, "Root"],
             ["S3.1", "coassembly_0-genome_1_transcripts", "AAB", 1, 2.0, "Root"],
             ["S3.1", "coassembly_0-genome_1_transcripts", "BBB", 1, 2.0, "Root"],
+            ["S3.1", "coassembly_0-genome_1_transcripts", "CCC", 1, 2.0, "Root"],
+            ["S3.1", "coassembly_0-genome_1_transcripts", "DDD", 1, 2.0, "Root"],
         ], schema=SINGLEM_COLUMNS)
         recovered_bins = {
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "Root"],
-            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
+            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1", "Root"],
+            ["coassembly_0", "S3.1", "CCC", "genome_1_transcripts", None, None, "sample_1,sample_2", "Root"],
+            ["coassembly_0", "S3.1", "DDD", "genome_1_transcripts", None, None, "sample_1", "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 1, 0, 1, 100],
             ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
-            ["coassembly_0", "nontarget_sequences", "recovery", 1, 2, 3, 33.33],
-            ["coassembly_0", "novel_sequences", "recovery", 1, 2, 3, 33.33],
+            ["coassembly_0", "nontarget_bin_sequences", "recovery", 1, 4, 5, 20.00],
+            ["coassembly_0", "nontarget_unbin_sequences", "recovery", 2, 3, 5, 40.00],
+            ["coassembly_0", "novel_sequences", "recovery", 1, 4, 5, 20.00],
             ["coassembly_0", "bins", "recovery", 1, 1, 2, 50],
         ], schema=SUMMARY_COLUMNS)
 
-        observed_matches, observed_unmatched, observed_summary = evaluate(targets, nontargets, clusters, edges, recovered, recovered_bins)
+        observed_matches, observed_unmatched, observed_summary = evaluate(targets, binned, clusters, edges, recovered, recovered_bins)
         self.assertDataFrameEqual(expected_matches, observed_matches)
         self.assertDataFrameEqual(expected_unmatched, observed_unmatched)
         self.assertDataFrameEqual(expected_summary, observed_summary)
 
     def test_evaluate_script_all_targets(self):
         targets = pl.DataFrame([
             ["S3.1", "sample_1.1", "AAA", 5, 10.0, "Root; old", 10],
             ["S3.1", "sample_2.1", "AAA", 5, 10.0, "Root; old", 10],
         ], schema=TARGET_COLUMNS)
-        nontargets = pl.DataFrame([
+        binned = pl.DataFrame([
             ["S3.1", "sample_1.1", "BBB", 5, 10.0, "Root; old", "oldgenome_1"],
         ], schema=APPRAISE_COLUMNS)
         clusters = pl.DataFrame([
             ["sample_1,sample_2", 2, 1, 1, 100, "sample_1,sample_2,sample_3", "coassembly_0"],
         ], schema=CLUSTER_COLUMNS)
         edges = pl.DataFrame([
             ["Root", 1, "10", "sample_1.1", "sample_2.1"],
@@ -99,37 +108,38 @@
         ], schema=SINGLEM_COLUMNS)
         recovered_bins = {
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 1, 0, 1, 100],
             ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
-            ["coassembly_0", "nontarget_sequences", "recovery", 0, 1, 1, 0],
+            ["coassembly_0", "nontarget_bin_sequences", "recovery", 0, 1, 1, 0],
+            ["coassembly_0", "nontarget_unbin_sequences", "recovery", 0, 1, 1, 0],
             ["coassembly_0", "novel_sequences", "recovery", 0, 1, 1, 0],
             ["coassembly_0", "bins", "recovery", 1, 1, 2, 50],
         ], schema=SUMMARY_COLUMNS)
 
-        observed_matches, observed_unmatched, observed_summary = evaluate(targets, nontargets, clusters, edges, recovered, recovered_bins)
+        observed_matches, observed_unmatched, observed_summary = evaluate(targets, binned, clusters, edges, recovered, recovered_bins)
         self.assertDataFrameEqual(expected_matches, observed_matches)
         self.assertDataFrameEqual(expected_unmatched, observed_unmatched)
         self.assertDataFrameEqual(expected_summary, observed_summary)
 
     def test_evaluate_script_none_targets(self):
         targets = pl.DataFrame([
             ["S3.1", "sample_1.1", "AAA", 5, 10.0, "Root; old", 10],
             ["S3.1", "sample_2.1", "AAA", 5, 10.0, "Root; old", 10],
         ], schema=TARGET_COLUMNS)
-        nontargets = pl.DataFrame([
+        binned = pl.DataFrame([
             ["S3.1", "sample_1.1", "BBB", 5, 10.0, "Root; old", "oldgenome_1"],
         ], schema=APPRAISE_COLUMNS)
         clusters = pl.DataFrame([
             ["sample_1,sample_2", 2, 1, 1, 100, "sample_1,sample_2,sample_3", "coassembly_0"],
         ], schema=CLUSTER_COLUMNS)
         edges = pl.DataFrame([
             ["Root", 1, "10", "sample_1.1", "sample_2.1"],
@@ -139,38 +149,41 @@
         ], schema=SINGLEM_COLUMNS)
         recovered_bins = {
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", None, "10", None, "Root; old"],
+            ["coassembly_0", "S3.1", "AAA", None, "10", None, "sample_1,sample_2", "Root; old"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 0, 1, 1, 0],
             ["coassembly_0", "taxonomy", "targets", 0, 1, 1, 0],
-            ["coassembly_0", "nontarget_sequences", "recovery", 0, 1, 1, 0],
+            ["coassembly_0", "nontarget_bin_sequences", "recovery", 0, 1, 1, 0],
+            ["coassembly_0", "nontarget_unbin_sequences", "recovery", 0, 1, 1, 0],
             ["coassembly_0", "novel_sequences", "recovery", 1, 0, 1, 100],
             ["coassembly_0", "bins", "recovery", 0, 2, 2, 0],
         ], schema=SUMMARY_COLUMNS)
 
-        observed_matches, observed_unmatched, observed_summary = evaluate(targets, nontargets, clusters, edges, recovered, recovered_bins)
+        observed_matches, observed_unmatched, observed_summary = evaluate(targets, binned, clusters, edges, recovered, recovered_bins)
         self.assertDataFrameEqual(expected_matches, observed_matches)
         self.assertDataFrameEqual(expected_unmatched, observed_unmatched)
         self.assertDataFrameEqual(expected_summary, observed_summary)
 
     def test_evaluate_script_empty_recovery(self):
         targets = pl.DataFrame([
             ["S3.1", "sample_1.1", "AAA", 5, 10.0, "Root; old", 10],
             ["S3.1", "sample_2.1", "AAA", 5, 10.0, "Root; old", 10],
+            ["S3.1", "sample_1.1", "CCC", 1, 2.0, "Root; old", 11],
+            ["S3.1", "sample_2.1", "CCC", 1, 2.0, "Root; old", 11],
         ], schema=TARGET_COLUMNS)
-        nontargets = pl.DataFrame([
+        binned = pl.DataFrame([
             ["S3.1", "sample_1.1", "BBB", 5, 10.0, "Root; old", "oldgenome_1"],
         ], schema=APPRAISE_COLUMNS)
         clusters = pl.DataFrame([
             ["sample_1,sample_2", 2, 1, 1, 100, "sample_1,sample_2,sample_3", "coassembly_0"],
         ], schema=CLUSTER_COLUMNS)
         edges = pl.DataFrame([
             ["Root", 1, "10", "sample_1.1", "sample_2.1"],
@@ -183,25 +196,25 @@
         expected_matches = pl.DataFrame([
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
         ], schema=SUMMARY_COLUMNS)
 
-        observed_matches, observed_unmatched, observed_summary = evaluate(targets, nontargets, clusters, edges, recovered, recovered_bins)
+        observed_matches, observed_unmatched, observed_summary = evaluate(targets, binned, clusters, edges, recovered, recovered_bins)
         self.assertDataFrameEqual(expected_matches, observed_matches)
         self.assertDataFrameEqual(expected_unmatched, observed_unmatched)
         self.assertDataFrameEqual(expected_summary, observed_summary)
 
     def test_evaluate_script_nontarget_wrong_sample(self):
         targets = pl.DataFrame([
             ["S3.1", "sample_1.1", "AAA", 5, 10.0, "Root; old", 10],
             ["S3.1", "sample_2.1", "AAA", 5, 10.0, "Root; old", 10],
         ], schema=TARGET_COLUMNS)
-        nontargets = pl.DataFrame([
+        binned = pl.DataFrame([
             ["S3.1", "sample_3.1", "BBB", 5, 10.0, "Root; old", "oldgenome_1"],
         ], schema=APPRAISE_COLUMNS)
         clusters = pl.DataFrame([
             ["sample_1,sample_2", 2, 1, 1, 100, "sample_1,sample_2,sample_3", "coassembly_0"],
         ], schema=CLUSTER_COLUMNS)
         edges = pl.DataFrame([
             ["Root", 1, "10", "sample_1.1", "sample_2.1"],
@@ -213,39 +226,40 @@
         ], schema=SINGLEM_COLUMNS)
         recovered_bins = {
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, "Root"],
-            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
+            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 1, 0, 1, 100],
             ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
-            ["coassembly_0", "nontarget_sequences", "recovery", 0, 3, 3, 0],
+            ["coassembly_0", "nontarget_bin_sequences", "recovery", 0, 3, 3, 0],
+            ["coassembly_0", "nontarget_unbin_sequences", "recovery", 0, 3, 3, 0],
             ["coassembly_0", "novel_sequences", "recovery", 2, 1, 3, 66.67],
             ["coassembly_0", "bins", "recovery", 1, 1, 2, 50],
         ], schema=SUMMARY_COLUMNS)
 
-        observed_matches, observed_unmatched, observed_summary = evaluate(targets, nontargets, clusters, edges, recovered, recovered_bins)
+        observed_matches, observed_unmatched, observed_summary = evaluate(targets, binned, clusters, edges, recovered, recovered_bins)
         self.assertDataFrameEqual(expected_matches, observed_matches)
         self.assertDataFrameEqual(expected_unmatched, observed_unmatched)
         self.assertDataFrameEqual(expected_summary, observed_summary)
 
     def test_evaluate_script_samples_with_same_sequence(self):
         targets = pl.DataFrame([
             ["S3.1", "sample_1.1", "AAA", 5, 10.0, "Root; old", 10],
             ["S3.1", "sample_2.1", "AAA", 5, 10.0, "Root; old", 10],
         ], schema=TARGET_COLUMNS)
-        nontargets = pl.DataFrame([
+        binned = pl.DataFrame([
             ["S3.1", "sample_1.1", "BBB", 5, 10.0, "Root; old", "oldgenome_1"],
             ["S3.1", "sample_2.1", "BBB", 5, 10.0, "Root; old", "oldgenome_1"],
         ], schema=APPRAISE_COLUMNS)
         clusters = pl.DataFrame([
             ["sample_1,sample_2", 2, 1, 1, 100, "sample_1,sample_2,sample_3", "coassembly_0"],
         ], schema=CLUSTER_COLUMNS)
         edges = pl.DataFrame([
@@ -258,41 +272,44 @@
         ], schema=SINGLEM_COLUMNS)
         recovered_bins = {
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "Root"],
-            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
+            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1,sample_2", "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 1, 0, 1, 100],
             ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
-            ["coassembly_0", "nontarget_sequences", "recovery", 1, 2, 3, 33.33],
+            ["coassembly_0", "nontarget_bin_sequences", "recovery", 1, 2, 3, 33.33],
+            ["coassembly_0", "nontarget_unbin_sequences", "recovery", 0, 3, 3, 0],
             ["coassembly_0", "novel_sequences", "recovery", 1, 2, 3, 33.33],
             ["coassembly_0", "bins", "recovery", 1, 1, 2, 50],
         ], schema=SUMMARY_COLUMNS)
 
-        observed_matches, observed_unmatched, observed_summary = evaluate(targets, nontargets, clusters, edges, recovered, recovered_bins)
+        observed_matches, observed_unmatched, observed_summary = evaluate(targets, binned, clusters, edges, recovered, recovered_bins)
         self.assertDataFrameEqual(expected_matches, observed_matches)
         self.assertDataFrameEqual(expected_unmatched, observed_unmatched)
         self.assertDataFrameEqual(expected_summary, observed_summary)
 
     def test_evaluate_script_multiple_coassemblies(self):
         targets = pl.DataFrame([
             ["S3.1", "sample_1.1", "AAA", 5, 10.0, "Root; old", 10],
             ["S3.1", "sample_2.1", "AAA", 5, 10.0, "Root; old", 10],
             ["S3.1", "sample_1.1", "CCC", 5, 10.0, "Root; old", 11],
             ["S3.1", "sample_3.1", "CCC", 5, 10.0, "Root; old", 11],
+            ["S3.1", "sample_1.1", "EEE", 1, 2.0, "Root; old", 12],
+            ["S3.1", "sample_3.1", "EEE", 1, 2.0, "Root; old", 12],
         ], schema=TARGET_COLUMNS)
-        nontargets = pl.DataFrame([
+        binned = pl.DataFrame([
             ["S3.1", "sample_1.1", "BBB", 5, 10.0, "Root; old", "oldgenome_1"],
             ["S3.1", "sample_3.1", "DDD", 5, 10.0, "Root; old", "oldgenome_2"],
         ], schema=APPRAISE_COLUMNS)
         clusters = pl.DataFrame([
             ["sample_1,sample_2", 2, 1, 1, 100, "sample_1,sample_2,sample_3", "coassembly_0"],
             ["sample_1,sample_3", 2, 1, 1, 100, "sample_1,sample_2,sample_3", "coassembly_1"],
         ], schema=CLUSTER_COLUMNS)
@@ -303,58 +320,62 @@
         recovered = pl.DataFrame([
             ["S3.1", "coassembly_0-genome_1_transcripts", "AAA", 1, 2.0, "Root"],
             ["S3.1", "coassembly_0-genome_1_transcripts", "AAB", 1, 2.0, "Root"],
             ["S3.1", "coassembly_0-genome_1_transcripts", "BBB", 1, 2.0, "Root"],
             ["S3.1", "coassembly_1-genome_1_transcripts", "CCC", 1, 2.0, "Root"],
             ["S3.1", "coassembly_1-genome_1_transcripts", "CCD", 1, 2.0, "Root"],
             ["S3.1", "coassembly_1-genome_1_transcripts", "DDD", 1, 2.0, "Root"],
+            ["S3.1", "coassembly_1-genome_1_transcripts", "EEE", 1, 2.0, "Root"],
         ], schema=SINGLEM_COLUMNS)
         recovered_bins = {
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             "coassembly_1-genome_0": "genome_0.fna",
             "coassembly_1-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "Root"],
-            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "Root"],
-            ["coassembly_1", "S3.1", "CCC", "genome_1_transcripts", "11", None, "Root"],
-            ["coassembly_1", "S3.1", "DDD", "genome_1_transcripts", None, "oldgenome_2", "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
+            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1", "Root"],
+            ["coassembly_1", "S3.1", "CCC", "genome_1_transcripts", "11", None, "sample_1,sample_3", "Root"],
+            ["coassembly_1", "S3.1", "DDD", "genome_1_transcripts", None, "oldgenome_2", "sample_3", "Root"],
+            ["coassembly_1", "S3.1", "EEE", "genome_1_transcripts", None, None, "sample_1,sample_3", "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, "Root"],
-            ["coassembly_1", "S3.1", "CCD", "genome_1_transcripts", None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
+            ["coassembly_1", "S3.1", "CCD", "genome_1_transcripts", None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 1, 0, 1, 100],
             ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
-            ["coassembly_0", "nontarget_sequences", "recovery", 1, 2, 3, 33.33],
+            ["coassembly_0", "nontarget_bin_sequences", "recovery", 1, 2, 3, 33.33],
+            ["coassembly_0", "nontarget_unbin_sequences", "recovery", 0, 3, 3, 0],
             ["coassembly_0", "novel_sequences", "recovery", 1, 2, 3, 33.33],
             ["coassembly_0", "bins", "recovery", 1, 1, 2, 50],
             ["coassembly_1", "sequences", "targets", 1, 0, 1, 100],
             ["coassembly_1", "taxonomy", "targets", 1, 0, 1, 100],
-            ["coassembly_1", "nontarget_sequences", "recovery", 1, 2, 3, 33.33],
-            ["coassembly_1", "novel_sequences", "recovery", 1, 2, 3, 33.33],
+            ["coassembly_1", "nontarget_bin_sequences", "recovery", 1, 3, 4, 25.0],
+            ["coassembly_1", "nontarget_unbin_sequences", "recovery", 1, 3, 4, 25.0],
+            ["coassembly_1", "novel_sequences", "recovery", 1, 3, 4, 25.0],
             ["coassembly_1", "bins", "recovery", 1, 1, 2, 50],
         ], schema=SUMMARY_COLUMNS)
 
-        observed_matches, observed_unmatched, observed_summary = evaluate(targets, nontargets, clusters, edges, recovered, recovered_bins)
+        observed_matches, observed_unmatched, observed_summary = evaluate(targets, binned, clusters, edges, recovered, recovered_bins)
         self.assertDataFrameEqual(expected_matches, observed_matches)
         self.assertDataFrameEqual(expected_unmatched, observed_unmatched)
         self.assertDataFrameEqual(expected_summary, observed_summary)
 
     def test_evaluate_script_subset_coassembly(self):
         targets = pl.DataFrame([
             ["S3.1", "sample_1.1", "AAA", 5, 10.0, "Root; old", 10],
             ["S3.1", "sample_2.1", "AAA", 5, 10.0, "Root; old", 10],
             ["S3.1", "sample_1.1", "CCC", 5, 10.0, "Root; old", 11],
             ["S3.1", "sample_3.1", "CCC", 5, 10.0, "Root; old", 11],
         ], schema=TARGET_COLUMNS)
-        nontargets = pl.DataFrame([
+        binned = pl.DataFrame([
             ["S3.1", "sample_1.1", "BBB", 5, 10.0, "Root; old", "oldgenome_1"],
             ["S3.1", "sample_3.1", "DDD", 5, 10.0, "Root; old", "oldgenome_2"],
         ], schema=APPRAISE_COLUMNS)
         clusters = pl.DataFrame([
             ["sample_1,sample_2,sample_3", 3, 1, 1, 100, "sample_1,sample_2,sample_3", "coassembly_0"],
             ["sample_1,sample_2", 2, 1, 1, 100, "sample_1,sample_2,sample_3", "coassembly_1"],
         ], schema=CLUSTER_COLUMNS)
@@ -377,40 +398,42 @@
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             "coassembly_1-genome_0": "genome_0.fna",
             "coassembly_1-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "Root"],
-            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "Root"],
-            ["coassembly_0", "S3.1", "CCC", "genome_1_transcripts", "11", None, "Root"],
-            ["coassembly_0", "S3.1", "DDD", "genome_1_transcripts", None, "oldgenome_2", "Root"],
-            ["coassembly_1", "S3.1", "AAA", "genome_1_transcripts", "10", None, "Root"],
-            ["coassembly_1", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
+            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1", "Root"],
+            ["coassembly_0", "S3.1", "CCC", "genome_1_transcripts", "11", None, "sample_1,sample_3", "Root"],
+            ["coassembly_0", "S3.1", "DDD", "genome_1_transcripts", None, "oldgenome_2", "sample_3", "Root"],
+            ["coassembly_1", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
+            ["coassembly_1", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1", "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, "Root"],
-            ["coassembly_0", "S3.1", "CCD", "genome_1_transcripts", None, None, "Root"],
-            ["coassembly_1", "S3.1", "AAB", "genome_1_transcripts", None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
+            ["coassembly_0", "S3.1", "CCD", "genome_1_transcripts", None, None, None, "Root"],
+            ["coassembly_1", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 2, 0, 2, 100],
             ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
-            ["coassembly_0", "nontarget_sequences", "recovery", 2, 4, 6, 33.33],
+            ["coassembly_0", "nontarget_bin_sequences", "recovery", 2, 4, 6, 33.33],
+            ["coassembly_0", "nontarget_unbin_sequences", "recovery", 0, 6, 6, 0],
             ["coassembly_0", "novel_sequences", "recovery", 2, 4, 6, 33.33],
             ["coassembly_0", "bins", "recovery", 1, 1, 2, 50],
             ["coassembly_1", "sequences", "targets", 1, 0, 1, 100],
             ["coassembly_1", "taxonomy", "targets", 1, 0, 1, 100],
-            ["coassembly_1", "nontarget_sequences", "recovery", 1, 2, 3, 33.33],
+            ["coassembly_1", "nontarget_bin_sequences", "recovery", 1, 2, 3, 33.33],
+            ["coassembly_1", "nontarget_unbin_sequences", "recovery", 0, 3, 3, 0],
             ["coassembly_1", "novel_sequences", "recovery", 1, 2, 3, 33.33],
             ["coassembly_1", "bins", "recovery", 1, 1, 2, 50],
         ], schema=SUMMARY_COLUMNS)
 
-        observed_matches, observed_unmatched, observed_summary = evaluate(targets, nontargets, clusters, edges, recovered, recovered_bins)
+        observed_matches, observed_unmatched, observed_summary = evaluate(targets, binned, clusters, edges, recovered, recovered_bins)
         self.assertDataFrameEqual(expected_matches, observed_matches)
         self.assertDataFrameEqual(expected_unmatched, observed_unmatched)
         self.assertDataFrameEqual(expected_summary, observed_summary)
 
     def test_evaluate_script_duplicate_sequences(self):
         targets = pl.DataFrame([
             ["S3.1", "sample_1.1", "AAA", 5, 10.0, "Root; old", 10],
@@ -418,15 +441,15 @@
             ["S3.1", "sample_1.1", "CCC", 5, 10.0, "Root; old", 11],
             ["S3.1", "sample_2.1", "CCC", 5, 10.0, "Root; old", 11],
             ["S3.1", "sample_1.1", "YYY", 5, 10.0, "Root; old", 98],
             ["S3.1", "sample_2.1", "YYY", 5, 10.0, "Root; old", 98],
             ["S3.1", "sample_2.1", "ZZZ", 5, 10.0, "Root; old", 99],
             ["S3.1", "sample_3.1", "ZZZ", 5, 10.0, "Root; old", 99],
         ], schema=TARGET_COLUMNS)
-        nontargets = pl.DataFrame([
+        binned = pl.DataFrame([
             ["S3.1", "sample_3.1", "BBB", 5, 10.0, "Root; old", "oldgenome_1"],
             ["S3.1", "sample_1.1", "DDD", 5, 10.0, "Root; old", "oldgenome_2"],
         ], schema=APPRAISE_COLUMNS)
         clusters = pl.DataFrame([
             ["sample_1,sample_2,sample_3", 3, 2, 2, 3000, "sample_1,sample_2,sample_3", "coassembly_0"],
             ["sample_1,sample_2", 2, 2, 2, 2000, "sample_1,sample_2,sample_3", "coassembly_1"],
         ], schema=CLUSTER_COLUMNS)
@@ -449,42 +472,89 @@
             "coassembly_0-genome_1": "genome_1.fna",
             "coassembly_1-genome_0": "genome_0.fna",
             "coassembly_1-genome_1": "genome_1.fna",
             "coassembly_1-genome_2": "genome_2.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_0_transcripts", "10", None, "Root"],
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "Root"],
-            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "Root"],
-            ["coassembly_0", "S3.1", "CCC", None, "11", None, "Root; old"],
-            ["coassembly_0", "S3.1", "YYY", None, "98", None, "Root; old"],
-            ["coassembly_0", "S3.1", "ZZZ", None, "99", None, "Root; old"],
-            ["coassembly_1", "S3.1", "CCC", "genome_1_transcripts", "11", None, "Root"],
-            ["coassembly_1", "S3.1", "DDD", "genome_1_transcripts", None, "oldgenome_2", "Root"],
-            ["coassembly_1", "S3.1", "YYY", None, "98", None, "Root; old"],
+            ["coassembly_0", "S3.1", "AAA", "genome_0_transcripts", "10", None, "sample_1,sample_3", "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_3", "Root"],
+            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_3", "Root"],
+            ["coassembly_0", "S3.1", "CCC", None, "11", None, "sample_1,sample_2", "Root; old"],
+            ["coassembly_0", "S3.1", "YYY", None, "98", None, "sample_1,sample_2", "Root; old"],
+            ["coassembly_0", "S3.1", "ZZZ", None, "99", None, "sample_2,sample_3", "Root; old"],
+            ["coassembly_1", "S3.1", "CCC", "genome_1_transcripts", "11", None, "sample_1,sample_2", "Root"],
+            ["coassembly_1", "S3.1", "DDD", "genome_1_transcripts", None, "oldgenome_2", "sample_1", "Root"],
+            ["coassembly_1", "S3.1", "YYY", None, "98", None, "sample_1,sample_2", "Root; old"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, "Root"],
-            ["coassembly_1", "S3.1", "CCD", "genome_1_transcripts", None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
+            ["coassembly_1", "S3.1", "CCD", "genome_1_transcripts", None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 1, 3, 4, 25],
             ["coassembly_0", "taxonomy", "targets", 1, 1, 2, 50],
-            ["coassembly_0", "nontarget_sequences", "recovery", 1, 3, 4, 25],
+            ["coassembly_0", "nontarget_bin_sequences", "recovery", 1, 3, 4, 25],
+            ["coassembly_0", "nontarget_unbin_sequences", "recovery", 0, 4, 4, 0],
             ["coassembly_0", "novel_sequences", "recovery", 1, 3, 4, 25],
             ["coassembly_0", "bins", "recovery", 2, 0, 2, 100],
             ["coassembly_1", "sequences", "targets", 1, 1, 2, 50],
             ["coassembly_1", "taxonomy", "targets", 1, 1, 2, 50],
-            ["coassembly_1", "nontarget_sequences", "recovery", 1, 2, 3, 33.33],
+            ["coassembly_1", "nontarget_bin_sequences", "recovery", 1, 2, 3, 33.33],
+            ["coassembly_1", "nontarget_unbin_sequences", "recovery", 0, 3, 3, 0],
             ["coassembly_1", "novel_sequences", "recovery", 1, 2, 3, 33.33],
             ["coassembly_1", "bins", "recovery", 1, 2, 3, 33.33],
         ], schema=SUMMARY_COLUMNS)
 
-        observed_matches, observed_unmatched, observed_summary = evaluate(targets, nontargets, clusters, edges, recovered, recovered_bins)
+        observed_matches, observed_unmatched, observed_summary = evaluate(targets, binned, clusters, edges, recovered, recovered_bins)
+        self.assertDataFrameEqual(expected_matches, observed_matches)
+        self.assertDataFrameEqual(expected_unmatched, observed_unmatched)
+        self.assertDataFrameEqual(expected_summary, observed_summary)
+
+    def test_evaluate_script_other_sample_target(self):
+        targets = pl.DataFrame([
+            ["S3.1", "sample_1.1", "AAA", 5, 10.0, "Root; old", 10],
+            ["S3.1", "sample_2.1", "AAA", 5, 10.0, "Root; old", 10],
+            ["S3.1", "sample_1.1", "CCC", 1, 2.0, "Root; old", 11],
+            ["S3.1", "sample_3.1", "CCC", 1, 2.0, "Root; old", 11],
+        ], schema=TARGET_COLUMNS)
+        binned = pl.DataFrame([
+            ["S3.1", "sample_1.1", "BBB", 5, 10.0, "Root; old", "oldgenome_1"],
+        ], schema=APPRAISE_COLUMNS)
+        clusters = pl.DataFrame([
+            ["sample_1,sample_2", 2, 1, 1, 100, "sample_1,sample_2,sample_3", "coassembly_0"],
+        ], schema=CLUSTER_COLUMNS)
+        edges = pl.DataFrame([
+            ["Root", 1, "10", "sample_1.1", "sample_2.1"],
+        ], schema=EDGE_COLUMNS)
+        recovered = pl.DataFrame([
+            ["S3.1", "coassembly_0-genome_1_transcripts", "AAA", 1, 2.0, "Root"],
+            ["S3.1", "coassembly_0-genome_1_transcripts", "CCC", 1, 2.0, "Root"],
+        ], schema=SINGLEM_COLUMNS)
+        recovered_bins = {
+            "coassembly_0-genome_0": "genome_0.fna",
+            "coassembly_0-genome_1": "genome_1.fna",
+            }
+
+        expected_matches = pl.DataFrame([
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
+            ["coassembly_0", "S3.1", "CCC", "genome_1_transcripts", None, None, "sample_1", "Root"],
+        ], schema=OUTPUT_COLUMNS)
+        expected_unmatched = pl.DataFrame([
+        ], schema=OUTPUT_COLUMNS)
+        expected_summary = pl.DataFrame([
+            ["coassembly_0", "sequences", "targets", 1, 0, 1, 100],
+            ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
+            ["coassembly_0", "nontarget_bin_sequences", "recovery", 0, 2, 2, 0],
+            ["coassembly_0", "nontarget_unbin_sequences", "recovery", 1, 1, 2, 50.0],
+            ["coassembly_0", "novel_sequences", "recovery", 0, 2, 2, 0],
+            ["coassembly_0", "bins", "recovery", 1, 1, 2, 50],
+        ], schema=SUMMARY_COLUMNS)
+
+        observed_matches, observed_unmatched, observed_summary = evaluate(targets, binned, clusters, edges, recovered, recovered_bins)
         self.assertDataFrameEqual(expected_matches, observed_matches)
         self.assertDataFrameEqual(expected_unmatched, observed_unmatched)
         self.assertDataFrameEqual(expected_summary, observed_summary)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ibis-genome-0.6.0/test/test_iterate.py` & `ibis-genome-0.7.1/test/test_iterate.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.6.0/test/test_query_processing.py` & `ibis-genome-0.7.1/test/test_query_processing.py`

 * *Files 8% similar despite different names*

```diff
@@ -195,10 +195,35 @@
             ["S3.1", "sample_1", "AAB", 5, 10, "Root", None],
         ], schema=APPRAISE_COLUMNS)
 
         observed_binned, observed_unbinned = processing(query, pipe, SEQUENCE_IDENTITY = 0.94)
         self.assertDataFrameEqual(expected_binned, observed_binned)
         self.assertDataFrameEqual(expected_unbinned, observed_unbinned)
 
+    def test_query_processing_remove_EIF(self):
+        query = pl.DataFrame([
+            ["sample_1", "AAA", 1, 5, 10, "genome_1", "S3.1", "AAA", "Root"],
+            ["sample_1", "AAB", 10, 5, 10, "genome_1", "S3.1", "AAA", "Root"],
+            ["sample_1", "CCC", 1, 5, 10, "genome_1", "S3.18.EIF_2_alpha", "AAA", "Root"],
+            ["sample_1", "CCD", 10, 5, 10, "genome_1", "S3.18.EIF_2_alpha", "AAA", "Root"],
+        ], schema=QUERY_COLUMNS)
+        pipe = pl.DataFrame([
+            ["S3.1", "sample_1", "AAA", 5, 10, "Root"],
+            ["S3.1", "sample_1", "AAB", 5, 10, "Root"],
+            ["S3.18.EIF_2_alpha", "sample_1", "CCC", 5, 10, "Root"],
+            ["S3.18.EIF_2_alpha", "sample_1", "CCD", 5, 10, "Root"],
+        ], schema=PIPE_COLUMNS)
+
+        expected_binned = pl.DataFrame([
+            ["S3.1", "sample_1", "AAA", 5, 10, "Root", "genome_1"],
+        ], schema=APPRAISE_COLUMNS)
+        expected_unbinned = pl.DataFrame([
+            ["S3.1", "sample_1", "AAB", 5, 10, "Root", None],
+        ], schema=APPRAISE_COLUMNS)
+
+        observed_binned, observed_unbinned = processing(query, pipe)
+        self.assertDataFrameEqual(expected_binned, observed_binned)
+        self.assertDataFrameEqual(expected_unbinned, observed_unbinned)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ibis-genome-0.6.0/test/test_target_elusive.py` & `ibis-genome-0.7.1/test/test_target_elusive.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.6.0/test/test_unmap.py` & `ibis-genome-0.7.1/test/test_unmap.py`

 * *Files identical despite different names*

