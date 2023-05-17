# Comparing `tmp/labxpipe-0.6.0.tar.gz` & `tmp/labxpipe-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labxpipe-0.6.0.tar", last modified: Wed Apr 19 16:00:19 2023, max compression
+gzip compressed data, was "labxpipe-0.7.0.tar", last modified: Wed May 17 02:14:01 2023, max compression
```

## Comparing `labxpipe-0.6.0.tar` & `labxpipe-0.7.0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.572254 labxpipe-0.6.0/
--rw-r--r--   0 build     (1000) build     (1001)       17 2023-04-19 15:59:30.000000 labxpipe-0.6.0/.gitignore
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.562253 labxpipe-0.6.0/.sourcehut/
--rw-r--r--   0 build     (1000) build     (1001)     1272 2023-04-19 15:59:30.000000 labxpipe-0.6.0/.sourcehut/arch.yml
--rw-r--r--   0 build     (1000) build     (1001)    16726 2023-04-19 15:59:30.000000 labxpipe-0.6.0/LICENSE
--rw-r--r--   0 build     (1000) build     (1001)    12773 2023-04-19 16:00:19.568920 labxpipe-0.6.0/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1001)    12477 2023-04-19 15:59:30.000000 labxpipe-0.6.0/README.md
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.562253 labxpipe-0.6.0/config/
--rw-r--r--   0 build     (1000) build     (1001)     1065 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/labxpipe.json
--rw-r--r--   0 build     (1000) build     (1001)     1123 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/labxpipe_trackhub.json
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.562253 labxpipe-0.6.0/config/pipelines/
--rw-r--r--   0 build     (1000) build     (1001)     2189 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/pipelines/chip_seq.json
--rw-r--r--   0 build     (1000) build     (1001)     2440 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/pipelines/mrna_seq.json
--rw-r--r--   0 build     (1000) build     (1001)     2226 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/pipelines/mrna_seq_cufflinks.json
--rw-r--r--   0 build     (1000) build     (1001)     2898 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/pipelines/mrna_seq_no_db.json
--rw-r--r--   0 build     (1000) build     (1001)     2802 2023-04-19 15:59:30.000000 labxpipe-0.6.0/config/pipelines/mrna_seq_with_plotting.json
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.562253 labxpipe-0.6.0/img/
--rw-r--r--   0 build     (1000) build     (1001)     5728 2023-04-19 15:59:30.000000 labxpipe-0.6.0/img/logo.svg
--rw-r--r--   0 build     (1000) build     (1001)      581 2023-04-19 15:59:30.000000 labxpipe-0.6.0/pyproject.toml
--rw-r--r--   0 build     (1000) build     (1001)       38 2023-04-19 16:00:19.572254 labxpipe-0.6.0/setup.cfg
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.562253 labxpipe-0.6.0/src/
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.565586 labxpipe-0.6.0/src/labxpipe/
--rw-r--r--   0 build     (1000) build     (1001)        0 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/__init__.py
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.565586 labxpipe-0.6.0/src/labxpipe/interfaces/
--rw-r--r--   0 build     (1000) build     (1001)        0 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/__init__.py
--rw-r--r--   0 build     (1000) build     (1001)     1547 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_bg2bw.py
--rw-r--r--   0 build     (1000) build     (1001)     5817 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_bowtie2.py
--rw-r--r--   0 build     (1000) build     (1001)     2336 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_cufflinks.py
--rw-r--r--   0 build     (1000) build     (1001)     8069 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_geneabacus.py
--rw-r--r--   0 build     (1000) build     (1001)     4642 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_minimap2.py
--rw-r--r--   0 build     (1000) build     (1001)     4564 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_readknead.py
--rw-r--r--   0 build     (1000) build     (1001)     2423 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_samtools.py
--rw-r--r--   0 build     (1000) build     (1001)     6569 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_star.py
--rw-r--r--   0 build     (1000) build     (1001)     2876 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/parallel_helpers.py
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.568920 labxpipe-0.6.0/src/labxpipe/steps/
--rw-r--r--   0 build     (1000) build     (1001)      423 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/__init__.py
--rw-r--r--   0 build     (1000) build     (1001)     4181 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/bowtie2.py
--rw-r--r--   0 build     (1000) build     (1001)     1431 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/cleaning.py
--rw-r--r--   0 build     (1000) build     (1001)     2413 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/cufflinks.py
--rw-r--r--   0 build     (1000) build     (1001)     6565 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/geneabacus.py
--rw-r--r--   0 build     (1000) build     (1001)     3677 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/minimap2.py
--rw-r--r--   0 build     (1000) build     (1001)     5492 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/readknead.py
--rw-r--r--   0 build     (1000) build     (1001)     2950 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/samtools_sort.py
--rw-r--r--   0 build     (1000) build     (1001)     3625 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/samtools_uniquify.py
--rw-r--r--   0 build     (1000) build     (1001)     3235 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/steps/star.py
--rw-r--r--   0 build     (1000) build     (1001)     8654 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/trackhub.py
--rw-r--r--   0 build     (1000) build     (1001)     1739 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe/utils.py
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.565586 labxpipe-0.6.0/src/labxpipe.egg-info/
--rw-r--r--   0 build     (1000) build     (1001)    12773 2023-04-19 16:00:19.000000 labxpipe-0.6.0/src/labxpipe.egg-info/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1001)     1715 2023-04-19 16:00:19.000000 labxpipe-0.6.0/src/labxpipe.egg-info/SOURCES.txt
--rw-r--r--   0 build     (1000) build     (1001)        1 2023-04-19 16:00:19.000000 labxpipe-0.6.0/src/labxpipe.egg-info/dependency_links.txt
--rw-r--r--   0 build     (1000) build     (1001)       56 2023-04-19 16:00:19.000000 labxpipe-0.6.0/src/labxpipe.egg-info/entry_points.txt
--rw-r--r--   0 build     (1000) build     (1001)       44 2023-04-19 16:00:19.000000 labxpipe-0.6.0/src/labxpipe.egg-info/requires.txt
--rw-r--r--   0 build     (1000) build     (1001)       26 2023-04-19 16:00:19.000000 labxpipe-0.6.0/src/labxpipe.egg-info/top_level.txt
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-04-19 16:00:19.568920 labxpipe-0.6.0/src/labxpipe_scripts/
--rw-r--r--   0 build     (1000) build     (1001)        0 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/__init__.py
--rwxr-xr-x   0 build     (1000) build     (1001)     2440 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe.py
--rwxr-xr-x   0 build     (1000) build     (1001)    15493 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_demultiplex.py
--rwxr-xr-x   0 build     (1000) build     (1001)     7803 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_extract.py
--rwxr-xr-x   0 build     (1000) build     (1001)     7704 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_generate.py
--rwxr-xr-x   0 build     (1000) build     (1001)    17284 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_merge_count.py
--rwxr-xr-x   0 build     (1000) build     (1001)     4243 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_profile.py
--rwxr-xr-x   0 build     (1000) build     (1001)    13924 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_report.py
--rwxr-xr-x   0 build     (1000) build     (1001)    16815 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_run.py
--rwxr-xr-x   0 build     (1000) build     (1001)    21424 2023-04-19 15:59:30.000000 labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_trackhub.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.047361 labxpipe-0.7.0/
+-rw-r--r--   0 build     (1000) build     (1001)       17 2023-05-17 02:13:32.000000 labxpipe-0.7.0/.gitignore
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.037437 labxpipe-0.7.0/.sourcehut/
+-rw-r--r--   0 build     (1000) build     (1001)     1272 2023-05-17 02:13:32.000000 labxpipe-0.7.0/.sourcehut/arch.yml
+-rw-r--r--   0 build     (1000) build     (1001)    16726 2023-05-17 02:13:32.000000 labxpipe-0.7.0/LICENSE
+-rw-r--r--   0 build     (1000) build     (1001)    12773 2023-05-17 02:14:01.047361 labxpipe-0.7.0/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1001)    12477 2023-05-17 02:13:32.000000 labxpipe-0.7.0/README.md
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.037437 labxpipe-0.7.0/config/
+-rw-r--r--   0 build     (1000) build     (1001)     1065 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/labxpipe.json
+-rw-r--r--   0 build     (1000) build     (1001)     1123 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/labxpipe_trackhub.json
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.037437 labxpipe-0.7.0/config/pipelines/
+-rw-r--r--   0 build     (1000) build     (1001)     2189 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/pipelines/chip_seq.json
+-rw-r--r--   0 build     (1000) build     (1001)     2440 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/pipelines/mrna_seq.json
+-rw-r--r--   0 build     (1000) build     (1001)     2226 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/pipelines/mrna_seq_cufflinks.json
+-rw-r--r--   0 build     (1000) build     (1001)     2898 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/pipelines/mrna_seq_no_db.json
+-rw-r--r--   0 build     (1000) build     (1001)     2802 2023-05-17 02:13:32.000000 labxpipe-0.7.0/config/pipelines/mrna_seq_with_plotting.json
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.040745 labxpipe-0.7.0/img/
+-rw-r--r--   0 build     (1000) build     (1001)     5728 2023-05-17 02:13:32.000000 labxpipe-0.7.0/img/logo.svg
+-rw-r--r--   0 build     (1000) build     (1001)      581 2023-05-17 02:13:32.000000 labxpipe-0.7.0/pyproject.toml
+-rw-r--r--   0 build     (1000) build     (1001)       38 2023-05-17 02:14:01.047361 labxpipe-0.7.0/setup.cfg
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.037437 labxpipe-0.7.0/src/
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.040745 labxpipe-0.7.0/src/labxpipe/
+-rw-r--r--   0 build     (1000) build     (1001)        0 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/__init__.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.044053 labxpipe-0.7.0/src/labxpipe/interfaces/
+-rw-r--r--   0 build     (1000) build     (1001)        0 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/__init__.py
+-rw-r--r--   0 build     (1000) build     (1001)     1547 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_bg2bw.py
+-rw-r--r--   0 build     (1000) build     (1001)     5817 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_bowtie2.py
+-rw-r--r--   0 build     (1000) build     (1001)     4700 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_bwa_mem2.py
+-rw-r--r--   0 build     (1000) build     (1001)     2336 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_cufflinks.py
+-rw-r--r--   0 build     (1000) build     (1001)     8069 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_geneabacus.py
+-rw-r--r--   0 build     (1000) build     (1001)     4642 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_minimap2.py
+-rw-r--r--   0 build     (1000) build     (1001)     4564 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_readknead.py
+-rw-r--r--   0 build     (1000) build     (1001)     2733 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_samtools.py
+-rw-r--r--   0 build     (1000) build     (1001)     6569 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_star.py
+-rw-r--r--   0 build     (1000) build     (1001)     2876 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/parallel_helpers.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.044053 labxpipe-0.7.0/src/labxpipe/steps/
+-rw-r--r--   0 build     (1000) build     (1001)      423 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/__init__.py
+-rw-r--r--   0 build     (1000) build     (1001)     4181 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/bowtie2.py
+-rw-r--r--   0 build     (1000) build     (1001)     4152 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/bwa_mem2.py
+-rw-r--r--   0 build     (1000) build     (1001)     1431 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/cleaning.py
+-rw-r--r--   0 build     (1000) build     (1001)     2413 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/cufflinks.py
+-rw-r--r--   0 build     (1000) build     (1001)     6565 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/geneabacus.py
+-rw-r--r--   0 build     (1000) build     (1001)     4238 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/minimap2.py
+-rw-r--r--   0 build     (1000) build     (1001)     5492 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/readknead.py
+-rw-r--r--   0 build     (1000) build     (1001)     2950 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/samtools_sort.py
+-rw-r--r--   0 build     (1000) build     (1001)     3625 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/samtools_uniquify.py
+-rw-r--r--   0 build     (1000) build     (1001)     3235 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/steps/star.py
+-rw-r--r--   0 build     (1000) build     (1001)     8654 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/trackhub.py
+-rw-r--r--   0 build     (1000) build     (1001)     1739 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe/utils.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.040745 labxpipe-0.7.0/src/labxpipe.egg-info/
+-rw-r--r--   0 build     (1000) build     (1001)    12773 2023-05-17 02:14:00.000000 labxpipe-0.7.0/src/labxpipe.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1001)     1789 2023-05-17 02:14:01.000000 labxpipe-0.7.0/src/labxpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1001)        1 2023-05-17 02:14:01.000000 labxpipe-0.7.0/src/labxpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1001)       56 2023-05-17 02:14:01.000000 labxpipe-0.7.0/src/labxpipe.egg-info/entry_points.txt
+-rw-r--r--   0 build     (1000) build     (1001)       44 2023-05-17 02:14:01.000000 labxpipe-0.7.0/src/labxpipe.egg-info/requires.txt
+-rw-r--r--   0 build     (1000) build     (1001)       26 2023-05-17 02:14:01.000000 labxpipe-0.7.0/src/labxpipe.egg-info/top_level.txt
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-05-17 02:14:01.047361 labxpipe-0.7.0/src/labxpipe_scripts/
+-rw-r--r--   0 build     (1000) build     (1001)        0 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/__init__.py
+-rwxr-xr-x   0 build     (1000) build     (1001)     2440 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    15493 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_demultiplex.py
+-rwxr-xr-x   0 build     (1000) build     (1001)     7803 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_extract.py
+-rwxr-xr-x   0 build     (1000) build     (1001)     7704 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_generate.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    17284 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_merge_count.py
+-rwxr-xr-x   0 build     (1000) build     (1001)     4243 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_profile.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    13924 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_report.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    16815 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_run.py
+-rwxr-xr-x   0 build     (1000) build     (1001)    21424 2023-05-17 02:13:32.000000 labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_trackhub.py
```

### Comparing `labxpipe-0.6.0/.sourcehut/arch.yml` & `labxpipe-0.7.0/.sourcehut/arch.yml`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/LICENSE` & `labxpipe-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/PKG-INFO` & `labxpipe-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labxpipe
-Version: 0.6.0
+Version: 0.7.0
 Summary: Genomics pipelines
 Author: Charles E. Vejnar
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: homepage, https://git.sr.ht/~vejnar/LabxPipe
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `labxpipe-0.6.0/README.md` & `labxpipe-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/config/labxpipe.json` & `labxpipe-0.7.0/config/labxpipe.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/config/labxpipe_trackhub.json` & `labxpipe-0.7.0/config/labxpipe_trackhub.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/config/pipelines/chip_seq.json` & `labxpipe-0.7.0/config/pipelines/chip_seq.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/config/pipelines/mrna_seq.json` & `labxpipe-0.7.0/config/pipelines/mrna_seq.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/config/pipelines/mrna_seq_cufflinks.json` & `labxpipe-0.7.0/config/pipelines/mrna_seq_cufflinks.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/config/pipelines/mrna_seq_no_db.json` & `labxpipe-0.7.0/config/pipelines/mrna_seq_no_db.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/config/pipelines/mrna_seq_with_plotting.json` & `labxpipe-0.7.0/config/pipelines/mrna_seq_with_plotting.json`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/img/logo.svg` & `labxpipe-0.7.0/img/logo.svg`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/pyproject.toml` & `labxpipe-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_bg2bw.py` & `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_bg2bw.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_bowtie2.py` & `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_bowtie2.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_cufflinks.py` & `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_cufflinks.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_geneabacus.py` & `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_geneabacus.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_minimap2.py` & `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_minimap2.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_readknead.py` & `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_readknead.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_samtools.py` & `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_samtools.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,18 +62,28 @@
 def sam_stats(bam_fname, exe=None, logger=None):
     # Defaults
     if exe is None:
         exe = 'samtools'
     if logger is None:
         import logging as logger
     # Command
-    cmd = [exe, 'stats', bam_fname]
+    cmd = [exe, 'stats']
+    # Input
+    if bam_fname.endswith('.zst'):
+        p_input = subprocess.Popen(['zstdcat', bam_fname], stdout=subprocess.PIPE)
+        p_stdin = p_input.stdout
+    else:
+        cmd.append(bam_fname)
+        p_stdin = None
     logger.info('Compute SAM statistics with ' + str(cmd))
     # Run
-    p = subprocess.run(cmd, check=True, stdout=subprocess.PIPE, text=True)
+    p = subprocess.run(cmd, check=True, stdin=p_stdin, stdout=subprocess.PIPE, text=True)
+    # Wait for input process
+    if p_stdin is not None:
+        p_input.wait()
     # Parse
     report = {}
     for rec in [l.strip().split('\t') for l in p.stdout.split('\n') if l.startswith('SN')]:
         f = rec[1].strip(':')
         if '.' in rec[2]:
             report[f] = float(rec[2])
         else:
```

### Comparing `labxpipe-0.6.0/src/labxpipe/interfaces/if_exe_star.py` & `labxpipe-0.7.0/src/labxpipe/interfaces/if_exe_star.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/parallel_helpers.py` & `labxpipe-0.7.0/src/labxpipe/parallel_helpers.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/steps/bowtie2.py` & `labxpipe-0.7.0/src/labxpipe/steps/bowtie2.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/steps/cleaning.py` & `labxpipe-0.7.0/src/labxpipe/steps/cleaning.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/steps/cufflinks.py` & `labxpipe-0.7.0/src/labxpipe/steps/cufflinks.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/steps/geneabacus.py` & `labxpipe-0.7.0/src/labxpipe/steps/geneabacus.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/steps/minimap2.py` & `labxpipe-0.7.0/src/labxpipe/steps/bwa_mem2.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 # Copyright © 2023 Charles E. Vejnar
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://www.mozilla.org/MPL/2.0/.
 #
 
+import glob
 import logging
 import os
 
-from ..interfaces import if_exe_minimap2
+from ..interfaces import if_exe_bwa_mem2
 from ..interfaces import if_exe_samtools
 from ..utils import get_fastqs_per_end
 from ..utils import write_report
 
-functions = ['minimap2']
+functions = ['bwa-mem2']
 
 
 def get_max_ram(num_processor):
     # Assume 8GB per core
     return int((8 * 1024 * 1024 * 1024) / (num_processor * 0.2))
 
 
@@ -28,49 +29,49 @@
     # Parameters
     logger = logging.getLogger(params['logger_name'] + '.' + params['step_name'])
 
     # Keep output SAM if BAM is requested by user
     compress_output_cmd = params.get('compress_output_cmd')
     if params.get('compress_output', False) and compress_output_cmd is None:
         if params.get('create_bam', False) or params.get('index_bam', False):
-            compress_output_cmd = ['zstd', '--keep', '-12']
+            compress_output_cmd = ['zstd', '--keep', '-12', f"-T{params['num_processor']}"]
         else:
-            compress_output_cmd = ['zstd', '--rm', '-12']
+            compress_output_cmd = ['zstd', '--rm', '-12', f"-T{params['num_processor']}"]
         logger.info(f'Output compression using {compress_output_cmd}')
 
     # Input
     fq_files = get_fastqs_per_end(path_in, params.get('paired'), params.get('fastq_exts'), params.get('read_regexs_in'))
     # Check input
     if len(fq_files) == 0:
         raise ValueError('No input FASTQ file found')
 
-    # Minimap2 suppl. parameters
+    # bwa-mem2 suppl. parameters
     others = []
     if 'options' in params:
         others.extend(params['options'])
 
     # Executable
-    if 'path_minimap2' in params:
-        minimap2_exe = os.path.join(params['path_minimap2'], 'minimap2')
+    if 'path_bwa-mem2' in params:
+        bwa_mem2_exe = os.path.join(params['path_bwa-mem2'], 'bwa-mem2')
     else:
-        minimap2_exe = None
+        bwa_mem2_exe = None
 
     # Version
-    logger.info(f'Using Minimap2 {if_exe_minimap2.get_minimap2_version(minimap2_exe)}')
+    logger.info(f'Using bwa-mem2 {if_exe_bwa_mem2.get_bwa_mem2_version(bwa_mem2_exe)}')
 
     # Align
-    stdout, stderr = if_exe_minimap2.minimap2(
+    stdout, stderr = if_exe_bwa_mem2.bwa_mem2(
         [f for fqfs in fq_files for f in fqfs],
         outfile=os.path.join(path_out, params['output']),
-        index=os.path.join(params['path_minimap2_index'], params['index']),
+        index=os.path.join(params['path_bwa-mem2_index'], params['index']),
         num_processor=str(params['num_processor']),
         compress_output=params.get('compress_output', False),
         compress_output_cmd=compress_output_cmd,
         others=others,
-        exe=minimap2_exe,
+        exe=bwa_mem2_exe,
         return_std=True,
         cwd=path_out,
         logger=logger,
     )
 
     # Create and index BAM file
     if params.get('create_bam', False):
@@ -84,24 +85,31 @@
         )
         if_exe_samtools.create_bam_index(
             os.path.join(path_out, params['output'].replace('.sam', '.bam')), logger=logger
         )
 
     # Logs
     logger.info('Report: Writing logs')
-    with open(os.path.join(path_out, 'minimap2_err.log'), 'wt') as f:
+    with open(os.path.join(path_out, 'bwa-mem2_err.log'), 'wt') as f:
         f.write(stderr)
-    with open(os.path.join(path_out, 'minimap2_out.log'), 'wt') as f:
+    with open(os.path.join(path_out, 'bwa-mem2_out.log'), 'wt') as f:
         f.write(stdout)
 
     # Compute report
     logger.info('Report')
     report = {}
     # Input
-    report = if_exe_minimap2.get_minimap2_report(os.path.join(path_out, 'minimap2_err.log'))
-    # Output: If output is SAM
-    if '-a' in others:
-        raw_report = if_exe_samtools.sam_stats(os.path.join(path_out, params['output']), logger=logger)
-        report['output'] = raw_report['reads mapped']
+    report = if_exe_bwa_mem2.get_bwa_mem2_report(os.path.join(path_out, 'bwa-mem2_err.log'))
+    # Find output
+    if params.get('create_bam', False) or params.get('index_bam', False):
+        path_output_sam = params['output'].replace('.sam', '.bam')
+    elif params.get('compress_output', False):
+        # Get the first output file with an extension added by compression software
+        path_output_sam = os.path.basename(glob.glob(os.path.join(path_out, params['output'] + '.*'))[0])
+    else:
+        path_output_sam = params['output']
+    # Output
+    raw_report = if_exe_samtools.sam_stats(os.path.join(path_out, path_output_sam), logger=logger)
+    report['output'] = raw_report['reads mapped']
     # Report
     logger.info('Report: Writing stats')
     write_report(os.path.join(path_out, params['step_name'] + '_report'), report)
```

### Comparing `labxpipe-0.6.0/src/labxpipe/steps/readknead.py` & `labxpipe-0.7.0/src/labxpipe/steps/readknead.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/steps/samtools_sort.py` & `labxpipe-0.7.0/src/labxpipe/steps/samtools_sort.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/steps/samtools_uniquify.py` & `labxpipe-0.7.0/src/labxpipe/steps/samtools_uniquify.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/steps/star.py` & `labxpipe-0.7.0/src/labxpipe/steps/star.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/trackhub.py` & `labxpipe-0.7.0/src/labxpipe/trackhub.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe/utils.py` & `labxpipe-0.7.0/src/labxpipe/utils.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe.egg-info/PKG-INFO` & `labxpipe-0.7.0/src/labxpipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labxpipe
-Version: 0.6.0
+Version: 0.7.0
 Summary: Genomics pipelines
 Author: Charles E. Vejnar
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: homepage, https://git.sr.ht/~vejnar/LabxPipe
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `labxpipe-0.6.0/src/labxpipe.egg-info/SOURCES.txt` & `labxpipe-0.7.0/src/labxpipe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,24 @@
 src/labxpipe.egg-info/dependency_links.txt
 src/labxpipe.egg-info/entry_points.txt
 src/labxpipe.egg-info/requires.txt
 src/labxpipe.egg-info/top_level.txt
 src/labxpipe/interfaces/__init__.py
 src/labxpipe/interfaces/if_exe_bg2bw.py
 src/labxpipe/interfaces/if_exe_bowtie2.py
+src/labxpipe/interfaces/if_exe_bwa_mem2.py
 src/labxpipe/interfaces/if_exe_cufflinks.py
 src/labxpipe/interfaces/if_exe_geneabacus.py
 src/labxpipe/interfaces/if_exe_minimap2.py
 src/labxpipe/interfaces/if_exe_readknead.py
 src/labxpipe/interfaces/if_exe_samtools.py
 src/labxpipe/interfaces/if_exe_star.py
 src/labxpipe/steps/__init__.py
 src/labxpipe/steps/bowtie2.py
+src/labxpipe/steps/bwa_mem2.py
 src/labxpipe/steps/cleaning.py
 src/labxpipe/steps/cufflinks.py
 src/labxpipe/steps/geneabacus.py
 src/labxpipe/steps/minimap2.py
 src/labxpipe/steps/readknead.py
 src/labxpipe/steps/samtools_sort.py
 src/labxpipe/steps/samtools_uniquify.py
```

### Comparing `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe.py` & `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_demultiplex.py` & `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_demultiplex.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_extract.py` & `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_extract.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_generate.py` & `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_generate.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_merge_count.py` & `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_merge_count.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_profile.py` & `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_profile.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_report.py` & `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_report.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_run.py` & `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_run.py`

 * *Files identical despite different names*

### Comparing `labxpipe-0.6.0/src/labxpipe_scripts/lxpipe_trackhub.py` & `labxpipe-0.7.0/src/labxpipe_scripts/lxpipe_trackhub.py`

 * *Files identical despite different names*

