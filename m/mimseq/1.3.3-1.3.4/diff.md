# Comparing `tmp/mimseq-1.3.3.tar.gz` & `tmp/mimseq-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mimseq-1.3.3.tar", last modified: Tue Apr 18 09:35:23 2023, max compression
+gzip compressed data, was "mimseq-1.3.4.tar", last modified: Wed May 17 14:21:11 2023, max compression
```

## Comparing `mimseq-1.3.3.tar` & `mimseq-1.3.4.tar`

### file list

```diff
@@ -1,201 +1,204 @@
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/
--rw-r--r--   0 drew      (1000) users      (100)    35147 2020-01-30 14:46:45.000000 mimseq-1.3.3/LICENSE.txt
--rw-r--r--   0 drew      (1000) users      (100)      264 2021-09-24 14:42:07.000000 mimseq-1.3.3/MANIFEST.in
--rw-r--r--   0 drew      (1000) users      (100)      740 2023-04-18 09:35:23.000000 mimseq-1.3.3/PKG-INFO
--rw-r--r--   0 drew      (1000) users      (100)     5091 2023-02-08 15:18:34.000000 mimseq-1.3.3/README.md
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/
--rw-r--r--   0 drew      (1000) users      (100)        0 2020-03-19 10:56:10.000000 mimseq-1.3.3/mimseq/__init__.py
--rw-r--r--   0 drew      (1000) users      (100)     8451 2023-03-09 11:17:02.000000 mimseq-1.3.3/mimseq/ccaPlots.R
--rw-r--r--   0 drew      (1000) users      (100)     7683 2022-05-27 09:54:54.000000 mimseq-1.3.3/mimseq/coveragePlot.R
--rw-r--r--   0 drew      (1000) users      (100)     3793 2023-02-08 10:12:49.000000 mimseq-1.3.3/mimseq/crosstalks.py
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/
--rw-r--r--   0 drew      (1000) users      (100)     1397 2021-11-02 13:17:22.000000 mimseq-1.3.3/mimseq/data/additionalMods.txt
--rw-r--r--   0 drew      (1000) users      (100)     2762 2020-06-01 14:20:50.000000 mimseq-1.3.3/mimseq/data/additionalMods_all.txt
--rw-r--r--   0 drew      (1000) users      (100)     1452 2020-06-02 15:55:40.000000 mimseq-1.3.3/mimseq/data/additionalMods_original.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1593 2023-03-14 10:33:16.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)     1191 2023-03-14 10:34:44.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)    18749 2022-05-27 08:41:38.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-mito-searchResults.txt
--rw-r--r--   0 drew      (1000) users      (100)    17539 2022-03-07 09:38:20.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-plastid-searchResults.txt
--rw-r--r--   0 drew      (1000) users      (100)    13643 2019-02-21 17:02:30.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-filtered-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   124283 2019-02-21 17:02:30.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-mature-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)     4384 2022-05-27 09:19:19.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)     4120 2022-05-27 09:19:19.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-plastidtRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   126268 2023-03-14 10:34:39.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    52698 2018-04-18 00:58:34.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.out
--rw-r--r--   0 drew      (1000) users      (100)   230054 2018-04-18 00:58:34.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.ss
--rw-r--r--   0 drew      (1000) users      (100)    64333 2022-02-25 14:22:30.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   253880 2018-04-18 00:58:33.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.ss
--rw-r--r--   0 drew      (1000) users      (100)    48286 2023-03-14 10:25:34.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)   116013 2022-03-08 15:21:29.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    18895 2019-02-21 16:51:34.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs_name_map.txt
--rwxr-xr-x   0 drew      (1000) users      (100)      596 2022-05-27 09:19:14.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/convertPtRNAdbSearch.py
--rw-r--r--   0 drew      (1000) users      (100)     3325 2023-03-14 09:57:56.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/hg38README.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/ce11-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2387 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    64329 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)    53802 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)   116662 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    21452 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs_name_map.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)      361 2020-10-13 15:34:52.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2460 2020-07-14 08:21:01.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   820216 2020-07-14 08:18:14.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)  1748099 2020-07-14 08:15:10.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11_eColitK.fa
--rw-r--r--   0 drew      (1000) users      (100)  1699762 2020-10-13 15:33:53.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa
--rw-r--r--   0 drew      (1000) users      (100)  2070516 2020-07-14 08:17:34.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11_eschColi-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)     3196 2020-10-07 14:47:35.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/filterList.txt
--rwxr-xr-x   0 drew      (1000) users      (100)      603 2020-10-13 15:34:55.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/filtertRNAs.py
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/dm6-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)     2630 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    22311 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    56907 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6_eColitK-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    31271 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6_eschColi-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/dm6-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2630 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    22311 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    57209 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    24907 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     6233 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    19253 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)     6364 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)    35045 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.ss.sort
--rw-r--r--   0 drew      (1000) users      (100)     2515 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs_name_map.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/eschColi-tRNA_Lys/
--rw-r--r--   0 drew      (1000) users      (100)     6364 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-tRNA_Lys/eschColi_K_12_MG1655-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)     6884 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-tRNA_Lys/eschColi_modomics.fa
--rw-r--r--   0 drew      (1000) users      (100)      211 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-tRNA_Lys/eschColi_tRNA_Lys.fa
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1588 2021-07-05 08:53:55.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)     3012 2021-07-09 13:07:40.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2502 2021-07-07 13:15:36.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   108501 2021-07-05 09:02:35.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    67892 2021-07-05 08:48:49.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.tmp.fa
--rw-r--r--   0 drew      (1000) users      (100)    63236 2021-07-05 09:01:36.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   107333 2021-07-09 13:08:29.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered.fa
--rw-r--r--   0 drew      (1000) users      (100)   107126 2021-07-09 13:07:44.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered2.fa
--rw-r--r--   0 drew      (1000) users      (100)    44065 2021-07-05 08:34:36.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    80347 2021-07-05 08:35:51.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    16883 2021-07-05 08:35:37.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_name_map.txt
--rw-r--r--   0 drew      (1000) users      (100)    42271 2021-07-05 08:48:46.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_noChr.bed
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-04-27 14:50:02.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)      540 2022-04-27 14:52:24.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2436 2021-07-08 09:56:41.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   113031 2022-04-27 14:53:02.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    59255 2018-03-06 03:17:41.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)    46331 2019-07-29 22:32:21.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    17526 2019-07-29 22:32:21.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs_name_map.txt
--rw-r--r--   0 drew      (1000) users      (100)    65619 2022-04-27 14:53:56.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19_eschColi-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2435 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    46331 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    80399 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    48831 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19_eschColi-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1585 2020-10-19 12:52:59.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)     3325 2022-07-20 11:41:08.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2436 2022-04-26 11:17:07.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   117384 2021-01-22 10:06:35.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    67912 2020-10-05 13:31:33.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   115259 2022-09-07 13:10:51.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs-filtered.fa
--rw-r--r--   0 drew      (1000) users      (100)    48137 2020-10-06 09:27:32.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    82347 2020-10-05 11:41:27.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    18218 2020-10-05 12:36:55.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs_name_map.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/
--rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)      931 2022-03-30 09:32:29.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2436 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   117384 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    67912 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   115376 2022-03-30 09:26:15.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-filtered.fa
--rw-r--r--   0 drew      (1000) users      (100)    48137 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    82347 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    18218 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs_name_map.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/mm10-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)     2452 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/mm10-eColitK/mm10-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    84788 2020-01-31 16:59:36.000000 mimseq-1.3.3/mimseq/data/mm10-eColitK/mm10_eColitK-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    47202 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/mm10-eColitK/mm10_eschColi-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/mm10-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2452 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/mm10-tRNAs/mm10-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    84575 2020-01-31 17:01:17.000000 mimseq-1.3.3/mimseq/data/mm10-tRNAs/mm10-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    40838 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/mm10-tRNAs/mm10-tRNAs.out.filtered-noPseudo-noChrM
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-04-27 08:57:47.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)      758 2022-04-26 15:03:49.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2452 2022-04-27 08:22:42.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   218566 2022-04-27 08:59:25.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)  4027115 2022-04-26 15:02:32.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   218353 2022-10-27 11:20:21.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs-noeColi.fa
--rw-r--r--   0 drew      (1000) users      (100)    89234 2021-05-11 08:57:13.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)  1352197 2021-05-16 08:53:54.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs_name_map.txt
--rwxr-xr-x   0 drew      (1000) users      (100)   112128 2020-09-10 10:00:52.000000 mimseq-1.3.3/mimseq/data/modomics
--rwxr-xr-x   0 drew      (1000) users      (100)   112128 2020-06-10 14:49:20.000000 mimseq-1.3.3/mimseq/data/modomics_orig
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)      585 2021-11-03 07:29:18.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2560 2021-11-02 09:01:00.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    43272 2021-05-10 08:04:02.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-tRNAs-confidence-set.out
--rw-r--r--   0 drew      (1000) users      (100)    92538 2021-05-20 20:42:36.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    83026 2021-11-03 07:29:35.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    49636 2021-11-02 08:58:59.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7_eColitK-tRNAs-confidence-set.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/sacCer3-Phe_SynVsPur/
--rw-r--r--   0 drew      (1000) users      (100)      429 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-Phe.fa
--rw-r--r--   0 drew      (1000) users      (100)    56689 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    20382 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.out-noChrM
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/sacCer3-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)      816 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-eColitK/Turk_2013_mitotRNAbounds_Tab1.bed
--rw-r--r--   0 drew      (1000) users      (100)     2821 2020-07-07 08:03:00.000000 mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    19475 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    26478 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3_eschColi-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)    56686 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3_eschColitK.fa
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2821 2020-07-07 08:03:30.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    19475 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    56473 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    20382 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.out-noChrM
--rw-r--r--   0 drew      (1000) users      (100)   111081 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.ss.sort
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/
--rw-r--r--   0 drew      (1000) users      (100)     1107 2021-09-23 14:11:39.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/README.txt
--rw-r--r--   0 drew      (1000) users      (100)      816 2021-09-24 12:57:51.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/Turk_2013_mitotRNAbounds_Tab1.bed
--rw-r--r--   0 drew      (1000) users      (100)     2821 2021-09-24 12:57:51.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    19475 2021-09-24 12:57:51.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    26478 2021-09-24 12:57:51.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColi-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)    57096 2021-09-24 12:59:06.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColitK.fa
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/sacCer3_modOligos/
--rw-r--r--   0 drew      (1000) users      (100)    26595 2020-03-26 14:57:08.000000 mimseq-1.3.3/mimseq/data/sacCer3_modOligos/sacCer3_eschColi-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)    56987 2020-03-26 14:51:11.000000 mimseq-1.3.3/mimseq/data/sacCer3_modOligos/sacCer3_eschColitK.fa
--rw-r--r--   0 drew      (1000) users      (100)      320 2020-03-27 13:55:28.000000 mimseq-1.3.3/mimseq/data/sacCer3_modOligos/sacCer3_oligoRefsOnly.fa
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/schiPomb-972H/
--rw-r--r--   0 drew      (1000) users      (100)     3385 2020-03-11 16:27:56.000000 mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    12387 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    33731 2020-03-11 16:25:12.000000 mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    14240 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.out.noChrM
--rw-r--r--   0 drew      (1000) users      (100)    67540 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.ss.sort
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/schiPomb-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)     3385 2020-03-11 16:28:18.000000 mimseq-1.3.3/mimseq/data/schiPomb-eColitK/schiPomb-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    33944 2020-03-11 16:24:55.000000 mimseq-1.3.3/mimseq/data/schiPomb-eColitK/schiPomb_972H-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    20604 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/schiPomb-eColitK/schiPomb_eschColi-tRNAs.out
--rwxr-xr-x   0 drew      (1000) users      (100)    67935 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/tRNAmatureseq.cm
--rw-r--r--   0 drew      (1000) users      (100)    32195 2022-09-23 11:55:49.000000 mimseq-1.3.3/mimseq/deseq.R
--rwxr-xr-x   0 drew      (1000) users      (100)     7883 2022-06-22 09:54:11.000000 mimseq-1.3.3/mimseq/getCoverage.py
--rwxr-xr-x   0 drew      (1000) users      (100)    28210 2023-03-14 10:38:15.000000 mimseq-1.3.3/mimseq/mimseq.py
--rw-r--r--   0 drew      (1000) users      (100)    52638 2023-04-18 08:46:34.000000 mimseq-1.3.3/mimseq/mmQuant.py
--rw-r--r--   0 drew      (1000) users      (100)    38088 2023-01-17 10:59:49.000000 mimseq-1.3.3/mimseq/modPlot.R
--rw-r--r--   0 drew      (1000) users      (100)     6580 2020-03-17 16:13:32.000000 mimseq-1.3.3/mimseq/modifications
--rw-r--r--   0 drew      (1000) users      (100)    31520 2023-04-18 08:45:46.000000 mimseq-1.3.3/mimseq/splitClusters.py
--rwxr-xr-x   0 drew      (1000) users      (100)    11682 2023-04-18 08:47:35.000000 mimseq-1.3.3/mimseq/ssAlign.py
--rwxr-xr-x   0 drew      (1000) users      (100)     7272 2022-03-08 14:29:47.000000 mimseq-1.3.3/mimseq/tRNAmap.py
--rwxr-xr-x   0 drew      (1000) users      (100)    48869 2023-03-10 13:59:11.000000 mimseq-1.3.3/mimseq/tRNAtools.py
--rw-r--r--   0 drew      (1000) users      (100)       23 2023-04-18 09:33:02.000000 mimseq-1.3.3/mimseq/version.py
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq.egg-info/
--rw-r--r--   0 drew      (1000) users      (100)      740 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/PKG-INFO
--rw-r--r--   0 drew      (1000) users      (100)     7719 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/SOURCES.txt
--rw-r--r--   0 drew      (1000) users      (100)        1 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/dependency_links.txt
--rw-r--r--   0 drew      (1000) users      (100)       47 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/entry_points.txt
--rw-r--r--   0 drew      (1000) users      (100)        1 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/not-zip-safe
--rw-r--r--   0 drew      (1000) users      (100)       80 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/requires.txt
--rw-r--r--   0 drew      (1000) users      (100)        7 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/top_level.txt
--rw-r--r--   0 drew      (1000) users      (100)      124 2023-01-17 11:01:06.000000 mimseq-1.3.3/sampleData_HEKvsK562.txt
--rw-r--r--   0 drew      (1000) users      (100)       38 2023-04-18 09:35:23.000000 mimseq-1.3.3/setup.cfg
--rwxr-xr-x   0 drew      (1000) users      (100)     1913 2023-02-08 10:12:49.000000 mimseq-1.3.3/setup.py
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.357772 mimseq-1.3.4/
+-rw-r--r--   0 drew      (1000) users      (100)    35147 2020-01-30 14:46:45.000000 mimseq-1.3.4/LICENSE.txt
+-rw-r--r--   0 drew      (1000) users      (100)      264 2021-09-24 14:42:07.000000 mimseq-1.3.4/MANIFEST.in
+-rw-r--r--   0 drew      (1000) users      (100)      712 2023-05-17 14:21:11.357772 mimseq-1.3.4/PKG-INFO
+-rw-r--r--   0 drew      (1000) users      (100)     5091 2023-02-08 15:18:34.000000 mimseq-1.3.4/README.md
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.189758 mimseq-1.3.4/mimseq/
+-rw-r--r--   0 drew      (1000) users      (100)        0 2020-03-19 10:56:10.000000 mimseq-1.3.4/mimseq/__init__.py
+-rw-r--r--   0 drew      (1000) users      (100)     8451 2023-03-09 11:17:02.000000 mimseq-1.3.4/mimseq/ccaPlots.R
+-rw-r--r--   0 drew      (1000) users      (100)     7683 2022-05-27 09:54:54.000000 mimseq-1.3.4/mimseq/coveragePlot.R
+-rw-r--r--   0 drew      (1000) users      (100)     3793 2023-02-08 10:12:49.000000 mimseq-1.3.4/mimseq/crosstalks.py
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.193759 mimseq-1.3.4/mimseq/data/
+-rw-r--r--   0 drew      (1000) users      (100)     1677 2023-05-12 08:26:45.000000 mimseq-1.3.4/mimseq/data/additionalMods.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2762 2020-06-01 14:20:50.000000 mimseq-1.3.4/mimseq/data/additionalMods_all.txt
+-rw-r--r--   0 drew      (1000) users      (100)     1452 2020-06-02 15:55:40.000000 mimseq-1.3.4/mimseq/data/additionalMods_original.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.209760 mimseq-1.3.4/mimseq/data/araTha1-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1593 2023-03-14 10:33:16.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)     1191 2023-03-14 10:34:44.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)    18749 2022-05-27 08:41:38.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-mito-searchResults.txt
+-rw-r--r--   0 drew      (1000) users      (100)    17539 2022-03-07 09:38:20.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-plastid-searchResults.txt
+-rw-r--r--   0 drew      (1000) users      (100)    13643 2019-02-21 17:02:30.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-filtered-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   124283 2019-02-21 17:02:30.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-mature-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)     4384 2022-05-27 09:19:19.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)     4120 2022-05-27 09:19:19.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-plastidtRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   126268 2023-03-14 10:34:39.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    52698 2018-04-18 00:58:34.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.out
+-rw-r--r--   0 drew      (1000) users      (100)   230054 2018-04-18 00:58:34.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.ss
+-rw-r--r--   0 drew      (1000) users      (100)    64333 2022-02-25 14:22:30.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   253880 2018-04-18 00:58:33.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.ss
+-rw-r--r--   0 drew      (1000) users      (100)    48286 2023-03-14 10:25:34.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)   116013 2022-03-08 15:21:29.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    18895 2019-02-21 16:51:34.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs_name_map.txt
+-rwxr-xr-x   0 drew      (1000) users      (100)      596 2022-05-27 09:19:14.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/convertPtRNAdbSearch.py
+-rw-r--r--   0 drew      (1000) users      (100)     3325 2023-03-14 09:57:56.000000 mimseq-1.3.4/mimseq/data/araTha1-eColitK/hg38README.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.213760 mimseq-1.3.4/mimseq/data/ce11-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1595 2023-05-12 07:56:59.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)     1058 2023-05-12 07:59:05.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2387 2023-05-12 08:06:56.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   143203 2023-05-12 08:00:15.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    86974 2023-05-12 07:55:09.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs-all.tmp.fa
+-rw-r--r--   0 drew      (1000) users      (100)    70692 2023-05-12 08:00:57.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)    53802 2018-11-13 17:14:05.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    21452 2018-11-13 17:14:05.000000 mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs_name_map.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.221761 mimseq-1.3.4/mimseq/data/danRer11-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)      361 2020-10-13 15:34:52.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2460 2020-07-14 08:21:01.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   820216 2020-07-14 08:18:14.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)  1748099 2020-07-14 08:15:10.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11_eColitK.fa
+-rw-r--r--   0 drew      (1000) users      (100)  1699762 2020-10-13 15:33:53.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa
+-rw-r--r--   0 drew      (1000) users      (100)  2070516 2020-07-14 08:17:34.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11_eschColi-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)     3196 2020-10-07 14:47:35.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/filterList.txt
+-rwxr-xr-x   0 drew      (1000) users      (100)      603 2020-10-13 15:34:55.000000 mimseq-1.3.4/mimseq/data/danRer11-eColitK/filtertRNAs.py
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.221761 mimseq-1.3.4/mimseq/data/dm6-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)     2630 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    22311 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    56907 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6_eColitK-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    31271 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6_eschColi-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.221761 mimseq-1.3.4/mimseq/data/dm6-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     2630 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    22311 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    57209 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    24907 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.221761 mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     6233 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    19253 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)     6364 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)    35045 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.ss.sort
+-rw-r--r--   0 drew      (1000) users      (100)     2515 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs_name_map.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.225762 mimseq-1.3.4/mimseq/data/eschColi-tRNA_Lys/
+-rw-r--r--   0 drew      (1000) users      (100)     6364 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-tRNA_Lys/eschColi_K_12_MG1655-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)     6884 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-tRNA_Lys/eschColi_modomics.fa
+-rw-r--r--   0 drew      (1000) users      (100)      211 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/eschColi-tRNA_Lys/eschColi_tRNA_Lys.fa
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.257764 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1588 2021-07-05 08:53:55.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)     3012 2021-07-09 13:07:40.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2502 2021-07-07 13:15:36.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   108501 2021-07-05 09:02:35.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    67892 2021-07-05 08:48:49.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.tmp.fa
+-rw-r--r--   0 drew      (1000) users      (100)    63236 2021-07-05 09:01:36.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   107333 2021-07-09 13:08:29.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered.fa
+-rw-r--r--   0 drew      (1000) users      (100)   107126 2021-07-09 13:07:44.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered2.fa
+-rw-r--r--   0 drew      (1000) users      (100)    44065 2021-07-05 08:34:36.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    80347 2021-07-05 08:35:51.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    16883 2021-07-05 08:35:37.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_name_map.txt
+-rw-r--r--   0 drew      (1000) users      (100)    42271 2021-07-05 08:48:46.000000 mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_noChr.bed
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.261764 mimseq-1.3.4/mimseq/data/hg19-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-04-27 14:50:02.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)      540 2022-04-27 14:52:24.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2436 2021-07-08 09:56:41.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   113031 2022-04-27 14:53:02.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    59255 2018-03-06 03:17:41.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)    46331 2019-07-29 22:32:21.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    17526 2019-07-29 22:32:21.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs_name_map.txt
+-rw-r--r--   0 drew      (1000) users      (100)    65619 2022-04-27 14:53:56.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19_eschColi-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.261764 mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     2435 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    46331 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    80399 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    48831 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19_eschColi-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.265765 mimseq-1.3.4/mimseq/data/hg38-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1585 2020-10-19 12:52:59.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)     3325 2022-07-20 11:41:08.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2436 2022-04-26 11:17:07.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   117384 2021-01-22 10:06:35.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    67912 2020-10-05 13:31:33.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   115259 2022-09-07 13:10:51.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs-filtered.fa
+-rw-r--r--   0 drew      (1000) users      (100)    48137 2020-10-06 09:27:32.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    82347 2020-10-05 11:41:27.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    18218 2020-10-05 12:36:55.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs_name_map.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.269765 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)      931 2022-03-30 09:32:29.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2436 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   117384 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    67912 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   115376 2022-03-30 09:26:15.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-filtered.fa
+-rw-r--r--   0 drew      (1000) users      (100)    48137 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    82347 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    18218 2022-03-30 09:22:21.000000 mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs_name_map.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.273765 mimseq-1.3.4/mimseq/data/mm10-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)     2452 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/mm10-eColitK/mm10-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    84788 2020-01-31 16:59:36.000000 mimseq-1.3.4/mimseq/data/mm10-eColitK/mm10_eColitK-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    47202 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/mm10-eColitK/mm10_eschColi-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.273765 mimseq-1.3.4/mimseq/data/mm10-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     2452 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/mm10-tRNAs/mm10-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    84575 2020-01-31 17:01:17.000000 mimseq-1.3.4/mimseq/data/mm10-tRNAs/mm10-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    40838 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/mm10-tRNAs/mm10-tRNAs.out.filtered-noPseudo-noChrM
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.277766 mimseq-1.3.4/mimseq/data/mm39-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-04-27 08:57:47.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)      758 2022-04-26 15:03:49.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2452 2022-04-27 08:22:42.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   218566 2022-04-27 08:59:25.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)  4027115 2022-04-26 15:02:32.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   218353 2022-10-27 11:20:21.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs-noeColi.fa
+-rw-r--r--   0 drew      (1000) users      (100)    89234 2021-05-11 08:57:13.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)  1352197 2021-05-16 08:53:54.000000 mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs_name_map.txt
+-rwxr-xr-x   0 drew      (1000) users      (100)   112128 2020-09-10 10:00:52.000000 mimseq-1.3.4/mimseq/data/modomics
+-rwxr-xr-x   0 drew      (1000) users      (100)   112128 2020-06-10 14:49:20.000000 mimseq-1.3.4/mimseq/data/modomics_orig
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.281766 mimseq-1.3.4/mimseq/data/rn7-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)      585 2021-11-03 07:29:18.000000 mimseq-1.3.4/mimseq/data/rn7-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2560 2021-11-02 09:01:00.000000 mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    43272 2021-05-10 08:04:02.000000 mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-tRNAs-confidence-set.out
+-rw-r--r--   0 drew      (1000) users      (100)    92538 2021-05-20 20:42:36.000000 mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    83026 2021-11-03 07:29:35.000000 mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    49636 2021-11-02 08:58:59.000000 mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7_eColitK-tRNAs-confidence-set.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.281766 mimseq-1.3.4/mimseq/data/sacCer3-Phe_SynVsPur/
+-rw-r--r--   0 drew      (1000) users      (100)      429 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-Phe.fa
+-rw-r--r--   0 drew      (1000) users      (100)    56689 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    20382 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.out-noChrM
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.349772 mimseq-1.3.4/mimseq/data/sacCer3-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)      816 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-eColitK/Turk_2013_mitotRNAbounds_Tab1.bed
+-rw-r--r--   0 drew      (1000) users      (100)     2821 2020-07-07 08:03:00.000000 mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    19475 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    26478 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3_eschColi-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)    56686 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3_eschColitK.fa
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.349772 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     2821 2020-07-07 08:03:30.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    19475 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    56473 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    20382 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.out-noChrM
+-rw-r--r--   0 drew      (1000) users      (100)   111081 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.ss.sort
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.353772 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/
+-rw-r--r--   0 drew      (1000) users      (100)     1107 2021-09-23 14:11:39.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)      816 2021-09-24 12:57:51.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/Turk_2013_mitotRNAbounds_Tab1.bed
+-rw-r--r--   0 drew      (1000) users      (100)     2821 2021-09-24 12:57:51.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    19475 2021-09-24 12:57:51.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    26478 2021-09-24 12:57:51.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColi-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)    57096 2021-09-24 12:59:06.000000 mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColitK.fa
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.353772 mimseq-1.3.4/mimseq/data/sacCer3_modOligos/
+-rw-r--r--   0 drew      (1000) users      (100)    26595 2020-03-26 14:57:08.000000 mimseq-1.3.4/mimseq/data/sacCer3_modOligos/sacCer3_eschColi-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)    56987 2020-03-26 14:51:11.000000 mimseq-1.3.4/mimseq/data/sacCer3_modOligos/sacCer3_eschColitK.fa
+-rw-r--r--   0 drew      (1000) users      (100)      320 2020-03-27 13:55:28.000000 mimseq-1.3.4/mimseq/data/sacCer3_modOligos/sacCer3_oligoRefsOnly.fa
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.357772 mimseq-1.3.4/mimseq/data/schiPomb-972H/
+-rw-r--r--   0 drew      (1000) users      (100)     3385 2020-03-11 16:27:56.000000 mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    12387 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    33731 2020-03-11 16:25:12.000000 mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    14240 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.out.noChrM
+-rw-r--r--   0 drew      (1000) users      (100)    67540 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.ss.sort
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.357772 mimseq-1.3.4/mimseq/data/schiPomb-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)     3385 2020-03-11 16:28:18.000000 mimseq-1.3.4/mimseq/data/schiPomb-eColitK/schiPomb-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    33944 2020-03-11 16:24:55.000000 mimseq-1.3.4/mimseq/data/schiPomb-eColitK/schiPomb_972H-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    20604 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/schiPomb-eColitK/schiPomb_eschColi-tRNAs.out
+-rwxr-xr-x   0 drew      (1000) users      (100)    67935 2020-01-30 14:46:45.000000 mimseq-1.3.4/mimseq/data/tRNAmatureseq.cm
+-rw-r--r--   0 drew      (1000) users      (100)    32195 2022-09-23 11:55:49.000000 mimseq-1.3.4/mimseq/deseq.R
+-rwxr-xr-x   0 drew      (1000) users      (100)     7883 2022-06-22 09:54:11.000000 mimseq-1.3.4/mimseq/getCoverage.py
+-rwxr-xr-x   0 drew      (1000) users      (100)    28571 2023-05-12 08:16:46.000000 mimseq-1.3.4/mimseq/mimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)    52638 2023-04-18 08:46:34.000000 mimseq-1.3.4/mimseq/mmQuant.py
+-rw-r--r--   0 drew      (1000) users      (100)    38088 2023-05-17 14:15:31.000000 mimseq-1.3.4/mimseq/modPlot.R
+-rw-r--r--   0 drew      (1000) users      (100)     6580 2020-03-17 16:13:32.000000 mimseq-1.3.4/mimseq/modifications
+-rw-r--r--   0 drew      (1000) users      (100)    31520 2023-04-18 08:45:46.000000 mimseq-1.3.4/mimseq/splitClusters.py
+-rwxr-xr-x   0 drew      (1000) users      (100)    11682 2023-04-18 08:47:35.000000 mimseq-1.3.4/mimseq/ssAlign.py
+-rwxr-xr-x   0 drew      (1000) users      (100)     7272 2022-03-08 14:29:47.000000 mimseq-1.3.4/mimseq/tRNAmap.py
+-rwxr-xr-x   0 drew      (1000) users      (100)    48869 2023-03-10 13:59:11.000000 mimseq-1.3.4/mimseq/tRNAtools.py
+-rw-r--r--   0 drew      (1000) users      (100)       23 2023-05-17 14:17:44.000000 mimseq-1.3.4/mimseq/version.py
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-05-17 14:21:11.193759 mimseq-1.3.4/mimseq.egg-info/
+-rw-r--r--   0 drew      (1000) users      (100)      712 2023-05-17 14:21:10.000000 mimseq-1.3.4/mimseq.egg-info/PKG-INFO
+-rw-r--r--   0 drew      (1000) users      (100)     7866 2023-05-17 14:21:10.000000 mimseq-1.3.4/mimseq.egg-info/SOURCES.txt
+-rw-r--r--   0 drew      (1000) users      (100)        1 2023-05-17 14:21:10.000000 mimseq-1.3.4/mimseq.egg-info/dependency_links.txt
+-rw-r--r--   0 drew      (1000) users      (100)       46 2023-05-17 14:21:10.000000 mimseq-1.3.4/mimseq.egg-info/entry_points.txt
+-rw-r--r--   0 drew      (1000) users      (100)        1 2023-05-17 14:17:29.000000 mimseq-1.3.4/mimseq.egg-info/not-zip-safe
+-rw-r--r--   0 drew      (1000) users      (100)       80 2023-05-17 14:21:10.000000 mimseq-1.3.4/mimseq.egg-info/requires.txt
+-rw-r--r--   0 drew      (1000) users      (100)        7 2023-05-17 14:21:10.000000 mimseq-1.3.4/mimseq.egg-info/top_level.txt
+-rw-r--r--   0 drew      (1000) users      (100)      124 2023-01-17 11:01:06.000000 mimseq-1.3.4/sampleData_HEKvsK562.txt
+-rw-r--r--   0 drew      (1000) users      (100)       38 2023-05-17 14:21:11.357772 mimseq-1.3.4/setup.cfg
+-rwxr-xr-x   0 drew      (1000) users      (100)     1913 2023-02-08 10:12:49.000000 mimseq-1.3.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mimseq-1.3.3/LICENSE.txt` & `mimseq-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/PKG-INFO` & `mimseq-1.3.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: mimseq
-Version: 1.3.3
+Version: 1.3.4
 Summary: Custom high-throughput tRNA sequencing alignment and quantification pipeline based on modification induced misincorporation cDNA synthesis.
 Home-page: https://github.com/nedialkova-lab/mim-tRNAseq
 Author: Drew Behrens
 Author-email: abehrens@biochem.mpg.de
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `mimseq-1.3.3/README.md` & `mimseq-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/ccaPlots.R` & `mimseq-1.3.4/mimseq/ccaPlots.R`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/coveragePlot.R` & `mimseq-1.3.4/mimseq/coveragePlot.R`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/crosstalks.py` & `mimseq-1.3.4/mimseq/crosstalks.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/additionalMods.txt` & `mimseq-1.3.4/mimseq/data/additionalMods.txt`

 * *Files 26% similar despite different names*

```diff
@@ -41,8 +41,16 @@
 Rattus norvegicus	Ala-AGC	I34
 Rattus norvegicus	Arg-ACG	I34
 Rattus norvegicus	Ile-AAT	I34
 Rattus norvegicus	Leu-AAG	I34
 Rattus norvegicus	Pro-AGG	I34
 Rattus norvegicus	Ser-AGA	I34
 Rattus norvegicus	Thr-AGT	I34
-Rattus norvegicus	Val-AAC	I34
+Rattus norvegicus	Val-AAC	I34
+Caenorhabditis elegans	Ala-AGC	I34
+Caenorhabditis elegans	Arg-ACG	I34
+Caenorhabditis elegans	Ile-AAT	I34
+Caenorhabditis elegans	Leu-AAG	I34
+Caenorhabditis elegans	Pro-AGG	I34
+Caenorhabditis elegans	Ser-AGA	I34
+Caenorhabditis elegans	Thr-AGT	I34
+Caenorhabditis elegans	Val-AAC	I34
```

### Comparing `mimseq-1.3.3/mimseq/data/additionalMods_all.txt` & `mimseq-1.3.4/mimseq/data/additionalMods_all.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/additionalMods_original.txt` & `mimseq-1.3.4/mimseq/data/additionalMods_original.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/README.txt` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-mito-searchResults.txt` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-mito-searchResults.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-plastid-searchResults.txt` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-plastid-searchResults.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-filtered-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-filtered-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-mature-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-mature-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-plastidtRNAs.fa` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-plastidtRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-all.fa` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.out` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.ss` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.ss`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.out` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.ss` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.ss`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs_name_map.txt` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/araTha1-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/convertPtRNAdbSearch.py` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/convertPtRNAdbSearch.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/araTha1-eColitK/hg38README.txt` & `mimseq-1.3.4/mimseq/data/araTha1-eColitK/hg38README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs-detailed.out` & `mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs-detailed.out`

 * *Files 5% similar despite different names*

```diff
@@ -718,7 +718,99 @@
 chrX	301	1433143	1433063	Undet	NNN	0	0	32.3	37.60	-5.30	Inf	Ala	24.3	pseudo
 chrX	302	1379674	1379603	Gly	TCC	0	0	71.7	41.10	30.60	Inf	Gly	92.5	high confidence set
 chrX	303	1089245	1089173	Arg	TCG	0	0	69.4	53.20	16.20	Inf	Arg	98.0	high confidence set
 chrX	304	865472	865389	Tyr	GTA	865435	865425	74.6	44.10	30.50	Inf	Tyr	117.7	high confidence set
 chrX	305	489939	489868	Asp	GTC	0	0	61.7	32.90	28.80	Inf	Asp	101.6	high confidence set
 chrX	306	353336	353255	Leu	AAG	0	0	72.6	44.40	28.20	Inf	Leu	113.7	high confidence set
 chrX	307	289587	289513	Lys	CTT	0	0	20.2	41.30	-21.10	Inf	Arg	15.0	pseudo,IPD:-25.30
+Sequence		tRNA   	Bounds 	tRNA	Anti	Intron Bounds	Inf	HMM	2'Str	Isotype	Isotype	      
+Name    	tRNA #	Begin  	End    	Type	Codon	Begin	End	Score	Score	Score	CM	Score	Note
+--------	------	-----  	------ 	----	-----	-----	----	------	-----	-----	-------	-------	------
+chr     	1	225381 	225457 	Ile	GAT	0	0	75.8	47.60	28.20	Ile	110.9	
+chr     	2	225500 	225575 	Ala	TGC	0	0	78.1	53.10	25.00	Ala	115.6	
+chr     	3	228928 	229004 	Asp	GTC	0	0	85.5	71.10	14.40	Asp	128.1	
+chr     	4	236931 	237007 	Asp	GTC	0	0	85.5	71.10	14.40	Asp	128.1	
+chr     	5	262871 	262946 	Thr	CGT	0	0	85.1	63.80	21.30	Thr	105.6	
+chr     	6	297184 	297254 	Thr	CGT	0	0	44.2	27.80	16.40	Thr	49.5	trunc_start:6
+chr     	7	564723 	564799 	Arg	TCT	0	0	86.6	61.20	25.40	Arg	103.5	
+chr     	8	586007 	586101 	Undet	NNN	0	0	31.7	35.00	-3.30	Arg	36.2	pseudo,trunc_start:8
+chr     	9	780554 	780629 	Lys	TTT	0	0	94.9	70.50	24.40	Lys	113.3	
+chr     	10	780765 	780840 	Val	TAC	0	0	84.6	59.00	25.60	Val	110.9	
+chr     	11	780843 	780918 	Lys	TTT	0	0	94.9	70.50	24.40	Lys	113.3	
+chr     	12	781068 	781143 	Val	TAC	0	0	84.6	59.00	25.60	Val	110.9	
+chr     	13	781147 	781222 	Lys	TTT	0	0	94.9	70.50	24.40	Lys	113.3	
+chr     	14	781369 	781444 	Lys	TTT	0	0	94.9	70.50	24.40	Lys	113.3	
+chr     	15	781577 	781652 	Lys	TTT	0	0	94.9	70.50	24.40	Lys	113.3	
+chr     	16	1746435	1746511	Val	GAC	0	0	82.5	53.40	29.10	Val	101.9	
+chr     	17	1746516	1746592	Val	GAC	0	0	85.9	59.60	26.30	Val	104.4	
+chr     	18	2044549	2044624	Asn	GTT	0	0	79.7	48.60	31.10	Asn	115.2	
+chr     	19	2059851	2059926	Asn	GTT	0	0	79.7	48.60	31.10	Asn	115.2	
+chr     	20	2062260	2062335	Asn	GTT	0	0	79.7	48.60	31.10	Asn	115.2	
+chr     	21	2286211	2286287	Pro	GGG	0	0	67.3	40.60	26.70	Pro	110.3	
+chr     	22	2466309	2466383	Arg	CCT	0	0	62.5	30.50	32.00	Arg	77.7	
+chr     	23	2520931	2521006	Val	TAC	0	0	84.6	59.00	25.60	Val	110.9	
+chr     	24	2521051	2521126	Val	TAC	0	0	84.6	59.00	25.60	Val	110.9	
+chr     	25	2521173	2521248	Val	TAC	0	0	84.6	59.00	25.60	Val	110.9	
+chr     	26	2521253	2521328	Lys	TTT	0	0	94.9	70.50	24.40	Lys	113.3	
+chr     	27	2755859	2755955	Undet	NNN	0	0	29.6	22.30	7.30	Ile2	28.4	trunc_start:6
+chr     	28	2947387	2947463	fMet	CAT	0	0	77.5	50.60	26.90	fMet	129.5	
+chr     	29	2947497	2947573	fMet	CAT	0	0	77.5	50.60	26.90	fMet	129.5	
+chr     	30	2947607	2947683	fMet	CAT	0	0	77.5	50.60	26.90	fMet	129.5	
+chr     	31	3110366	3110441	Phe	GAA	0	0	75.3	45.80	29.50	Phe	104.8	
+chr     	32	3215598	3215673	Ile2	CAT	0	0	85.1	56.20	28.90	Ile2	111.7	
+chr     	33	3836222	3836316	SeC	TCA	0	0	142.5	0.00	0.00	SeC	142.5	
+chr     	34	3943435	3943510	Glu	TTC	0	0	66.6	35.80	30.80	Glu	105.4	
+chr     	35	3946872	3946948	Asp	GTC	0	0	85.5	71.10	14.40	Asp	128.1	
+chr     	36	3946957	3947032	Trp	CCA	0	0	79.9	61.00	18.90	Trp	98.7	
+chr     	37	3982375	3982451	Arg	CCG	0	0	82.2	62.70	19.50	Arg	104.0	
+chr     	38	3982510	3982585	His	GTG	0	0	78.7	53.40	25.30	His	106.7	
+chr     	39	3982606	3982692	Leu	CAG	0	0	67.1	42.20	24.90	Leu	109.1	
+chr     	40	3982735	3982811	Pro	TGG	0	0	82.4	54.50	27.90	Pro	115.0	
+chr     	41	4037141	4037217	Ile	GAT	0	0	75.8	47.60	28.20	Ile	110.9	
+chr     	42	4037260	4037335	Ala	TGC	0	0	78.1	53.10	25.00	Ala	115.6	
+chr     	43	4168372	4168447	Glu	TTC	0	0	66.6	35.80	30.80	Glu	105.4	
+chr     	44	4175388	4175463	Thr	TGT	0	0	81.3	59.30	22.00	Thr	106.1	
+chr     	45	4175472	4175556	Tyr	GTA	0	0	73.0	42.20	30.80	Tyr	118.5	
+chr     	46	4175673	4175747	Gly	TCC	0	0	70.6	42.90	27.70	Gly	86.6	
+chr     	47	4175754	4175829	Thr	GGT	0	0	84.7	50.10	34.60	Thr	103.0	
+chr     	48	4209774	4209849	Glu	TTC	0	0	66.6	35.80	30.80	Glu	105.4	
+chr     	49	4392360	4392435	Gly	GCC	0	0	88.4	61.80	26.60	Gly	113.7	
+chr     	50	4392472	4392547	Gly	GCC	0	0	88.4	61.80	26.60	Gly	113.7	
+chr     	51	4392583	4392658	Gly	GCC	0	0	88.4	61.80	26.60	Gly	113.7	
+chr     	52	4496405	4496489	Leu	CAA	0	0	79.3	46.00	33.30	Leu	110.3	
+chr     	53	4606401	4606315	Leu	CAG	0	0	67.1	42.20	24.90	Leu	109.1	
+chr     	54	4606286	4606200	Leu	CAG	0	0	65.0	42.50	22.50	Leu	106.8	
+chr     	55	4606165	4606079	Leu	CAG	0	0	67.1	42.20	24.90	Leu	109.1	
+chr     	56	4362626	4362551	Phe	GAA	0	0	75.3	45.80	29.50	Phe	104.8	
+chr     	57	3708692	3708616	Pro	CGG	0	0	76.0	43.90	32.10	Pro	109.5	
+chr     	58	3427152	3427076	Ile	GAT	0	0	75.8	47.60	28.20	Ile	110.9	
+chr     	59	3427033	3426958	Ala	TGC	0	0	78.1	53.10	25.00	Ala	115.6	
+chr     	60	3423655	3423580	Thr	GGT	0	0	79.8	42.80	37.00	Thr	99.7	
+chr     	61	3322158	3322072	Leu	GAG	0	0	64.5	38.70	25.80	Leu	103.6	
+chr     	62	3318289	3318213	fMet	CAT	0	0	75.5	48.60	26.90	fMet	125.8	
+chr     	63	2999057	2998984	Gly	CCC	0	0	81.1	54.70	26.40	Gly	100.5	
+chr     	64	2818645	2818553	Ser	GCT	0	0	83.4	46.30	37.10	Ser	109.5	
+chr     	65	2818549	2818473	Arg	ACG	0	0	85.1	59.80	25.30	Arg	100.6	
+chr     	66	2818274	2818198	Arg	ACG	0	0	85.1	59.80	25.30	Arg	100.6	
+chr     	67	2818135	2818059	Arg	ACG	0	0	85.1	59.80	25.30	Arg	100.6	
+chr     	68	2817860	2817784	Arg	ACG	0	0	85.1	59.80	25.30	Arg	100.6	
+chr     	69	2785837	2785762	Ile2	CAT	0	0	84.7	55.50	29.20	Ile2	112.8	
+chr     	70	2729444	2729369	Glu	TTC	0	0	66.6	35.80	30.80	Glu	105.4	
+chr     	71	2518231	2518156	Ala	GGC	0	0	75.0	52.50	22.50	Ala	114.0	
+chr     	72	2518116	2518041	Ala	GGC	0	0	75.0	52.50	22.50	Ala	114.0	
+chr     	73	2058102	2058027	Asn	GTT	0	0	79.7	48.60	31.10	Asn	115.2	
+chr     	74	2043557	2043468	Ser	CGA	0	0	90.4	54.50	35.90	Ser	122.4	
+chr     	75	1992117	1992042	Gly	GCC	0	0	88.4	61.80	26.60	Gly	113.7	
+chr     	76	1991987	1991914	Cys	GCA	0	0	63.0	27.10	35.90	Cys	86.2	
+chr     	77	1991901	1991815	Leu	TAA	0	0	71.7	41.40	30.30	Leu	101.8	
+chr     	78	1287622	1287538	Tyr	GTA	0	0	72.2	43.00	29.20	Tyr	119.1	
+chr     	79	1287328	1287244	Tyr	GTA	0	0	72.2	43.00	29.20	Tyr	119.1	
+chr     	80	1097652	1097565	Ser	GGA	0	0	76.9	38.30	38.60	Ser	117.0	
+chr     	81	1031712	1031625	Ser	TGA	0	0	83.5	47.20	36.30	Ser	103.3	
+chr     	82	925971 	925884 	Ser	GGA	0	0	76.9	38.30	38.60	Ser	117.0	
+chr     	83	697133 	697057 	Met	CAT	0	0	84.4	63.20	21.20	Met	111.6	
+chr     	84	697047 	696963 	Leu	TAG	0	0	74.1	46.80	27.30	Leu	115.3	
+chr     	85	696939 	696865 	Gln	TTG	0	0	70.4	38.40	32.00	Gln	101.4	
+chr     	86	696830 	696756 	Gln	TTG	0	0	70.4	38.40	32.00	Gln	101.4	
+chr     	87	696740 	696664 	Met	CAT	0	0	84.4	63.20	21.20	Met	111.6	
+chr     	88	696616 	696542 	Gln	CTG	0	0	70.8	39.90	30.90	Gln	100.0	
+chr     	89	696504 	696430 	Gln	CTG	0	0	70.8	39.90	30.90	Gln	100.0
```

### Comparing `mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs-all.fa`

 * *Files 16% similar despite different names*

```diff
@@ -1,1749 +1,1444 @@
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-1 (tRNAscan-SE ID: chrII.trna6) Ala (AGC) 72 bp Sc: 74.8 chrII:4565389-4565460 (+)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-10 (tRNAscan-SE ID: chrX.trna272) Ala (AGC) 72 bp Sc: 74.8 chrX:7378784-7378855 (-)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-11 (tRNAscan-SE ID: chrX.trna271) Ala (AGC) 72 bp Sc: 74.8 chrX:7507290-7507361 (-)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-12 (tRNAscan-SE ID: chrX.trna79) Ala (AGC) 72 bp Sc: 74.8 chrX:9237811-9237882 (+)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-13 (tRNAscan-SE ID: chrX.trna80) Ala (AGC) 72 bp Sc: 74.8 chrX:9238864-9238935 (+)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-14 (tRNAscan-SE ID: chrX.trna229) Ala (AGC) 72 bp Sc: 74.8 chrX:9622824-9622895 (-)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-15 (tRNAscan-SE ID: chrX.trna228) Ala (AGC) 72 bp Sc: 74.8 chrX:9637852-9637923 (-)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-16 (tRNAscan-SE ID: chrX.trna82) Ala (AGC) 72 bp Sc: 74.8 chrX:9743747-9743818 (+)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-17 (tRNAscan-SE ID: chrX.trna208) Ala (AGC) 72 bp Sc: 74.8 chrX:12458176-12458247 (-)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-2 (tRNAscan-SE ID: chrII.trna9) Ala (AGC) 72 bp Sc: 74.8 chrII:5292332-5292403 (+)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-3 (tRNAscan-SE ID: chrII.trna47) Ala (AGC) 72 bp Sc: 74.8 chrII:7002993-7003064 (-)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-4 (tRNAscan-SE ID: chrII.trna28) Ala (AGC) 72 bp Sc: 74.8 chrII:12542634-12542705 (+)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-5 (tRNAscan-SE ID: chrIV.trna49) Ala (AGC) 72 bp Sc: 74.8 chrIV:16389211-16389282 (-)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-6 (tRNAscan-SE ID: chrIV.trna38) Ala (AGC) 72 bp Sc: 74.8 chrIV:16398384-16398455 (+)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-7 (tRNAscan-SE ID: chrIV.trna39) Ala (AGC) 72 bp Sc: 74.8 chrIV:16399184-16399255 (+)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-8 (tRNAscan-SE ID: chrV.trna89) Ala (AGC) 72 bp Sc: 74.8 chrV:13003509-13003580 (-)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-1-9 (tRNAscan-SE ID: chrX.trna46) Ala (AGC) 72 bp Sc: 74.8 chrX:7323753-7323824 (+)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-2-1 (tRNAscan-SE ID: chrIV.trna22) Ala (AGC) 72 bp Sc: 67.2 chrIV:6562202-6562273 (+)
-GGGGGTATAGCTCAGTAGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-3-1 (tRNAscan-SE ID: chrIII.trna71) Ala (AGC) 71 bp Sc: 65.7 chrIII:4428953-4429023 (-)
-GGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCC
-CCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-AGC-7-1 (tRNAscan-SE ID: chrIII.trna22) Ala (AGC) 395 bp Sc: 53.1 chrIII:6590174-6590568 (+)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGACACAGGTGATTCGCGAGTA
-CGAGTTTTATGCTTCATCCGAGGTTCGCGCGTGCTTCGAATGGGTACTTGAAAACATGAG
-CAAAAATGGAGAAAAATGCTCGTCTTTGCGAACGAACGCGAGCATAAAGGAGGCATTGCG
-AAAACAATTTATGCTTCTTTTTTTTCACTTATATCAGCTGAAAAAGTTCAAAATATAACT
-TCAGTTCTTGTATAAGCCACCCCCACTACCCGAAGACATGATTAAGCCACCTCAAGACAT
-TTTCGCAAACACGAGCATTGTGTGCGTCGAAGCATTTTGCTTACACTGCGAATCACCTGT
-GGGAGAGGGTTGGGGTTCAATTCCCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-CGC-1-1 (tRNAscan-SE ID: chrX.trna206) Ala (CGC) 72 bp Sc: 73.7 chrX:12890285-12890356 (-)
-GGGGGCATAGCTCAGGGGTAGAGCGCTCGCTTCGCATGCGAGAAGTCCGGGGTTCAATTC
-CCCGTGCCTCCA
->Caenorhabditis_elegans_tRNA-Ala-CGC-2-1 (tRNAscan-SE ID: chrV.trna82) Ala (CGC) 72 bp Sc: 72.3 chrV:15479985-15480056 (-)
-GGGGGCATAGCTCAGAGGTAGAGCGCCCGCTTCGCATGCGGGAAGTCCGGGGTTCAATCC
-CCCGTGCCTCCA
->Caenorhabditis_elegans_tRNA-Ala-CGC-3-1 (tRNAscan-SE ID: chrV.trna14) Ala (CGC) 72 bp Sc: 67.8 chrV:9503562-9503633 (+)
-GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTCGCATGCGAGAAGTCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-CGC-4-1 (tRNAscan-SE ID: chrV.trna13) Ala (CGC) 72 bp Sc: 63.4 chrV:9318202-9318273 (+)
-GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTCGCATGTGAGAAGTCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-TGC-1-1 (tRNAscan-SE ID: chrII.trna39) Ala (TGC) 72 bp Sc: 68.8 chrII:11334013-11334084 (-)
-GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-TGC-1-2 (tRNAscan-SE ID: chrII.trna22) Ala (TGC) 72 bp Sc: 68.8 chrII:11334508-11334579 (+)
-GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-TGC-1-3 (tRNAscan-SE ID: chrII.trna29) Ala (TGC) 72 bp Sc: 68.8 chrII:12678314-12678385 (+)
-GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-TGC-1-4 (tRNAscan-SE ID: chrIV.trna60) Ala (TGC) 72 bp Sc: 68.8 chrIV:14013805-14013876 (-)
-GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-TGC-1-5 (tRNAscan-SE ID: chrIV.trna53) Ala (TGC) 72 bp Sc: 68.8 chrIV:15604312-15604383 (-)
-GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-TGC-1-6 (tRNAscan-SE ID: chrX.trna42) Ala (TGC) 72 bp Sc: 68.8 chrX:6286321-6286392 (+)
-GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-TGC-1-7 (tRNAscan-SE ID: chrX.trna276) Ala (TGC) 72 bp Sc: 68.8 chrX:6292278-6292349 (-)
-GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Ala-TGC-1-8 (tRNAscan-SE ID: chrX.trna81) Ala (TGC) 72 bp Sc: 68.8 chrX:9743589-9743660 (+)
-GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Arg-ACG-1-1 (tRNAscan-SE ID: chrI.trna70) Arg (ACG) 73 bp Sc: 72.1 chrI:5843083-5843155 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGCAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-1-2 (tRNAscan-SE ID: chrIII.trna70) Arg (ACG) 73 bp Sc: 72.1 chrIII:4449533-4449605 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGCAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-1-3 (tRNAscan-SE ID: chrIII.trna69) Arg (ACG) 73 bp Sc: 72.1 chrIII:4450324-4450396 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGCAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-1-4 (tRNAscan-SE ID: chrIV.trna12) Arg (ACG) 73 bp Sc: 72.1 chrIV:3524819-3524891 (+)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGCAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-1-5 (tRNAscan-SE ID: chrIV.trna62) Arg (ACG) 73 bp Sc: 72.1 chrIV:12417926-12417998 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGCAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-1-6 (tRNAscan-SE ID: chrIV.trna58) Arg (ACG) 73 bp Sc: 72.1 chrIV:14611307-14611379 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGCAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-2-1 (tRNAscan-SE ID: chrX.trna226) Arg (ACG) 73 bp Sc: 71.6 chrX:10018425-10018497 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAAT
-CCTACCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-3-1 (tRNAscan-SE ID: chrX.trna277) Arg (ACG) 73 bp Sc: 68.7 chrX:6220070-6220142 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-3-10 (tRNAscan-SE ID: chrX.trna218) Arg (ACG) 73 bp Sc: 68.7 chrX:11252590-11252662 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-3-2 (tRNAscan-SE ID: chrX.trna267) Arg (ACG) 73 bp Sc: 68.7 chrX:8036685-8036757 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-3-3 (tRNAscan-SE ID: chrX.trna255) Arg (ACG) 73 bp Sc: 68.7 chrX:8624460-8624532 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-3-4 (tRNAscan-SE ID: chrX.trna252) Arg (ACG) 73 bp Sc: 68.7 chrX:8640794-8640866 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-3-5 (tRNAscan-SE ID: chrX.trna84) Arg (ACG) 73 bp Sc: 68.7 chrX:10132678-10132750 (+)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-3-6 (tRNAscan-SE ID: chrX.trna225) Arg (ACG) 73 bp Sc: 68.7 chrX:10132971-10133043 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-3-7 (tRNAscan-SE ID: chrX.trna85) Arg (ACG) 73 bp Sc: 68.7 chrX:10145156-10145228 (+)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-3-8 (tRNAscan-SE ID: chrX.trna224) Arg (ACG) 73 bp Sc: 68.7 chrX:10148649-10148721 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-3-9 (tRNAscan-SE ID: chrX.trna222) Arg (ACG) 73 bp Sc: 68.7 chrX:10731989-10732061 (-)
-GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-4-1 (tRNAscan-SE ID: chrX.trna253) Arg (ACG) 71 bp Sc: 54.4 chrX:8639225-8639295 (-)
-GGCCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAATCC
-TGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-ACG-5-1 (tRNAscan-SE ID: chrX.trna64) Arg (ACG) 73 bp Sc: 57.5 chrX:8623603-8623675 (+)
-GGCCGCGTGGGGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAAT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-CCG-1-1 (tRNAscan-SE ID: chrII.trna33) Arg (CCG) 72 bp Sc: 53.8 chrII:12728755-12728826 (-)
-GCTCGCGTGGCCTAATGGATAAGGCACCGGACTCCGGAACCGGGAATGGGGGTTCAAGTC
-CCTCCGCGAGCT
->Caenorhabditis_elegans_tRNA-Arg-CCT-1-1 (tRNAscan-SE ID: chrIV.trna1) Arg (CCT) 73 bp Sc: 69.7 chrIV:143982-144054 (+)
-GGCCGTGTGGCCTAATGGATAAGGCGTCGGTCTCCTAAACCGAAGACTGCAGGTTCGAGT
-CCTGCCTCGGTCG
->Caenorhabditis_elegans_tRNA-Arg-CCT-1-2 (tRNAscan-SE ID: chrX.trna122) Arg (CCT) 73 bp Sc: 69.7 chrX:14115691-14115763 (+)
-GGCCGTGTGGCCTAATGGATAAGGCGTCGGTCTCCTAAACCGAAGACTGCAGGTTCGAGT
-CCTGCCTCGGTCG
->Caenorhabditis_elegans_tRNA-Arg-CCT-2-1 (tRNAscan-SE ID: chrIII.trna60) Arg (CCT) 86 bp Sc: 68.7 chrIII:6726991-6727076 (-)
-GCCACGGTGGCCGAGTGTGGTCAAAGGCGTGAGACTCCTGATCTCTTTCGGGCAACCGAT
-CGCAGGTTCGAATCCTGCCCGTGGCA
->Caenorhabditis_elegans_tRNA-Arg-TCG-1-1 (tRNAscan-SE ID: chrX.trna10) Arg (TCG) 73 bp Sc: 71.3 chrX:1698674-1698746 (+)
-GGCCGCGTGGCCTAATGGATAAGGCACCAGACTTCGAATCTGGGGATTGCAGGTTCGATC
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-TCG-2-1 (tRNAscan-SE ID: chrI.trna13) Arg (TCG) 73 bp Sc: 71.0 chrI:9267122-9267194 (+)
-GGCCGCGTGGCCTAATGGATAAGGCACCAGACTTCGAATCTGGGGATTGCAGGTTCGAGT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-TCG-2-2 (tRNAscan-SE ID: chrII.trna17) Arg (TCG) 73 bp Sc: 71.0 chrII:9566241-9566313 (+)
-GGCCGCGTGGCCTAATGGATAAGGCACCAGACTTCGAATCTGGGGATTGCAGGTTCGAGT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-TCG-2-3 (tRNAscan-SE ID: chrIII.trna68) Arg (TCG) 73 bp Sc: 71.0 chrIII:4470886-4470958 (-)
-GGCCGCGTGGCCTAATGGATAAGGCACCAGACTTCGAATCTGGGGATTGCAGGTTCGAGT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-TCG-2-4 (tRNAscan-SE ID: chrX.trna211) Arg (TCG) 73 bp Sc: 71.0 chrX:12337998-12338070 (-)
-GGCCGCGTGGCCTAATGGATAAGGCACCAGACTTCGAATCTGGGGATTGCAGGTTCGAGT
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-TCG-3-1 (tRNAscan-SE ID: chrX.trna303) Arg (TCG) 73 bp Sc: 69.4 chrX:1089173-1089245 (-)
-GGCCGCGTGGCCTAATGGATAAGGCATCAGACTTCGAATCTGGGGATTGCAGGTTCGATC
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-TCG-3-2 (tRNAscan-SE ID: chrX.trna6) Arg (TCG) 73 bp Sc: 69.4 chrX:1089838-1089910 (+)
-GGCCGCGTGGCCTAATGGATAAGGCATCAGACTTCGAATCTGGGGATTGCAGGTTCGATC
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-TCG-4-1 (tRNAscan-SE ID: chrX.trna148) Arg (TCG) 73 bp Sc: 69.4 chrX:16461477-16461549 (+)
-GGCCGCGTGGCCTAATGGATAAGGCATCAGACTTCGAATCTGGGGATTGCAGGTTCGATC
-CCTGCCGTGGTCG
->Caenorhabditis_elegans_tRNA-Arg-TCT-1-1 (tRNAscan-SE ID: chrI.trna35) Arg (TCT) 73 bp Sc: 71.7 chrI:12198603-12198675 (+)
-GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGATC
-CCTGCCTGGGTCA
->Caenorhabditis_elegans_tRNA-Arg-TCT-2-1 (tRNAscan-SE ID: chrI.trna3) Arg (TCT) 73 bp Sc: 71.1 chrI:1447138-1447210 (+)
-GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGAGC
-CCTGCCTGGGTCA
->Caenorhabditis_elegans_tRNA-Arg-TCT-2-2 (tRNAscan-SE ID: chrI.trna4) Arg (TCT) 73 bp Sc: 71.1 chrI:1575720-1575792 (+)
-GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGAGC
-CCTGCCTGGGTCA
->Caenorhabditis_elegans_tRNA-Arg-TCT-2-3 (tRNAscan-SE ID: chrV.trna10) Arg (TCT) 73 bp Sc: 71.1 chrV:7506395-7506467 (+)
-GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGAGC
-CCTGCCTGGGTCA
->Caenorhabditis_elegans_tRNA-Arg-TCT-2-4 (tRNAscan-SE ID: chrX.trna60) Arg (TCT) 73 bp Sc: 71.1 chrX:8386204-8386276 (+)
-GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGAGC
-CCTGCCTGGGTCA
->Caenorhabditis_elegans_tRNA-Arg-TCT-2-5 (tRNAscan-SE ID: chrX.trna61) Arg (TCT) 73 bp Sc: 71.1 chrX:8386614-8386686 (+)
-GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGAGC
-CCTGCCTGGGTCA
->Caenorhabditis_elegans_tRNA-Arg-TCT-3-1 (tRNAscan-SE ID: chrX.trna263) Arg (TCT) 73 bp Sc: 68.8 chrX:8381795-8381867 (-)
-GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGACC
-CCTGCCTGGGTCA
->Caenorhabditis_elegans_tRNA-Arg-TCT-3-2 (tRNAscan-SE ID: chrX.trna182) Arg (TCT) 73 bp Sc: 68.8 chrX:15146562-15146634 (-)
-GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGACC
-CCTGCCTGGGTCA
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-1 (tRNAscan-SE ID: chrI.trna62) Asn (GTT) 73 bp Sc: 73.5 chrI:9051253-9051325 (-)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-10 (tRNAscan-SE ID: chrV.trna27) Asn (GTT) 73 bp Sc: 73.5 chrV:16341779-16341851 (+)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-11 (tRNAscan-SE ID: chrV.trna43) Asn (GTT) 73 bp Sc: 73.5 chrV:19723031-19723103 (+)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-12 (tRNAscan-SE ID: chrV.trna48) Asn (GTT) 73 bp Sc: 73.5 chrV:20347797-20347869 (-)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-13 (tRNAscan-SE ID: chrV.trna47) Asn (GTT) 73 bp Sc: 73.5 chrV:20350529-20350601 (-)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-14 (tRNAscan-SE ID: chrX.trna288) Asn (GTT) 73 bp Sc: 73.5 chrX:2549528-2549600 (-)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-15 (tRNAscan-SE ID: chrX.trna49) Asn (GTT) 73 bp Sc: 73.5 chrX:7773718-7773790 (+)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-16 (tRNAscan-SE ID: chrX.trna270) Asn (GTT) 73 bp Sc: 73.5 chrX:7773965-7774037 (-)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-17 (tRNAscan-SE ID: chrX.trna62) Asn (GTT) 73 bp Sc: 73.5 chrX:8404499-8404571 (+)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-18 (tRNAscan-SE ID: chrX.trna89) Asn (GTT) 73 bp Sc: 73.5 chrX:11645683-11645755 (+)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-2 (tRNAscan-SE ID: chrIII.trna23) Asn (GTT) 73 bp Sc: 73.5 chrIII:6805568-6805640 (+)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-3 (tRNAscan-SE ID: chrIII.trna51) Asn (GTT) 73 bp Sc: 73.5 chrIII:9104207-9104279 (-)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-4 (tRNAscan-SE ID: chrIII.trna43) Asn (GTT) 73 bp Sc: 73.5 chrIII:13225162-13225234 (-)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-5 (tRNAscan-SE ID: chrV.trna92) Asn (GTT) 73 bp Sc: 73.5 chrV:12331965-12332037 (-)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-6 (tRNAscan-SE ID: chrV.trna19) Asn (GTT) 73 bp Sc: 73.5 chrV:15156682-15156754 (+)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-7 (tRNAscan-SE ID: chrV.trna77) Asn (GTT) 73 bp Sc: 73.5 chrV:16338370-16338442 (-)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-8 (tRNAscan-SE ID: chrV.trna26) Asn (GTT) 73 bp Sc: 73.5 chrV:16338548-16338620 (+)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-1-9 (tRNAscan-SE ID: chrV.trna76) Asn (GTT) 73 bp Sc: 73.5 chrV:16341601-16341673 (-)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asn-GTT-2-1 (tRNAscan-SE ID: chrX.trna48) Asn (GTT) 73 bp Sc: 64.4 chrX:7773190-7773262 (+)
-GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGATTCGAGC
-CCACCCGGGAGCG
->Caenorhabditis_elegans_tRNA-Asp-GTC-1-1 (tRNAscan-SE ID: chrIV.trna8) Asp (GTC) 72 bp Sc: 63.3 chrIV:2800099-2800170 (+)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGGCCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-1 (tRNAscan-SE ID: chrI.trna24) Asp (GTC) 72 bp Sc: 61.7 chrI:10807204-10807275 (+)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-10 (tRNAscan-SE ID: chrV.trna72) Asp (GTC) 72 bp Sc: 61.7 chrV:16645706-16645777 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-11 (tRNAscan-SE ID: chrV.trna71) Asp (GTC) 72 bp Sc: 61.7 chrV:16648766-16648837 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-12 (tRNAscan-SE ID: chrX.trna305) Asp (GTC) 72 bp Sc: 61.7 chrX:489868-489939 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-13 (tRNAscan-SE ID: chrX.trna291) Asp (GTC) 72 bp Sc: 61.7 chrX:2227191-2227262 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-14 (tRNAscan-SE ID: chrX.trna20) Asp (GTC) 72 bp Sc: 61.7 chrX:2553565-2553636 (+)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-15 (tRNAscan-SE ID: chrX.trna54) Asp (GTC) 72 bp Sc: 61.7 chrX:8149156-8149227 (+)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-16 (tRNAscan-SE ID: chrX.trna266) Asp (GTC) 72 bp Sc: 61.7 chrX:8152546-8152617 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-17 (tRNAscan-SE ID: chrX.trna56) Asp (GTC) 72 bp Sc: 61.7 chrX:8154722-8154793 (+)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-18 (tRNAscan-SE ID: chrX.trna187) Asp (GTC) 72 bp Sc: 61.7 chrX:14162026-14162097 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-19 (tRNAscan-SE ID: chrX.trna163) Asp (GTC) 72 bp Sc: 61.7 chrX:16604720-16604791 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-2 (tRNAscan-SE ID: chrIV.trna82) Asp (GTC) 72 bp Sc: 61.7 chrIV:322632-322703 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-20 (tRNAscan-SE ID: chrX.trna161) Asp (GTC) 72 bp Sc: 61.7 chrX:16618296-16618367 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-21 (tRNAscan-SE ID: chrX.trna160) Asp (GTC) 72 bp Sc: 61.7 chrX:16619333-16619404 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-3 (tRNAscan-SE ID: chrIV.trna4) Asp (GTC) 72 bp Sc: 61.7 chrIV:683063-683134 (+)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-4 (tRNAscan-SE ID: chrIV.trna7) Asp (GTC) 72 bp Sc: 61.7 chrIV:1514592-1514663 (+)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-5 (tRNAscan-SE ID: chrIV.trna77) Asp (GTC) 72 bp Sc: 61.7 chrIV:2801151-2801222 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-6 (tRNAscan-SE ID: chrIV.trna52) Asp (GTC) 72 bp Sc: 61.7 chrIV:15931342-15931413 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-7 (tRNAscan-SE ID: chrIV.trna35) Asp (GTC) 72 bp Sc: 61.7 chrIV:15932010-15932081 (+)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-8 (tRNAscan-SE ID: chrV.trna78) Asp (GTC) 72 bp Sc: 61.7 chrV:15551799-15551870 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-2-9 (tRNAscan-SE ID: chrV.trna29) Asp (GTC) 72 bp Sc: 61.7 chrV:16640578-16640649 (+)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-3-1 (tRNAscan-SE ID: chrIV.trna9) Asp (GTC) 72 bp Sc: 60.5 chrIV:2802337-2802408 (+)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCGCATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-4-1 (tRNAscan-SE ID: chrIV.trna10) Asp (GTC) 72 bp Sc: 58.7 chrIV:2805627-2805698 (+)
-TCCTCGGTAGTGTAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-5-1 (tRNAscan-SE ID: chrIV.trna11) Asp (GTC) 72 bp Sc: 52.2 chrIV:2808355-2808426 (+)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGTGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-6-1 (tRNAscan-SE ID: chrX.trna162) Asp (GTC) 72 bp Sc: 52.1 chrX:16617892-16617963 (-)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCTGGTTCAATTC
-CCGGCCGGGGAG
->Caenorhabditis_elegans_tRNA-Asp-GTC-7-1 (tRNAscan-SE ID: chrX.trna58) Asp (GTC) 73 bp Sc: 54.8 chrX:8155752-8155824 (+)
-TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTC
-CCGGCCGGGAGAA
->Caenorhabditis_elegans_tRNA-Cys-GCA-1-1 (tRNAscan-SE ID: chrI.trna8) Cys (GCA) 72 bp Sc: 74.0 chrI:6781803-6781874 (+)
-GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTC
-CGGGTGCCCCCT
->Caenorhabditis_elegans_tRNA-Cys-GCA-1-10 (tRNAscan-SE ID: chrX.trna66) Cys (GCA) 72 bp Sc: 74.0 chrX:8638922-8638993 (+)
-GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTC
-CGGGTGCCCCCT
->Caenorhabditis_elegans_tRNA-Cys-GCA-1-11 (tRNAscan-SE ID: chrX.trna249) Cys (GCA) 72 bp Sc: 74.0 chrX:8818100-8818171 (-)
-GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTC
-CGGGTGCCCCCT
->Caenorhabditis_elegans_tRNA-Cys-GCA-1-12 (tRNAscan-SE ID: chrX.trna129) Cys (GCA) 72 bp Sc: 74.0 chrX:14804877-14804948 (+)
-GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTC
-CGGGTGCCCCCT
->Caenorhabditis_elegans_tRNA-Cys-GCA-1-2 (tRNAscan-SE ID: chrI.trna29) Cys (GCA) 72 bp Sc: 74.0 chrI:11505551-11505622 (+)
-GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTC
-CGGGTGCCCCCT
->Caenorhabditis_elegans_tRNA-Cys-GCA-1-3 (tRNAscan-SE ID: chrV.trna8) Cys (GCA) 72 bp Sc: 74.0 chrV:6559757-6559828 (+)
-GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTC
-CGGGTGCCCCCT
->Caenorhabditis_elegans_tRNA-Cys-GCA-1-4 (tRNAscan-SE ID: chrV.trna86) Cys (GCA) 72 bp Sc: 74.0 chrV:14855787-14855858 (-)
-GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTC
-CGGGTGCCCCCT
->Caenorhabditis_elegans_tRNA-Cys-GCA-1-5 (tRNAscan-SE ID: chrV.trna46) Cys (GCA) 72 bp Sc: 74.0 chrV:20694121-20694192 (-)
-GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTC
-CGGGTGCCCCCT
->Caenorhabditis_elegans_tRNA-Cys-GCA-1-6 (tRNAscan-SE ID: chrX.trna257) Cys (GCA) 72 bp Sc: 74.0 chrX:8623764-8623835 (-)
-GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTC
-CGGGTGCCCCCT
->Caenorhabditis_elegans_tRNA-Cys-GCA-1-7 (tRNAscan-SE ID: chrX.trna256) Cys (GCA) 72 bp Sc: 74.0 chrX:8623998-8624069 (-)
-GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTC
-CGGGTGCCCCCT
->Caenorhabditis_elegans_tRNA-Cys-GCA-1-8 (tRNAscan-SE ID: chrX.trna65) Cys (GCA) 72 bp Sc: 74.0 chrX:8624282-8624353 (+)
-GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTC
-CGGGTGCCCCCT
->Caenorhabditis_elegans_tRNA-Cys-GCA-1-9 (tRNAscan-SE ID: chrX.trna254) Cys (GCA) 72 bp Sc: 74.0 chrX:8638620-8638691 (-)
-GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTC
-CGGGTGCCCCCT
->Caenorhabditis_elegans_tRNA-Cys-GCA-2-1 (tRNAscan-SE ID: chrV.trna6) Cys (GCA) 72 bp Sc: 62.8 chrV:6335398-6335469 (+)
-TGGGGTATAGCTCAGTGGCAGAGCATTCGATTGCAGATCGAGAGGTCCCTGGTTCAACTC
-CGGGTGCCCCCT
->Caenorhabditis_elegans_tRNA-Gln-CTG-1-1 (tRNAscan-SE ID: chrV.trna17) Gln (CTG) 72 bp Sc: 74.0 chrV:14231364-14231435 (+)
-GGTTCCATGGTGTAGTGGTTAGCACTCAGGACTCTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGGACCT
->Caenorhabditis_elegans_tRNA-Gln-CTG-2-1 (tRNAscan-SE ID: chrIV.trna16) Gln (CTG) 72 bp Sc: 71.6 chrIV:5334712-5334783 (+)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTCTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGGACCT
->Caenorhabditis_elegans_tRNA-Gln-CTG-2-2 (tRNAscan-SE ID: chrIV.trna64) Gln (CTG) 72 bp Sc: 71.6 chrIV:12416942-12417013 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTCTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGGACCT
->Caenorhabditis_elegans_tRNA-Gln-CTG-2-3 (tRNAscan-SE ID: chrV.trna74) Gln (CTG) 72 bp Sc: 71.6 chrV:16592237-16592308 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTCTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGGACCT
->Caenorhabditis_elegans_tRNA-Gln-CTG-2-4 (tRNAscan-SE ID: chrX.trna258) Gln (CTG) 72 bp Sc: 71.6 chrX:8608834-8608905 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTCTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGGACCT
->Caenorhabditis_elegans_tRNA-Gln-CTG-2-5 (tRNAscan-SE ID: chrX.trna77) Gln (CTG) 72 bp Sc: 71.6 chrX:9090830-9090901 (+)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTCTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGGACCT
->Caenorhabditis_elegans_tRNA-Gln-CTG-3-1 (tRNAscan-SE ID: chrX.trna90) Gln (CTG) 72 bp Sc: 61.0 chrX:11872506-11872577 (+)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGTACTCTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGGACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-1 (tRNAscan-SE ID: chrII.trna46) Gln (TTG) 72 bp Sc: 72.0 chrII:7756949-7757020 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-10 (tRNAscan-SE ID: chrX.trna236) Gln (TTG) 72 bp Sc: 72.0 chrX:9078254-9078325 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-11 (tRNAscan-SE ID: chrX.trna235) Gln (TTG) 72 bp Sc: 72.0 chrX:9090627-9090698 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-12 (tRNAscan-SE ID: chrX.trna234) Gln (TTG) 72 bp Sc: 72.0 chrX:9091097-9091168 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-13 (tRNAscan-SE ID: chrX.trna233) Gln (TTG) 72 bp Sc: 72.0 chrX:9091557-9091628 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-14 (tRNAscan-SE ID: chrX.trna215) Gln (TTG) 72 bp Sc: 72.0 chrX:11872241-11872312 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-15 (tRNAscan-SE ID: chrX.trna98) Gln (TTG) 72 bp Sc: 72.0 chrX:12937701-12937772 (+)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-16 (tRNAscan-SE ID: chrX.trna99) Gln (TTG) 72 bp Sc: 72.0 chrX:12938182-12938253 (+)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-2 (tRNAscan-SE ID: chrII.trna32) Gln (TTG) 72 bp Sc: 72.0 chrII:14474842-14474913 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-3 (tRNAscan-SE ID: chrIII.trna45) Gln (TTG) 72 bp Sc: 72.0 chrIII:12399909-12399980 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-4 (tRNAscan-SE ID: chrIV.trna23) Gln (TTG) 72 bp Sc: 72.0 chrIV:7275327-7275398 (+)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-5 (tRNAscan-SE ID: chrIV.trna67) Gln (TTG) 72 bp Sc: 72.0 chrIV:10311231-10311302 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-6 (tRNAscan-SE ID: chrIV.trna63) Gln (TTG) 72 bp Sc: 72.0 chrIV:12417249-12417320 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-7 (tRNAscan-SE ID: chrV.trna106) Gln (TTG) 72 bp Sc: 72.0 chrV:5330139-5330210 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-8 (tRNAscan-SE ID: chrX.trna3) Gln (TTG) 72 bp Sc: 72.0 chrX:410391-410462 (+)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-1-9 (tRNAscan-SE ID: chrX.trna63) Gln (TTG) 72 bp Sc: 72.0 chrX:8609038-8609109 (+)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-2-1 (tRNAscan-SE ID: chrI.trna17) Gln (TTG) 83 bp Sc: 71.9 chrI:9558792-9558874 (+)
-GCCCCGGTGGCCGAGCGGTCGAAGGCGTGAGACTTGTTCTCATTGGGTTAAACCAGTCGC
-GGGTTCGAATCCCGCCCGGGGCA
->Caenorhabditis_elegans_tRNA-Gln-TTG-3-1 (tRNAscan-SE ID: chrX.trna78) Gln (TTG) 72 bp Sc: 64.1 chrX:9091310-9091381 (+)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCAGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-4-1 (tRNAscan-SE ID: chrX.trna73) Gln (TTG) 72 bp Sc: 62.2 chrX:8925641-8925712 (+)
-GGTTCCATGGTGTAGCGGTTAGCACTCATGACTTTGAATCCTGCGACCCGAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Gln-TTG-5-1 (tRNAscan-SE ID: chrX.trna237) Gln (TTG) 72 bp Sc: 61.2 chrX:9074672-9074743 (-)
-GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGATCCAAGTTCAAATC
-TCGGTGGAACCT
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-1 (tRNAscan-SE ID: chrI.trna64) Glu (CTC) 72 bp Sc: 77.9 chrI:8530128-8530199 (-)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-10 (tRNAscan-SE ID: chrX.trna29) Glu (CTC) 72 bp Sc: 77.9 chrX:4409784-4409855 (+)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-11 (tRNAscan-SE ID: chrX.trna30) Glu (CTC) 72 bp Sc: 77.9 chrX:4410652-4410723 (+)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-12 (tRNAscan-SE ID: chrX.trna47) Glu (CTC) 72 bp Sc: 77.9 chrX:7681040-7681111 (+)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-13 (tRNAscan-SE ID: chrX.trna268) Glu (CTC) 72 bp Sc: 77.9 chrX:7898308-7898379 (-)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-14 (tRNAscan-SE ID: chrX.trna108) Glu (CTC) 72 bp Sc: 77.9 chrX:13448677-13448748 (+)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-15 (tRNAscan-SE ID: chrX.trna120) Glu (CTC) 72 bp Sc: 77.9 chrX:14015944-14016015 (+)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-16 (tRNAscan-SE ID: chrX.trna168) Glu (CTC) 72 bp Sc: 77.9 chrX:16271296-16271367 (-)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-17 (tRNAscan-SE ID: chrX.trna167) Glu (CTC) 72 bp Sc: 77.9 chrX:16284323-16284394 (-)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-18 (tRNAscan-SE ID: chrX.trna166) Glu (CTC) 72 bp Sc: 77.9 chrX:16285295-16285366 (-)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-19 (tRNAscan-SE ID: chrX.trna146) Glu (CTC) 72 bp Sc: 77.9 chrX:16378113-16378184 (+)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-2 (tRNAscan-SE ID: chrI.trna47) Glu (CTC) 72 bp Sc: 77.9 chrI:11977191-11977262 (-)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-20 (tRNAscan-SE ID: chrX.trna153) Glu (CTC) 72 bp Sc: 77.9 chrX:16558942-16559013 (+)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-3 (tRNAscan-SE ID: chrI.trna31) Glu (CTC) 72 bp Sc: 77.9 chrI:11977992-11978063 (+)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-4 (tRNAscan-SE ID: chrI.trna32) Glu (CTC) 72 bp Sc: 77.9 chrI:11978764-11978835 (+)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-5 (tRNAscan-SE ID: chrII.trna10) Glu (CTC) 72 bp Sc: 77.9 chrII:5293452-5293523 (+)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-6 (tRNAscan-SE ID: chrIII.trna75) Glu (CTC) 72 bp Sc: 77.9 chrIII:1604702-1604773 (-)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-7 (tRNAscan-SE ID: chrIII.trna8) Glu (CTC) 72 bp Sc: 77.9 chrIII:2032518-2032589 (+)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-8 (tRNAscan-SE ID: chrIII.trna74) Glu (CTC) 72 bp Sc: 77.9 chrIII:2032897-2032968 (-)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-1-9 (tRNAscan-SE ID: chrX.trna287) Glu (CTC) 72 bp Sc: 77.9 chrX:3035976-3036047 (-)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-2-1 (tRNAscan-SE ID: chrIII.trna56) Glu (CTC) 72 bp Sc: 73.2 chrIII:7642158-7642229 (-)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACTCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-3-1 (tRNAscan-SE ID: chrX.trna51) Glu (CTC) 72 bp Sc: 73.4 chrX:7906585-7906656 (+)
-TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGAAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-4-1 (tRNAscan-SE ID: chrX.trna140) Glu (CTC) 72 bp Sc: 70.4 chrX:16273767-16273838 (+)
-TCCGTTGTGGTCTAGTAGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACGGAA
->Caenorhabditis_elegans_tRNA-Glu-CTC-5-1 (tRNAscan-SE ID: chrX.trna141) Glu (CTC) 72 bp Sc: 56.8 chrX:16274498-16274569 (+)
-TCCGTTGTTGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTC
-CCCGCAACAAAT
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-1 (tRNAscan-SE ID: chrI.trna21) Glu (TTC) 72 bp Sc: 75.3 chrI:9883696-9883767 (+)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-10 (tRNAscan-SE ID: chrX.trna67) Glu (TTC) 72 bp Sc: 75.3 chrX:8646480-8646551 (+)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-11 (tRNAscan-SE ID: chrX.trna70) Glu (TTC) 72 bp Sc: 75.3 chrX:8836113-8836184 (+)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-12 (tRNAscan-SE ID: chrX.trna223) Glu (TTC) 72 bp Sc: 75.3 chrX:10667022-10667093 (-)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-13 (tRNAscan-SE ID: chrX.trna86) Glu (TTC) 72 bp Sc: 75.3 chrX:10667593-10667664 (+)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-14 (tRNAscan-SE ID: chrX.trna221) Glu (TTC) 72 bp Sc: 75.3 chrX:10821327-10821398 (-)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-15 (tRNAscan-SE ID: chrX.trna209) Glu (TTC) 72 bp Sc: 75.3 chrX:12367642-12367713 (-)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-2 (tRNAscan-SE ID: chrII.trna14) Glu (TTC) 72 bp Sc: 75.3 chrII:6898194-6898265 (+)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-3 (tRNAscan-SE ID: chrIV.trna5) Glu (TTC) 72 bp Sc: 75.3 chrIV:842809-842880 (+)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-4 (tRNAscan-SE ID: chrIV.trna80) Glu (TTC) 72 bp Sc: 75.3 chrIV:1388216-1388287 (-)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-5 (tRNAscan-SE ID: chrIV.trna51) Glu (TTC) 72 bp Sc: 75.3 chrIV:15933161-15933232 (-)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-6 (tRNAscan-SE ID: chrIV.trna36) Glu (TTC) 72 bp Sc: 75.3 chrIV:15933353-15933424 (+)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-7 (tRNAscan-SE ID: chrV.trna39) Glu (TTC) 72 bp Sc: 75.3 chrV:19142788-19142859 (+)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-8 (tRNAscan-SE ID: chrX.trna14) Glu (TTC) 72 bp Sc: 75.3 chrX:1858819-1858890 (+)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-1-9 (tRNAscan-SE ID: chrX.trna31) Glu (TTC) 72 bp Sc: 75.3 chrX:4444262-4444333 (+)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-2-1 (tRNAscan-SE ID: chrIV.trna78) Glu (TTC) 72 bp Sc: 64.7 chrIV:2639809-2639880 (-)
-TCCTATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGTTTCGATTC
-CCGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Glu-TTC-3-1 (tRNAscan-SE ID: chrV.trna103) Glu (TTC) 71 bp Sc: 59.8 chrV:7069748-7069818 (-)
-TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGTTCGATTCC
-CGGCATGGGAA
->Caenorhabditis_elegans_tRNA-Gly-CCC-1-1 (tRNAscan-SE ID: chrI.trna55) Gly (CCC) 83 bp Sc: 79.1 chrI:10601133-10601215 (-)
-GCGGTGGTGGCCGAGCGGTCAAGGCGTAGGACTCCCGATCCTATTCTGGTAACAGAGCGC
-GGGTTCGAATCCCGTCCACCGCA
->Caenorhabditis_elegans_tRNA-Gly-CCC-1-2 (tRNAscan-SE ID: chrI.trna23) Gly (CCC) 83 bp Sc: 79.1 chrI:10601851-10601933 (+)
-GCGGTGGTGGCCGAGCGGTCAAGGCGTAGGACTCCCGATCCTATTCTGGTAACAGAGCGC
-GGGTTCGAATCCCGTCCACCGCA
->Caenorhabditis_elegans_tRNA-Gly-CCC-1-3 (tRNAscan-SE ID: chrI.trna54) Gly (CCC) 83 bp Sc: 79.1 chrI:10604134-10604216 (-)
-GCGGTGGTGGCCGAGCGGTCAAGGCGTAGGACTCCCGATCCTATTCTGGTAACAGAGCGC
-GGGTTCGAATCCCGTCCACCGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-1-1 (tRNAscan-SE ID: chrI.trna72) Gly (GCC) 71 bp Sc: 77.2 chrI:2272368-2272438 (-)
-GCATCGGTGGTTCAGTGGTAGAATGCTCGCCTGCCACGCGGGCGGCCCGGGTTCGATTCC
-CGGTCGATGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-1-10 (tRNAscan-SE ID: chrX.trna203) Gly (GCC) 71 bp Sc: 77.2 chrX:13121261-13121331 (-)
-GCATCGGTGGTTCAGTGGTAGAATGCTCGCCTGCCACGCGGGCGGCCCGGGTTCGATTCC
-CGGTCGATGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-1-11 (tRNAscan-SE ID: chrX.trna157) Gly (GCC) 71 bp Sc: 77.2 chrX:16928271-16928341 (-)
-GCATCGGTGGTTCAGTGGTAGAATGCTCGCCTGCCACGCGGGCGGCCCGGGTTCGATTCC
-CGGTCGATGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-1-2 (tRNAscan-SE ID: chrI.trna22) Gly (GCC) 71 bp Sc: 77.2 chrI:10593137-10593207 (+)
-GCATCGGTGGTTCAGTGGTAGAATGCTCGCCTGCCACGCGGGCGGCCCGGGTTCGATTCC
-CGGTCGATGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-1-3 (tRNAscan-SE ID: chrII.trna61) Gly (GCC) 71 bp Sc: 77.2 chrII:3062207-3062277 (-)
-GCATCGGTGGTTCAGTGGTAGAATGCTCGCCTGCCACGCGGGCGGCCCGGGTTCGATTCC
-CGGTCGATGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-1-4 (tRNAscan-SE ID: chrII.trna4) Gly (GCC) 71 bp Sc: 77.2 chrII:3062384-3062454 (+)
-GCATCGGTGGTTCAGTGGTAGAATGCTCGCCTGCCACGCGGGCGGCCCGGGTTCGATTCC
-CGGTCGATGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-1-5 (tRNAscan-SE ID: chrIII.trna17) Gly (GCC) 71 bp Sc: 77.2 chrIII:5762286-5762356 (+)
-GCATCGGTGGTTCAGTGGTAGAATGCTCGCCTGCCACGCGGGCGGCCCGGGTTCGATTCC
-CGGTCGATGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-1-6 (tRNAscan-SE ID: chrIII.trna65) Gly (GCC) 71 bp Sc: 77.2 chrIII:5782236-5782306 (-)
-GCATCGGTGGTTCAGTGGTAGAATGCTCGCCTGCCACGCGGGCGGCCCGGGTTCGATTCC
-CGGTCGATGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-1-7 (tRNAscan-SE ID: chrV.trna81) Gly (GCC) 71 bp Sc: 77.2 chrV:15505208-15505278 (-)
-GCATCGGTGGTTCAGTGGTAGAATGCTCGCCTGCCACGCGGGCGGCCCGGGTTCGATTCC
-CGGTCGATGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-1-8 (tRNAscan-SE ID: chrX.trna21) Gly (GCC) 71 bp Sc: 77.2 chrX:2613243-2613313 (+)
-GCATCGGTGGTTCAGTGGTAGAATGCTCGCCTGCCACGCGGGCGGCCCGGGTTCGATTCC
-CGGTCGATGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-1-9 (tRNAscan-SE ID: chrX.trna250) Gly (GCC) 71 bp Sc: 77.2 chrX:8796822-8796892 (-)
-GCATCGGTGGTTCAGTGGTAGAATGCTCGCCTGCCACGCGGGCGGCCCGGGTTCGATTCC
-CGGTCGATGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-2-1 (tRNAscan-SE ID: chrV.trna5) Gly (GCC) 71 bp Sc: 73.4 chrV:4310610-4310680 (+)
-GCATCGGTGGTTCAGTGGTAGAATGCTCGCCTGCCACGCGTGCGGCCCGGGTTCGATTCC
-CGGTCGATGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-3-1 (tRNAscan-SE ID: chrIII.trna66) Gly (GCC) 70 bp Sc: 67.6 chrIII:5762057-5762126 (-)
-GCATCGGTGGTTCAGTGGTAGAATGCTCGCCTGCCACGCGGCGGCCCGGGTTCGATTCCC
-GGTCGATGCA
->Caenorhabditis_elegans_tRNA-Gly-GCC-5-1 (tRNAscan-SE ID: chrII.trna48) Gly (GCC) 71 bp Sc: 66.1 chrII:5782212-5782282 (-)
-GCATCGGTGGTTCAGTGGTAGAAAGCTCGCCTGCCACGCGGGCGGCCCGGGTTCGATTCC
-CGGTCGATACA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-1 (tRNAscan-SE ID: chrI.trna60) Gly (TCC) 72 bp Sc: 71.7 chrI:9319965-9320036 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-10 (tRNAscan-SE ID: chrI.trna41) Gly (TCC) 72 bp Sc: 71.7 chrI:13331147-13331218 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-11 (tRNAscan-SE ID: chrIII.trna2) Gly (TCC) 72 bp Sc: 71.7 chrIII:1424491-1424562 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-12 (tRNAscan-SE ID: chrIII.trna58) Gly (TCC) 72 bp Sc: 71.7 chrIII:6888610-6888681 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-13 (tRNAscan-SE ID: chrIII.trna24) Gly (TCC) 72 bp Sc: 71.7 chrIII:6888806-6888877 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-14 (tRNAscan-SE ID: chrIV.trna59) Gly (TCC) 72 bp Sc: 71.7 chrIV:14576622-14576693 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-15 (tRNAscan-SE ID: chrIV.trna47) Gly (TCC) 72 bp Sc: 71.7 chrIV:16670866-16670937 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-16 (tRNAscan-SE ID: chrIV.trna43) Gly (TCC) 72 bp Sc: 71.7 chrIV:16682007-16682078 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-17 (tRNAscan-SE ID: chrIV.trna44) Gly (TCC) 72 bp Sc: 71.7 chrIV:16775182-16775253 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-18 (tRNAscan-SE ID: chrIV.trna45) Gly (TCC) 72 bp Sc: 71.7 chrIV:16776088-16776159 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-19 (tRNAscan-SE ID: chrX.trna302) Gly (TCC) 72 bp Sc: 71.7 chrX:1379603-1379674 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-2 (tRNAscan-SE ID: chrI.trna14) Gly (TCC) 72 bp Sc: 71.7 chrI:9320178-9320249 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-20 (tRNAscan-SE ID: chrX.trna22) Gly (TCC) 72 bp Sc: 71.7 chrX:3036164-3036235 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-21 (tRNAscan-SE ID: chrX.trna269) Gly (TCC) 72 bp Sc: 71.7 chrX:7794336-7794407 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-22 (tRNAscan-SE ID: chrX.trna50) Gly (TCC) 72 bp Sc: 71.7 chrX:7794603-7794674 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-23 (tRNAscan-SE ID: chrX.trna248) Gly (TCC) 72 bp Sc: 71.7 chrX:8818578-8818649 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-24 (tRNAscan-SE ID: chrX.trna247) Gly (TCC) 72 bp Sc: 71.7 chrX:8819924-8819995 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-25 (tRNAscan-SE ID: chrX.trna69) Gly (TCC) 72 bp Sc: 71.7 chrX:8820185-8820256 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-26 (tRNAscan-SE ID: chrX.trna246) Gly (TCC) 72 bp Sc: 71.7 chrX:8838338-8838409 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-27 (tRNAscan-SE ID: chrX.trna87) Gly (TCC) 72 bp Sc: 71.7 chrX:10963828-10963899 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-28 (tRNAscan-SE ID: chrX.trna181) Gly (TCC) 72 bp Sc: 71.7 chrX:15200817-15200888 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-29 (tRNAscan-SE ID: chrX.trna130) Gly (TCC) 72 bp Sc: 71.7 chrX:15201007-15201078 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-3 (tRNAscan-SE ID: chrI.trna59) Gly (TCC) 72 bp Sc: 71.7 chrI:9327424-9327495 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-4 (tRNAscan-SE ID: chrI.trna15) Gly (TCC) 72 bp Sc: 71.7 chrI:9327637-9327708 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-5 (tRNAscan-SE ID: chrI.trna58) Gly (TCC) 72 bp Sc: 71.7 chrI:9328416-9328487 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-6 (tRNAscan-SE ID: chrI.trna16) Gly (TCC) 72 bp Sc: 71.7 chrI:9328630-9328701 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-7 (tRNAscan-SE ID: chrI.trna52) Gly (TCC) 72 bp Sc: 71.7 chrI:10927413-10927484 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-8 (tRNAscan-SE ID: chrI.trna26) Gly (TCC) 72 bp Sc: 71.7 chrI:10927583-10927654 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-1-9 (tRNAscan-SE ID: chrI.trna42) Gly (TCC) 72 bp Sc: 71.7 chrI:13324180-13324251 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-2-1 (tRNAscan-SE ID: chrX.trna71) Gly (TCC) 72 bp Sc: 68.1 chrX:8846721-8846792 (+)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCTCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-3-1 (tRNAscan-SE ID: chrX.trna245) Gly (TCC) 73 bp Sc: 67.4 chrX:8846505-8846577 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-4-1 (tRNAscan-SE ID: chrX.trna68) Gly (TCC) 72 bp Sc: 61.8 chrX:8819681-8819752 (+)
-GAGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-5-1 (tRNAscan-SE ID: chrI.trna39) Gly (TCC) 72 bp Sc: 62.2 chrI:13324995-13325066 (+)
-GCGTTCGGGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-6-1 (tRNAscan-SE ID: chrIV.trna46) Gly (TCC) 72 bp Sc: 61.0 chrIV:16684383-16684454 (-)
-GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACCGGGGTTCGATTC
-CCCCCGAAGGCA
->Caenorhabditis_elegans_tRNA-Gly-TCC-7-1 (tRNAscan-SE ID: chrX.trna27) Gly (TCC) 77 bp Sc: 54.5 chrX:3994602-3994678 (+)
-GCGTTCGTGGTGTAATGGTCGGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTC
-CCCCCCCCCCGAACGCA
->Caenorhabditis_elegans_tRNA-His-GTG-1-1 (tRNAscan-SE ID: chrIV.trna25) His (GTG) 88 bp Sc: 79.2 chrIV:11721149-11721236 (+)
-GCCACGGTGGCCGAGTGGTCAAGGCGTGAGCTTGTGGGATGCGCTCATGGGGTTAAACCC
-ATCGCAGGTTCGAATCCTGCCCGTGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-2-1 (tRNAscan-SE ID: chrII.trna56) His (GTG) 72 bp Sc: 69.4 chrII:3521487-3521558 (-)
-GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCCGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-2-10 (tRNAscan-SE ID: chrX.trna188) His (GTG) 72 bp Sc: 69.4 chrX:14136939-14137010 (-)
-GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCCGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-2-11 (tRNAscan-SE ID: chrX.trna159) His (GTG) 72 bp Sc: 69.4 chrX:16634830-16634901 (-)
-GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCCGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-2-2 (tRNAscan-SE ID: chrIV.trna37) His (GTG) 72 bp Sc: 69.4 chrIV:16388456-16388527 (+)
-GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCCGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-2-3 (tRNAscan-SE ID: chrIV.trna41) His (GTG) 72 bp Sc: 69.4 chrIV:16400896-16400967 (+)
-GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCCGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-2-4 (tRNAscan-SE ID: chrX.trna213) His (GTG) 72 bp Sc: 69.4 chrX:11993521-11993592 (-)
-GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCCGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-2-5 (tRNAscan-SE ID: chrX.trna123) His (GTG) 72 bp Sc: 69.4 chrX:14135045-14135116 (+)
-GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCCGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-2-6 (tRNAscan-SE ID: chrX.trna190) His (GTG) 72 bp Sc: 69.4 chrX:14135308-14135379 (-)
-GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCCGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-2-7 (tRNAscan-SE ID: chrX.trna124) His (GTG) 72 bp Sc: 69.4 chrX:14135874-14135945 (+)
-GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCCGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-2-8 (tRNAscan-SE ID: chrX.trna189) His (GTG) 72 bp Sc: 69.4 chrX:14136124-14136195 (-)
-GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCCGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-2-9 (tRNAscan-SE ID: chrX.trna125) His (GTG) 72 bp Sc: 69.4 chrX:14136690-14136761 (+)
-GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCCGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-3-1 (tRNAscan-SE ID: chrIV.trna57) His (GTG) 72 bp Sc: 67.8 chrIV:14889022-14889093 (-)
-GCCTGCTTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCAGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-3-2 (tRNAscan-SE ID: chrIV.trna56) His (GTG) 72 bp Sc: 67.8 chrIV:15187654-15187725 (-)
-GCCTGCTTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCAGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-3-3 (tRNAscan-SE ID: chrV.trna24) His (GTG) 72 bp Sc: 67.8 chrV:15554030-15554101 (+)
-GCCTGCTTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCAGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-3-4 (tRNAscan-SE ID: chrX.trna284) His (GTG) 72 bp Sc: 67.8 chrX:5022817-5022888 (-)
-GCCTGCTTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTC
-CAGCAGCAGGCA
->Caenorhabditis_elegans_tRNA-His-GTG-4-1 (tRNAscan-SE ID: chrIV.trna30) His (GTG) 72 bp Sc: 62.0 chrIV:15187344-15187415 (+)
-GCCTGCTTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTAGATTC
-CAGCAGCAGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-1 (tRNAscan-SE ID: chrI.trna67) Ile (AAT) 74 bp Sc: 86.9 chrI:6163471-6163544 (-)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-10 (tRNAscan-SE ID: chrIII.trna79) Ile (AAT) 74 bp Sc: 86.9 chrIII:1218376-1218449 (-)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-11 (tRNAscan-SE ID: chrX.trna300) Ile (AAT) 74 bp Sc: 86.9 chrX:1589667-1589740 (-)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-12 (tRNAscan-SE ID: chrX.trna299) Ile (AAT) 74 bp Sc: 86.9 chrX:1590080-1590153 (-)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-13 (tRNAscan-SE ID: chrX.trna298) Ile (AAT) 74 bp Sc: 86.9 chrX:1590508-1590581 (-)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-14 (tRNAscan-SE ID: chrX.trna289) Ile (AAT) 74 bp Sc: 86.9 chrX:2526218-2526291 (-)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-15 (tRNAscan-SE ID: chrX.trna283) Ile (AAT) 74 bp Sc: 86.9 chrX:5085622-5085695 (-)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-16 (tRNAscan-SE ID: chrX.trna264) Ile (AAT) 74 bp Sc: 86.9 chrX:8156634-8156707 (-)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-17 (tRNAscan-SE ID: chrX.trna199) Ile (AAT) 74 bp Sc: 86.9 chrX:13415120-13415193 (-)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-18 (tRNAscan-SE ID: chrX.trna106) Ile (AAT) 74 bp Sc: 86.9 chrX:13435966-13436039 (+)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-19 (tRNAscan-SE ID: chrX.trna128) Ile (AAT) 74 bp Sc: 86.9 chrX:14679160-14679233 (+)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-2 (tRNAscan-SE ID: chrI.trna7) Ile (AAT) 74 bp Sc: 86.9 chrI:6164191-6164264 (+)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-20 (tRNAscan-SE ID: chrX.trna133) Ile (AAT) 74 bp Sc: 86.9 chrX:15297471-15297544 (+)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-3 (tRNAscan-SE ID: chrII.trna7) Ile (AAT) 74 bp Sc: 86.9 chrII:5032770-5032843 (+)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-4 (tRNAscan-SE ID: chrII.trna51) Ile (AAT) 74 bp Sc: 86.9 chrII:5057447-5057520 (-)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-5 (tRNAscan-SE ID: chrII.trna8) Ile (AAT) 74 bp Sc: 86.9 chrII:5237862-5237935 (+)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-6 (tRNAscan-SE ID: chrII.trna25) Ile (AAT) 74 bp Sc: 86.9 chrII:12362449-12362522 (+)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-7 (tRNAscan-SE ID: chrII.trna26) Ile (AAT) 74 bp Sc: 86.9 chrII:12494741-12494814 (+)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-8 (tRNAscan-SE ID: chrIII.trna81) Ile (AAT) 74 bp Sc: 86.9 chrIII:1163354-1163427 (-)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-1-9 (tRNAscan-SE ID: chrIII.trna80) Ile (AAT) 74 bp Sc: 86.9 chrIII:1164800-1164873 (-)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-AAT-2-1 (tRNAscan-SE ID: chrX.trna19) Ile (AAT) 74 bp Sc: 80.0 chrX:2531361-2531434 (+)
-GCCGCCATAGCCCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGAC
-CCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Ile-TAT-1-1 (tRNAscan-SE ID: chrI.trna10) Ile (TAT) 85 bp Sc: 84.7 chrI:7960837-7960921 (+)
-GCCCCGGTGGCCGAGCGGTCGAAGGCGTGAGACTTATGATCTCATTGGGTTAAACCAGTC
-GCGGGTTCGAATCCCGCCCGGGGCA
->Caenorhabditis_elegans_tRNA-Ile-TAT-1-2 (tRNAscan-SE ID: chrI.trna18) Ile (TAT) 85 bp Sc: 84.7 chrI:9562353-9562437 (+)
-GCCCCGGTGGCCGAGCGGTCGAAGGCGTGAGACTTATGATCTCATTGGGTTAAACCAGTC
-GCGGGTTCGAATCCCGCCCGGGGCA
->Caenorhabditis_elegans_tRNA-Ile-TAT-1-3 (tRNAscan-SE ID: chrI.trna57) Ile (TAT) 85 bp Sc: 84.7 chrI:9563843-9563927 (-)
-GCCCCGGTGGCCGAGCGGTCGAAGGCGTGAGACTTATGATCTCATTGGGTTAAACCAGTC
-GCGGGTTCGAATCCCGCCCGGGGCA
->Caenorhabditis_elegans_tRNA-Ile-TAT-1-4 (tRNAscan-SE ID: chrX.trna227) Ile (TAT) 85 bp Sc: 84.7 chrX:9829667-9829751 (-)
-GCCCCGGTGGCCGAGCGGTCGAAGGCGTGAGACTTATGATCTCATTGGGTTAAACCAGTC
-GCGGGTTCGAATCCCGCCCGGGGCA
->Caenorhabditis_elegans_tRNA-Ile-TAT-2-1 (tRNAscan-SE ID: chrV.trna9) Ile (TAT) 85 bp Sc: 76.7 chrV:6917466-6917550 (+)
-GCCCCATTGGCGCAGTCGGTTAGCGCGTGGTACTTATAGTTAATAGGGAATGCCAAGGTC
-GCCAGTTCGAGCCTGGCATGGGGCA
->Caenorhabditis_elegans_tRNA-Ile-TAT-2-2 (tRNAscan-SE ID: chrV.trna15) Ile (TAT) 85 bp Sc: 76.7 chrV:12002176-12002260 (+)
-GCCCCATTGGCGCAGTCGGTTAGCGCGTGGTACTTATAGTCTATAGGTTATGCCAAGGTC
-GCCAGTTCGAGCCTGGCATGGGGCA
->Caenorhabditis_elegans_tRNA-Ile-TAT-2-3 (tRNAscan-SE ID: chrX.trna94) Ile (TAT) 84 bp Sc: 76.7 chrX:12661164-12661247 (+)
-GCCCCATTGGCGCAGTCGGTTAGCGCGTGGTACTTATAGTTATAGGTCATGCCAAGGTCG
-CCAGTTCGAGCCTGGCATGGGGCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-1-1 (tRNAscan-SE ID: chrII.trna31) Leu (AAG) 82 bp Sc: 73.6 chrII:14635335-14635416 (-)
-GGTGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCATCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-2-1 (tRNAscan-SE ID: chrI.trna68) Leu (AAG) 82 bp Sc: 72.6 chrI:6051155-6051236 (-)
-GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-2-2 (tRNAscan-SE ID: chrI.trna49) Leu (AAG) 82 bp Sc: 72.6 chrI:11585370-11585451 (-)
-GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-2-3 (tRNAscan-SE ID: chrII.trna64) Leu (AAG) 82 bp Sc: 72.6 chrII:2735794-2735875 (-)
-GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-2-4 (tRNAscan-SE ID: chrII.trna63) Leu (AAG) 82 bp Sc: 72.6 chrII:2736276-2736357 (-)
-GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-2-5 (tRNAscan-SE ID: chrII.trna3) Leu (AAG) 82 bp Sc: 72.6 chrII:2860342-2860423 (+)
-GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-2-6 (tRNAscan-SE ID: chrII.trna62) Leu (AAG) 82 bp Sc: 72.6 chrII:2861550-2861631 (-)
-GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-2-7 (tRNAscan-SE ID: chrII.trna34) Leu (AAG) 82 bp Sc: 72.6 chrII:12541930-12542011 (-)
-GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-3-1 (tRNAscan-SE ID: chrX.trna306) Leu (AAG) 82 bp Sc: 72.6 chrX:353255-353336 (-)
-GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-3-2 (tRNAscan-SE ID: chrX.trna274) Leu (AAG) 82 bp Sc: 72.6 chrX:6903114-6903195 (-)
-GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-3-3 (tRNAscan-SE ID: chrX.trna261) Leu (AAG) 82 bp Sc: 72.6 chrX:8417912-8417993 (-)
-GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-3-4 (tRNAscan-SE ID: chrX.trna260) Leu (AAG) 82 bp Sc: 72.6 chrX:8419414-8419495 (-)
-GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-3-5 (tRNAscan-SE ID: chrX.trna74) Leu (AAG) 82 bp Sc: 72.6 chrX:8939550-8939631 (+)
-GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-3-6 (tRNAscan-SE ID: chrX.trna242) Leu (AAG) 82 bp Sc: 72.6 chrX:8955920-8956001 (-)
-GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-3-7 (tRNAscan-SE ID: chrX.trna220) Leu (AAG) 82 bp Sc: 72.6 chrX:11162919-11163000 (-)
-GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-3-8 (tRNAscan-SE ID: chrX.trna219) Leu (AAG) 82 bp Sc: 72.6 chrX:11163358-11163439 (-)
-GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-AAG-3-9 (tRNAscan-SE ID: chrX.trna100) Leu (AAG) 82 bp Sc: 72.6 chrX:12942458-12942539 (+)
-GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTG
-GGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-CAA-1-1 (tRNAscan-SE ID: chrIII.trna15) Leu (CAA) 120 bp Sc: 74.2 chrIII:4362524-4362643 (+)
-GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCGTAACGCTTACCTCAAGTTCG
-AGGTCTACTGGGTGTTCTGGTACTCGTATGGGTGCGTGGGTTCGAATCCCACTTCGTGCA
->Caenorhabditis_elegans_tRNA-Leu-CAA-1-2 (tRNAscan-SE ID: chrIII.trna27) Leu (CAA) 122 bp Sc: 74.1 chrIII:8109603-8109724 (+)
-GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCGTACATTGCTTGCCTCAAGTT
-CGAGGTTAACTGGGTGTTCTGGTACTCGTATGGGTGCGTGGGTTCGAATCCCACTTCGTG
-CA
->Caenorhabditis_elegans_tRNA-Leu-CAA-1-3 (tRNAscan-SE ID: chrIII.trna29) Leu (CAA) 120 bp Sc: 74.2 chrIII:8639306-8639425 (+)
-GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCGAAATGCTTGCCTCATGCTCG
-AGGTCGACTGGGTGTTCTGGTACTCGTATGGGTGCGTGGGTTCGAATCCCACTTCGTGCA
->Caenorhabditis_elegans_tRNA-Leu-CAA-1-4 (tRNAscan-SE ID: chrIV.trna66) Leu (CAA) 119 bp Sc: 74.2 chrIV:11928478-11928596 (-)
-GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCAATTGCTTGCCTCGAGTTCGA
-GGTCGACTGGGTGTTCTGGTACTCGTATGGGTGCGTGGGTTCGAATCCCACTTCGTGCA
->Caenorhabditis_elegans_tRNA-Leu-CAA-1-5 (tRNAscan-SE ID: chrX.trna210) Leu (CAA) 120 bp Sc: 74.2 chrX:12348007-12348126 (-)
-GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCGAATCGCTTGCCTCAAGTTCG
-AGGTCAACTGGGTGTTCTGGTACTCGTATGGGTGCGTGGGTTCGAATCCCACTTCGTGCA
->Caenorhabditis_elegans_tRNA-Leu-CAA-1-6 (tRNAscan-SE ID: chrX.trna110) Leu (CAA) 119 bp Sc: 74.2 chrX:13665555-13665673 (+)
-GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCGATTGCTTGCCTCAAGTACGA
-GGTCTCCTGGGTGTTCTGGTACTCGTATGGGTGCGTGGGTTCGAATCCCACTTCGTGCA
->Caenorhabditis_elegans_tRNA-Leu-CAA-2-1 (tRNAscan-SE ID: chrX.trna198) Leu (CAA) 119 bp Sc: 72.2 chrX:13443386-13443504 (-)
-GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCAATAGCTTGCTTCAAGTTCGA
-AGCCGATTGGGCGTTCTGGTACTCGTACGGGTGCGTGGGTTCGAATCCCACTTCGTGCA
->Caenorhabditis_elegans_tRNA-Leu-CAG-1-1 (tRNAscan-SE ID: chrIV.trna21) Leu (CAG) 84 bp Sc: 77.8 chrIV:6556818-6556901 (+)
-GCCGTTCTGGCCGAGTGGTCTAAGGCGCTGCGTTCAGGTCGCAGTCCTCTCAGGAGGGCG
-CAGGTTCGAACCCTGCGGACGGCA
->Caenorhabditis_elegans_tRNA-Leu-CAG-1-2 (tRNAscan-SE ID: chrX.trna135) Leu (CAG) 84 bp Sc: 77.8 chrX:15742050-15742133 (+)
-GCCGTTCTGGCCGAGTGGTCTAAGGCGCTGCGTTCAGGTCGCAGTCCTCTCAGGAGGGCG
-CAGGTTCGAACCCTGCGGACGGCA
->Caenorhabditis_elegans_tRNA-Leu-CAG-2-1 (tRNAscan-SE ID: chrI.trna2) Leu (CAG) 84 bp Sc: 76.8 chrI:754680-754763 (+)
-GCCGTTCTGGCCGAGTGGTCTAAGGCGCTGCGTTCAGGTCGCAGTCCTCTCCGGAGGGCG
-CAGGTTCGAATCCTGCGGACGGCA
->Caenorhabditis_elegans_tRNA-Leu-CAG-2-2 (tRNAscan-SE ID: chrV.trna95) Leu (CAG) 84 bp Sc: 76.8 chrV:11174790-11174873 (-)
-GCCGTTCTGGCCGAGTGGTCTAAGGCGCTGCGTTCAGGTCGCAGTCCTCTCCGGAGGGCG
-CAGGTTCGAATCCTGCGGACGGCA
->Caenorhabditis_elegans_tRNA-Leu-CAG-2-3 (tRNAscan-SE ID: chrX.trna205) Leu (CAG) 84 bp Sc: 76.8 chrX:13038960-13039043 (-)
-GCCGTTCTGGCCGAGTGGTCTAAGGCGCTGCGTTCAGGTCGCAGTCCTCTCCGGAGGGCG
-CAGGTTCGAATCCTGCGGACGGCA
->Caenorhabditis_elegans_tRNA-Leu-TAA-1-1 (tRNAscan-SE ID: chrII.trna49) Leu (TAA) 84 bp Sc: 77.4 chrII:5772916-5772999 (-)
-AGCACGATGGCCGAGTGGTTAAGGCGTTGGACTTAAGTTCCAATGGTGGATAACACCTCG
-TGGGTTCGAACCCCACTCGTGCTA
->Caenorhabditis_elegans_tRNA-Leu-TAA-1-2 (tRNAscan-SE ID: chrX.trna217) Leu (TAA) 84 bp Sc: 77.4 chrX:11757831-11757914 (-)
-AGCACGATGGCCGAGTGGTTAAGGCGTTGGACTTAAGTTCCAATGGTGGATAACACCTCG
-TGGGTTCGAACCCCACTCGTGCTA
->Caenorhabditis_elegans_tRNA-Leu-TAA-2-1 (tRNAscan-SE ID: chrII.trna45) Leu (TAA) 84 bp Sc: 70.5 chrII:8631957-8632040 (-)
-AGCACGATGGCCGAGTGGTTAAGGCGTTGGCCTTAAGTTCCAATGGTGGATAACACCGCG
-TGGGTTCGAACCCCACTCGTGCTA
->Caenorhabditis_elegans_tRNA-Leu-TAA-3-1 (tRNAscan-SE ID: chrII.trna12) Leu (AAG) 83 bp Sc: 65.0 chrII:6721766-6721848 (+)
-GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCAACCAGTAGCTTCGGGGGCGT
-GGGTTCGAATCCCACTCTCTTCA
->Caenorhabditis_elegans_tRNA-Leu-TAG-1-1 (tRNAscan-SE ID: chrII.trna13) Leu (TAG) 82 bp Sc: 75.3 chrII:6853204-6853285 (+)
-GGTGAGATGGCCGAGTGGTCTAAGGCGCTGGTTTTAGGCACCAGTCCCTCCGGGGGCGTG
-GGTTCGAATCCCACTCTCATCA
->Caenorhabditis_elegans_tRNA-Leu-TAG-1-2 (tRNAscan-SE ID: chrV.trna100) Leu (TAG) 82 bp Sc: 75.3 chrV:8235458-8235539 (-)
-GGTGAGATGGCCGAGTGGTCTAAGGCGCTGGTTTTAGGCACCAGTCCCTCCGGGGGCGTG
-GGTTCGAATCCCACTCTCATCA
->Caenorhabditis_elegans_tRNA-Leu-TAG-1-3 (tRNAscan-SE ID: chrX.trna88) Leu (TAG) 82 bp Sc: 75.3 chrX:11095673-11095754 (+)
-GGTGAGATGGCCGAGTGGTCTAAGGCGCTGGTTTTAGGCACCAGTCCCTCCGGGGGCGTG
-GGTTCGAATCCCACTCTCATCA
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-1 (tRNAscan-SE ID: chrI.trna6) Lys (CTT) 73 bp Sc: 85.9 chrI:6136597-6136669 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-10 (tRNAscan-SE ID: chrIII.trna14) Lys (CTT) 73 bp Sc: 85.9 chrIII:3389537-3389609 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-11 (tRNAscan-SE ID: chrIII.trna72) Lys (CTT) 73 bp Sc: 85.9 chrIII:3426913-3426985 (-)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-12 (tRNAscan-SE ID: chrIII.trna28) Lys (CTT) 73 bp Sc: 85.9 chrIII:8473473-8473545 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-13 (tRNAscan-SE ID: chrIV.trna18) Lys (CTT) 73 bp Sc: 85.9 chrIV:5967160-5967232 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-14 (tRNAscan-SE ID: chrIV.trna26) Lys (CTT) 73 bp Sc: 85.9 chrIV:12594740-12594812 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-15 (tRNAscan-SE ID: chrIV.trna34) Lys (CTT) 73 bp Sc: 85.9 chrIV:15793415-15793487 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-16 (tRNAscan-SE ID: chrX.trna212) Lys (CTT) 73 bp Sc: 85.9 chrX:12106147-12106219 (-)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-17 (tRNAscan-SE ID: chrX.trna195) Lys (CTT) 73 bp Sc: 85.9 chrX:13655917-13655989 (-)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-18 (tRNAscan-SE ID: chrX.trna111) Lys (CTT) 73 bp Sc: 85.9 chrX:13714888-13714960 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-19 (tRNAscan-SE ID: chrX.trna113) Lys (CTT) 73 bp Sc: 85.9 chrX:13717195-13717267 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-2 (tRNAscan-SE ID: chrI.trna51) Lys (CTT) 73 bp Sc: 85.9 chrI:11579706-11579778 (-)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-20 (tRNAscan-SE ID: chrX.trna115) Lys (CTT) 73 bp Sc: 85.9 chrX:13730357-13730429 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-21 (tRNAscan-SE ID: chrX.trna116) Lys (CTT) 73 bp Sc: 85.9 chrX:13730778-13730850 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-22 (tRNAscan-SE ID: chrX.trna117) Lys (CTT) 73 bp Sc: 85.9 chrX:13781640-13781712 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-23 (tRNAscan-SE ID: chrX.trna118) Lys (CTT) 73 bp Sc: 85.9 chrX:13782249-13782321 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-24 (tRNAscan-SE ID: chrX.trna184) Lys (CTT) 73 bp Sc: 85.9 chrX:14478877-14478949 (-)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-25 (tRNAscan-SE ID: chrX.trna180) Lys (CTT) 73 bp Sc: 85.9 chrX:15241355-15241427 (-)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-3 (tRNAscan-SE ID: chrI.trna50) Lys (CTT) 73 bp Sc: 85.9 chrI:11584122-11584194 (-)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-4 (tRNAscan-SE ID: chrI.trna30) Lys (CTT) 73 bp Sc: 85.9 chrI:11584787-11584859 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-5 (tRNAscan-SE ID: chrI.trna44) Lys (CTT) 73 bp Sc: 85.9 chrI:13297673-13297745 (-)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-6 (tRNAscan-SE ID: chrII.trna59) Lys (CTT) 73 bp Sc: 85.9 chrII:3439394-3439466 (-)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-7 (tRNAscan-SE ID: chrII.trna57) Lys (CTT) 73 bp Sc: 85.9 chrII:3519250-3519322 (-)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-8 (tRNAscan-SE ID: chrII.trna54) Lys (CTT) 73 bp Sc: 85.9 chrII:3567764-3567836 (-)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-1-9 (tRNAscan-SE ID: chrII.trna40) Lys (CTT) 73 bp Sc: 85.9 chrII:11157802-11157874 (-)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-2-1 (tRNAscan-SE ID: chrI.trna66) Lys (CTT) 73 bp Sc: 83.5 chrI:7279355-7279427 (-)
-GCCCGGTTAGCTCAGCCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-3-1 (tRNAscan-SE ID: chrX.trna114) Lys (CTT) 73 bp Sc: 79.6 chrX:13729905-13729977 (+)
-GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTCTCGCGGGTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-4-1 (tRNAscan-SE ID: chrIII.trna61) Lys (CTT) 86 bp Sc: 72.1 chrIII:6724135-6724220 (-)
-GACACGGTGGCCGAGTGGTTTAAGGCATGAGACACTTGATCTCAAACGGTTCTAACCGAA
-CGCAGGTTCGAATCCTGCCCGTGTCA
->Caenorhabditis_elegans_tRNA-Lys-CTT-5-1 (tRNAscan-SE ID: chrX.trna112) Lys (CTT) 73 bp Sc: 75.4 chrX:13716493-13716565 (+)
-GCCTGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGTTTCGAGC
-CCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-CTT-7-1 (tRNAscan-SE ID: chrX.trna194) Lys (CTT) 89 bp Sc: 71.5 chrX:13713639-13713727 (-)
-GCCCGGTTAGCTCAGTCGCGAGTCGCGAGTCGCGGTAGAGCACCAGATTCTTAATCTGGT
-TGTCGCGGGTTCGAGCCCCGCATTGGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-1 (tRNAscan-SE ID: chrII.trna11) Lys (TTT) 73 bp Sc: 77.8 chrII:6565248-6565320 (+)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-10 (tRNAscan-SE ID: chrX.trna33) Lys (TTT) 73 bp Sc: 77.8 chrX:4789132-4789204 (+)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-11 (tRNAscan-SE ID: chrX.trna279) Lys (TTT) 73 bp Sc: 77.8 chrX:5451204-5451276 (-)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-12 (tRNAscan-SE ID: chrX.trna40) Lys (TTT) 73 bp Sc: 77.8 chrX:5713652-5713724 (+)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-13 (tRNAscan-SE ID: chrX.trna191) Lys (TTT) 73 bp Sc: 77.8 chrX:14063946-14064018 (-)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-14 (tRNAscan-SE ID: chrX.trna169) Lys (TTT) 73 bp Sc: 77.8 chrX:16217895-16217967 (-)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-2 (tRNAscan-SE ID: chrII.trna35) Lys (TTT) 73 bp Sc: 77.8 chrII:12541688-12541760 (-)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-3 (tRNAscan-SE ID: chrIII.trna59) Lys (TTT) 73 bp Sc: 77.8 chrIII:6887728-6887800 (-)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-4 (tRNAscan-SE ID: chrIV.trna15) Lys (TTT) 73 bp Sc: 77.8 chrIV:5038920-5038992 (+)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-5 (tRNAscan-SE ID: chrV.trna12) Lys (TTT) 73 bp Sc: 77.8 chrV:8495302-8495374 (+)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-6 (tRNAscan-SE ID: chrV.trna98) Lys (TTT) 73 bp Sc: 77.8 chrV:8499564-8499636 (-)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-7 (tRNAscan-SE ID: chrV.trna88) Lys (TTT) 73 bp Sc: 77.8 chrV:13027028-13027100 (-)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-8 (tRNAscan-SE ID: chrV.trna20) Lys (TTT) 73 bp Sc: 77.8 chrV:15465086-15465158 (+)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Lys-TTT-1-9 (tRNAscan-SE ID: chrV.trna73) Lys (TTT) 73 bp Sc: 77.8 chrV:16622059-16622131 (-)
-GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGT
-CCCCTAGGTGGCT
->Caenorhabditis_elegans_tRNA-Met-CAT-1-1 (tRNAscan-SE ID: chrI.trna71) Met (CAT) 73 bp Sc: 77.0 chrI:3638852-3638924 (-)
-GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGC
-CTCACCGGGAGCA
->Caenorhabditis_elegans_tRNA-Met-CAT-1-2 (tRNAscan-SE ID: chrIII.trna26) Met (CAT) 73 bp Sc: 77.0 chrIII:8106653-8106725 (+)
-GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGC
-CTCACCGGGAGCA
->Caenorhabditis_elegans_tRNA-Met-CAT-1-3 (tRNAscan-SE ID: chrV.trna110) Met (CAT) 73 bp Sc: 77.0 chrV:3455326-3455398 (-)
-GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGC
-CTCACCGGGAGCA
->Caenorhabditis_elegans_tRNA-Met-CAT-1-4 (tRNAscan-SE ID: chrV.trna101) Met (CAT) 73 bp Sc: 77.0 chrV:8230206-8230278 (-)
-GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGC
-CTCACCGGGAGCA
->Caenorhabditis_elegans_tRNA-Met-CAT-1-5 (tRNAscan-SE ID: chrX.trna23) Met (CAT) 73 bp Sc: 77.0 chrX:3697756-3697828 (+)
-GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGC
-CTCACCGGGAGCA
->Caenorhabditis_elegans_tRNA-Met-CAT-1-6 (tRNAscan-SE ID: chrX.trna280) Met (CAT) 73 bp Sc: 77.0 chrX:5407413-5407485 (-)
-GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGC
-CTCACCGGGAGCA
->Caenorhabditis_elegans_tRNA-Met-CAT-1-7 (tRNAscan-SE ID: chrX.trna35) Met (CAT) 73 bp Sc: 77.0 chrX:5485112-5485184 (+)
-GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGC
-CTCACCGGGAGCA
->Caenorhabditis_elegans_tRNA-Met-CAT-1-8 (tRNAscan-SE ID: chrX.trna36) Met (CAT) 73 bp Sc: 77.0 chrX:5485455-5485527 (+)
-GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGC
-CTCACCGGGAGCA
->Caenorhabditis_elegans_tRNA-Met-CAT-1-9 (tRNAscan-SE ID: chrX.trna37) Met (CAT) 73 bp Sc: 77.0 chrX:5485746-5485818 (+)
-GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGC
-CTCACCGGGAGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-1-1 (tRNAscan-SE ID: chrII.trna43) Phe (GAA) 73 bp Sc: 82.3 chrII:9713224-9713296 (-)
-GCCTCGATAGCTCAGTTGGGAGAGCGCACGACTGAAGATCGTGAGGTCACCAGTTCGATC
-CTGGTTCGGGGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-2-1 (tRNAscan-SE ID: chrIII.trna55) Phe (GAA) 73 bp Sc: 82.5 chrIII:7978471-7978543 (-)
-GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATC
-CTGGTTCGGGGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-2-2 (tRNAscan-SE ID: chrIII.trna31) Phe (GAA) 73 bp Sc: 82.5 chrIII:8653055-8653127 (+)
-GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATC
-CTGGTTCGGGGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-2-3 (tRNAscan-SE ID: chrIII.trna53) Phe (GAA) 73 bp Sc: 82.5 chrIII:8653608-8653680 (-)
-GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATC
-CTGGTTCGGGGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-2-4 (tRNAscan-SE ID: chrIII.trna36) Phe (GAA) 73 bp Sc: 82.5 chrIII:11554825-11554897 (+)
-GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATC
-CTGGTTCGGGGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-2-5 (tRNAscan-SE ID: chrV.trna85) Phe (GAA) 73 bp Sc: 82.5 chrV:14876389-14876461 (-)
-GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATC
-CTGGTTCGGGGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-3-1 (tRNAscan-SE ID: chrV.trna38) Phe (GAA) 73 bp Sc: 82.3 chrV:19126044-19126116 (+)
-GCCTCGATAGCTCAGTTGGGAGAGCGCACGACTGAAGATCGTGAGGTCACCAGTTCGATC
-CTGGTTCGGGGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-4-1 (tRNAscan-SE ID: chrX.trna44) Phe (GAA) 73 bp Sc: 82.5 chrX:6593596-6593668 (+)
-GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATC
-CTGGTTCGGGGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-4-2 (tRNAscan-SE ID: chrX.trna165) Phe (GAA) 73 bp Sc: 82.5 chrX:16503144-16503216 (-)
-GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATC
-CTGGTTCGGGGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-4-3 (tRNAscan-SE ID: chrX.trna150) Phe (GAA) 73 bp Sc: 82.5 chrX:16523344-16523416 (+)
-GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATC
-CTGGTTCGGGGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-4-4 (tRNAscan-SE ID: chrX.trna151) Phe (GAA) 73 bp Sc: 82.5 chrX:16523923-16523995 (+)
-GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATC
-CTGGTTCGGGGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-4-5 (tRNAscan-SE ID: chrX.trna152) Phe (GAA) 73 bp Sc: 82.5 chrX:16551511-16551583 (+)
-GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATC
-CTGGTTCGGGGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-5-1 (tRNAscan-SE ID: chrX.trna281) Phe (GAA) 73 bp Sc: 81.2 chrX:5319385-5319457 (-)
-GCCTCAATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATC
-CTGGTTTGGGGCA
->Caenorhabditis_elegans_tRNA-Phe-GAA-6-1 (tRNAscan-SE ID: chrI.trna27) Phe (GAA) 82 bp Sc: 56.6 chrI:10945821-10945902 (+)
-GCCTCGATAGCTCAGTTGGGGTGAGCGTACGACTGAAAATCGTTAGGTCACCAGTTCGAT
-CCTGGTTCGGGCATTCGGTGCT
->Caenorhabditis_elegans_tRNA-Pro-AGG-1-1 (tRNAscan-SE ID: chrX.trna25) Pro (AGG) 72 bp Sc: 72.1 chrX:3970096-3970167 (+)
-GGCCGGATGGTCTAGTGGTATGATTCTCGCTTAGGGTGCGAGAGGTCCCGGGATCGATCC
-CCGGTCCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-AGG-2-1 (tRNAscan-SE ID: chrX.trna26) Pro (AGG) 72 bp Sc: 71.1 chrX:3970265-3970336 (+)
-GGCCGGATGGTCTAGTGGTATGATTCTCGCTTAGGGTGCGAGAGGTCCCGGGATCGATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-AGG-3-1 (tRNAscan-SE ID: chrX.trna52) Pro (AGG) 72 bp Sc: 71.4 chrX:8037507-8037578 (+)
-GGTCGGATGGCCTAGAGGTAAGGCGCTTGCTTAGGGTGCAAGAGATCCCGGGTTCGATCC
-CCGGTTCGACCC
->Caenorhabditis_elegans_tRNA-Pro-AGG-4-1 (tRNAscan-SE ID: chrI.trna69) Pro (AGG) 72 bp Sc: 70.1 chrI:5854794-5854865 (-)
-GGCTGAGTGGTCTAGTGGTATGATTCTCGCTTAGGGTGCGAGAGGTCCCGGGATCGATCC
-CCGGCTCAGCCC
->Caenorhabditis_elegans_tRNA-Pro-AGG-4-2 (tRNAscan-SE ID: chrI.trna61) Pro (AGG) 72 bp Sc: 70.1 chrI:9268928-9268999 (-)
-GGCTGAGTGGTCTAGTGGTATGATTCTCGCTTAGGGTGCGAGAGGTCCCGGGATCGATCC
-CCGGCTCAGCCC
->Caenorhabditis_elegans_tRNA-Pro-AGG-4-3 (tRNAscan-SE ID: chrIV.trna24) Pro (AGG) 72 bp Sc: 70.1 chrIV:11231565-11231636 (+)
-GGCTGAGTGGTCTAGTGGTATGATTCTCGCTTAGGGTGCGAGAGGTCCCGGGATCGATCC
-CCGGCTCAGCCC
->Caenorhabditis_elegans_tRNA-Pro-AGG-5-1 (tRNAscan-SE ID: chrX.trna238) Pro (AGG) 115 bp Sc: 68.5 chrX:9059280-9059394 (-)
-GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGCCAAGGCCCAAGGTCGCCCAAGGCCCAAG
-GTCGCCCAAGGCCAAGGTAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
->Caenorhabditis_elegans_tRNA-Pro-CGG-1-1 (tRNAscan-SE ID: chrIII.trna54) Pro (CGG) 72 bp Sc: 71.5 chrIII:8650381-8650452 (-)
-GGCCGGATGGTCTAGAGGTATGATTCTCGCTTCGGGTGCGAGAGGTCCCGGGTTCGATTC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-CGG-1-2 (tRNAscan-SE ID: chrIV.trna75) Pro (CGG) 72 bp Sc: 71.5 chrIV:3552189-3552260 (-)
-GGCCGGATGGTCTAGAGGTATGATTCTCGCTTCGGGTGCGAGAGGTCCCGGGTTCGATTC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-CGG-1-3 (tRNAscan-SE ID: chrIV.trna65) Pro (CGG) 72 bp Sc: 71.5 chrIV:12005598-12005669 (-)
-GGCCGGATGGTCTAGAGGTATGATTCTCGCTTCGGGTGCGAGAGGTCCCGGGTTCGATTC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-CGG-1-4 (tRNAscan-SE ID: chrX.trna294) Pro (CGG) 72 bp Sc: 71.5 chrX:1880817-1880888 (-)
-GGCCGGATGGTCTAGAGGTATGATTCTCGCTTCGGGTGCGAGAGGTCCCGGGTTCGATTC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-1 (tRNAscan-SE ID: chrII.trna20) Pro (TGG) 72 bp Sc: 75.2 chrII:10302399-10302470 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-10 (tRNAscan-SE ID: chrV.trna16) Pro (TGG) 72 bp Sc: 75.2 chrV:13509693-13509764 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-11 (tRNAscan-SE ID: chrV.trna83) Pro (TGG) 72 bp Sc: 75.2 chrV:15465225-15465296 (-)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-12 (tRNAscan-SE ID: chrX.trna24) Pro (TGG) 72 bp Sc: 75.2 chrX:3969556-3969627 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-13 (tRNAscan-SE ID: chrX.trna278) Pro (TGG) 72 bp Sc: 75.2 chrX:5801211-5801282 (-)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-14 (tRNAscan-SE ID: chrX.trna41) Pro (TGG) 72 bp Sc: 75.2 chrX:5801472-5801543 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-15 (tRNAscan-SE ID: chrX.trna241) Pro (TGG) 72 bp Sc: 75.2 chrX:8969488-8969559 (-)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-16 (tRNAscan-SE ID: chrX.trna75) Pro (TGG) 72 bp Sc: 75.2 chrX:8969738-8969809 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-17 (tRNAscan-SE ID: chrX.trna231) Pro (TGG) 72 bp Sc: 75.2 chrX:9467729-9467800 (-)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-18 (tRNAscan-SE ID: chrX.trna105) Pro (TGG) 72 bp Sc: 75.2 chrX:13308030-13308101 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-19 (tRNAscan-SE ID: chrX.trna196) Pro (TGG) 72 bp Sc: 75.2 chrX:13511970-13512041 (-)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-2 (tRNAscan-SE ID: chrII.trna21) Pro (TGG) 72 bp Sc: 75.2 chrII:10305011-10305082 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-20 (tRNAscan-SE ID: chrX.trna185) Pro (TGG) 72 bp Sc: 75.2 chrX:14437873-14437944 (-)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-21 (tRNAscan-SE ID: chrX.trna127) Pro (TGG) 72 bp Sc: 75.2 chrX:14438102-14438173 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-22 (tRNAscan-SE ID: chrX.trna137) Pro (TGG) 72 bp Sc: 75.2 chrX:15751420-15751491 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-23 (tRNAscan-SE ID: chrX.trna175) Pro (TGG) 72 bp Sc: 75.2 chrX:15796623-15796694 (-)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-24 (tRNAscan-SE ID: chrX.trna139) Pro (TGG) 72 bp Sc: 75.2 chrX:15796855-15796926 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-3 (tRNAscan-SE ID: chrIII.trna9) Pro (TGG) 72 bp Sc: 75.2 chrIII:2711711-2711782 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-4 (tRNAscan-SE ID: chrIII.trna46) Pro (TGG) 72 bp Sc: 75.2 chrIII:11066848-11066919 (-)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-5 (tRNAscan-SE ID: chrIII.trna32) Pro (TGG) 72 bp Sc: 75.2 chrIII:11067027-11067098 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-6 (tRNAscan-SE ID: chrIV.trna29) Pro (TGG) 72 bp Sc: 75.2 chrIV:14225102-14225173 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-7 (tRNAscan-SE ID: chrV.trna3) Pro (TGG) 72 bp Sc: 75.2 chrV:3582320-3582391 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-8 (tRNAscan-SE ID: chrV.trna4) Pro (TGG) 72 bp Sc: 75.2 chrV:3588503-3588574 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-1-9 (tRNAscan-SE ID: chrV.trna87) Pro (TGG) 72 bp Sc: 75.2 chrV:13507203-13507274 (-)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-2-1 (tRNAscan-SE ID: chrII.trna42) Pro (TGG) 72 bp Sc: 69.2 chrII:10302159-10302230 (-)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGCTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-3-1 (tRNAscan-SE ID: chrX.trna207) Pro (TGG) 72 bp Sc: 66.7 chrX:12854840-12854911 (-)
-GGCCGAATGGTCTATTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-4-1 (tRNAscan-SE ID: chrIII.trna25) Pro (TGG) 72 bp Sc: 66.3 chrIII:8069405-8069476 (+)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTGAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-5-1 (tRNAscan-SE ID: chrV.trna108) Pro (TGG) 72 bp Sc: 64.7 chrV:3588314-3588385 (-)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGCGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-6-1 (tRNAscan-SE ID: chrV.trna109) Pro (TGG) 72 bp Sc: 67.2 chrV:3582131-3582202 (-)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCC
-CCAGTTCGGCCC
->Caenorhabditis_elegans_tRNA-Pro-TGG-7-1 (tRNAscan-SE ID: chrII.trna41) Pro (TGG) 72 bp Sc: 65.7 chrII:10304771-10304842 (-)
-GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCTGGTTCAATCC
-CCGGTTCGGCCC
->Caenorhabditis_elegans_tRNA-SeC-TCA-1-1 (tRNAscan-SE ID: chrIV.trna3) SeC (TCA) 87 bp Sc: 107.4 chrIV:658181-658267 (+)
-GCCCGGATGAACCATGGCGGTCTGTGGTGCAGACTTCAAATCTGTAGGCGGTTAGCGCCG
-CAGTGGTTCGACTCCACCTTTCGGGTG
->Caenorhabditis_elegans_tRNA-Ser-AGA-1-1 (tRNAscan-SE ID: chrIII.trna49) Ser (AGA) 82 bp Sc: 82.3 chrIII:9862022-9862103 (-)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTTTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-1-2 (tRNAscan-SE ID: chrX.trna126) Ser (AGA) 82 bp Sc: 82.3 chrX:14162215-14162296 (+)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTTTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-2-1 (tRNAscan-SE ID: chrII.trna2) Ser (AGA) 82 bp Sc: 81.6 chrII:1520035-1520116 (+)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-2-10 (tRNAscan-SE ID: chrX.trna76) Ser (AGA) 82 bp Sc: 81.6 chrX:8971600-8971681 (+)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-2-11 (tRNAscan-SE ID: chrX.trna101) Ser (AGA) 82 bp Sc: 81.6 chrX:13046578-13046659 (+)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-2-2 (tRNAscan-SE ID: chrII.trna5) Ser (AGA) 82 bp Sc: 81.6 chrII:3267989-3268070 (+)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-2-3 (tRNAscan-SE ID: chrIII.trna20) Ser (AGA) 82 bp Sc: 81.6 chrIII:6158778-6158859 (+)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-2-4 (tRNAscan-SE ID: chrIII.trna30) Ser (AGA) 82 bp Sc: 81.6 chrIII:8646167-8646248 (+)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-2-5 (tRNAscan-SE ID: chrIV.trna55) Ser (AGA) 82 bp Sc: 81.6 chrIV:15311118-15311199 (-)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-2-6 (tRNAscan-SE ID: chrIV.trna54) Ser (AGA) 82 bp Sc: 81.6 chrIV:15318478-15318559 (-)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-2-7 (tRNAscan-SE ID: chrX.trna265) Ser (AGA) 82 bp Sc: 81.6 chrX:8152812-8152893 (-)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-2-8 (tRNAscan-SE ID: chrX.trna55) Ser (AGA) 82 bp Sc: 81.6 chrX:8154445-8154526 (+)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-2-9 (tRNAscan-SE ID: chrX.trna57) Ser (AGA) 82 bp Sc: 81.6 chrX:8155462-8155543 (+)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-3-1 (tRNAscan-SE ID: chrX.trna138) Ser (AGA) 82 bp Sc: 75.1 chrX:15773527-15773608 (+)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGTCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-AGA-4-1 (tRNAscan-SE ID: chrX.trna177) Ser (AGA) 82 bp Sc: 74.8 chrX:15770009-15770090 (-)
-GCCGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-CGA-1-1 (tRNAscan-SE ID: chrI.trna48) Ser (CGA) 82 bp Sc: 84.2 chrI:11803316-11803397 (-)
-GCAGTCATGTCCGAGTGGTTAAGGAGTTTGACTCGAAATCAAATGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-CGA-1-2 (tRNAscan-SE ID: chrIII.trna50) Ser (CGA) 82 bp Sc: 84.2 chrIII:9861607-9861688 (-)
-GCAGTCATGTCCGAGTGGTTAAGGAGTTTGACTCGAAATCAAATGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-CGA-1-3 (tRNAscan-SE ID: chrX.trna204) Ser (CGA) 82 bp Sc: 84.2 chrX:13046366-13046447 (-)
-GCAGTCATGTCCGAGTGGTTAAGGAGTTTGACTCGAAATCAAATGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-CGA-2-1 (tRNAscan-SE ID: chrIII.trna62) Ser (CGA) 82 bp Sc: 81.6 chrIII:6513937-6514018 (-)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTCGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-CGA-2-2 (tRNAscan-SE ID: chrX.trna176) Ser (CGA) 82 bp Sc: 81.6 chrX:15773331-15773412 (-)
-GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTCGAAATCAATTGGGCTCTGCCCGCGTA
-GGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-CGA-3-1 (tRNAscan-SE ID: chrIII.trna21) Ser (CGA) 86 bp Sc: 59.1 chrIII:6158965-6159050 (+)
-GTGGTTAAGAATGTCCGAGTGGTTAAGGAGTTTGACTCGAAATCAAATGGGCTCTGTCCG
-CGTAGGTTCGAATCCTGCTGACTGCG
->Caenorhabditis_elegans_tRNA-Ser-GCT-1-1 (tRNAscan-SE ID: chrI.trna40) Ser (GCT) 82 bp Sc: 84.4 chrI:14162848-14162929 (+)
-GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTG
-AGTTCGAATCTCATCCTGATCG
->Caenorhabditis_elegans_tRNA-Ser-GCT-1-2 (tRNAscan-SE ID: chrIII.trna64) Ser (GCT) 82 bp Sc: 84.4 chrIII:6056299-6056380 (-)
-GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTG
-AGTTCGAATCTCATCCTGATCG
->Caenorhabditis_elegans_tRNA-Ser-GCT-1-3 (tRNAscan-SE ID: chrV.trna104) Ser (GCT) 82 bp Sc: 84.4 chrV:6551854-6551935 (-)
-GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTG
-AGTTCGAATCTCATCCTGATCG
->Caenorhabditis_elegans_tRNA-Ser-GCT-1-4 (tRNAscan-SE ID: chrX.trna38) Ser (GCT) 82 bp Sc: 84.4 chrX:5708028-5708109 (+)
-GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTG
-AGTTCGAATCTCATCCTGATCG
->Caenorhabditis_elegans_tRNA-Ser-GCT-1-5 (tRNAscan-SE ID: chrX.trna39) Ser (GCT) 82 bp Sc: 84.4 chrX:5709375-5709456 (+)
-GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTG
-AGTTCGAATCTCATCCTGATCG
->Caenorhabditis_elegans_tRNA-Ser-GCT-1-6 (tRNAscan-SE ID: chrX.trna197) Ser (GCT) 82 bp Sc: 84.4 chrX:13448873-13448954 (-)
-GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTG
-AGTTCGAATCTCATCCTGATCG
->Caenorhabditis_elegans_tRNA-Ser-GCT-1-7 (tRNAscan-SE ID: chrX.trna158) Ser (GCT) 82 bp Sc: 84.4 chrX:16689985-16690066 (-)
-GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTG
-AGTTCGAATCTCATCCTGATCG
->Caenorhabditis_elegans_tRNA-Ser-GCT-2-1 (tRNAscan-SE ID: chrX.trna107) Ser (GCT) 82 bp Sc: 83.4 chrX:13442643-13442724 (+)
-GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTG
-AGTTCGAATCTCATCTTGATCG
->Caenorhabditis_elegans_tRNA-Ser-GCT-3-1 (tRNAscan-SE ID: chrIII.trna38) Ser (GCT) 77 bp Sc: 54.4 chrIII:13009423-13009499 (+)
-GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTC
-AAATCTCATCCTGATCG
->Caenorhabditis_elegans_tRNA-Ser-TGA-1-1 (tRNAscan-SE ID: chrX.trna83) Ser (TGA) 82 bp Sc: 84.9 chrX:10124498-10124579 (+)
-GCTGCGATGTCCGAGTGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCGTA
-GGTTCAAATCCTGCTCGCAGCG
->Caenorhabditis_elegans_tRNA-Ser-TGA-2-1 (tRNAscan-SE ID: chrV.trna90) Ser (TGA) 82 bp Sc: 85.6 chrV:12780386-12780467 (-)
-GCTGCGATGTCCGAGTGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCGTA
-GGTTCGAACCCTGCTCGCAGCG
->Caenorhabditis_elegans_tRNA-Ser-TGA-2-2 (tRNAscan-SE ID: chrX.trna174) Ser (TGA) 82 bp Sc: 85.6 chrX:16042608-16042689 (-)
-GCTGCGATGTCCGAGTGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCGTA
-GGTTCGAACCCTGCTCGCAGCG
->Caenorhabditis_elegans_tRNA-Ser-TGA-3-1 (tRNAscan-SE ID: chrI.trna19) Ser (TGA) 82 bp Sc: 85.5 chrI:9605756-9605837 (+)
-GCAGCGATGTCCGAGTGGTTAAGGAGTTGGACTTGAAATCCAATGGGCTTTGCCCGCGTA
-GGTTCGAACCCTGCTCGCTGCG
->Caenorhabditis_elegans_tRNA-Ser-TGA-4-1 (tRNAscan-SE ID: chrX.trna97) Ser (TGA) 82 bp Sc: 81.8 chrX:12889940-12890021 (+)
-GCAACGATGTCCGAGTGGTTAAGGAGATGGACTTGAAATCCATTGGGCTTTGCCCGCGTA
-GGTTCGATTCCTGCTCGTTGCG
->Caenorhabditis_elegans_tRNA-Ser-TGA-5-1 (tRNAscan-SE ID: chrV.trna79) Ser (TGA) 82 bp Sc: 84.6 chrV:15547875-15547956 (-)
-GCTGCGATGTCCGAGTGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCGTA
-GGTTCGAACCCTGCTTGCAGCG
->Caenorhabditis_elegans_tRNA-Ser-TGA-6-1 (tRNAscan-SE ID: chrIV.trna42) Ser (TGA) 82 bp Sc: 82.4 chrIV:16577306-16577387 (+)
-GCTGCGATGTCCGAGCGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCGTA
-GGTTCAAATCCTGCTCGCAGCG
->Caenorhabditis_elegans_tRNA-Ser-TGA-6-2 (tRNAscan-SE ID: chrIV.trna48) Ser (TGA) 82 bp Sc: 82.4 chrIV:16583742-16583823 (-)
-GCTGCGATGTCCGAGCGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCGTA
-GGTTCAAATCCTGCTCGCAGCG
->Caenorhabditis_elegans_tRNA-Ser-TGA-7-1 (tRNAscan-SE ID: chrV.trna23) Ser (TGA) 82 bp Sc: 74.4 chrV:15550612-15550693 (+)
-GCTGCGATGCCCGAGTGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCATA
-GGTTCGAACCCTGCTTGCAGCG
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-1 (tRNAscan-SE ID: chrII.trna60) Thr (AGT) 72 bp Sc: 85.3 chrII:3439219-3439290 (-)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-10 (tRNAscan-SE ID: chrX.trna286) Thr (AGT) 72 bp Sc: 85.3 chrX:3371422-3371493 (-)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-11 (tRNAscan-SE ID: chrX.trna32) Thr (AGT) 72 bp Sc: 85.3 chrX:4445014-4445085 (+)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-12 (tRNAscan-SE ID: chrX.trna273) Thr (AGT) 72 bp Sc: 85.3 chrX:7176983-7177054 (-)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-13 (tRNAscan-SE ID: chrX.trna102) Thr (AGT) 72 bp Sc: 85.3 chrX:13261203-13261274 (+)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-14 (tRNAscan-SE ID: chrX.trna201) Thr (AGT) 72 bp Sc: 85.3 chrX:13283637-13283708 (-)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-15 (tRNAscan-SE ID: chrX.trna103) Thr (AGT) 72 bp Sc: 85.3 chrX:13293192-13293263 (+)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-2 (tRNAscan-SE ID: chrII.trna55) Thr (AGT) 72 bp Sc: 85.3 chrII:3567610-3567681 (-)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-3 (tRNAscan-SE ID: chrIII.trna57) Thr (AGT) 72 bp Sc: 85.3 chrIII:7030557-7030628 (-)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-4 (tRNAscan-SE ID: chrIII.trna48) Thr (AGT) 72 bp Sc: 85.3 chrIII:10624742-10624813 (-)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-5 (tRNAscan-SE ID: chrV.trna111) Thr (AGT) 72 bp Sc: 85.3 chrV:2664667-2664738 (-)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-6 (tRNAscan-SE ID: chrV.trna2) Thr (AGT) 72 bp Sc: 85.3 chrV:2674010-2674081 (+)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-7 (tRNAscan-SE ID: chrV.trna99) Thr (AGT) 72 bp Sc: 85.3 chrV:8496104-8496175 (-)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-8 (tRNAscan-SE ID: chrV.trna97) Thr (AGT) 72 bp Sc: 85.3 chrV:9407040-9407111 (-)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-1-9 (tRNAscan-SE ID: chrX.trna18) Thr (AGT) 72 bp Sc: 85.3 chrX:2528042-2528113 (+)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCA
->Caenorhabditis_elegans_tRNA-Thr-AGT-2-1 (tRNAscan-SE ID: chrII.trna58) Thr (AGT) 72 bp Sc: 81.2 chrII:3519086-3519157 (-)
-GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTC
-CAGCATGAGGCC
->Caenorhabditis_elegans_tRNA-Thr-AGT-3-1 (tRNAscan-SE ID: chrII.trna16) Thr (AGT) 72 bp Sc: 74.8 chrII:7003273-7003344 (+)
-GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGTATGGGAGAGGGCTGGGGTTCAATTC
-CCCATACCTCCA
->Caenorhabditis_elegans_tRNA-Thr-CGT-1-1 (tRNAscan-SE ID: chrX.trna239) Thr (CGT) 72 bp Sc: 83.8 chrX:9025663-9025734 (-)
-GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTCGTAAACCAAAGGTCCGTAGTTCAATCC
-TGCGTGAGGGCA
->Caenorhabditis_elegans_tRNA-Thr-CGT-2-1 (tRNAscan-SE ID: chrIII.trna37) Thr (CGT) 72 bp Sc: 76.0 chrIII:11792782-11792853 (+)
-GCCCGTATAGCTCAGTGGCAGAGCGTCTGTCTCGTAAACAGAAGGTCGGCGGTTCAATCC
-CGCCTGGGGGCA
->Caenorhabditis_elegans_tRNA-Thr-CGT-2-2 (tRNAscan-SE ID: chrIII.trna44) Thr (CGT) 72 bp Sc: 76.0 chrIII:13016107-13016178 (-)
-GCCCGTATAGCTCAGTGGCAGAGCGTCTGTCTCGTAAACAGAAGGTCGGCGGTTCAATCC
-CGCCTGGGGGCA
->Caenorhabditis_elegans_tRNA-Thr-CGT-3-1 (tRNAscan-SE ID: chrV.trna25) Thr (CGT) 72 bp Sc: 76.0 chrV:16219159-16219230 (+)
-GCCCGTATAGCTCAGTGGCAGAGCGTCTGTCTCGTAAACAGAAGGCCGGCGGTTCAATCC
-CGCCTGGGGGCA
->Caenorhabditis_elegans_tRNA-Thr-CGT-4-1 (tRNAscan-SE ID: chrX.trna214) Thr (CGT) 72 bp Sc: 76.0 chrX:11935080-11935151 (-)
-GCCCGTATAGCTCAGTGGCAGAGCGTCTGTCTCGTAAACAGAAGGTCGGCGGTTCAATCC
-CGCCTGGGGGCA
->Caenorhabditis_elegans_tRNA-Thr-CGT-5-1 (tRNAscan-SE ID: chrV.trna102) Thr (CGT) 72 bp Sc: 75.1 chrV:7730654-7730725 (-)
-GCCCGTATAGCTCAGTGGCAGAGCGTCTGTCTCGTAAACAGAAGGTCGACGGTTCAATCC
-CGTCTGGGGGCA
->Caenorhabditis_elegans_tRNA-Thr-CGT-6-1 (tRNAscan-SE ID: chrX.trna91) Thr (CGT) 72 bp Sc: 75.7 chrX:11933728-11933799 (+)
-GCCCGTATAGCTCAGAGGCAGAGCGTCTGTCTCGTAAACAGAAGGTCGGCGGTTCAATCC
-CGCCTGTGGGCA
->Caenorhabditis_elegans_tRNA-Thr-TGT-1-1 (tRNAscan-SE ID: chrI.trna43) Thr (TGT) 72 bp Sc: 81.0 chrI:13310345-13310416 (-)
-GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCC
-TGCGTGGGGGCA
->Caenorhabditis_elegans_tRNA-Thr-TGT-1-2 (tRNAscan-SE ID: chrIII.trna16) Thr (TGT) 72 bp Sc: 81.0 chrIII:5305905-5305976 (+)
-GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCC
-TGCGTGGGGGCA
->Caenorhabditis_elegans_tRNA-Thr-TGT-1-3 (tRNAscan-SE ID: chrIII.trna42) Thr (TGT) 72 bp Sc: 81.0 chrIII:13411366-13411437 (-)
-GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCC
-TGCGTGGGGGCA
->Caenorhabditis_elegans_tRNA-Thr-TGT-1-4 (tRNAscan-SE ID: chrIV.trna69) Thr (TGT) 72 bp Sc: 81.0 chrIV:9000804-9000875 (-)
-GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCC
-TGCGTGGGGGCA
->Caenorhabditis_elegans_tRNA-Thr-TGT-1-5 (tRNAscan-SE ID: chrV.trna62) Thr (TGT) 72 bp Sc: 81.0 chrV:18412483-18412554 (-)
-GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCC
-TGCGTGGGGGCA
->Caenorhabditis_elegans_tRNA-Thr-TGT-1-6 (tRNAscan-SE ID: chrX.trna4) Thr (TGT) 72 bp Sc: 81.0 chrX:487815-487886 (+)
-GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCC
-TGCGTGGGGGCA
->Caenorhabditis_elegans_tRNA-Thr-TGT-1-7 (tRNAscan-SE ID: chrX.trna240) Thr (TGT) 72 bp Sc: 81.0 chrX:9024413-9024484 (-)
-GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCC
-TGCGTGGGGGCA
->Caenorhabditis_elegans_tRNA-Thr-TGT-1-8 (tRNAscan-SE ID: chrX.trna93) Thr (TGT) 72 bp Sc: 81.0 chrX:12563788-12563859 (+)
-GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCC
-TGCGTGGGGGCA
->Caenorhabditis_elegans_tRNA-Thr-TGT-1-9 (tRNAscan-SE ID: chrX.trna109) Thr (TGT) 72 bp Sc: 81.0 chrX:13653728-13653799 (+)
-GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCC
-TGCGTGGGGGCA
->Caenorhabditis_elegans_tRNA-Trp-CCA-1-1 (tRNAscan-SE ID: chrI.trna73) Trp (CCA) 72 bp Sc: 71.5 chrI:946044-946115 (-)
-GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCC
-GCTCAGTGGTCA
->Caenorhabditis_elegans_tRNA-Trp-CCA-1-10 (tRNAscan-SE ID: chrX.trna243) Trp (CCA) 72 bp Sc: 71.5 chrX:8945160-8945231 (-)
-GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCC
-GCTCAGTGGTCA
->Caenorhabditis_elegans_tRNA-Trp-CCA-1-2 (tRNAscan-SE ID: chrIII.trna52) Trp (CCA) 72 bp Sc: 71.5 chrIII:8678497-8678568 (-)
-GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCC
-GCTCAGTGGTCA
->Caenorhabditis_elegans_tRNA-Trp-CCA-1-3 (tRNAscan-SE ID: chrIV.trna73) Trp (CCA) 72 bp Sc: 71.5 chrIV:3681880-3681951 (-)
-GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCC
-GCTCAGTGGTCA
->Caenorhabditis_elegans_tRNA-Trp-CCA-1-4 (tRNAscan-SE ID: chrIV.trna71) Trp (CCA) 72 bp Sc: 71.5 chrIV:5344300-5344371 (-)
-GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCC
-GCTCAGTGGTCA
->Caenorhabditis_elegans_tRNA-Trp-CCA-1-5 (tRNAscan-SE ID: chrIV.trna70) Trp (CCA) 72 bp Sc: 71.5 chrIV:7344156-7344227 (-)
-GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCC
-GCTCAGTGGTCA
->Caenorhabditis_elegans_tRNA-Trp-CCA-1-6 (tRNAscan-SE ID: chrIV.trna33) Trp (CCA) 72 bp Sc: 71.5 chrIV:15289703-15289774 (+)
-GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCC
-GCTCAGTGGTCA
->Caenorhabditis_elegans_tRNA-Trp-CCA-1-7 (tRNAscan-SE ID: chrX.trna43) Trp (CCA) 72 bp Sc: 71.5 chrX:6371378-6371449 (+)
-GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCC
-GCTCAGTGGTCA
->Caenorhabditis_elegans_tRNA-Trp-CCA-1-8 (tRNAscan-SE ID: chrX.trna72) Trp (CCA) 72 bp Sc: 71.5 chrX:8877340-8877411 (+)
-GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCC
-GCTCAGTGGTCA
->Caenorhabditis_elegans_tRNA-Trp-CCA-1-9 (tRNAscan-SE ID: chrX.trna244) Trp (CCA) 72 bp Sc: 71.5 chrX:8944232-8944303 (-)
-GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCC
-GCTCAGTGGTCA
->Caenorhabditis_elegans_tRNA-Trp-CCA-2-1 (tRNAscan-SE ID: chrX.trna186) Trp (CCA) 72 bp Sc: 68.3 chrX:14228920-14228991 (-)
-GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGATTGGGCGTTCGATCC
-GCTCAGTGGTCA
->Caenorhabditis_elegans_tRNA-Trp-CCA-3-1 (tRNAscan-SE ID: chrII.trna27) Trp (CCA) 72 bp Sc: 64.3 chrII:12539597-12539668 (+)
-GACTGCTTGGCGCAATGATAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCC
-GCTCAGTGGTCA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-1-1 (tRNAscan-SE ID: chrV.trna11) Tyr (GTA) 84 bp Sc: 76.8 chrV:8247481-8247564 (+)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGTGGGTATCCTTAGGTCG
-CTGGTTCGAATCCGGCTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-1-2 (tRNAscan-SE ID: chrV.trna21) Tyr (GTA) 84 bp Sc: 76.8 chrV:15480694-15480777 (+)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGTGGGTATCCTTAGGTCG
-CTGGTTCGAATCCGGCTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-2-1 (tRNAscan-SE ID: chrI.trna5) Tyr (GTA) 84 bp Sc: 74.6 chrI:6135830-6135913 (+)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTTCGCAGATATCCTTAGGTCA
-CTGGTTCGAATCCGGTTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-2-10 (tRNAscan-SE ID: chrX.trna172) Tyr (GTA) 84 bp Sc: 74.6 chrX:16208825-16208908 (-)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCA
-CTGGTTCGAATCCGGTTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-2-11 (tRNAscan-SE ID: chrX.trna171) Tyr (GTA) 84 bp Sc: 74.6 chrX:16209228-16209311 (-)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCA
-CTGGTTCGAATCCGGTTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-2-12 (tRNAscan-SE ID: chrX.trna170) Tyr (GTA) 84 bp Sc: 74.6 chrX:16209769-16209852 (-)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCA
-CTGGTTCGAATCCGGTTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-2-2 (tRNAscan-SE ID: chrIII.trna1) Tyr (GTA) 84 bp Sc: 74.6 chrIII:535382-535465 (+)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTTAGCAGGTATCCTTAGGTCA
-CTGGTTCGAATCCGGTTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-2-3 (tRNAscan-SE ID: chrIII.trna39) Tyr (GTA) 84 bp Sc: 74.6 chrIII:13224566-13224649 (+)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTTAGCAGGTATCCTTAGGTCA
-CTGGTTCGAATCCGGTTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-2-4 (tRNAscan-SE ID: chrV.trna18) Tyr (GTA) 84 bp Sc: 74.6 chrV:14689532-14689615 (+)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTTTGCAGATATCCTTAGGTCA
-CTGGTTCGAATCCGGTTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-2-5 (tRNAscan-SE ID: chrV.trna69) Tyr (GTA) 84 bp Sc: 74.6 chrV:17542446-17542529 (-)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTTGGCAGATATCCTTAGGTCA
-CTGGTTCGAATCCGGTTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-2-6 (tRNAscan-SE ID: chrX.trna304) Tyr (GTA) 84 bp Sc: 74.6 chrX:865389-865472 (-)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCA
-CTGGTTCGAATCCGGTTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-2-7 (tRNAscan-SE ID: chrX.trna95) Tyr (GTA) 84 bp Sc: 74.6 chrX:12665228-12665311 (+)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCA
-CTGGTTCGAATCCGGTTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-2-8 (tRNAscan-SE ID: chrX.trna202) Tyr (GTA) 84 bp Sc: 74.6 chrX:13264683-13264766 (-)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCGGGTATCCTTAGGTCA
-CTGGTTCGAATCCGGTTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-2-9 (tRNAscan-SE ID: chrX.trna173) Tyr (GTA) 84 bp Sc: 74.6 chrX:16208263-16208346 (-)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCA
-CTGGTTCGAATCCGGTTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-3-1 (tRNAscan-SE ID: chrV.trna70) Tyr (GTA) 84 bp Sc: 67.4 chrV:17317879-17317962 (-)
-CCGTCGATAGCTCAGTTGGTAGAGCGCAGGACTGTAGAGTTAGCAGATATCCTTAGGTCA
-CTGGTTCGAATCCGGTTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-4-1 (tRNAscan-SE ID: chrII.trna44) Tyr (GTA) 84 bp Sc: 67.0 chrII:9211804-9211887 (-)
-CAGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGTGGTTATCCTTAGGTCG
-CTGGTTCGAATCCGGCTCGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-5-1 (tRNAscan-SE ID: chrX.trna200) Tyr (GTA) 84 bp Sc: 68.8 chrX:13284766-13284849 (-)
-CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCA
-CTGGTTCGAATCCGGTTGGACGGA
->Caenorhabditis_elegans_tRNA-Tyr-GTA-6-1 (tRNAscan-SE ID: chrV.trna96) Tyr (GTA) 87 bp Sc: 66.9 chrV:9412205-9412291 (-)
-CCGTCGATAGCTCAGTAGTTGGTAGAGCGGAGGACTGTAGAGTCAGTGGGTATCCTTAGA
-TCGCTGGTTCGAATCCGGCTCGACGGA
->Caenorhabditis_elegans_tRNA-Val-AAC-1-1 (tRNAscan-SE ID: chrX.trna142) Val (AAC) 73 bp Sc: 77.4 chrX:16298341-16298413 (+)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGCGGTTCGATC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-1-2 (tRNAscan-SE ID: chrX.trna143) Val (AAC) 73 bp Sc: 77.4 chrX:16299393-16299465 (+)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGCGGTTCGATC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-1-3 (tRNAscan-SE ID: chrX.trna144) Val (AAC) 73 bp Sc: 77.4 chrX:16300063-16300135 (+)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGCGGTTCGATC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-1-4 (tRNAscan-SE ID: chrX.trna145) Val (AAC) 73 bp Sc: 77.4 chrX:16300589-16300661 (+)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGCGGTTCGATC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-2-1 (tRNAscan-SE ID: chrI.trna33) Val (AAC) 73 bp Sc: 76.6 chrI:12065865-12065937 (+)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-2-10 (tRNAscan-SE ID: chrX.trna230) Val (AAC) 73 bp Sc: 76.6 chrX:9561088-9561160 (-)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-2-11 (tRNAscan-SE ID: chrX.trna96) Val (AAC) 73 bp Sc: 76.6 chrX:12843688-12843760 (+)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-2-12 (tRNAscan-SE ID: chrX.trna131) Val (AAC) 73 bp Sc: 76.6 chrX:15236124-15236196 (+)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-2-2 (tRNAscan-SE ID: chrI.trna45) Val (AAC) 73 bp Sc: 76.6 chrI:13156357-13156429 (-)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-2-3 (tRNAscan-SE ID: chrI.trna38) Val (AAC) 73 bp Sc: 76.6 chrI:13161061-13161133 (+)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-2-4 (tRNAscan-SE ID: chrIII.trna33) Val (AAC) 73 bp Sc: 76.6 chrIII:11353029-11353101 (+)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-2-5 (tRNAscan-SE ID: chrIII.trna34) Val (AAC) 73 bp Sc: 76.6 chrIII:11353628-11353700 (+)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-2-6 (tRNAscan-SE ID: chrIV.trna50) Val (AAC) 73 bp Sc: 76.6 chrIV:16382431-16382503 (-)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-2-7 (tRNAscan-SE ID: chrIV.trna40) Val (AAC) 73 bp Sc: 76.6 chrIV:16400130-16400202 (+)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-2-8 (tRNAscan-SE ID: chrV.trna84) Val (AAC) 73 bp Sc: 76.6 chrV:15013034-15013106 (-)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-2-9 (tRNAscan-SE ID: chrX.trna251) Val (AAC) 73 bp Sc: 76.6 chrX:8650709-8650781 (-)
-GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-3-1 (tRNAscan-SE ID: chrIV.trna32) Val (AAC) 73 bp Sc: 75.2 chrIV:15235388-15235460 (+)
-GGTTTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-3-2 (tRNAscan-SE ID: chrX.trna156) Val (AAC) 73 bp Sc: 75.2 chrX:17611503-17611575 (-)
-GGTTTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCA
->Caenorhabditis_elegans_tRNA-Val-AAC-4-1 (tRNAscan-SE ID: chrX.trna155) Val (AAC) 73 bp Sc: 73.3 chrX:17611289-17611361 (+)
-GGTTTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGC
-CCGCCCGAGATCT
->Caenorhabditis_elegans_tRNA-Val-CAC-1-1 (tRNAscan-SE ID: chrIV.trna20) Val (CAC) 73 bp Sc: 80.7 chrIV:6481161-6481233 (+)
-GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTCACACGCAGAAGGTCGCCGGTTCGAAC
-CCGGCCAGGACCT
->Caenorhabditis_elegans_tRNA-Val-CAC-1-2 (tRNAscan-SE ID: chrV.trna93) Val (CAC) 73 bp Sc: 80.7 chrV:11412235-11412307 (-)
-GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTCACACGCAGAAGGTCGCCGGTTCGAAC
-CCGGCCAGGACCT
->Caenorhabditis_elegans_tRNA-Val-CAC-1-3 (tRNAscan-SE ID: chrV.trna80) Val (CAC) 73 bp Sc: 80.7 chrV:15515506-15515578 (-)
-GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTCACACGCAGAAGGTCGCCGGTTCGAAC
-CCGGCCAGGACCT
->Caenorhabditis_elegans_tRNA-Val-CAC-1-4 (tRNAscan-SE ID: chrX.trna154) Val (CAC) 73 bp Sc: 80.7 chrX:16590395-16590467 (+)
-GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTCACACGCAGAAGGTCGCCGGTTCGAAC
-CCGGCCAGGACCT
->Caenorhabditis_elegans_tRNA-Val-CAC-1-5 (tRNAscan-SE ID: chrX.trna164) Val (CAC) 73 bp Sc: 80.7 chrX:16590931-16591003 (-)
-GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTCACACGCAGAAGGTCGCCGGTTCGAAC
-CCGGCCAGGACCT
->Caenorhabditis_elegans_tRNA-Val-CAC-2-1 (tRNAscan-SE ID: chrIV.trna2) Val (CAC) 73 bp Sc: 78.8 chrIV:620482-620554 (+)
-GGTCCTCTGGTGTAGTGGTTATCACGTCTGCTTCACACGCAGAAGGTCGCCGGTTCGAAC
-CCGGCGAGGACCT
->Caenorhabditis_elegans_tRNA-Val-TAC-1-1 (tRNAscan-SE ID: chrV.trna91) Val (TAC) 73 bp Sc: 77.5 chrV:12683351-12683423 (-)
-GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTTACACGCAGAAGATCGCCGGTTCGAAC
-CCGGCCAGGACCT
->Caenorhabditis_elegans_tRNA-Val-TAC-2-1 (tRNAscan-SE ID: chrX.trna285) Val (TAC) 73 bp Sc: 77.5 chrX:3793564-3793636 (-)
-GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTTACACGCAGAAGATCGCCGGTTCGATC
-CCGGCCAGGACCT
->Caenorhabditis_elegans_tRNA-Val-TAC-3-1 (tRNAscan-SE ID: chrII.trna50) Val (TAC) 73 bp Sc: 77.2 chrII:5577200-5577272 (-)
-GGTCCTATGGTGTAGTGGTTATCACGTCTGCTTTACACGCAGAAGATCGCCGGTTCGAAC
-CCGGCTAGGACCT
->Caenorhabditis_elegans_tRNA-Val-TAC-3-2 (tRNAscan-SE ID: chrX.trna104) Val (TAC) 73 bp Sc: 77.2 chrX:13307034-13307106 (+)
-GGTCCTATGGTGTAGTGGTTATCACGTCTGCTTTACACGCAGAAGATCGCCGGTTCGAAC
-CCGGCTAGGACCT
->Caenorhabditis_elegans_tRNA-Val-TAC-4-1 (tRNAscan-SE ID: chrII.trna24) Val (TAC) 73 bp Sc: 72.9 chrII:11959375-11959447 (+)
-GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTTACACGCAGTAGGCCGCCGGTTCGATC
-CCGGCCAGGACCT
->Caenorhabditis_elegans_tRNA-iMet-CAT-1-1 (tRNAscan-SE ID: chrI.trna34) iMet (CAT) 72 bp Sc: 61.2 chrI:12142911-12142982 (+)
-AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAAC
-CACTCGCTGCTA
->Caenorhabditis_elegans_tRNA-iMet-CAT-1-2 (tRNAscan-SE ID: chrI.trna46) iMet (CAT) 72 bp Sc: 61.2 chrI:12225426-12225497 (-)
-AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAAC
-CACTCGCTGCTA
->Caenorhabditis_elegans_tRNA-iMet-CAT-1-3 (tRNAscan-SE ID: chrI.trna36) iMet (CAT) 72 bp Sc: 61.2 chrI:12229309-12229380 (+)
-AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAAC
-CACTCGCTGCTA
->Caenorhabditis_elegans_tRNA-iMet-CAT-1-4 (tRNAscan-SE ID: chrII.trna36) iMet (CAT) 72 bp Sc: 61.2 chrII:12435580-12435651 (-)
-AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAAC
-CACTCGCTGCTA
->Caenorhabditis_elegans_tRNA-iMet-CAT-1-5 (tRNAscan-SE ID: chrIII.trna7) iMet (CAT) 72 bp Sc: 61.2 chrIII:1604582-1604653 (+)
-AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAAC
-CACTCGCTGCTA
->Caenorhabditis_elegans_tRNA-iMet-CAT-1-6 (tRNAscan-SE ID: chrIII.trna67) iMet (CAT) 72 bp Sc: 61.2 chrIII:5294979-5295050 (-)
-AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAAC
-CACTCGCTGCTA
->Caenorhabditis_elegans_tRNA-iMet-CAT-1-7 (tRNAscan-SE ID: chrX.trna59) iMet (CAT) 72 bp Sc: 61.2 chrX:8156178-8156249 (+)
-AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAAC
-CACTCGCTGCTA
->Caenorhabditis_elegans_tRNA-iMet-CAT-1-8 (tRNAscan-SE ID: chrX.trna232) iMet (CAT) 72 bp Sc: 61.2 chrX:9373150-9373221 (-)
-AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAAC
-CACTCGCTGCTA
->Caenorhabditis_elegans_tRNA-iMet-CAT-1-9 (tRNAscan-SE ID: chrX.trna147) iMet (CAT) 72 bp Sc: 61.2 chrX:16441146-16441217 (+)
-AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAAC
-CACTCGCTGCTA
+>Escherichia_coli_str_K_12_substr_MG1655_tRNA-eColiLys-TTT-1-1 (tRNAscan-SE ID: chr.trna9) chr:780554-780629 (+) Lys (TTT) 76 bp Sc: 94.9
+GGGTCGTTAGCTCAGTTGGTAGAGCAGTTGACTTTTAATCAATTGGtCGCAGGTTCGAATCCTGCACGACCCA
+>Caenorhabditis_elegans_tRX-Lys-CTT-7-1 (tRNAscan-SE ID: chrI.trna1) Lys (CTT) 75 bp Sc: 20.2 chrI:185334-185409(+)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttta
+>Caenorhabditis_elegans_tRNA-Leu-CAG-2-1 (tRNAscan-SE ID: chrI.trna2) Leu (CAG) 84 bp Sc: 76.8 chrI:754679-754763(+)
+GCCGTTCTGGCCGAGTGGTCTAAGGCGCTGCGTTCAGGTCGCAGTCCTCTCCGGAGGGCGCAGGTTCGAATCCTGCGGACGGCA
+>Caenorhabditis_elegans_tRNA-Trp-CCA-1-1 (tRNAscan-SE ID: chrI.trna73) Trp (CCA) 72 bp Sc: 71.5 chrI:946043-946115(-)
+GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCCGCTCAGTGGTCA
+>Caenorhabditis_elegans_tRNA-Arg-TCT-2-1 (tRNAscan-SE ID: chrI.trna3) Arg (TCT) 73 bp Sc: 71.1 chrI:1447137-1447210(+)
+GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGAGCCCTGCCTGGGTCA
+>Caenorhabditis_elegans_tRNA-Arg-TCT-2-2 (tRNAscan-SE ID: chrI.trna4) Arg (TCT) 73 bp Sc: 71.1 chrI:1575719-1575792(+)
+GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGAGCCCTGCCTGGGTCA
+>Caenorhabditis_elegans_tRNA-Gly-GCC-1-1 (tRNAscan-SE ID: chrI.trna72) Gly (GCC) 71 bp Sc: 77.2 chrI:2272367-2272438(-)
+gcatcggtggttcagtggtagaatgctcgcctgccacgcgggcggcccgggttcgattcccggtcgatgca
+>Caenorhabditis_elegans_tRNA-Met-CAT-1-1 (tRNAscan-SE ID: chrI.trna71) Met (CAT) 73 bp Sc: 77.0 chrI:3638851-3638924(-)
+GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGCCTCACCGGGAGCA
+>Caenorhabditis_elegans_tRNA-Arg-ACG-1-1 (tRNAscan-SE ID: chrI.trna70) Arg (ACG) 73 bp Sc: 72.1 chrI:5843082-5843155(-)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGCAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Pro-AGG-4-1 (tRNAscan-SE ID: chrI.trna69) Pro (AGG) 72 bp Sc: 70.1 chrI:5854793-5854865(-)
+GGCTGAGTGGTCTAGTGGTATGATTCTCGCTTAGGGTGCGAGAGGTCCCGGGATCGATCCCCGGCTCAGCCC
+>Caenorhabditis_elegans_tRNA-Leu-AAG-2-1 (tRNAscan-SE ID: chrI.trna68) Leu (AAG) 82 bp Sc: 72.6 chrI:6051154-6051236(-)
+GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-2-1 (tRNAscan-SE ID: chrI.trna5) Tyr (GTA) 84 bp Sc: 74.6 chrI:6135829-6135913(+)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTTCGCAGATATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGA
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-1 (tRNAscan-SE ID: chrI.trna6) Lys (CTT) 73 bp Sc: 85.9 chrI:6136596-6136669(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-1 (tRNAscan-SE ID: chrI.trna67) Ile (AAT) 74 bp Sc: 86.9 chrI:6163470-6163544(-)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-2 (tRNAscan-SE ID: chrI.trna7) Ile (AAT) 74 bp Sc: 86.9 chrI:6164190-6164264(+)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Cys-GCA-1-1 (tRNAscan-SE ID: chrI.trna8) Cys (GCA) 72 bp Sc: 74.0 chrI:6781802-6781874(+)
+GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTCCGGGTGCCCCCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-2-1 (tRNAscan-SE ID: chrI.trna66) Lys (CTT) 73 bp Sc: 83.5 chrI:7279354-7279427(-)
+GCCCGGTTAGCTCAGCCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Asn-GTT-3-1 (tRNAscan-SE ID: chrI.trna65) Asn (GTT) 77 bp Sc: 56.4 chrI:7718881-7718958(-)
+GCTTTACCTGTGGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGAGAGCG
+>Caenorhabditis_elegans_tRX-Lys-CTT-7-2 (tRNAscan-SE ID: chrI.trna9) Lys (CTT) 75 bp Sc: 20.2 chrI:7842913-7842988(+)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttta
+>Caenorhabditis_elegans_tRNA-Ile-TAT-1-1 (tRNAscan-SE ID: chrI.trna10) Ile (TAT) 85 bp Sc: 84.7 chrI:7960836-7960921(+)
+GCCCCGGTGGCCGAGCGGTCGAAGGCGTGAGACTTATGATCTCATTGGGTTAAACCAGTCGCGGGTTCGAATCCCGCCCGGGGCA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-1 (tRNAscan-SE ID: chrI.trna64) Glu (CTC) 72 bp Sc: 77.9 chrI:8530127-8530199(-)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRX-Und-NNN-1-1 (tRNAscan-SE ID: chrI.trna63) Und (NNN) 85 bp Sc: 54.1 chrI:8781153-8781238(-)
+GTCGAGGTGGCCGAGTGGGGCAAGGCATGAGTTTTCAGACTCAAAGGGCACTAGCCCGATGCAGGTTCAAATCCTGTCCTCGGCG
+>Caenorhabditis_elegans_tRX-Lys-CTT-8-1 (tRNAscan-SE ID: chrI.trna11) Lys (CTT) 62 bp Sc: 20.7 chrI:8791359-8791421(+)
+gtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRX-Lys-TTT-2-1 (tRNAscan-SE ID: chrI.trna12) Lys (TTT) 73 bp Sc: 64.6 chrI:8953168-8953241(+)
+GTGTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-1 (tRNAscan-SE ID: chrI.trna62) Asn (GTT) 73 bp Sc: 73.5 chrI:9051252-9051325(-)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Arg-TCG-2-1 (tRNAscan-SE ID: chrI.trna13) Arg (TCG) 73 bp Sc: 71.0 chrI:9267121-9267194(+)
+GGCCGCGTGGCCTAATGGATAAGGCACCAGACTTCGAATCTGGGGATTGCAGGTTCGAGTCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Pro-AGG-4-2 (tRNAscan-SE ID: chrI.trna61) Pro (AGG) 72 bp Sc: 70.1 chrI:9268927-9268999(-)
+GGCTGAGTGGTCTAGTGGTATGATTCTCGCTTAGGGTGCGAGAGGTCCCGGGATCGATCCCCGGCTCAGCCC
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-1 (tRNAscan-SE ID: chrI.trna60) Gly (TCC) 72 bp Sc: 71.7 chrI:9319964-9320036(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-2 (tRNAscan-SE ID: chrI.trna14) Gly (TCC) 72 bp Sc: 71.7 chrI:9320177-9320249(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-3 (tRNAscan-SE ID: chrI.trna59) Gly (TCC) 72 bp Sc: 71.7 chrI:9327423-9327495(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-4 (tRNAscan-SE ID: chrI.trna15) Gly (TCC) 72 bp Sc: 71.7 chrI:9327636-9327708(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-5 (tRNAscan-SE ID: chrI.trna58) Gly (TCC) 72 bp Sc: 71.7 chrI:9328415-9328487(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-6 (tRNAscan-SE ID: chrI.trna16) Gly (TCC) 72 bp Sc: 71.7 chrI:9328629-9328701(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gln-TTG-2-1 (tRNAscan-SE ID: chrI.trna17) Gln (TTG) 83 bp Sc: 71.9 chrI:9558791-9558874(+)
+GCCCCGGTGGCCGAGCGGTCGAAGGCGTGAGACTTGTTCTCATTGGGTTAAACCAGTCGCGGGTTCGAATCCCGCCCGGGGCA
+>Caenorhabditis_elegans_tRNA-Ile-TAT-1-2 (tRNAscan-SE ID: chrI.trna18) Ile (TAT) 85 bp Sc: 84.7 chrI:9562352-9562437(+)
+GCCCCGGTGGCCGAGCGGTCGAAGGCGTGAGACTTATGATCTCATTGGGTTAAACCAGTCGCGGGTTCGAATCCCGCCCGGGGCA
+>Caenorhabditis_elegans_tRNA-Ile-TAT-1-3 (tRNAscan-SE ID: chrI.trna57) Ile (TAT) 85 bp Sc: 84.7 chrI:9563842-9563927(-)
+GCCCCGGTGGCCGAGCGGTCGAAGGCGTGAGACTTATGATCTCATTGGGTTAAACCAGTCGCGGGTTCGAATCCCGCCCGGGGCA
+>Caenorhabditis_elegans_tRNA-Ser-TGA-3-1 (tRNAscan-SE ID: chrI.trna19) Ser (TGA) 82 bp Sc: 85.5 chrI:9605755-9605837(+)
+GCAGCGATGTCCGAGTGGTTAAGGAGTTGGACTTGAAATCCAATGGGCTTTGCCCGCGTAGGTTCGAACCCTGCTCGCTGCG
+>Caenorhabditis_elegans_tRX-Lys-CTT-7-3 (tRNAscan-SE ID: chrI.trna20) Lys (CTT) 75 bp Sc: 20.2 chrI:9679643-9679718(+)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttta
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-1 (tRNAscan-SE ID: chrI.trna21) Glu (TTC) 72 bp Sc: 75.3 chrI:9883695-9883767(+)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRX-Pro-TGG-4-1 (tRNAscan-SE ID: chrI.trna56) Pro (TGG) 79 bp Sc: 25.1 chrI:10133600-10133679(-)
+AGCTAGTGGTATGACTAGCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCTCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Gly-GCC-1-2 (tRNAscan-SE ID: chrI.trna22) Gly (GCC) 71 bp Sc: 77.2 chrI:10593136-10593207(+)
+gcatcggtggttcagtggtagaatgctcgcctgccacgcgggcggcccgggttcgattcccggtcgatgca
+>Caenorhabditis_elegans_tRNA-Gly-CCC-1-1 (tRNAscan-SE ID: chrI.trna55) Gly (CCC) 83 bp Sc: 79.1 chrI:10601132-10601215(-)
+GCGGTGGTGGCCGAGCGGTCAAGGCGTAGGACTCCCGATCCTATTCTGGTAACAGAGCGCGGGTTCGAATCCCGTCCACCGCA
+>Caenorhabditis_elegans_tRNA-Gly-CCC-1-2 (tRNAscan-SE ID: chrI.trna23) Gly (CCC) 83 bp Sc: 79.1 chrI:10601850-10601933(+)
+GCGGTGGTGGCCGAGCGGTCAAGGCGTAGGACTCCCGATCCTATTCTGGTAACAGAGCGCGGGTTCGAATCCCGTCCACCGCA
+>Caenorhabditis_elegans_tRNA-Gly-CCC-1-3 (tRNAscan-SE ID: chrI.trna54) Gly (CCC) 83 bp Sc: 79.1 chrI:10604133-10604216(-)
+GCGGTGGTGGCCGAGCGGTCAAGGCGTAGGACTCCCGATCCTATTCTGGTAACAGAGCGCGGGTTCGAATCCCGTCCACCGCA
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-1 (tRNAscan-SE ID: chrI.trna24) Asp (GTC) 72 bp Sc: 61.7 chrI:10807203-10807275(+)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRX-Lys-CTT-8-2 (tRNAscan-SE ID: chrI.trna25) Lys (CTT) 62 bp Sc: 20.7 chrI:10871623-10871685(+)
+gtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRX-Lys-CTT-8-3 (tRNAscan-SE ID: chrI.trna53) Lys (CTT) 62 bp Sc: 20.7 chrI:10872693-10872755(-)
+gtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-7 (tRNAscan-SE ID: chrI.trna52) Gly (TCC) 72 bp Sc: 71.7 chrI:10927412-10927484(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-8 (tRNAscan-SE ID: chrI.trna26) Gly (TCC) 72 bp Sc: 71.7 chrI:10927582-10927654(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Phe-GAA-6-1 (tRNAscan-SE ID: chrI.trna27) Phe (GAA) 82 bp Sc: 56.6 chrI:10945820-10945902(+)
+GCCTCGATAGCTCAGTTGGGGTGAGCGTACGACTGAAAATCGTTAGGTCACCAGTTCGATCCTGGTTCGGGCATTCGGTGCT
+>Caenorhabditis_elegans_tRNA-Gly-GCC-4-1 (tRNAscan-SE ID: chrI.trna28) Gly (GCC) 71 bp Sc: 54.8 chrI:11158626-11158697(+)
+gcattggtggctcagtggtagaatgctcgcctgccacgcgggcagcccgggtccaattcccggtcgatgca
+>Caenorhabditis_elegans_tRNA-Cys-GCA-1-2 (tRNAscan-SE ID: chrI.trna29) Cys (GCA) 72 bp Sc: 74.0 chrI:11505550-11505622(+)
+GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTCCGGGTGCCCCCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-2 (tRNAscan-SE ID: chrI.trna51) Lys (CTT) 73 bp Sc: 85.9 chrI:11579705-11579778(-)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-3 (tRNAscan-SE ID: chrI.trna50) Lys (CTT) 73 bp Sc: 85.9 chrI:11584121-11584194(-)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-4 (tRNAscan-SE ID: chrI.trna30) Lys (CTT) 73 bp Sc: 85.9 chrI:11584786-11584859(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Leu-AAG-2-2 (tRNAscan-SE ID: chrI.trna49) Leu (AAG) 82 bp Sc: 72.6 chrI:11585369-11585451(-)
+GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Ser-CGA-1-1 (tRNAscan-SE ID: chrI.trna48) Ser (CGA) 82 bp Sc: 84.2 chrI:11803315-11803397(-)
+GCAGTCATGTCCGAGTGGTTAAGGAGTTTGACTCGAAATCAAATGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-2 (tRNAscan-SE ID: chrI.trna47) Glu (CTC) 72 bp Sc: 77.9 chrI:11977190-11977262(-)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-3 (tRNAscan-SE ID: chrI.trna31) Glu (CTC) 72 bp Sc: 77.9 chrI:11977991-11978063(+)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-4 (tRNAscan-SE ID: chrI.trna32) Glu (CTC) 72 bp Sc: 77.9 chrI:11978763-11978835(+)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Val-AAC-2-1 (tRNAscan-SE ID: chrI.trna33) Val (AAC) 73 bp Sc: 76.6 chrI:12065864-12065937(+)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-iMet-CAT-1-1 (tRNAscan-SE ID: chrI.trna34) iMet (CAT) 72 bp Sc: 61.2 chrI:12142910-12142982(+)
+AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAACCACTCGCTGCTA
+>Caenorhabditis_elegans_tRNA-Arg-TCT-1-1 (tRNAscan-SE ID: chrI.trna35) Arg (TCT) 73 bp Sc: 71.7 chrI:12198602-12198675(+)
+GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGATCCCTGCCTGGGTCA
+>Caenorhabditis_elegans_tRNA-iMet-CAT-1-2 (tRNAscan-SE ID: chrI.trna46) iMet (CAT) 72 bp Sc: 61.2 chrI:12225425-12225497(-)
+AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAACCACTCGCTGCTA
+>Caenorhabditis_elegans_tRNA-iMet-CAT-1-3 (tRNAscan-SE ID: chrI.trna36) iMet (CAT) 72 bp Sc: 61.2 chrI:12229308-12229380(+)
+AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAACCACTCGCTGCTA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-4-1 (tRNAscan-SE ID: chrI.trna37) Ala (AGC) 74 bp Sc: 55.3 chrI:12601777-12601851(+)
+GTGTAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATAACTCCAGAAACT
+>Caenorhabditis_elegans_tRNA-Val-AAC-2-2 (tRNAscan-SE ID: chrI.trna45) Val (AAC) 73 bp Sc: 76.6 chrI:13156356-13156429(-)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Val-AAC-2-3 (tRNAscan-SE ID: chrI.trna38) Val (AAC) 73 bp Sc: 76.6 chrI:13161060-13161133(+)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-5 (tRNAscan-SE ID: chrI.trna44) Lys (CTT) 73 bp Sc: 85.9 chrI:13297672-13297745(-)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Thr-TGT-1-1 (tRNAscan-SE ID: chrI.trna43) Thr (TGT) 72 bp Sc: 81.0 chrI:13310344-13310416(-)
+GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCCTGCGTGGGGGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-9 (tRNAscan-SE ID: chrI.trna42) Gly (TCC) 72 bp Sc: 71.7 chrI:13324179-13324251(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-5-1 (tRNAscan-SE ID: chrI.trna39) Gly (TCC) 72 bp Sc: 62.2 chrI:13324994-13325066(+)
+GCGTTCGGGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-10 (tRNAscan-SE ID: chrI.trna41) Gly (TCC) 72 bp Sc: 71.7 chrI:13331146-13331218(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Ser-GCT-1-1 (tRNAscan-SE ID: chrI.trna40) Ser (GCT) 82 bp Sc: 84.4 chrI:14162847-14162929(+)
+GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTGAGTTCGAATCTCATCCTGATCG
+>Caenorhabditis_elegans_tRX-Thr-TGT-5-1 (tRNAscan-SE ID: chrII.trna66) Thr (TGT) 74 bp Sc: 22.7 chrII:1102356-1102430(-)
+GTTTTGGCTCGACTGGTAAGAGGTGTGACTTGTGATCAATAGGTCCGGGGTTCGACCCCTCGTAAGGGTCAACA
+>Caenorhabditis_elegans_tRX-Pro-GGG-11-1 (tRNAscan-SE ID: chrII.trna1) Pro (GGG) 72 bp Sc: 24.1 chrII:1331983-1332055(+)
+GCCAGCGTGGCCTAGTGGCTAAGAGTGATGACTGGGGAGCACAAGACCGGGGTTCGAGTCCCCGTTCGGGtt
+>Caenorhabditis_elegans_tRX-Thr-GGT-4-1 (tRNAscan-SE ID: chrII.trna65) Thr (GGT) 79 bp Sc: 29.9 chrII:1476153-1476232(-)
+GAGTTTTTGGCTCAGTCGGTAAGATGAGTGGCTGGTAACCAATAGGTCCGGGGTTCGACCCCCGGTGGTGGAAAACTTT
+>Caenorhabditis_elegans_tRNA-Ser-AGA-2-1 (tRNAscan-SE ID: chrII.trna2) Ser (AGA) 82 bp Sc: 81.6 chrII:1520034-1520116(+)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Leu-AAG-2-3 (tRNAscan-SE ID: chrII.trna64) Leu (AAG) 82 bp Sc: 72.6 chrII:2735793-2735875(-)
+GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Leu-AAG-2-4 (tRNAscan-SE ID: chrII.trna63) Leu (AAG) 82 bp Sc: 72.6 chrII:2736275-2736357(-)
+GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Leu-AAG-2-5 (tRNAscan-SE ID: chrII.trna3) Leu (AAG) 82 bp Sc: 72.6 chrII:2860341-2860423(+)
+GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Leu-AAG-2-6 (tRNAscan-SE ID: chrII.trna62) Leu (AAG) 82 bp Sc: 72.6 chrII:2861549-2861631(-)
+GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Gly-GCC-1-3 (tRNAscan-SE ID: chrII.trna61) Gly (GCC) 71 bp Sc: 77.2 chrII:3062206-3062277(-)
+gcatcggtggttcagtggtagaatgctcgcctgccacgcgggcggcccgggttcgattcccggtcgatgca
+>Caenorhabditis_elegans_tRNA-Gly-GCC-1-4 (tRNAscan-SE ID: chrII.trna4) Gly (GCC) 71 bp Sc: 77.2 chrII:3062383-3062454(+)
+gcatcggtggttcagtggtagaatgctcgcctgccacgcgggcggcccgggttcgattcccggtcgatgca
+>Caenorhabditis_elegans_tRNA-Ser-AGA-2-2 (tRNAscan-SE ID: chrII.trna5) Ser (AGA) 82 bp Sc: 81.6 chrII:3267988-3268070(+)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-1 (tRNAscan-SE ID: chrII.trna60) Thr (AGT) 72 bp Sc: 85.3 chrII:3439218-3439290(-)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-6 (tRNAscan-SE ID: chrII.trna59) Lys (CTT) 73 bp Sc: 85.9 chrII:3439393-3439466(-)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Thr-AGT-2-1 (tRNAscan-SE ID: chrII.trna58) Thr (AGT) 72 bp Sc: 81.2 chrII:3519085-3519157(-)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCC
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-7 (tRNAscan-SE ID: chrII.trna57) Lys (CTT) 73 bp Sc: 85.9 chrII:3519249-3519322(-)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-His-GTG-2-1 (tRNAscan-SE ID: chrII.trna56) His (GTG) 72 bp Sc: 69.4 chrII:3521486-3521558(-)
+GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCCGCAGGCA
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-2 (tRNAscan-SE ID: chrII.trna55) Thr (AGT) 72 bp Sc: 85.3 chrII:3567609-3567681(-)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-8 (tRNAscan-SE ID: chrII.trna54) Lys (CTT) 73 bp Sc: 85.9 chrII:3567763-3567836(-)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRX-Gln-TTG-5-1 (tRNAscan-SE ID: chrII.trna53) Gln (TTG) 70 bp Sc: 22.9 chrII:3980949-3981019(-)
+CGGATGGCTCAGTGGGTAAGAGCAATGCCTTTGGAGCAAAAGGTCAAGGGATCGAGTCCCCGTGAAAAGG
+>Caenorhabditis_elegans_tRNA-Ala-AGC-5-1 (tRNAscan-SE ID: chrII.trna52) Ala (AGC) 74 bp Sc: 49.2 chrII:4565013-4565087(-)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCATTTTCCGTTCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-1 (tRNAscan-SE ID: chrII.trna6) Ala (AGC) 72 bp Sc: 74.8 chrII:4565388-4565460(+)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-3 (tRNAscan-SE ID: chrII.trna7) Ile (AAT) 74 bp Sc: 86.9 chrII:5032769-5032843(+)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-4 (tRNAscan-SE ID: chrII.trna51) Ile (AAT) 74 bp Sc: 86.9 chrII:5057446-5057520(-)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-5 (tRNAscan-SE ID: chrII.trna8) Ile (AAT) 74 bp Sc: 86.9 chrII:5237861-5237935(+)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-2 (tRNAscan-SE ID: chrII.trna9) Ala (AGC) 72 bp Sc: 74.8 chrII:5292331-5292403(+)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-5 (tRNAscan-SE ID: chrII.trna10) Glu (CTC) 72 bp Sc: 77.9 chrII:5293451-5293523(+)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Val-TAC-3-1 (tRNAscan-SE ID: chrII.trna50) Val (TAC) 73 bp Sc: 77.2 chrII:5577199-5577272(-)
+GGTCCTATGGTGTAGTGGTTATCACGTCTGCTTTACACGCAGAAGATCGCCGGTTCGAACCCGGCTAGGACCT
+>Caenorhabditis_elegans_tRNA-Leu-TAA-1-1 (tRNAscan-SE ID: chrII.trna49) Leu (TAA) 84 bp Sc: 77.4 chrII:5772915-5772999(-)
+AGCACGATGGCCGAGTGGTTAAGGCGTTGGACTTAAGTTCCAATGGTGGATAACACCTCGTGGGTTCGAACCCCACTCGTGCTA
+>Caenorhabditis_elegans_tRNA-Gly-GCC-5-1 (tRNAscan-SE ID: chrII.trna48) Gly (GCC) 71 bp Sc: 66.1 chrII:5782211-5782282(-)
+gcatcggtggttcagtggtagaaagctcgcctgccacgcgggcggcccgggttcgattcccggtcgataca
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-1 (tRNAscan-SE ID: chrII.trna11) Lys (TTT) 73 bp Sc: 77.8 chrII:6565247-6565320(+)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-Leu-TAA-3-1 (tRNAscan-SE ID: chrII.trna12) Leu (AAG) 83 bp Sc: 65.0 chrII:6721765-6721848(+)
+GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCAACCAGTAGCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Leu-TAG-1-1 (tRNAscan-SE ID: chrII.trna13) Leu (TAG) 82 bp Sc: 75.3 chrII:6853203-6853285(+)
+GGTGAGATGGCCGAGTGGTCTAAGGCGCTGGTTTTAGGCACCAGTCCCTCCGGGGGCGTGGGTTCGAATCCCACTCTCATCA
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-2 (tRNAscan-SE ID: chrII.trna14) Glu (TTC) 72 bp Sc: 75.3 chrII:6898193-6898265(+)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Ala-TGC-2-1 (tRNAscan-SE ID: chrII.trna15) Ala (TGC) 77 bp Sc: 49.7 chrII:7001621-7001698(+)
+GGGTTACCTGTGTAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-3 (tRNAscan-SE ID: chrII.trna47) Ala (AGC) 72 bp Sc: 74.8 chrII:7002992-7003064(-)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Thr-AGT-3-1 (tRNAscan-SE ID: chrII.trna16) Thr (AGT) 72 bp Sc: 74.8 chrII:7003272-7003344(+)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGTATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-1 (tRNAscan-SE ID: chrII.trna46) Gln (TTG) 72 bp Sc: 72.0 chrII:7756948-7757020(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Leu-TAA-2-1 (tRNAscan-SE ID: chrII.trna45) Leu (TAA) 84 bp Sc: 70.5 chrII:8631956-8632040(-)
+AGCACGATGGCCGAGTGGTTAAGGCGTTGGCCTTAAGTTCCAATGGTGGATAACACCGCGTGGGTTCGAACCCCACTCGTGCTA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-4-1 (tRNAscan-SE ID: chrII.trna44) Tyr (GTA) 84 bp Sc: 67.0 chrII:9211803-9211887(-)
+CAGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGTGGTTATCCTTAGGTCGCTGGTTCGAATCCGGCTCGACGGA
+>Caenorhabditis_elegans_tRNA-Arg-TCG-2-2 (tRNAscan-SE ID: chrII.trna17) Arg (TCG) 73 bp Sc: 71.0 chrII:9566240-9566313(+)
+GGCCGCGTGGCCTAATGGATAAGGCACCAGACTTCGAATCTGGGGATTGCAGGTTCGAGTCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Phe-GAA-1-1 (tRNAscan-SE ID: chrII.trna43) Phe (GAA) 73 bp Sc: 82.3 chrII:9713223-9713296(-)
+GCCTCGATAGCTCAGTTGGGAGAGCGCACGACTGAAGATCGTGAGGTCACCAGTTCGATCCTGGTTCGGGGCA
+>Caenorhabditis_elegans_tRX-Lys-CTT-3-1 (tRNAscan-SE ID: chrII.trna18) Lys (CTT) 75 bp Sc: 47.6 chrII:9773653-9773728(+)
+GCCCGGTTAGCTCAGTCTACCGACTGCACCAGACTCTTAATCTGGTTGTCGTGGGTTCGAGTCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRX-Met-CAT-2-1 (tRNAscan-SE ID: chrII.trna19) Met (CAT) 77 bp Sc: 24.8 chrII:10009014-10009091(+)
+GTACTCTACTCTAGACACTATGAGAGCGCGTCAGTCTCATATTCTGAAGGTCGTGAGTTCGAGCCTCACCGGGAGCA
+>Caenorhabditis_elegans_tRNA-Pro-TGG-2-1 (tRNAscan-SE ID: chrII.trna42) Pro (TGG) 72 bp Sc: 69.2 chrII:10302158-10302230(-)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGCTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-1 (tRNAscan-SE ID: chrII.trna20) Pro (TGG) 72 bp Sc: 75.2 chrII:10302398-10302470(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-TGG-7-1 (tRNAscan-SE ID: chrII.trna41) Pro (TGG) 72 bp Sc: 65.7 chrII:10304770-10304842(-)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCTGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-2 (tRNAscan-SE ID: chrII.trna21) Pro (TGG) 72 bp Sc: 75.2 chrII:10305010-10305082(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-9 (tRNAscan-SE ID: chrII.trna40) Lys (CTT) 73 bp Sc: 85.9 chrII:11157801-11157874(-)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Ala-TGC-1-1 (tRNAscan-SE ID: chrII.trna39) Ala (TGC) 72 bp Sc: 68.8 chrII:11334012-11334084(-)
+GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ala-TGC-1-2 (tRNAscan-SE ID: chrII.trna22) Ala (TGC) 72 bp Sc: 68.8 chrII:11334507-11334579(+)
+GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRX-Lys-CTT-9-1 (tRNAscan-SE ID: chrII.trna23) Lys (CTT) 75 bp Sc: 24.6 chrII:11441189-11441264(+)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttca
+>Caenorhabditis_elegans_tRX-Lys-CTT-7-4 (tRNAscan-SE ID: chrII.trna38) Lys (CTT) 75 bp Sc: 20.2 chrII:11442249-11442324(-)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttta
+>Caenorhabditis_elegans_tRX-Ser-AGA-1-1 (tRNAscan-SE ID: chrII.trna37) Ser (AGA) 97 bp Sc: 30.0 chrII:11518856-11518953(-)
+GGCATTATGCGTCCGTGGCGAATCACCTGTGTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCGTTA
+>Caenorhabditis_elegans_tRNA-Val-TAC-4-1 (tRNAscan-SE ID: chrII.trna24) Val (TAC) 73 bp Sc: 72.9 chrII:11959374-11959447(+)
+GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTTACACGCAGTAGGCCGCCGGTTCGATCCCGGCCAGGACCT
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-6 (tRNAscan-SE ID: chrII.trna25) Ile (AAT) 74 bp Sc: 86.9 chrII:12362448-12362522(+)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-iMet-CAT-1-4 (tRNAscan-SE ID: chrII.trna36) iMet (CAT) 72 bp Sc: 61.2 chrII:12435579-12435651(-)
+AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAACCACTCGCTGCTA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-7 (tRNAscan-SE ID: chrII.trna26) Ile (AAT) 74 bp Sc: 86.9 chrII:12494740-12494814(+)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Trp-CCA-3-1 (tRNAscan-SE ID: chrII.trna27) Trp (CCA) 72 bp Sc: 64.3 chrII:12539596-12539668(+)
+GACTGCTTGGCGCAATGATAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCCGCTCAGTGGTCA
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-2 (tRNAscan-SE ID: chrII.trna35) Lys (TTT) 73 bp Sc: 77.8 chrII:12541687-12541760(-)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCt
+>Caenorhabditis_elegans_tRNA-Leu-AAG-2-7 (tRNAscan-SE ID: chrII.trna34) Leu (AAG) 82 bp Sc: 72.6 chrII:12541929-12542011(-)
+GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-4 (tRNAscan-SE ID: chrII.trna28) Ala (AGC) 72 bp Sc: 74.8 chrII:12542633-12542705(+)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ala-TGC-1-3 (tRNAscan-SE ID: chrII.trna29) Ala (TGC) 72 bp Sc: 68.8 chrII:12678313-12678385(+)
+GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Arg-CCG-1-1 (tRNAscan-SE ID: chrII.trna33) Arg (CCG) 72 bp Sc: 53.8 chrII:12728754-12728826(-)
+GCTCGCGTGGCCTAATGGATAAGGCACCGGACTCCGGAACCGGGAATGGGGGTTCAAGTCCCTCCGCGAGCT
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-2 (tRNAscan-SE ID: chrII.trna32) Gln (TTG) 72 bp Sc: 72.0 chrII:14474841-14474913(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRX-Asn-GTT-2-1 (tRNAscan-SE ID: chrII.trna30) Asn (GTT) 71 bp Sc: 21.6 chrII:14617081-14617152(+)
+TCGCGTGGCGCAGGCGGTAGCGCATTTCGCTGTTGATCAAGAGGCCACAGGTTCGCCTCCCGTGCGATGAA
+>Caenorhabditis_elegans_tRNA-Leu-AAG-1-1 (tRNAscan-SE ID: chrII.trna31) Leu (AAG) 82 bp Sc: 73.6 chrII:14635334-14635416(-)
+GGTGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCATCA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-2-2 (tRNAscan-SE ID: chrIII.trna1) Tyr (GTA) 84 bp Sc: 74.6 chrIII:535381-535465(+)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTTAGCAGGTATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-8 (tRNAscan-SE ID: chrIII.trna81) Ile (AAT) 74 bp Sc: 86.9 chrIII:1163353-1163427(-)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-9 (tRNAscan-SE ID: chrIII.trna80) Ile (AAT) 74 bp Sc: 86.9 chrIII:1164799-1164873(-)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-10 (tRNAscan-SE ID: chrIII.trna79) Ile (AAT) 74 bp Sc: 86.9 chrIII:1218375-1218449(-)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-11 (tRNAscan-SE ID: chrIII.trna2) Gly (TCC) 72 bp Sc: 71.7 chrIII:1424490-1424562(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRX-Arg-TCG-7-1 (tRNAscan-SE ID: chrIII.trna3) Arg (TCG) 75 bp Sc: 20.2 chrIII:1575428-1575503(+)
+CACCCCGTGGCGCAGTGGCTAACAGGCTTGACTTCGGAGCAAATGGTCCCGGGGTTCGAGTCCCCGCAGTGGTGT
+>Caenorhabditis_elegans_tRX-Gln-TTG-3-1 (tRNAscan-SE ID: chrIII.trna78) Gln (TTG) 76 bp Sc: 20.4 chrIII:1575774-1575850(-)
+GCAACGCGTGGCGCAGTGGCTAAGCGGCTCGCCTTTGGAGCAAAAGGTCCGGGGTTCGATTCTCCGTGGGGGTGTA
+>Caenorhabditis_elegans_tRX-Arg-TCG-6-1 (tRNAscan-SE ID: chrIII.trna4) Arg (TCG) 73 bp Sc: 29.8 chrIII:1575871-1575944(+)
+GCACCGGTGGCGCAGTGGCTAACAGGCTTGACTTCGGAGCAAAAGGTCCGGGGTTCGAGTCCCCGTGGGAGTA
+>Caenorhabditis_elegans_tRX-Gln-TTG-2-1 (tRNAscan-SE ID: chrIII.trna77) Gln (TTG) 71 bp Sc: 29.8 chrIII:1577007-1577078(-)
+ACCGGTGGCGCAGTGGCTAAGCGGCTTGCCTTTGGAGCAAAAGGTCCCGGGTTCGAGTCCCCGTGGAGGTA
+>Caenorhabditis_elegans_tRX-Ser-CGA-6-1 (tRNAscan-SE ID: chrIII.trna5) Ser (CGA) 73 bp Sc: 30.1 chrIII:1577100-1577173(+)
+GCACCGGTGGCGCAGTGGCTAAGAGGTTTGCCTTTGGAGCAAAAGGTCGGGGGTTCGAGTCCCCGTGGGGGTA
+>Caenorhabditis_elegans_tRX-Ser-CGA-5-1 (tRNAscan-SE ID: chrIII.trna76) Ser (CGA) 75 bp Sc: 30.4 chrIII:1577315-1577390(-)
+GCACCGGTGGCGCAGTGGCTAAGAGGTTTGCCTTCGGAGCAAAAGGTCGGGGGTTCGAGTCCCCGCAGTGGTATA
+>Caenorhabditis_elegans_tRX-Ser-CGA-7-1 (tRNAscan-SE ID: chrIII.trna6) Ser (CGA) 70 bp Sc: 32.1 chrIII:1577412-1577482(+)
+ACCGGTGGCGCAGTGGCTAAGAGGTTTGCCTTTGGAGCAAAAGGTCGGGGTTCGAGTCCCCGTGGGGGTA
+>Caenorhabditis_elegans_tRNA-iMet-CAT-1-5 (tRNAscan-SE ID: chrIII.trna7) iMet (CAT) 72 bp Sc: 61.2 chrIII:1604581-1604653(+)
+AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAACCACTCGCTGCTA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-6 (tRNAscan-SE ID: chrIII.trna75) Glu (CTC) 72 bp Sc: 77.9 chrIII:1604701-1604773(-)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-7 (tRNAscan-SE ID: chrIII.trna8) Glu (CTC) 72 bp Sc: 77.9 chrIII:2032517-2032589(+)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-8 (tRNAscan-SE ID: chrIII.trna74) Glu (CTC) 72 bp Sc: 77.9 chrIII:2032896-2032968(-)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-3 (tRNAscan-SE ID: chrIII.trna9) Pro (TGG) 72 bp Sc: 75.2 chrIII:2711710-2711782(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRX-Leu-GAG-5-1 (tRNAscan-SE ID: chrIII.trna10) Leu (GAG) 70 bp Sc: 21.4 chrIII:3101087-3101157(+)
+ttttggcgcagtggctaacagggatggctgagacccataagaccggggttcgaatccccgctgtggTGAA
+>Caenorhabditis_elegans_tRX-Leu-GAG-6-1 (tRNAscan-SE ID: chrIII.trna73) Leu (GAG) 72 bp Sc: 20.2 chrIII:3104057-3104129(-)
+TTTTGGCCTAGTGGTTAACACGGATGGCTGAGACCCATAGGGCCGGGGTTCGAGCCCCCACCGGGGTAAAAT
+>Caenorhabditis_elegans_tRX-Pro-GGG-7-1 (tRNAscan-SE ID: chrIII.trna11) Pro (GGG) 77 bp Sc: 23.0 chrIII:3105137-3105214(+)
+AGCTGAACGTTTGGCGTAGTGGCTAACACGGATGGCTGGGACtcacaagaccggggttcgagtccccgctgtggcca
+>Caenorhabditis_elegans_tRX-Pro-GGG-9-1 (tRNAscan-SE ID: chrIII.trna12) Pro (GGG) 73 bp Sc: 20.9 chrIII:3110797-3110870(+)
+GAATTTTTGGCCTAGTGGCTAAGAGGGATGGCTGGGGCCCACAAGACCGGGGTTCGAGTCCCTGAGGGGGTCA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-7-1 (tRNAscan-SE ID: chrIII.trna13) Tyr (GTA) 85 bp Sc: 49.5 chrIII:3195437-3195522(+)
+ACCTGTGAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGATT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-10 (tRNAscan-SE ID: chrIII.trna14) Lys (CTT) 73 bp Sc: 85.9 chrIII:3389536-3389609(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-11 (tRNAscan-SE ID: chrIII.trna72) Lys (CTT) 73 bp Sc: 85.9 chrIII:3426912-3426985(-)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Leu-CAA-1-1 (tRNAscan-SE ID: chrIII.trna15) Leu (CAA) 120 bp Sc: 74.2 chrIII:4362523-4362643(+)
+GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCGTAACGCTTACCTCAAGTTCGAGGTCTACTGGGTGTTCTGGTACTCGTATGGGTGCGTGGGTTCGAATCCCACTTCGTGCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-3-1 (tRNAscan-SE ID: chrIII.trna71) Ala (AGC) 71 bp Sc: 65.7 chrIII:4428952-4429023(-)
+GGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Arg-ACG-1-2 (tRNAscan-SE ID: chrIII.trna70) Arg (ACG) 73 bp Sc: 72.1 chrIII:4449532-4449605(-)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGCAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Arg-ACG-1-3 (tRNAscan-SE ID: chrIII.trna69) Arg (ACG) 73 bp Sc: 72.1 chrIII:4450323-4450396(-)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGCAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Arg-TCG-2-3 (tRNAscan-SE ID: chrIII.trna68) Arg (TCG) 73 bp Sc: 71.0 chrIII:4470885-4470958(-)
+GGCCGCGTGGCCTAATGGATAAGGCACCAGACTTCGAATCTGGGGATTGCAGGTTCGAGTCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-iMet-CAT-1-6 (tRNAscan-SE ID: chrIII.trna67) iMet (CAT) 72 bp Sc: 61.2 chrIII:5294978-5295050(-)
+AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAACCACTCGCTGCTA
+>Caenorhabditis_elegans_tRNA-Thr-TGT-1-2 (tRNAscan-SE ID: chrIII.trna16) Thr (TGT) 72 bp Sc: 81.0 chrIII:5305904-5305976(+)
+GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCCTGCGTGGGGGCA
+>Caenorhabditis_elegans_tRNA-Gly-GCC-3-1 (tRNAscan-SE ID: chrIII.trna66) Gly (GCC) 70 bp Sc: 67.6 chrIII:5762056-5762126(-)
+gcatcggtggttcagtggtagaatgctcgcctgccacgcggcggcccgggttcgattcccggtcgatgca
+>Caenorhabditis_elegans_tRNA-Gly-GCC-1-5 (tRNAscan-SE ID: chrIII.trna17) Gly (GCC) 71 bp Sc: 77.2 chrIII:5762285-5762356(+)
+gcatcggtggttcagtggtagaatgctcgcctgccacgcgggcggcccgggttcgattcccggtcgatgca
+>Caenorhabditis_elegans_tRNA-Leu-AAG-5-1 (tRNAscan-SE ID: chrIII.trna18) Leu (AAG) 82 bp Sc: 50.1 chrIII:5769903-5769985(+)
+GGAGAGATGGCCGAGCGGTCCAAGGCGCTGGTTTAAGGCACCGTTCCATTCGGGGGCGTGGGTTCGAATCCCACTCTCTTAA
+>Caenorhabditis_elegans_tRNA-Gly-GCC-1-6 (tRNAscan-SE ID: chrIII.trna65) Gly (GCC) 71 bp Sc: 77.2 chrIII:5782235-5782306(-)
+gcatcggtggttcagtggtagaatgctcgcctgccacgcgggcggcccgggttcgattcccggtcgatgca
+>Caenorhabditis_elegans_tRNA-Ser-GCT-1-2 (tRNAscan-SE ID: chrIII.trna64) Ser (GCT) 82 bp Sc: 84.4 chrIII:6056298-6056380(-)
+GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTGAGTTCGAATCTCATCCTGATCG
+>Caenorhabditis_elegans_tRX-Phe-GAA-2-1 (tRNAscan-SE ID: chrIII.trna19) Phe (GAA) 73 bp Sc: 36.5 chrIII:6153389-6153462(+)
+GCTTTACCTGTGCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATCCTGGTTTGGGGCA
+>Caenorhabditis_elegans_tRNA-Ser-AGA-2-3 (tRNAscan-SE ID: chrIII.trna20) Ser (AGA) 82 bp Sc: 81.6 chrIII:6158777-6158859(+)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Ser-CGA-3-1 (tRNAscan-SE ID: chrIII.trna21) Ser (CGA) 86 bp Sc: 59.1 chrIII:6158964-6159050(+)
+GTGGTTAAGAATGTCCGAGTGGTTAAGGAGTTTGACTCGAAATCAAATGGGCTCTGTCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRX-Ser-GCT-4-1 (tRNAscan-SE ID: chrIII.trna63) Ser (GCT) 77 bp Sc: 20.4 chrIII:6501555-6501632(-)
+CGGTATACCTGTGTAAGGCGATGGACTGCTAATCCATTGGGATTTTCCCGCGTGAGTTCGAATCTCATCCTGATCGA
+>Caenorhabditis_elegans_tRNA-Ser-CGA-2-1 (tRNAscan-SE ID: chrIII.trna62) Ser (CGA) 82 bp Sc: 81.6 chrIII:6513936-6514018(-)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTCGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Ala-AGC-7-1 (tRNAscan-SE ID: chrIII.trna22) Ala (AGC) 395 bp Sc: 53.1 chrIII:6590173-6590568(+)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGACACAGGTGATTCGCGAGTACGAGTTTTATGCTTCATCCGAGGTTCGCGCGTGCTTCGAATGGGTACTTGAAAACATGAGCAAAAATGGAGAAAAATGCTCGTCTTTGCGAACGAACGCGAGCATAAAGGAGGCATTGCGAAAACAATTTATGCTTCTTTTTTTTCACTTATATCAGCTGAAAAAGTTCAAAATATAACTTCAGTTCTTGTATAAGCCACCCCCACTACCCGAAGACATGATTAAGCCACCTCAAGACATTTTCGCAAACACGAGCATTGTGTGCGTCGAAGCATTTTGCTTACACTGCGAATCACCTGTGGGAGAGGGTTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Lys-CTT-4-1 (tRNAscan-SE ID: chrIII.trna61) Lys (CTT) 86 bp Sc: 72.1 chrIII:6724134-6724220(-)
+GACACGGTGGCCGAGTGGTTTAAGGCATGAGACACTTGATCTCAAACGGTTCTAACCGAACGCAGGTTCGAATCCTGCCCGTGTCA
+>Caenorhabditis_elegans_tRNA-Arg-CCT-2-1 (tRNAscan-SE ID: chrIII.trna60) Arg (CCT) 86 bp Sc: 68.7 chrIII:6726990-6727076(-)
+GCCACGGTGGCCGAGTGTGGTCAAAGGCGTGAGACTCCTGATCTCTTTCGGGCAACCGATCGCAGGTTCGAATCCTGCCCGTGGCA
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-2 (tRNAscan-SE ID: chrIII.trna23) Asn (GTT) 73 bp Sc: 73.5 chrIII:6805567-6805640(+)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-3 (tRNAscan-SE ID: chrIII.trna59) Lys (TTT) 73 bp Sc: 77.8 chrIII:6887727-6887800(-)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-12 (tRNAscan-SE ID: chrIII.trna58) Gly (TCC) 72 bp Sc: 71.7 chrIII:6888609-6888681(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-13 (tRNAscan-SE ID: chrIII.trna24) Gly (TCC) 72 bp Sc: 71.7 chrIII:6888805-6888877(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-3 (tRNAscan-SE ID: chrIII.trna57) Thr (AGT) 72 bp Sc: 85.3 chrIII:7030556-7030628(-)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-2-1 (tRNAscan-SE ID: chrIII.trna56) Glu (CTC) 72 bp Sc: 73.2 chrIII:7642157-7642229(-)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACTCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Phe-GAA-2-1 (tRNAscan-SE ID: chrIII.trna55) Phe (GAA) 73 bp Sc: 82.5 chrIII:7978470-7978543(-)
+gcctcgatagctcagttgggagagcgtacgactgaagatcgtaaggtcaccagttcgatccTGGTTCGGGGCA
+>Caenorhabditis_elegans_tRNA-Pro-TGG-4-1 (tRNAscan-SE ID: chrIII.trna25) Pro (TGG) 72 bp Sc: 66.3 chrIII:8069404-8069476(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTGAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Met-CAT-1-2 (tRNAscan-SE ID: chrIII.trna26) Met (CAT) 73 bp Sc: 77.0 chrIII:8106652-8106725(+)
+GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGCCTCACCGGGAGCA
+>Caenorhabditis_elegans_tRNA-Leu-CAA-1-2 (tRNAscan-SE ID: chrIII.trna27) Leu (CAA) 122 bp Sc: 74.1 chrIII:8109602-8109724(+)
+GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCGTACATTGCTTGCCTCAAGTTCGAGGTTAACTGGGTGTTCTGGTACTCGTATGGGTGCGTGGGTTCGAATCCCACTTCGTGCA
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-12 (tRNAscan-SE ID: chrIII.trna28) Lys (CTT) 73 bp Sc: 85.9 chrIII:8473472-8473545(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Leu-CAA-1-3 (tRNAscan-SE ID: chrIII.trna29) Leu (CAA) 120 bp Sc: 74.2 chrIII:8639305-8639425(+)
+GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCGAAATGCTTGCCTCATGCTCGAGGTCGACTGGGTGTTCTGGTACTCGTATGGGTGCGTGGGTTCGAATCCCACTTCGTGCA
+>Caenorhabditis_elegans_tRNA-Ser-AGA-2-4 (tRNAscan-SE ID: chrIII.trna30) Ser (AGA) 82 bp Sc: 81.6 chrIII:8646166-8646248(+)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Pro-CGG-1-1 (tRNAscan-SE ID: chrIII.trna54) Pro (CGG) 72 bp Sc: 71.5 chrIII:8650380-8650452(-)
+GGCCGGATGGTCTAGAGGTATGATTCTCGCTTCGGGTGCGAGAGGTCCCGGGTTCGATTCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Phe-GAA-2-2 (tRNAscan-SE ID: chrIII.trna31) Phe (GAA) 73 bp Sc: 82.5 chrIII:8653054-8653127(+)
+GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATCCTGGTTCGGGGCA
+>Caenorhabditis_elegans_tRNA-Phe-GAA-2-3 (tRNAscan-SE ID: chrIII.trna53) Phe (GAA) 73 bp Sc: 82.5 chrIII:8653607-8653680(-)
+GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATCCTGGTTCGGGGCA
+>Caenorhabditis_elegans_tRNA-Trp-CCA-1-2 (tRNAscan-SE ID: chrIII.trna52) Trp (CCA) 72 bp Sc: 71.5 chrIII:8678496-8678568(-)
+GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCCGCTCAGTGGTCA
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-3 (tRNAscan-SE ID: chrIII.trna51) Asn (GTT) 73 bp Sc: 73.5 chrIII:9104206-9104279(-)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Ser-CGA-1-2 (tRNAscan-SE ID: chrIII.trna50) Ser (CGA) 82 bp Sc: 84.2 chrIII:9861606-9861688(-)
+GCAGTCATGTCCGAGTGGTTAAGGAGTTTGACTCGAAATCAAATGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Ser-AGA-1-1 (tRNAscan-SE ID: chrIII.trna49) Ser (AGA) 82 bp Sc: 82.3 chrIII:9862021-9862103(-)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTTTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-4 (tRNAscan-SE ID: chrIII.trna48) Thr (AGT) 72 bp Sc: 85.3 chrIII:10624741-10624813(-)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRX-Arg-GCG-8-1 (tRNAscan-SE ID: chrIII.trna47) Arg (GCG) 69 bp Sc: 23.8 chrIII:10961846-10961915(-)
+GCAGTGGCTCAACTGGGTAGAGCTTTGCCTGCGACGCATAAGACCAGGGTTCGAGTCCCGCTGTAGGTT
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-4 (tRNAscan-SE ID: chrIII.trna46) Pro (TGG) 72 bp Sc: 75.2 chrIII:11066847-11066919(-)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-5 (tRNAscan-SE ID: chrIII.trna32) Pro (TGG) 72 bp Sc: 75.2 chrIII:11067026-11067098(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Val-AAC-2-4 (tRNAscan-SE ID: chrIII.trna33) Val (AAC) 73 bp Sc: 76.6 chrIII:11353028-11353101(+)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Val-AAC-2-5 (tRNAscan-SE ID: chrIII.trna34) Val (AAC) 73 bp Sc: 76.6 chrIII:11353627-11353700(+)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRX-Ala-CGC-5-1 (tRNAscan-SE ID: chrIII.trna35) Ala (CGC) 65 bp Sc: 20.9 chrIII:11478961-11479026(+)
+GATAGCTCAGTCGGTAGGGCGGATGACTCGCGCTCTGAAGATCGTGGGTTCGAGTCCGCGCACCA
+>Caenorhabditis_elegans_tRNA-Phe-GAA-2-4 (tRNAscan-SE ID: chrIII.trna36) Phe (GAA) 73 bp Sc: 82.5 chrIII:11554824-11554897(+)
+GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATCCTGGTTCGGGGCA
+>Caenorhabditis_elegans_tRNA-Thr-CGT-2-1 (tRNAscan-SE ID: chrIII.trna37) Thr (CGT) 72 bp Sc: 76.0 chrIII:11792781-11792853(+)
+GCCCGTATAGCTCAGTGGCAGAGCGTCTGTCTCGTAAACAGAAGGTCGGCGGTTCAATCCCGCCTGGGGGCA
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-3 (tRNAscan-SE ID: chrIII.trna45) Gln (TTG) 72 bp Sc: 72.0 chrIII:12399908-12399980(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Ser-GCT-3-1 (tRNAscan-SE ID: chrIII.trna38) Ser (GCT) 77 bp Sc: 54.4 chrIII:13009422-13009499(+)
+GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTCAAATCTCATCCTGATCG
+>Caenorhabditis_elegans_tRNA-Thr-CGT-2-2 (tRNAscan-SE ID: chrIII.trna44) Thr (CGT) 72 bp Sc: 76.0 chrIII:13016106-13016178(-)
+GCCCGTATAGCTCAGTGGCAGAGCGTCTGTCTCGTAAACAGAAGGTCGGCGGTTCAATCCCGCCTGGGGGCA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-2-3 (tRNAscan-SE ID: chrIII.trna39) Tyr (GTA) 84 bp Sc: 74.6 chrIII:13224565-13224649(+)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTTAGCAGGTATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGA
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-4 (tRNAscan-SE ID: chrIII.trna43) Asn (GTT) 73 bp Sc: 73.5 chrIII:13225161-13225234(-)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Thr-TGT-1-3 (tRNAscan-SE ID: chrIII.trna42) Thr (TGT) 72 bp Sc: 81.0 chrIII:13411365-13411437(-)
+GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCCTGCGTGGGGGCA
+>Caenorhabditis_elegans_tRX-Lys-CTT-7-5 (tRNAscan-SE ID: chrIII.trna40) Lys (CTT) 75 bp Sc: 20.2 chrIII:13522278-13522353(+)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttta
+>Caenorhabditis_elegans_tRX-Lys-CTT-7-6 (tRNAscan-SE ID: chrIII.trna41) Lys (CTT) 75 bp Sc: 20.2 chrIII:13523339-13523414(-)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttta
+>Caenorhabditis_elegans_tRNA-Arg-CCT-1-1 (tRNAscan-SE ID: chrIV.trna1) Arg (CCT) 73 bp Sc: 69.7 chrIV:143981-144054(+)
+GGCCGTGTGGCCTAATGGATAAGGCGTCGGTCTCCTAAACCGAAGACTGCAGGTTCGAGTCCTGCCTCGGTCG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-2 (tRNAscan-SE ID: chrIV.trna82) Asp (GTC) 72 bp Sc: 61.7 chrIV:322631-322703(-)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Val-CAC-2-1 (tRNAscan-SE ID: chrIV.trna2) Val (CAC) 73 bp Sc: 78.8 chrIV:620481-620554(+)
+GGTCCTCTGGTGTAGTGGTTATCACGTCTGCTTCACACGCAGAAGGTCGCCGGTTCGAACCCGGCGAGGACCT
+>Caenorhabditis_elegans_tRNA-SeC-TCA-1-1 (tRNAscan-SE ID: chrIV.trna3) SeC (TCA) 87 bp Sc: 107.4 chrIV:658180-658267(+)
+GCCCGGATGAACCATGGCGGTCTGTGGTGCAGACTTCAAATCTGTAGGCGGTTAGCGCCGCAGTGGTTCGACTCCACCTTTCGGGTG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-3 (tRNAscan-SE ID: chrIV.trna4) Asp (GTC) 72 bp Sc: 61.7 chrIV:683062-683134(+)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-3 (tRNAscan-SE ID: chrIV.trna5) Glu (TTC) 72 bp Sc: 75.3 chrIV:842808-842880(+)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRX-Und-NNN-6-1 (tRNAscan-SE ID: chrIV.trna81) Und (NNN) 73 bp Sc: 21.9 chrIV:1144683-1144756(-)
+GGCCAACTGGCTCAGCCGGGTAGGAGCTCTACTGGCAATCACAAGGCCGGGGTTCGAACCCCCGACGTGGCTA
+>Caenorhabditis_elegans_tRX-Arg-TCG-9-1 (tRNAscan-SE ID: chrIV.trna6) Arg (TCG) 72 bp Sc: 24.5 chrIV:1365190-1365262(+)
+GTCGCAGTGGCTCAACTGGGTAGAGGTTGGGCTTCGACTCAGAAGCCCGGGGTTCGAACCCCGGGTGTGGCG
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-4 (tRNAscan-SE ID: chrIV.trna80) Glu (TTC) 72 bp Sc: 75.3 chrIV:1388215-1388287(-)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRX-Asp-GTC-1-1 (tRNAscan-SE ID: chrIV.trna79) Asp (GTC) 86 bp Sc: 36.6 chrIV:1462857-1462943(-)
+TCCTCGGTAGTGGTGAGTATCCGCGTCTGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTCCCGGCCGGGGAG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-4 (tRNAscan-SE ID: chrIV.trna7) Asp (GTC) 72 bp Sc: 61.7 chrIV:1514591-1514663(+)
+TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTCCCGGCCGGGGAG
+>Caenorhabditis_elegans_tRNA-Glu-TTC-2-1 (tRNAscan-SE ID: chrIV.trna78) Glu (TTC) 72 bp Sc: 64.7 chrIV:2639808-2639880(-)
+TCCTATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGTTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Asp-GTC-1-1 (tRNAscan-SE ID: chrIV.trna8) Asp (GTC) 72 bp Sc: 63.3 chrIV:2800098-2800170(+)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgaggcccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-5 (tRNAscan-SE ID: chrIV.trna77) Asp (GTC) 72 bp Sc: 61.7 chrIV:2801150-2801222(-)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-3-1 (tRNAscan-SE ID: chrIV.trna9) Asp (GTC) 72 bp Sc: 60.5 chrIV:2802336-2802408(+)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcgcatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-4-1 (tRNAscan-SE ID: chrIV.trna10) Asp (GTC) 72 bp Sc: 58.7 chrIV:2805626-2805698(+)
+TCCtcggtagtgtagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-5-1 (tRNAscan-SE ID: chrIV.trna11) Asp (GTC) 72 bp Sc: 52.2 chrIV:2808354-2808426(+)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccggtgAG
+>Caenorhabditis_elegans_tRX-Lys-CTT-7-7 (tRNAscan-SE ID: chrIV.trna76) Lys (CTT) 75 bp Sc: 20.2 chrIV:3501646-3501721(-)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttta
+>Caenorhabditis_elegans_tRNA-Arg-ACG-1-4 (tRNAscan-SE ID: chrIV.trna12) Arg (ACG) 73 bp Sc: 72.1 chrIV:3524818-3524891(+)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGCAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Pro-CGG-1-2 (tRNAscan-SE ID: chrIV.trna75) Pro (CGG) 72 bp Sc: 71.5 chrIV:3552188-3552260(-)
+GGCCGGATGGTCTAGAGGTATGATTCTCGCTTCGGGTGCGAGAGGTCCCGGGTTCGATTCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRX-Lys-CTT-5-1 (tRNAscan-SE ID: chrIV.trna13) Lys (CTT) 62 bp Sc: 26.1 chrIV:3589268-3589330(+)
+gtggccgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRX-Lys-CTT-5-2 (tRNAscan-SE ID: chrIV.trna74) Lys (CTT) 62 bp Sc: 26.1 chrIV:3590295-3590357(-)
+gtggccgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRNA-Trp-CCA-1-3 (tRNAscan-SE ID: chrIV.trna73) Trp (CCA) 72 bp Sc: 71.5 chrIV:3681879-3681951(-)
+GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCCGCTCAGTGGTCA
+>Caenorhabditis_elegans_tRX-Und-NNN-3-1 (tRNAscan-SE ID: chrIV.trna72) Und (NNN) 70 bp Sc: 35.6 chrIV:4106573-4106643(-)
+GCGGTGGCTCAGTCGGTAAGAGAGTTGGTTGGGGTGCAGAAGGCCGCGGGTTCGATTCCCGCTAGCTGCA
+>Caenorhabditis_elegans_tRNA-His-GTG-5-1 (tRNAscan-SE ID: chrIV.trna14) His (GTG) 84 bp Sc: 56.3 chrIV:4861739-4861823(+)
+GCCTGCTTAGTATATACTACTATACAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCAGCAGGCA
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-4 (tRNAscan-SE ID: chrIV.trna15) Lys (TTT) 73 bp Sc: 77.8 chrIV:5038919-5038992(+)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-Gln-CTG-2-1 (tRNAscan-SE ID: chrIV.trna16) Gln (CTG) 72 bp Sc: 71.6 chrIV:5334711-5334783(+)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTCTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGGACCT
+>Caenorhabditis_elegans_tRNA-Trp-CCA-1-4 (tRNAscan-SE ID: chrIV.trna71) Trp (CCA) 72 bp Sc: 71.5 chrIV:5344299-5344371(-)
+GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCCGCTCAGTGGTCA
+>Caenorhabditis_elegans_tRX-Lys-CTT-8-4 (tRNAscan-SE ID: chrIV.trna17) Lys (CTT) 62 bp Sc: 20.7 chrIV:5349354-5349416(+)
+gtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-13 (tRNAscan-SE ID: chrIV.trna18) Lys (CTT) 73 bp Sc: 85.9 chrIV:5967159-5967232(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRX-Val-AAC-1-1 (tRNAscan-SE ID: chrIV.trna19) Val (AAC) 82 bp Sc: 47.9 chrIV:6470290-6470372(+)
+GGTTTCGTGGTGTACACACTATAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTTGAGCCGGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Val-CAC-1-1 (tRNAscan-SE ID: chrIV.trna20) Val (CAC) 73 bp Sc: 80.7 chrIV:6481160-6481233(+)
+GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTCACACGCAGAAGGTCGCCGGTTCGAACCCGGCCAGGACCT
+>Caenorhabditis_elegans_tRNA-Leu-CAG-1-1 (tRNAscan-SE ID: chrIV.trna21) Leu (CAG) 84 bp Sc: 77.8 chrIV:6556817-6556901(+)
+GCCGTTCTGGCCGAGTGGTCTAAGGCGCTGCGTTCAGGTCGCAGTCCTCTCAGGAGGGCGCAGGTTCGAACCCTGCGGACGGCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-2-1 (tRNAscan-SE ID: chrIV.trna22) Ala (AGC) 72 bp Sc: 67.2 chrIV:6562201-6562273(+)
+GGGGGTATAGCTCAGTAGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-4 (tRNAscan-SE ID: chrIV.trna23) Gln (TTG) 72 bp Sc: 72.0 chrIV:7275326-7275398(+)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Trp-CCA-1-5 (tRNAscan-SE ID: chrIV.trna70) Trp (CCA) 72 bp Sc: 71.5 chrIV:7344155-7344227(-)
+GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCCGCTCAGTGGTCA
+>Caenorhabditis_elegans_tRNA-Thr-TGT-1-4 (tRNAscan-SE ID: chrIV.trna69) Thr (TGT) 72 bp Sc: 81.0 chrIV:9000803-9000875(-)
+GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCCTGCGTGGGGGCA
+>Caenorhabditis_elegans_tRX-Gln-TTG-1-1 (tRNAscan-SE ID: chrIV.trna68) Gln (TTG) 78 bp Sc: 21.3 chrIV:10305189-10305267(-)
+GCATGAAACGCGAATCACCTGTGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTTGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-5 (tRNAscan-SE ID: chrIV.trna67) Gln (TTG) 72 bp Sc: 72.0 chrIV:10311230-10311302(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Pro-AGG-4-3 (tRNAscan-SE ID: chrIV.trna24) Pro (AGG) 72 bp Sc: 70.1 chrIV:11231564-11231636(+)
+GGCTGAGTGGTCTAGTGGTATGATTCTCGCTTAGGGTGCGAGAGGTCCCGGGATCGATCCCCGGCTCAGCCC
+>Caenorhabditis_elegans_tRNA-His-GTG-1-1 (tRNAscan-SE ID: chrIV.trna25) His (GTG) 88 bp Sc: 79.2 chrIV:11721148-11721236(+)
+GCCACGGTGGCCGAGTGGTCAAGGCGTGAGCTTGTGGGATGCGCTCATGGGGTTAAACCCATCGCAGGTTCGAATCCTGCCCGTGGCA
+>Caenorhabditis_elegans_tRNA-Leu-CAA-1-4 (tRNAscan-SE ID: chrIV.trna66) Leu (CAA) 119 bp Sc: 74.2 chrIV:11928477-11928596(-)
+GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCAATTGCTTGCCTCGAGTTCGAGGTCGACTGGGTGTTCTGGTACTCGTATGGGTGCGTGGGTTCGAATCCCACTTCGTGCA
+>Caenorhabditis_elegans_tRNA-Pro-CGG-1-3 (tRNAscan-SE ID: chrIV.trna65) Pro (CGG) 72 bp Sc: 71.5 chrIV:12005597-12005669(-)
+GGCCGGATGGTCTAGAGGTATGATTCTCGCTTCGGGTGCGAGAGGTCCCGGGTTCGATTCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Gln-CTG-2-2 (tRNAscan-SE ID: chrIV.trna64) Gln (CTG) 72 bp Sc: 71.6 chrIV:12416941-12417013(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTCTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGGACCT
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-6 (tRNAscan-SE ID: chrIV.trna63) Gln (TTG) 72 bp Sc: 72.0 chrIV:12417248-12417320(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Arg-ACG-1-5 (tRNAscan-SE ID: chrIV.trna62) Arg (ACG) 73 bp Sc: 72.1 chrIV:12417925-12417998(-)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGCAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-14 (tRNAscan-SE ID: chrIV.trna26) Lys (CTT) 73 bp Sc: 85.9 chrIV:12594739-12594812(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRX-Lys-CTT-8-5 (tRNAscan-SE ID: chrIV.trna27) Lys (CTT) 62 bp Sc: 20.7 chrIV:13043697-13043759(+)
+gtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRX-Lys-CTT-8-6 (tRNAscan-SE ID: chrIV.trna61) Lys (CTT) 62 bp Sc: 20.7 chrIV:13044464-13044526(-)
+gtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRX-His-GTG-2-1 (tRNAscan-SE ID: chrIV.trna28) His (GTG) 72 bp Sc: 40.4 chrIV:13870264-13870336(+)
+GCCCTCTTAGTATAGTGGCTAGTACTCCACGTTGTGGTCGTGGCAACGCGGGTTCGATTCCAGCAGCAGGCA
+>Caenorhabditis_elegans_tRNA-Ala-TGC-1-4 (tRNAscan-SE ID: chrIV.trna60) Ala (TGC) 72 bp Sc: 68.8 chrIV:14013804-14013876(-)
+GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-6 (tRNAscan-SE ID: chrIV.trna29) Pro (TGG) 72 bp Sc: 75.2 chrIV:14225101-14225173(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-14 (tRNAscan-SE ID: chrIV.trna59) Gly (TCC) 72 bp Sc: 71.7 chrIV:14576621-14576693(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Arg-ACG-1-6 (tRNAscan-SE ID: chrIV.trna58) Arg (ACG) 73 bp Sc: 72.1 chrIV:14611306-14611379(-)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGCAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-His-GTG-3-1 (tRNAscan-SE ID: chrIV.trna57) His (GTG) 72 bp Sc: 67.8 chrIV:14889021-14889093(-)
+GCCTGCTTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCAGCAGGCA
+>Caenorhabditis_elegans_tRNA-His-GTG-4-1 (tRNAscan-SE ID: chrIV.trna30) His (GTG) 72 bp Sc: 62.0 chrIV:15187343-15187415(+)
+GCCTGCTTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTAGATTCCAGCAGCAGGCA
+>Caenorhabditis_elegans_tRNA-His-GTG-3-2 (tRNAscan-SE ID: chrIV.trna56) His (GTG) 72 bp Sc: 67.8 chrIV:15187653-15187725(-)
+GCCTGCTTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCAGCAGGCA
+>Caenorhabditis_elegans_tRX-Und-NNN-2-1 (tRNAscan-SE ID: chrIV.trna31) Und (NNN) 68 bp Sc: 30.2 chrIV:15188017-15188085(+)
+GCCTGCTTAGTATAGTGGCTAGTACTCTGAGTTGTGCGGAGGGCGTGGTTCGATTCCAGCAGCAGGCA
+>Caenorhabditis_elegans_tRNA-Val-AAC-3-1 (tRNAscan-SE ID: chrIV.trna32) Val (AAC) 73 bp Sc: 75.2 chrIV:15235387-15235460(+)
+GGTTTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Trp-CCA-1-6 (tRNAscan-SE ID: chrIV.trna33) Trp (CCA) 72 bp Sc: 71.5 chrIV:15289702-15289774(+)
+GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCCGCTCAGTGGTCA
+>Caenorhabditis_elegans_tRNA-Ser-AGA-2-5 (tRNAscan-SE ID: chrIV.trna55) Ser (AGA) 82 bp Sc: 81.6 chrIV:15311117-15311199(-)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Ser-AGA-2-6 (tRNAscan-SE ID: chrIV.trna54) Ser (AGA) 82 bp Sc: 81.6 chrIV:15318477-15318559(-)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Ala-TGC-1-5 (tRNAscan-SE ID: chrIV.trna53) Ala (TGC) 72 bp Sc: 68.8 chrIV:15604311-15604383(-)
+GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-15 (tRNAscan-SE ID: chrIV.trna34) Lys (CTT) 73 bp Sc: 85.9 chrIV:15793414-15793487(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-6 (tRNAscan-SE ID: chrIV.trna52) Asp (GTC) 72 bp Sc: 61.7 chrIV:15931341-15931413(-)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-7 (tRNAscan-SE ID: chrIV.trna35) Asp (GTC) 72 bp Sc: 61.7 chrIV:15932009-15932081(+)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-5 (tRNAscan-SE ID: chrIV.trna51) Glu (TTC) 72 bp Sc: 75.3 chrIV:15933160-15933232(-)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-6 (tRNAscan-SE ID: chrIV.trna36) Glu (TTC) 72 bp Sc: 75.3 chrIV:15933352-15933424(+)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Val-AAC-2-6 (tRNAscan-SE ID: chrIV.trna50) Val (AAC) 73 bp Sc: 76.6 chrIV:16382430-16382503(-)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-His-GTG-2-2 (tRNAscan-SE ID: chrIV.trna37) His (GTG) 72 bp Sc: 69.4 chrIV:16388455-16388527(+)
+GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCCGCAGGCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-5 (tRNAscan-SE ID: chrIV.trna49) Ala (AGC) 72 bp Sc: 74.8 chrIV:16389210-16389282(-)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-6 (tRNAscan-SE ID: chrIV.trna38) Ala (AGC) 72 bp Sc: 74.8 chrIV:16398383-16398455(+)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-7 (tRNAscan-SE ID: chrIV.trna39) Ala (AGC) 72 bp Sc: 74.8 chrIV:16399183-16399255(+)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Val-AAC-2-7 (tRNAscan-SE ID: chrIV.trna40) Val (AAC) 73 bp Sc: 76.6 chrIV:16400129-16400202(+)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-His-GTG-2-3 (tRNAscan-SE ID: chrIV.trna41) His (GTG) 72 bp Sc: 69.4 chrIV:16400895-16400967(+)
+GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCCGCAGGCA
+>Caenorhabditis_elegans_tRNA-Ser-TGA-6-1 (tRNAscan-SE ID: chrIV.trna42) Ser (TGA) 82 bp Sc: 82.4 chrIV:16577305-16577387(+)
+GCTGCGATGTCCGAGCGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCGTAGGTTCAAATCCTGCTCGCAGCG
+>Caenorhabditis_elegans_tRNA-Ser-TGA-6-2 (tRNAscan-SE ID: chrIV.trna48) Ser (TGA) 82 bp Sc: 82.4 chrIV:16583741-16583823(-)
+GCTGCGATGTCCGAGCGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCGTAGGTTCAAATCCTGCTCGCAGCG
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-15 (tRNAscan-SE ID: chrIV.trna47) Gly (TCC) 72 bp Sc: 71.7 chrIV:16670865-16670937(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-16 (tRNAscan-SE ID: chrIV.trna43) Gly (TCC) 72 bp Sc: 71.7 chrIV:16682006-16682078(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-6-1 (tRNAscan-SE ID: chrIV.trna46) Gly (TCC) 72 bp Sc: 61.0 chrIV:16684382-16684454(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACCGGGGTTCGATTCCCCCCGAAGGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-17 (tRNAscan-SE ID: chrIV.trna44) Gly (TCC) 72 bp Sc: 71.7 chrIV:16775181-16775253(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-18 (tRNAscan-SE ID: chrIV.trna45) Gly (TCC) 72 bp Sc: 71.7 chrIV:16776087-16776159(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-6-1 (tRNAscan-SE ID: chrV.trna1) Ala (AGC) 72 bp Sc: 47.1 chrV:857324-857396(+)
+GGGGGTATAACTCAGTGGTAGATCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCAAACCTCCA
+>Caenorhabditis_elegans_tRX-Und-NNN-9-1 (tRNAscan-SE ID: chrV.trna112) Und (NNN) 78 bp Sc: 24.8 chrV:2149172-2149250(-)
+ggcggaagtagctcagtcggtaatggtggtagctagtagtctagaggtcacaggttcaagtcctgcctccctccgcca
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-5 (tRNAscan-SE ID: chrV.trna111) Thr (AGT) 72 bp Sc: 85.3 chrV:2664666-2664738(-)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-6 (tRNAscan-SE ID: chrV.trna2) Thr (AGT) 72 bp Sc: 85.3 chrV:2674009-2674081(+)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Met-CAT-1-3 (tRNAscan-SE ID: chrV.trna110) Met (CAT) 73 bp Sc: 77.0 chrV:3455325-3455398(-)
+GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGCCTCACCGGGAGCA
+>Caenorhabditis_elegans_tRNA-Pro-TGG-6-1 (tRNAscan-SE ID: chrV.trna109) Pro (TGG) 72 bp Sc: 67.2 chrV:3582130-3582202(-)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCAGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-7 (tRNAscan-SE ID: chrV.trna3) Pro (TGG) 72 bp Sc: 75.2 chrV:3582319-3582391(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-TGG-5-1 (tRNAscan-SE ID: chrV.trna108) Pro (TGG) 72 bp Sc: 64.7 chrV:3588313-3588385(-)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGCGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-8 (tRNAscan-SE ID: chrV.trna4) Pro (TGG) 72 bp Sc: 75.2 chrV:3588502-3588574(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Gly-GCC-2-1 (tRNAscan-SE ID: chrV.trna5) Gly (GCC) 71 bp Sc: 73.4 chrV:4310609-4310680(+)
+gcatcggtggttcagtggtagaatgctcgcctgccacgcgtgcggcccgggttcgattcccggtcgatgca
+>Caenorhabditis_elegans_tRX-Lys-CTT-6-1 (tRNAscan-SE ID: chrV.trna107) Lys (CTT) 62 bp Sc: 23.2 chrV:4782233-4782295(-)
+gtggtcgagtggtgaacgcattcgcctcttgagcaaaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-7 (tRNAscan-SE ID: chrV.trna106) Gln (TTG) 72 bp Sc: 72.0 chrV:5330138-5330210(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Cys-GCA-2-1 (tRNAscan-SE ID: chrV.trna6) Cys (GCA) 72 bp Sc: 62.8 chrV:6335397-6335469(+)
+TGGGGTATAGCTCAGTGGCAGAGCATTCGATTGCAGATCGAGAGGTCCCTGGTTCAACTCCGGGTGCCCCCT
+>Caenorhabditis_elegans_tRX-Lys-CTT-4-1 (tRNAscan-SE ID: chrV.trna7) Lys (CTT) 73 bp Sc: 24.7 chrV:6417974-6418047(+)
+gcttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacacgtggtt
+>Caenorhabditis_elegans_tRX-Lys-CTT-4-2 (tRNAscan-SE ID: chrV.trna105) Lys (CTT) 73 bp Sc: 24.7 chrV:6421725-6421798(-)
+gcttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacacgtggtt
+>Caenorhabditis_elegans_tRNA-Ser-GCT-1-3 (tRNAscan-SE ID: chrV.trna104) Ser (GCT) 82 bp Sc: 84.4 chrV:6551853-6551935(-)
+GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTGAGTTCGAATCTCATCCTGATCG
+>Caenorhabditis_elegans_tRNA-Cys-GCA-1-3 (tRNAscan-SE ID: chrV.trna8) Cys (GCA) 72 bp Sc: 74.0 chrV:6559756-6559828(+)
+GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTCCGGGTGCCCCCT
+>Caenorhabditis_elegans_tRNA-Ile-TAT-2-1 (tRNAscan-SE ID: chrV.trna9) Ile (TAT) 85 bp Sc: 76.7 chrV:6917465-6917550(+)
+GCCCCATTGGCGCAGTCGGTTAGCGCGTGGTACTTATAGTTAATAGGGAATGCCAAGGTCGCCAGTTCGAGCCTGGCATGGGGCA
+>Caenorhabditis_elegans_tRNA-Glu-TTC-3-1 (tRNAscan-SE ID: chrV.trna103) Glu (TTC) 71 bp Sc: 59.8 chrV:7069747-7069818(-)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Arg-TCT-2-3 (tRNAscan-SE ID: chrV.trna10) Arg (TCT) 73 bp Sc: 71.1 chrV:7506394-7506467(+)
+GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGAGCCCTGCCTGGGTCA
+>Caenorhabditis_elegans_tRNA-Thr-CGT-5-1 (tRNAscan-SE ID: chrV.trna102) Thr (CGT) 72 bp Sc: 75.1 chrV:7730653-7730725(-)
+GCCCGTATAGCTCAGTGGCAGAGCGTCTGTCTCGTAAACAGAAGGTCGACGGTTCAATCCCGTCTGGGGGCA
+>Caenorhabditis_elegans_tRNA-Met-CAT-1-4 (tRNAscan-SE ID: chrV.trna101) Met (CAT) 73 bp Sc: 77.0 chrV:8230205-8230278(-)
+GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGCCTCACCGGGAGCA
+>Caenorhabditis_elegans_tRNA-Leu-TAG-1-2 (tRNAscan-SE ID: chrV.trna100) Leu (TAG) 82 bp Sc: 75.3 chrV:8235457-8235539(-)
+GGTGAGATGGCCGAGTGGTCTAAGGCGCTGGTTTTAGGCACCAGTCCCTCCGGGGGCGTGGGTTCGAATCCCACTCTCATCA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-1-1 (tRNAscan-SE ID: chrV.trna11) Tyr (GTA) 84 bp Sc: 76.8 chrV:8247480-8247564(+)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGTGGGTATCCTTAGGTCGCTGGTTCGAATCCGGCTCGACGGA
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-5 (tRNAscan-SE ID: chrV.trna12) Lys (TTT) 73 bp Sc: 77.8 chrV:8495301-8495374(+)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-7 (tRNAscan-SE ID: chrV.trna99) Thr (AGT) 72 bp Sc: 85.3 chrV:8496103-8496175(-)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-6 (tRNAscan-SE ID: chrV.trna98) Lys (TTT) 73 bp Sc: 77.8 chrV:8499563-8499636(-)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-Ala-CGC-4-1 (tRNAscan-SE ID: chrV.trna13) Ala (CGC) 72 bp Sc: 63.4 chrV:9318201-9318273(+)
+GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTCGCATGTGAGAAGTCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-8 (tRNAscan-SE ID: chrV.trna97) Thr (AGT) 72 bp Sc: 85.3 chrV:9407039-9407111(-)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-6-1 (tRNAscan-SE ID: chrV.trna96) Tyr (GTA) 87 bp Sc: 66.9 chrV:9412204-9412291(-)
+CCGTCGATAGCTCAGTAGTTGGTAGAGCGGAGGACTGTAGAGTCAGTGGGTATCCTTAGATCGCTGGTTCGAATCCGGCTCGACGGA
+>Caenorhabditis_elegans_tRNA-Ala-CGC-3-1 (tRNAscan-SE ID: chrV.trna14) Ala (CGC) 72 bp Sc: 67.8 chrV:9503561-9503633(+)
+GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTCGCATGCGAGAAGTCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Leu-CAG-2-2 (tRNAscan-SE ID: chrV.trna95) Leu (CAG) 84 bp Sc: 76.8 chrV:11174789-11174873(-)
+GCCGTTCTGGCCGAGTGGTCTAAGGCGCTGCGTTCAGGTCGCAGTCCTCTCCGGAGGGCGCAGGTTCGAATCCTGCGGACGGCA
+>Caenorhabditis_elegans_tRX-Leu-CAG-3-1 (tRNAscan-SE ID: chrV.trna94) Leu (CAG) 100 bp Sc: 42.7 chrV:11183665-11183765(-)
+GCTGTTTTGCATGGCCGAGTGGTCTAATTAGAGCCTTAAGGCGCTGCGTTCAGGTCGCAGTCCTCTCAGGAGGGCGCAGGTTCAAATCCTGCGGACAGCA
+>Caenorhabditis_elegans_tRNA-Val-CAC-1-2 (tRNAscan-SE ID: chrV.trna93) Val (CAC) 73 bp Sc: 80.7 chrV:11412234-11412307(-)
+GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTCACACGCAGAAGGTCGCCGGTTCGAACCCGGCCAGGACCT
+>Caenorhabditis_elegans_tRNA-Ile-TAT-2-2 (tRNAscan-SE ID: chrV.trna15) Ile (TAT) 85 bp Sc: 76.7 chrV:12002175-12002260(+)
+GCCCCATTGGCGCAGTCGGTTAGCGCGTGGTACTTATAGTCTATAGGTTATGCCAAGGTCGCCAGTTCGAGCCTGGCATGGGGCA
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-5 (tRNAscan-SE ID: chrV.trna92) Asn (GTT) 73 bp Sc: 73.5 chrV:12331964-12332037(-)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Val-TAC-1-1 (tRNAscan-SE ID: chrV.trna91) Val (TAC) 73 bp Sc: 77.5 chrV:12683350-12683423(-)
+GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTTACACGCAGAAGATCGCCGGTTCGAACCCGGCCAGGACCT
+>Caenorhabditis_elegans_tRNA-Ser-TGA-2-1 (tRNAscan-SE ID: chrV.trna90) Ser (TGA) 82 bp Sc: 85.6 chrV:12780385-12780467(-)
+GCTGCGATGTCCGAGTGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCGTAGGTTCGAACCCTGCTCGCAGCG
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-8 (tRNAscan-SE ID: chrV.trna89) Ala (AGC) 72 bp Sc: 74.8 chrV:13003508-13003580(-)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-7 (tRNAscan-SE ID: chrV.trna88) Lys (TTT) 73 bp Sc: 77.8 chrV:13027027-13027100(-)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-9 (tRNAscan-SE ID: chrV.trna87) Pro (TGG) 72 bp Sc: 75.2 chrV:13507202-13507274(-)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-10 (tRNAscan-SE ID: chrV.trna16) Pro (TGG) 72 bp Sc: 75.2 chrV:13509692-13509764(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Gln-CTG-1-1 (tRNAscan-SE ID: chrV.trna17) Gln (CTG) 72 bp Sc: 74.0 chrV:14231363-14231435(+)
+GGTTCCATGGTGTAGTGGTTAGCACTCAGGACTCTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGGACCT
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-2-4 (tRNAscan-SE ID: chrV.trna18) Tyr (GTA) 84 bp Sc: 74.6 chrV:14689531-14689615(+)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTTTGCAGATATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGA
+>Caenorhabditis_elegans_tRNA-Cys-GCA-1-4 (tRNAscan-SE ID: chrV.trna86) Cys (GCA) 72 bp Sc: 74.0 chrV:14855786-14855858(-)
+GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTCCGGGTGCCCCCT
+>Caenorhabditis_elegans_tRNA-Phe-GAA-2-5 (tRNAscan-SE ID: chrV.trna85) Phe (GAA) 73 bp Sc: 82.5 chrV:14876388-14876461(-)
+GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATCCTGGTTCGGGGCA
+>Caenorhabditis_elegans_tRNA-Val-AAC-2-8 (tRNAscan-SE ID: chrV.trna84) Val (AAC) 73 bp Sc: 76.6 chrV:15013033-15013106(-)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-6 (tRNAscan-SE ID: chrV.trna19) Asn (GTT) 73 bp Sc: 73.5 chrV:15156681-15156754(+)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-8 (tRNAscan-SE ID: chrV.trna20) Lys (TTT) 73 bp Sc: 77.8 chrV:15465085-15465158(+)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-11 (tRNAscan-SE ID: chrV.trna83) Pro (TGG) 72 bp Sc: 75.2 chrV:15465224-15465296(-)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Ala-CGC-2-1 (tRNAscan-SE ID: chrV.trna82) Ala (CGC) 72 bp Sc: 72.3 chrV:15479984-15480056(-)
+GGGGGCATAGCTCAGAGGTAGAGCGCCCGCTTCGCATGCGGGAAGTCCGGGGTTCAATCCCCCGTGCCTCCA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-1-2 (tRNAscan-SE ID: chrV.trna21) Tyr (GTA) 84 bp Sc: 76.8 chrV:15480693-15480777(+)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGTGGGTATCCTTAGGTCGCTGGTTCGAATCCGGCTCGACGGA
+>Caenorhabditis_elegans_tRNA-Gly-GCC-1-7 (tRNAscan-SE ID: chrV.trna81) Gly (GCC) 71 bp Sc: 77.2 chrV:15505207-15505278(-)
+gcatcggtggttcagtggtagaatgctcgcctgccacgcgggcggcccgggttcgattcccggtcgatgca
+>Caenorhabditis_elegans_tRNA-Val-CAC-1-3 (tRNAscan-SE ID: chrV.trna80) Val (CAC) 73 bp Sc: 80.7 chrV:15515505-15515578(-)
+GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTCACACGCAGAAGGTCGCCGGTTCGAACCCGGCCAGGACCT
+>Caenorhabditis_elegans_tRNA-Met-CAT-2-1 (tRNAscan-SE ID: chrV.trna22) Met (CAT) 69 bp Sc: 43.0 chrV:15517399-15517468(+)
+GGGTCCTGTAGTGGTTATCACGTCTGCTTCATACACAGAAGGTCGCCGGTTCGAACCCGGCCAGGACCT
+>Caenorhabditis_elegans_tRNA-Ser-TGA-5-1 (tRNAscan-SE ID: chrV.trna79) Ser (TGA) 82 bp Sc: 84.6 chrV:15547874-15547956(-)
+GCTGCGATGTCCGAGTGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCGTAGGTTCGAACCCTGCTTGCAGCG
+>Caenorhabditis_elegans_tRNA-Ser-TGA-7-1 (tRNAscan-SE ID: chrV.trna23) Ser (TGA) 82 bp Sc: 74.4 chrV:15550611-15550693(+)
+GCTGCGATGCCCGAGTGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCATAGGTTCGAACCCTGCTTGCAGCG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-8 (tRNAscan-SE ID: chrV.trna78) Asp (GTC) 72 bp Sc: 61.7 chrV:15551798-15551870(-)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-His-GTG-3-3 (tRNAscan-SE ID: chrV.trna24) His (GTG) 72 bp Sc: 67.8 chrV:15554029-15554101(+)
+GCCTGCTTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCAGCAGGCA
+>Caenorhabditis_elegans_tRNA-Thr-CGT-3-1 (tRNAscan-SE ID: chrV.trna25) Thr (CGT) 72 bp Sc: 76.0 chrV:16219158-16219230(+)
+GCCCGTATAGCTCAGTGGCAGAGCGTCTGTCTCGTAAACAGAAGGCCGGCGGTTCAATCCCGCCTGGGGGCA
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-7 (tRNAscan-SE ID: chrV.trna77) Asn (GTT) 73 bp Sc: 73.5 chrV:16338369-16338442(-)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-8 (tRNAscan-SE ID: chrV.trna26) Asn (GTT) 73 bp Sc: 73.5 chrV:16338547-16338620(+)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-9 (tRNAscan-SE ID: chrV.trna76) Asn (GTT) 73 bp Sc: 73.5 chrV:16341600-16341673(-)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-10 (tRNAscan-SE ID: chrV.trna27) Asn (GTT) 73 bp Sc: 73.5 chrV:16341778-16341851(+)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRX-Lys-CTT-8-7 (tRNAscan-SE ID: chrV.trna28) Lys (CTT) 62 bp Sc: 20.7 chrV:16564067-16564129(+)
+gtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRX-Lys-CTT-8-8 (tRNAscan-SE ID: chrV.trna75) Lys (CTT) 62 bp Sc: 20.7 chrV:16565137-16565199(-)
+gtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRNA-Gln-CTG-2-3 (tRNAscan-SE ID: chrV.trna74) Gln (CTG) 72 bp Sc: 71.6 chrV:16592236-16592308(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTCTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGGACCT
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-9 (tRNAscan-SE ID: chrV.trna73) Lys (TTT) 73 bp Sc: 77.8 chrV:16622058-16622131(-)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-9 (tRNAscan-SE ID: chrV.trna29) Asp (GTC) 72 bp Sc: 61.7 chrV:16640577-16640649(+)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-10 (tRNAscan-SE ID: chrV.trna72) Asp (GTC) 72 bp Sc: 61.7 chrV:16645705-16645777(-)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-11 (tRNAscan-SE ID: chrV.trna71) Asp (GTC) 72 bp Sc: 61.7 chrV:16648765-16648837(-)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-3-1 (tRNAscan-SE ID: chrV.trna70) Tyr (GTA) 84 bp Sc: 67.4 chrV:17317878-17317962(-)
+CCGTCGATAGCTCAGTTGGTAGAGCGCAGGACTGTAGAGTTAGCAGATATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-2-5 (tRNAscan-SE ID: chrV.trna69) Tyr (GTA) 84 bp Sc: 74.6 chrV:17542445-17542529(-)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTTGGCAGATATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGA
+>Caenorhabditis_elegans_tRX-His-ATG-3-1 (tRNAscan-SE ID: chrV.trna30) His (ATG) 72 bp Sc: 21.2 chrV:17686380-17686452(+)
+GTCTTCGTGGCTCAGTTGGGAAGAGGTTTGACTATGGTTCAGAAGGTCAGGGGTTCGACCCCATCGGTGGCT
+>Caenorhabditis_elegans_tRX-Val-GAC-2-1 (tRNAscan-SE ID: chrV.trna68) Val (GAC) 73 bp Sc: 25.6 chrV:17693798-17693871(-)
+GACCCGGTGGCTCAGTCGGGTAGAGGTTTAGCTTTGACATAGAAGGTCCCGGGTTCAATCCCCACTGCGGTCA
+>Caenorhabditis_elegans_tRX-Und-NNN-7-1 (tRNAscan-SE ID: chrV.trna67) Und (NNN) 76 bp Sc: 20.0 chrV:17694091-17694167(-)
+TTGACCTGTGGCTCAGTCGGGTAGAGGTTCAGCTATGACACAGAAGGTCCGGGGTTCAATCCTCGCTGCAGTCAAA
+>Caenorhabditis_elegans_tRX-Leu-TAG-7-1 (tRNAscan-SE ID: chrV.trna66) Leu (TAG) 70 bp Sc: 26.0 chrV:17739488-17739558(-)
+GCGTAGCTCAGTCGGTAAGACGCTTGACTTTAGAGAGACAGGTCGCGGGTTCGAGCCCCGCAGAGGTGTA
+>Caenorhabditis_elegans_tRX-Gly-CCC-8-1 (tRNAscan-SE ID: chrV.trna31) Gly (CCC) 74 bp Sc: 31.2 chrV:17930791-17930865(+)
+GTGTGCAAGTGGCTCAGTGGGTTAGAGTGATGGCTCCCGCCCACACGTCCGGGGTTCGACCCCCGGTGCGGGCG
+>Caenorhabditis_elegans_tRX-Gly-GCC-7-1 (tRNAscan-SE ID: chrV.trna32) Gly (GCC) 78 bp Sc: 20.5 chrV:17931075-17931153(+)
+TGTGCAAGTGGCTCAATCGGTTAGAGAGATGGTTGCCACCCACAAGTCCGGGGTTCGAACCCCGACTGTGGTTCATAA
+>Caenorhabditis_elegans_tRX-Gly-GCC-6-1 (tRNAscan-SE ID: chrV.trna33) Gly (GCC) 74 bp Sc: 25.6 chrV:17933328-17933402(+)
+TGTTTTGTGGCTCAGTCGGGTAAAGCGATGACTGCCGCCCACACGTCCGGGGTTCGAACCCCGGCTGGGGCCAA
+>Caenorhabditis_elegans_tRX-Ser-CGA-9-1 (tRNAscan-SE ID: chrV.trna34) Ser (CGA) 72 bp Sc: 21.2 chrV:18367138-18367210(+)
+GTTCCGGTGGCTCAGCTGGGTAGAGAGATGGCTATGGGGCAAATGTCCGGGGTTCGATTCCCCGCTAGAGTT
+>Caenorhabditis_elegans_tRX-Und-NNN-8-1 (tRNAscan-SE ID: chrV.trna35) Und (NNN) 73 bp Sc: 21.9 chrV:18371228-18371301(+)
+GTCGAAGTGGCTCAGGTGGGAAGAGGGATAGCTATGGGGAATAGGGTCCTGGGTTCGAGTCCCCGCTTGGGCA
+>Caenorhabditis_elegans_tRX-Cys-ACA-1-1 (tRNAscan-SE ID: chrV.trna65) Cys (ACA) 74 bp Sc: 28.3 chrV:18372879-18372953(-)
+GTCCAAGTAGCTCAGGCGGGTAGAGGGATAACAATGGGGAAATAGGTCCGGGGTTCGAGTCCCCGCTTGGGTCA
+>Caenorhabditis_elegans_tRX-Und-NNN-4-1 (tRNAscan-SE ID: chrV.trna64) Und (NNN) 70 bp Sc: 28.5 chrV:18373665-18373735(-)
+GCAGTGGCTCAGGTGGGTAGAGAGATGGCTATGGAGAAATAGGTCCGGGGTTCGAGCCCCCGCTGGTGCA
+>Caenorhabditis_elegans_tRX-Pro-GGG-6-1 (tRNAscan-SE ID: chrV.trna63) Pro (GGG) 74 bp Sc: 27.9 chrV:18373962-18374036(-)
+GTCGCAGTGGCTCAGGTGGGTAGAGTAATGACTATGGGGAAATAGGTCCGGGGTTCGAGCCCCCGCTGATGGCA
+>Caenorhabditis_elegans_tRNA-Thr-TGT-1-5 (tRNAscan-SE ID: chrV.trna62) Thr (TGT) 72 bp Sc: 81.0 chrV:18412482-18412554(-)
+GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCCTGCGTGGGGGCA
+>Caenorhabditis_elegans_tRX-Gly-ACC-4-1 (tRNAscan-SE ID: chrV.trna61) Gly (ACC) 71 bp Sc: 25.7 chrV:18801974-18802045(-)
+gccagaatggctcagtgggatttttgctgactaccaatcacaagaccggggttcgggtccccgctttggta
+>Caenorhabditis_elegans_tRX-Gly-ACC-9-1 (tRNAscan-SE ID: chrV.trna60) Gly (ACC) 71 bp Sc: 20.9 chrV:18827875-18827946(-)
+gccaaaatggcgcagtgggattttcaccgactaccaatcacaagaccagggttcgagtccccgttgtggca
+>Caenorhabditis_elegans_tRX-Thr-GGT-7-1 (tRNAscan-SE ID: chrV.trna59) Thr (GGT) 79 bp Sc: 23.4 chrV:19057497-19057576(-)
+GCATTTTTGGCTCAAGTGGGTAGAGGTTTGACTGGTGAGcagaagaccggggttcgactccccactgtggtaaaaTACT
+>Caenorhabditis_elegans_tRX-Thr-GGT-6-1 (tRNAscan-SE ID: chrV.trna58) Thr (GGT) 74 bp Sc: 23.9 chrV:19059284-19059358(-)
+TGCACTtttagctcaagtgggtagagatttgactggtgagcagaagaccggggttcgagtccccgctgtggtaa
+>Caenorhabditis_elegans_tRX-Pro-GGG-10-1 (tRNAscan-SE ID: chrV.trna36) Pro (GGG) 72 bp Sc: 21.7 chrV:19082941-19083013(+)
+GAACTTTTAGCTCAACTGGTTAGAGGTTTGCCTGGGaatcacaagaccggggttcgagcccccgctgtggca
+>Caenorhabditis_elegans_tRX-Pro-GGG-8-1 (tRNAscan-SE ID: chrV.trna37) Pro (GGG) 72 bp Sc: 26.9 chrV:19084604-19084676(+)
+GCATTTTTGGCTCAACTGGGAAGAGGTTTGCCTGGGaatcacaagaccggggttcgagcccccgctggggca
+>Caenorhabditis_elegans_tRNA-Phe-GAA-3-1 (tRNAscan-SE ID: chrV.trna38) Phe (GAA) 73 bp Sc: 82.3 chrV:19126043-19126116(+)
+GCCTCGATAGCTCAGTTGGGAGAGCGCACGACTGAAGATCGTGAGGTCACCAGTTCGATCCTGGTTCGGGGCA
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-7 (tRNAscan-SE ID: chrV.trna39) Glu (TTC) 72 bp Sc: 75.3 chrV:19142787-19142859(+)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRX-His-ATG-9-1 (tRNAscan-SE ID: chrV.trna57) His (ATG) 73 bp Sc: 20.0 chrV:19396988-19397061(-)
+GCACCGGTGGCTCAGCTGGGTAGAGGGACGGCTATGGCTCAGGAGGTCAGGGGTTCGACTCCCTGCTGTGGCT
+>Caenorhabditis_elegans_tRX-His-ATG-8-1 (tRNAscan-SE ID: chrV.trna40) His (ATG) 71 bp Sc: 20.2 chrV:19398587-19398658(+)
+GCCAGTGGCTCAGTCGGGTAGGGCTTTGGCTATGGCTCTGAGGGTCAGGAGTTCGAGTCCCCGTTGTGGCA
+>Caenorhabditis_elegans_tRX-His-ATG-4-1 (tRNAscan-SE ID: chrV.trna41) His (ATG) 72 bp Sc: 21.9 chrV:19577389-19577461(+)
+GCCTCGGTGGCTCAGTTGGGTAGAGGTTTGGCTATGGCCCAGAAGGTCAAGAGTTCGAACCCTGCAGAGGCC
+>Caenorhabditis_elegans_tRX-Ala-GGC-7-1 (tRNAscan-SE ID: chrV.trna56) Ala (GGC) 73 bp Sc: 23.2 chrV:19587263-19587336(-)
+GGTCGCAGTGGCTCAGCTGGGAAGAGGTTTGGCTCTGGCGCAGAGGACCAGGGTTCGACCCCCGGTGGGGCCA
+>Caenorhabditis_elegans_tRX-His-ATG-5-1 (tRNAscan-SE ID: chrV.trna55) His (ATG) 74 bp Sc: 23.4 chrV:19595586-19595660(-)
+TGCGCCGATGGCTCAGGTGGGTAGAGGTTTGGCTATGACGCAGAAGGTCACGGGTTCGACCCCCGGTGGGGTAA
+>Caenorhabditis_elegans_tRX-His-GTG-6-1 (tRNAscan-SE ID: chrV.trna42) His (GTG) 73 bp Sc: 21.7 chrV:19596965-19597038(+)
+GGCAAAATGGCTCAGTCGGGTAGAGGTTTAGGTGTGGCCCAGAAGGTCATGGGTTCAATCCCCACTGCTGGCA
+>Caenorhabditis_elegans_tRX-Pro-TGG-5-1 (tRNAscan-SE ID: chrV.trna54) Pro (TGG) 73 bp Sc: 32.2 chrV:19665947-19666020(-)
+GTCGCAGTGGCTCAGTCGGGTAGAGGTTTGGCTTGGGATCTGATGGTCCGGGGTTCGAGCCCCGGCTGTGGTG
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-11 (tRNAscan-SE ID: chrV.trna43) Asn (GTT) 73 bp Sc: 73.5 chrV:19723030-19723103(+)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRX-His-ATG-7-1 (tRNAscan-SE ID: chrV.trna53) His (ATG) 73 bp Sc: 20.7 chrV:20016574-20016647(-)
+GCCCGGGTGGCTTTGTGGCGAAGAGTGATGCCTATGGAGTGGTAGGTCAGGGGTTCGAGCCCCCGCATGGGTG
+>Caenorhabditis_elegans_tRX-Gly-GCC-5-1 (tRNAscan-SE ID: chrV.trna52) Gly (GCC) 74 bp Sc: 22.7 chrV:20119905-20119979(-)
+GCCGCGGTGGCTCAGTCGGTAAGAGAGATGACTGCCGTCCAAGAGGTCACGGGTTCGACCCCCAGTGGTGGGCA
+>Caenorhabditis_elegans_tRX-Gln-TTG-4-1 (tRNAscan-SE ID: chrV.trna51) Gln (TTG) 73 bp Sc: 25.4 chrV:20123733-20123806(-)
+TCCCAGGTGGCTCAGTGGCTAAGAGGGATGACTTTGGAGCAAAAGGTCCGGGGTTCGAACCCCTGTGCGGGCA
+>Caenorhabditis_elegans_tRX-Ser-CGA-10-1 (tRNAscan-SE ID: chrV.trna50) Ser (CGA) 74 bp Sc: 29.0 chrV:20126169-20126243(-)
+GCGCCACATGGCTCAGTGGGTAAGAGGGACGACTTTGGAGTGAAAGGCCCTGGGTTCGAACCCCTGTGCGGGTA
+>Caenorhabditis_elegans_tRX-Ser-AGA-11-1 (tRNAscan-SE ID: chrV.trna44) Ser (AGA) 73 bp Sc: 30.3 chrV:20127760-20127833(+)
+GCCCGGGTGGCTCAGTGGGTAAGAGGGATGACCTTAGAGTGGAAGGCCAGGGGTTCGAGCCCCCGCGCTGGTT
+>Caenorhabditis_elegans_tRX-Ser-GGA-12-1 (tRNAscan-SE ID: chrV.trna49) Ser (GGA) 74 bp Sc: 20.1 chrV:20134911-20134985(-)
+GCGCCTCGTGGCTCAGTGGCTAAGAGAGATGACTTTGGAGTGGAAGGTCGGGGGTTCGATTCCTCGGGAGGGTA
+>Caenorhabditis_elegans_tRX-Ser-AGA-8-1 (tRNAscan-SE ID: chrV.trna45) Ser (AGA) 73 bp Sc: 30.2 chrV:20135002-20135075(+)
+GCCCGAGTGGCTCAGTGGGTAAGAGGGATGACTTTAGAGTGGAAGGTCAGGGGTTCGAGCCCCCGCACGGGTG
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-12 (tRNAscan-SE ID: chrV.trna48) Asn (GTT) 73 bp Sc: 73.5 chrV:20347796-20347869(-)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-13 (tRNAscan-SE ID: chrV.trna47) Asn (GTT) 73 bp Sc: 73.5 chrV:20350528-20350601(-)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Cys-GCA-1-5 (tRNAscan-SE ID: chrV.trna46) Cys (GCA) 72 bp Sc: 74.0 chrV:20694120-20694192(-)
+GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTCCGGGTGCCCCCT
+>Caenorhabditis_elegans_tRX-Glu-CTC-1-1 (tRNAscan-SE ID: chrX.trna1) Glu (CTC) 74 bp Sc: 34.2 chrX:86885-86959(+)
+GGCCTGAGTGGTCAAGTGGGTAAGAGGCGCGGCTCTCACCCACACGGTGTGGGTTCGATCCCCGCACCAGGTCA
+>Caenorhabditis_elegans_tRX-Lys-CTT-7-8 (tRNAscan-SE ID: chrX.trna2) Lys (CTT) 75 bp Sc: 20.2 chrX:288446-288521(+)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttta
+>Caenorhabditis_elegans_tRX-Lys-CTT-7-9 (tRNAscan-SE ID: chrX.trna307) Lys (CTT) 75 bp Sc: 20.2 chrX:289512-289587(-)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttta
+>Caenorhabditis_elegans_tRNA-Leu-AAG-3-1 (tRNAscan-SE ID: chrX.trna306) Leu (AAG) 82 bp Sc: 72.6 chrX:353254-353336(-)
+GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-8 (tRNAscan-SE ID: chrX.trna3) Gln (TTG) 72 bp Sc: 72.0 chrX:410390-410462(+)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Thr-TGT-1-6 (tRNAscan-SE ID: chrX.trna4) Thr (TGT) 72 bp Sc: 81.0 chrX:487814-487886(+)
+GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCCTGCGTGGGGGCA
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-12 (tRNAscan-SE ID: chrX.trna305) Asp (GTC) 72 bp Sc: 61.7 chrX:489867-489939(-)
+TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTCCCGGCCGGGGAG
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-2-6 (tRNAscan-SE ID: chrX.trna304) Tyr (GTA) 84 bp Sc: 74.6 chrX:865388-865472(-)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGA
+>Caenorhabditis_elegans_tRNA-Arg-TCG-3-1 (tRNAscan-SE ID: chrX.trna303) Arg (TCG) 73 bp Sc: 69.4 chrX:1089172-1089245(-)
+GGCCGCGTGGCCTAATGGATAAGGCATCAGACTTCGAATCTGGGGATTGCAGGTTCGATCCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRX-Arg-TCG-1-1 (tRNAscan-SE ID: chrX.trna5) Arg (TCG) 75 bp Sc: 58.9 chrX:1089399-1089474(+)
+GGCCGCGTGGCCTAATGGATAAGGCATCAGACTTCGAATCTATGGGGATTGCAGGTTCGATCCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Arg-TCG-3-2 (tRNAscan-SE ID: chrX.trna6) Arg (TCG) 73 bp Sc: 69.4 chrX:1089837-1089910(+)
+GGCCGCGTGGCCTAATGGATAAGGCATCAGACTTCGAATCTGGGGATTGCAGGTTCGATCCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-19 (tRNAscan-SE ID: chrX.trna302) Gly (TCC) 72 bp Sc: 71.7 chrX:1379602-1379674(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRX-Und-NNN-5-1 (tRNAscan-SE ID: chrX.trna301) Und (NNN) 81 bp Sc: 32.3 chrX:1433062-1433143(-)
+GGAGGCATGGCTCAGTGGCAACAAGTTCGACTAACAATCAAAAATGATCATATGTTTTGGGTTCAATTCCCACTGCCTCCG
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-11 (tRNAscan-SE ID: chrX.trna300) Ile (AAT) 74 bp Sc: 86.9 chrX:1589666-1589740(-)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-12 (tRNAscan-SE ID: chrX.trna299) Ile (AAT) 74 bp Sc: 86.9 chrX:1590079-1590153(-)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-13 (tRNAscan-SE ID: chrX.trna298) Ile (AAT) 74 bp Sc: 86.9 chrX:1590507-1590581(-)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRX-Asp-ATC-2-1 (tRNAscan-SE ID: chrX.trna7) Asp (ATC) 81 bp Sc: 25.5 chrX:1620274-1620355(+)
+GGAGGCATGGCTCAATGGCAACGAGTTCGACTATCAATACGAGATGCTTCTATGATTTGGGTTCAATCCCCACTGCCTCCG
+>Caenorhabditis_elegans_tRX-Arg-CCG-2-1 (tRNAscan-SE ID: chrX.trna297) Arg (CCG) 72 bp Sc: 53.0 chrX:1629880-1629952(-)
+GCCCGCGTGGCCTAATGGATAAGGCACCGGACTCCGGAACCGGGAATGGGGGTTCGAGTCCCCCCGCGAGCT
+>Caenorhabditis_elegans_tRX-Asp-ATC-3-1 (tRNAscan-SE ID: chrX.trna8) Asp (ATC) 73 bp Sc: 26.2 chrX:1643849-1643922(+)
+CGGAGGATGGCTCAGTGGAAAACAGCTCGACTATCAATCCAAGCACGCGGGTTCGATTCCCCGACTCTTCCGT
+>Caenorhabditis_elegans_tRX-Ser-CGA-2-1 (tRNAscan-SE ID: chrX.trna296) Ser (CGA) 68 bp Sc: 28.1 chrX:1691082-1691150(-)
+TCAACTGTGAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRX-Ser-CGA-2-2 (tRNAscan-SE ID: chrX.trna9) Ser (CGA) 68 bp Sc: 28.1 chrX:1692733-1692801(+)
+TCAACTGTGAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Arg-TCG-1-1 (tRNAscan-SE ID: chrX.trna10) Arg (TCG) 73 bp Sc: 71.3 chrX:1698673-1698746(+)
+GGCCGCGTGGCCTAATGGATAAGGCACCAGACTTCGAATCTGGGGATTGCAGGTTCGATCCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRX-Phe-GAA-3-1 (tRNAscan-SE ID: chrX.trna11) Phe (GAA) 84 bp Sc: 26.2 chrX:1713606-1713690(+)
+GGCGGAGGATGGCTGAGTGGCTCAAGGCGCTGGTTTGAAGCAATCCTCCGAAGGACGTGATGAGTTCGATTCCCACTCCCCCCG
+>Caenorhabditis_elegans_tRX-Thr-TGT-2-1 (tRNAscan-SE ID: chrX.trna12) Thr (TGT) 104 bp Sc: 37.7 chrX:1744549-1744653(+)
+GGGCCTGTGGTGTAGTGGTTAACACACTGGTCTTGTGAGTCGGACTTTAAATCCCGGCTTCAAGTTCAAAGCCAGAGACGTCGGTTCGAATCCTTCCGGGTTTC
+>Caenorhabditis_elegans_tRNA-Arg-CCT-3-1 (tRNAscan-SE ID: chrX.trna295) Arg (CCT) 74 bp Sc: 56.3 chrX:1764253-1764327(-)
+ACCCGTGTAGCCTAAATGGATAAGGCATCGGTCTCCTAAACCAAAGGATGCGGGTTCGAGTCCTGCCACGGGTG
+>Caenorhabditis_elegans_tRX-Arg-CCT-5-1 (tRNAscan-SE ID: chrX.trna13) Arg (CCT) 73 bp Sc: 42.0 chrX:1775487-1775560(+)
+ACCCGTGTAGCCTAATGGATAAGGCGTCGGTATCCTAATCCAAAGTATGCGGGTTCGAGTCCTGCCACAGGTG
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-8 (tRNAscan-SE ID: chrX.trna14) Glu (TTC) 72 bp Sc: 75.3 chrX:1858818-1858890(+)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Pro-CGG-1-4 (tRNAscan-SE ID: chrX.trna294) Pro (CGG) 72 bp Sc: 71.5 chrX:1880816-1880888(-)
+GGCCGGATGGTCTAGAGGTATGATTCTCGCTTCGGGTGCGAGAGGTCCCGGGTTCGATTCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRX-Leu-TAA-4-1 (tRNAscan-SE ID: chrX.trna15) Leu (TAA) 75 bp Sc: 31.0 chrX:1891445-1891520(+)
+GGCGGCGTGGCCAAGTGGTAAAGCACTGGGCTTAAAAACCAAGTATCCGGGGTTCGACCCCCGGTGCCGGATTTA
+>Caenorhabditis_elegans_tRX-Tyr-ATA-2-1 (tRNAscan-SE ID: chrX.trna293) Tyr (ATA) 89 bp Sc: 20.2 chrX:1982846-1982935(-)
+GGCGGGGGATGGCCGAGTGGTGAAAGGCGCTGTTAGGCGCTATAAAGGACATCGGATGTCTCTGGTTCGATCCCCACGACCCCCCGCCA
+>Caenorhabditis_elegans_tRNA-Thr-TGT-2-1 (tRNAscan-SE ID: chrX.trna16) Thr (TGT) 104 bp Sc: 48.1 chrX:1993447-1993551(+)
+GGGCCTGTGGTGTAGTGGTTAACACACTGGTCTTGTGAGTCGGATTTCATCTCCCGGCTTCAAGTTCAAAGCCAGAGACGTCGGTTCGAATCCTTCCGGGTCCA
+>Caenorhabditis_elegans_tRNA-Thr-TGT-2-2 (tRNAscan-SE ID: chrX.trna292) Thr (TGT) 104 bp Sc: 48.1 chrX:1994212-1994316(-)
+GGGCCTGTGGTGTAGTGGTTAACACACTGGTCTTGTGAGTCGGATTTCATCTCCCGGCTTCAAGTTCAAAGCCAGAGACGTCGGTTCGAATCCTTCCGGGTCCA
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-13 (tRNAscan-SE ID: chrX.trna291) Asp (GTC) 72 bp Sc: 61.7 chrX:2227190-2227262(-)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRX-Lys-CTT-8-9 (tRNAscan-SE ID: chrX.trna17) Lys (CTT) 62 bp Sc: 20.7 chrX:2462560-2462622(+)
+gtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRX-Lys-CTT-8-10 (tRNAscan-SE ID: chrX.trna290) Lys (CTT) 62 bp Sc: 20.7 chrX:2463490-2463552(-)
+gtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-14 (tRNAscan-SE ID: chrX.trna289) Ile (AAT) 74 bp Sc: 86.9 chrX:2526217-2526291(-)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-9 (tRNAscan-SE ID: chrX.trna18) Thr (AGT) 72 bp Sc: 85.3 chrX:2528041-2528113(+)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-2-1 (tRNAscan-SE ID: chrX.trna19) Ile (AAT) 74 bp Sc: 80.0 chrX:2531360-2531434(+)
+GCCGCCATAGCCCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-14 (tRNAscan-SE ID: chrX.trna288) Asn (GTT) 73 bp Sc: 73.5 chrX:2549527-2549600(-)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-14 (tRNAscan-SE ID: chrX.trna20) Asp (GTC) 72 bp Sc: 61.7 chrX:2553564-2553636(+)
+tcctcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Gly-GCC-1-8 (tRNAscan-SE ID: chrX.trna21) Gly (GCC) 71 bp Sc: 77.2 chrX:2613242-2613313(+)
+gcatcggtggttcagtggtagaatgctcgcctgccacgcgggcggcccgggttcgattcccggtcgatgca
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-9 (tRNAscan-SE ID: chrX.trna287) Glu (CTC) 72 bp Sc: 77.9 chrX:3035975-3036047(-)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-20 (tRNAscan-SE ID: chrX.trna22) Gly (TCC) 72 bp Sc: 71.7 chrX:3036163-3036235(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-10 (tRNAscan-SE ID: chrX.trna286) Thr (AGT) 72 bp Sc: 85.3 chrX:3371421-3371493(-)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Met-CAT-1-5 (tRNAscan-SE ID: chrX.trna23) Met (CAT) 73 bp Sc: 77.0 chrX:3697755-3697828(+)
+GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGCCTCACCGGGAGCA
+>Caenorhabditis_elegans_tRNA-Val-TAC-2-1 (tRNAscan-SE ID: chrX.trna285) Val (TAC) 73 bp Sc: 77.5 chrX:3793563-3793636(-)
+GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTTACACGCAGAAGATCGCCGGTTCGATCCCGGCCAGGACCT
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-12 (tRNAscan-SE ID: chrX.trna24) Pro (TGG) 72 bp Sc: 75.2 chrX:3969555-3969627(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-AGG-1-1 (tRNAscan-SE ID: chrX.trna25) Pro (AGG) 72 bp Sc: 72.1 chrX:3970095-3970167(+)
+GGCCGGATGGTCTAGTGGTATGATTCTCGCTTAGGGTGCGAGAGGTCCCGGGATCGATCCCCGGTCCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-AGG-2-1 (tRNAscan-SE ID: chrX.trna26) Pro (AGG) 72 bp Sc: 71.1 chrX:3970264-3970336(+)
+GGCCGGATGGTCTAGTGGTATGATTCTCGCTTAGGGTGCGAGAGGTCCCGGGATCGATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Gly-TCC-7-1 (tRNAscan-SE ID: chrX.trna27) Gly (TCC) 77 bp Sc: 54.5 chrX:3994601-3994678(+)
+GCGTTCGTGGTGTAATGGTCGGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRX-Ile-AAT-1-1 (tRNAscan-SE ID: chrX.trna28) Ile (AAT) 83 bp Sc: 40.4 chrX:4242516-4242599(+)
+ACCTGTGGCGCTTTACCTGTGCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-10 (tRNAscan-SE ID: chrX.trna29) Glu (CTC) 72 bp Sc: 77.9 chrX:4409783-4409855(+)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-11 (tRNAscan-SE ID: chrX.trna30) Glu (CTC) 72 bp Sc: 77.9 chrX:4410651-4410723(+)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-9 (tRNAscan-SE ID: chrX.trna31) Glu (TTC) 72 bp Sc: 75.3 chrX:4444261-4444333(+)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-11 (tRNAscan-SE ID: chrX.trna32) Thr (AGT) 72 bp Sc: 85.3 chrX:4445013-4445085(+)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-10 (tRNAscan-SE ID: chrX.trna33) Lys (TTT) 73 bp Sc: 77.8 chrX:4789131-4789204(+)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-His-GTG-3-4 (tRNAscan-SE ID: chrX.trna284) His (GTG) 72 bp Sc: 67.8 chrX:5022816-5022888(-)
+GCCTGCTTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCAGCAGGCA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-15 (tRNAscan-SE ID: chrX.trna283) Ile (AAT) 74 bp Sc: 86.9 chrX:5085621-5085695(-)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRX-Lys-CTT-7-10 (tRNAscan-SE ID: chrX.trna34) Lys (CTT) 75 bp Sc: 20.2 chrX:5284418-5284493(+)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttta
+>Caenorhabditis_elegans_tRX-Lys-CTT-7-11 (tRNAscan-SE ID: chrX.trna282) Lys (CTT) 75 bp Sc: 20.2 chrX:5285478-5285553(-)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttta
+>Caenorhabditis_elegans_tRNA-Phe-GAA-5-1 (tRNAscan-SE ID: chrX.trna281) Phe (GAA) 73 bp Sc: 81.2 chrX:5319384-5319457(-)
+GCCTCAATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATCCTGGTTTGGGGCA
+>Caenorhabditis_elegans_tRNA-Met-CAT-1-6 (tRNAscan-SE ID: chrX.trna280) Met (CAT) 73 bp Sc: 77.0 chrX:5407412-5407485(-)
+GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGCCTCACCGGGAGCA
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-11 (tRNAscan-SE ID: chrX.trna279) Lys (TTT) 73 bp Sc: 77.8 chrX:5451203-5451276(-)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-Met-CAT-1-7 (tRNAscan-SE ID: chrX.trna35) Met (CAT) 73 bp Sc: 77.0 chrX:5485111-5485184(+)
+GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGCCTCACCGGGAGCA
+>Caenorhabditis_elegans_tRNA-Met-CAT-1-8 (tRNAscan-SE ID: chrX.trna36) Met (CAT) 73 bp Sc: 77.0 chrX:5485454-5485527(+)
+GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGCCTCACCGGGAGCA
+>Caenorhabditis_elegans_tRNA-Met-CAT-1-9 (tRNAscan-SE ID: chrX.trna37) Met (CAT) 73 bp Sc: 77.0 chrX:5485745-5485818(+)
+GCTTCCGTAGCGCAGTAGGCAGCGCGTCAGTCTCATAATCTGAAGGTCGTGAGTTCGAGCCTCACCGGGAGCA
+>Caenorhabditis_elegans_tRNA-Ser-GCT-1-4 (tRNAscan-SE ID: chrX.trna38) Ser (GCT) 82 bp Sc: 84.4 chrX:5708027-5708109(+)
+GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTGAGTTCGAATCTCATCCTGATCG
+>Caenorhabditis_elegans_tRNA-Ser-GCT-1-5 (tRNAscan-SE ID: chrX.trna39) Ser (GCT) 82 bp Sc: 84.4 chrX:5709374-5709456(+)
+GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTGAGTTCGAATCTCATCCTGATCG
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-12 (tRNAscan-SE ID: chrX.trna40) Lys (TTT) 73 bp Sc: 77.8 chrX:5713651-5713724(+)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-13 (tRNAscan-SE ID: chrX.trna278) Pro (TGG) 72 bp Sc: 75.2 chrX:5801210-5801282(-)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-14 (tRNAscan-SE ID: chrX.trna41) Pro (TGG) 72 bp Sc: 75.2 chrX:5801471-5801543(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Arg-ACG-3-1 (tRNAscan-SE ID: chrX.trna277) Arg (ACG) 73 bp Sc: 68.7 chrX:6220069-6220142(-)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Ala-TGC-1-6 (tRNAscan-SE ID: chrX.trna42) Ala (TGC) 72 bp Sc: 68.8 chrX:6286320-6286392(+)
+GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ala-TGC-1-7 (tRNAscan-SE ID: chrX.trna276) Ala (TGC) 72 bp Sc: 68.8 chrX:6292277-6292349(-)
+GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Trp-CCA-1-7 (tRNAscan-SE ID: chrX.trna43) Trp (CCA) 72 bp Sc: 71.5 chrX:6371377-6371449(+)
+GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCCGCTCAGTGGTCA
+>Caenorhabditis_elegans_tRNA-Phe-GAA-4-1 (tRNAscan-SE ID: chrX.trna44) Phe (GAA) 73 bp Sc: 82.5 chrX:6593595-6593668(+)
+GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATCCTGGTTCGGGGCA
+>Caenorhabditis_elegans_tRX-Lys-CTT-6-2 (tRNAscan-SE ID: chrX.trna45) Lys (CTT) 62 bp Sc: 23.2 chrX:6600233-6600295(+)
+gtggtcgagtggtgaacgcattcgcctcttgagcaaaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRX-Lys-CTT-6-3 (tRNAscan-SE ID: chrX.trna275) Lys (CTT) 62 bp Sc: 23.2 chrX:6601313-6601375(-)
+gtggtcgagtggtgaacgcattcgcctcttgagcaaaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRNA-Leu-AAG-3-2 (tRNAscan-SE ID: chrX.trna274) Leu (AAG) 82 bp Sc: 72.6 chrX:6903113-6903195(-)
+GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-12 (tRNAscan-SE ID: chrX.trna273) Thr (AGT) 72 bp Sc: 85.3 chrX:7176982-7177054(-)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-9 (tRNAscan-SE ID: chrX.trna46) Ala (AGC) 72 bp Sc: 74.8 chrX:7323752-7323824(+)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-10 (tRNAscan-SE ID: chrX.trna272) Ala (AGC) 72 bp Sc: 74.8 chrX:7378783-7378855(-)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-11 (tRNAscan-SE ID: chrX.trna271) Ala (AGC) 72 bp Sc: 74.8 chrX:7507289-7507361(-)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-12 (tRNAscan-SE ID: chrX.trna47) Glu (CTC) 72 bp Sc: 77.9 chrX:7681039-7681111(+)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Asn-GTT-2-1 (tRNAscan-SE ID: chrX.trna48) Asn (GTT) 73 bp Sc: 64.4 chrX:7773189-7773262(+)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGATTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-15 (tRNAscan-SE ID: chrX.trna49) Asn (GTT) 73 bp Sc: 73.5 chrX:7773717-7773790(+)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-16 (tRNAscan-SE ID: chrX.trna270) Asn (GTT) 73 bp Sc: 73.5 chrX:7773964-7774037(-)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-21 (tRNAscan-SE ID: chrX.trna269) Gly (TCC) 72 bp Sc: 71.7 chrX:7794335-7794407(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-22 (tRNAscan-SE ID: chrX.trna50) Gly (TCC) 72 bp Sc: 71.7 chrX:7794602-7794674(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-13 (tRNAscan-SE ID: chrX.trna268) Glu (CTC) 72 bp Sc: 77.9 chrX:7898307-7898379(-)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-3-1 (tRNAscan-SE ID: chrX.trna51) Glu (CTC) 72 bp Sc: 73.4 chrX:7906584-7906656(+)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGAAA
+>Caenorhabditis_elegans_tRNA-Arg-ACG-3-2 (tRNAscan-SE ID: chrX.trna267) Arg (ACG) 73 bp Sc: 68.7 chrX:8036684-8036757(-)
+GGCCGCgtggcgcaatggataacgcgtctgcctacggagcagaagattgtaggttcgaatcctgccgtggtcg
+>Caenorhabditis_elegans_tRNA-Pro-AGG-3-1 (tRNAscan-SE ID: chrX.trna52) Pro (AGG) 72 bp Sc: 71.4 chrX:8037506-8037578(+)
+GGTCGGATGGCCTAGAGGTAAGGCGCTTGCTTAGGGTGCAAGAGATCCCGGGTTCGATCCCCGGTTCGACCC
+>Caenorhabditis_elegans_tRX-Ser-AGA-3-1 (tRNAscan-SE ID: chrX.trna53) Ser (AGA) 99 bp Sc: 24.7 chrX:8148872-8148971(+)
+GCAGGTTGCCACTAACCTGACGCGCTTTACCTGTGTTAAGGAGATTAACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-15 (tRNAscan-SE ID: chrX.trna54) Asp (GTC) 72 bp Sc: 61.7 chrX:8149155-8149227(+)
+TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTCCCGGCCGGGGAG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-16 (tRNAscan-SE ID: chrX.trna266) Asp (GTC) 72 bp Sc: 61.7 chrX:8152545-8152617(-)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Ser-AGA-2-7 (tRNAscan-SE ID: chrX.trna265) Ser (AGA) 82 bp Sc: 81.6 chrX:8152811-8152893(-)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Ser-AGA-2-8 (tRNAscan-SE ID: chrX.trna55) Ser (AGA) 82 bp Sc: 81.6 chrX:8154444-8154526(+)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-17 (tRNAscan-SE ID: chrX.trna56) Asp (GTC) 72 bp Sc: 61.7 chrX:8154721-8154793(+)
+TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTCCCGGCCGGGGAG
+>Caenorhabditis_elegans_tRNA-Ser-AGA-2-9 (tRNAscan-SE ID: chrX.trna57) Ser (AGA) 82 bp Sc: 81.6 chrX:8155461-8155543(+)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-7-1 (tRNAscan-SE ID: chrX.trna58) Asp (GTC) 73 bp Sc: 54.8 chrX:8155751-8155824(+)
+TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTCCCGGCCGGGAGAA
+>Caenorhabditis_elegans_tRNA-iMet-CAT-1-7 (tRNAscan-SE ID: chrX.trna59) iMet (CAT) 72 bp Sc: 61.2 chrX:8156177-8156249(+)
+AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAACCACTCGCTGCTA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-16 (tRNAscan-SE ID: chrX.trna264) Ile (AAT) 74 bp Sc: 86.9 chrX:8156633-8156707(-)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Arg-TCT-3-1 (tRNAscan-SE ID: chrX.trna263) Arg (TCT) 73 bp Sc: 68.8 chrX:8381794-8381867(-)
+GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGACCCCTGCCTGGGTCA
+>Caenorhabditis_elegans_tRNA-Arg-TCT-2-4 (tRNAscan-SE ID: chrX.trna60) Arg (TCT) 73 bp Sc: 71.1 chrX:8386203-8386276(+)
+GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGAGCCCTGCCTGGGTCA
+>Caenorhabditis_elegans_tRNA-Arg-TCT-2-5 (tRNAscan-SE ID: chrX.trna61) Arg (TCT) 73 bp Sc: 71.1 chrX:8386613-8386686(+)
+GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGAGCCCTGCCTGGGTCA
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-17 (tRNAscan-SE ID: chrX.trna62) Asn (GTT) 73 bp Sc: 73.5 chrX:8404498-8404571(+)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Leu-AAG-6-1 (tRNAscan-SE ID: chrX.trna262) Leu (AAG) 82 bp Sc: 32.9 chrX:8409295-8409377(-)
+GGAGAGATGCCCGAGCTGTCTAAGGCGCTGATTTAAGGCACCAGCCTTTTCGGGGGCGTGAGTTCGAATCCCACTCTCTTCT
+>Caenorhabditis_elegans_tRNA-Leu-AAG-3-3 (tRNAscan-SE ID: chrX.trna261) Leu (AAG) 82 bp Sc: 72.6 chrX:8417911-8417993(-)
+GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Leu-AAG-3-4 (tRNAscan-SE ID: chrX.trna260) Leu (AAG) 82 bp Sc: 72.6 chrX:8419413-8419495(-)
+GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRX-Lys-CTT-8-11 (tRNAscan-SE ID: chrX.trna259) Lys (CTT) 62 bp Sc: 20.7 chrX:8459043-8459105(-)
+gtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRNA-Gln-CTG-2-4 (tRNAscan-SE ID: chrX.trna258) Gln (CTG) 72 bp Sc: 71.6 chrX:8608833-8608905(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTCTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGGACCT
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-9 (tRNAscan-SE ID: chrX.trna63) Gln (TTG) 72 bp Sc: 72.0 chrX:8609037-8609109(+)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Arg-ACG-5-1 (tRNAscan-SE ID: chrX.trna64) Arg (ACG) 73 bp Sc: 57.5 chrX:8623602-8623675(+)
+GGCCGCGTGGGGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Cys-GCA-1-6 (tRNAscan-SE ID: chrX.trna257) Cys (GCA) 72 bp Sc: 74.0 chrX:8623763-8623835(-)
+GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTCCGGGTGCCCCCT
+>Caenorhabditis_elegans_tRNA-Cys-GCA-1-7 (tRNAscan-SE ID: chrX.trna256) Cys (GCA) 72 bp Sc: 74.0 chrX:8623997-8624069(-)
+GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTCCGGGTGCCCCCT
+>Caenorhabditis_elegans_tRNA-Cys-GCA-1-8 (tRNAscan-SE ID: chrX.trna65) Cys (GCA) 72 bp Sc: 74.0 chrX:8624281-8624353(+)
+GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTCCGGGTGCCCCCT
+>Caenorhabditis_elegans_tRNA-Arg-ACG-3-3 (tRNAscan-SE ID: chrX.trna255) Arg (ACG) 73 bp Sc: 68.7 chrX:8624459-8624532(-)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Cys-GCA-1-9 (tRNAscan-SE ID: chrX.trna254) Cys (GCA) 72 bp Sc: 74.0 chrX:8638619-8638691(-)
+GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTCCGGGTGCCCCCT
+>Caenorhabditis_elegans_tRNA-Cys-GCA-1-10 (tRNAscan-SE ID: chrX.trna66) Cys (GCA) 72 bp Sc: 74.0 chrX:8638921-8638993(+)
+GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTCCGGGTGCCCCCT
+>Caenorhabditis_elegans_tRNA-Arg-ACG-4-1 (tRNAscan-SE ID: chrX.trna253) Arg (ACG) 71 bp Sc: 54.4 chrX:8639224-8639295(-)
+GGCCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Arg-ACG-3-4 (tRNAscan-SE ID: chrX.trna252) Arg (ACG) 73 bp Sc: 68.7 chrX:8640793-8640866(-)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-10 (tRNAscan-SE ID: chrX.trna67) Glu (TTC) 72 bp Sc: 75.3 chrX:8646479-8646551(+)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Val-AAC-2-9 (tRNAscan-SE ID: chrX.trna251) Val (AAC) 73 bp Sc: 76.6 chrX:8650708-8650781(-)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Gly-GCC-1-9 (tRNAscan-SE ID: chrX.trna250) Gly (GCC) 71 bp Sc: 77.2 chrX:8796821-8796892(-)
+gcatcggtggttcagtggtagaatgctcgcctgccacgcgggcggcccgggttcgattcccggtcgatgca
+>Caenorhabditis_elegans_tRNA-Cys-GCA-1-11 (tRNAscan-SE ID: chrX.trna249) Cys (GCA) 72 bp Sc: 74.0 chrX:8818099-8818171(-)
+GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTCCGGGTGCCCCCT
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-23 (tRNAscan-SE ID: chrX.trna248) Gly (TCC) 72 bp Sc: 71.7 chrX:8818577-8818649(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-4-1 (tRNAscan-SE ID: chrX.trna68) Gly (TCC) 72 bp Sc: 61.8 chrX:8819680-8819752(+)
+GAGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-24 (tRNAscan-SE ID: chrX.trna247) Gly (TCC) 72 bp Sc: 71.7 chrX:8819923-8819995(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-25 (tRNAscan-SE ID: chrX.trna69) Gly (TCC) 72 bp Sc: 71.7 chrX:8820184-8820256(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-11 (tRNAscan-SE ID: chrX.trna70) Glu (TTC) 72 bp Sc: 75.3 chrX:8836112-8836184(+)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-26 (tRNAscan-SE ID: chrX.trna246) Gly (TCC) 72 bp Sc: 71.7 chrX:8838337-8838409(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-3-1 (tRNAscan-SE ID: chrX.trna245) Gly (TCC) 73 bp Sc: 67.4 chrX:8846504-8846577(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-2-1 (tRNAscan-SE ID: chrX.trna71) Gly (TCC) 72 bp Sc: 68.1 chrX:8846720-8846792(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCTCGAACGCA
+>Caenorhabditis_elegans_tRNA-Trp-CCA-1-8 (tRNAscan-SE ID: chrX.trna72) Trp (CCA) 72 bp Sc: 71.5 chrX:8877339-8877411(+)
+GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCCGCTCAGTGGTCA
+>Caenorhabditis_elegans_tRNA-Gln-TTG-4-1 (tRNAscan-SE ID: chrX.trna73) Gln (TTG) 72 bp Sc: 62.2 chrX:8925640-8925712(+)
+GGTTCCATGGTGTAGCGGTTAGCACTCATGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Leu-AAG-3-5 (tRNAscan-SE ID: chrX.trna74) Leu (AAG) 82 bp Sc: 72.6 chrX:8939549-8939631(+)
+GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Trp-CCA-1-9 (tRNAscan-SE ID: chrX.trna244) Trp (CCA) 72 bp Sc: 71.5 chrX:8944231-8944303(-)
+GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCCGCTCAGTGGTCA
+>Caenorhabditis_elegans_tRNA-Trp-CCA-1-10 (tRNAscan-SE ID: chrX.trna243) Trp (CCA) 72 bp Sc: 71.5 chrX:8945159-8945231(-)
+GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGGTTGGGCGTTCGATCCGCTCAGTGGTCA
+>Caenorhabditis_elegans_tRNA-Leu-AAG-3-6 (tRNAscan-SE ID: chrX.trna242) Leu (AAG) 82 bp Sc: 72.6 chrX:8955919-8956001(-)
+GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-15 (tRNAscan-SE ID: chrX.trna241) Pro (TGG) 72 bp Sc: 75.2 chrX:8969487-8969559(-)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-16 (tRNAscan-SE ID: chrX.trna75) Pro (TGG) 72 bp Sc: 75.2 chrX:8969737-8969809(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Ser-AGA-2-10 (tRNAscan-SE ID: chrX.trna76) Ser (AGA) 82 bp Sc: 81.6 chrX:8971599-8971681(+)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Thr-TGT-1-7 (tRNAscan-SE ID: chrX.trna240) Thr (TGT) 72 bp Sc: 81.0 chrX:9024412-9024484(-)
+GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCCTGCGTGGGGGCA
+>Caenorhabditis_elegans_tRNA-Thr-CGT-1-1 (tRNAscan-SE ID: chrX.trna239) Thr (CGT) 72 bp Sc: 83.8 chrX:9025662-9025734(-)
+GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTCGTAAACCAAAGGTCCGTAGTTCAATCCTGCGTGAGGGCA
+>Caenorhabditis_elegans_tRNA-Pro-AGG-5-1 (tRNAscan-SE ID: chrX.trna238) Pro (AGG) 115 bp Sc: 68.5 chrX:9059279-9059394(-)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGCCAAGGCCCAAGGTCGCCCAAGGCCCAAGGTCGCCCAAGGCCAAGGTAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Gln-TTG-5-1 (tRNAscan-SE ID: chrX.trna237) Gln (TTG) 72 bp Sc: 61.2 chrX:9074671-9074743(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGATCCAAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-10 (tRNAscan-SE ID: chrX.trna236) Gln (TTG) 72 bp Sc: 72.0 chrX:9078253-9078325(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-11 (tRNAscan-SE ID: chrX.trna235) Gln (TTG) 72 bp Sc: 72.0 chrX:9090626-9090698(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Gln-CTG-2-5 (tRNAscan-SE ID: chrX.trna77) Gln (CTG) 72 bp Sc: 71.6 chrX:9090829-9090901(+)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTCTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGGACCT
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-12 (tRNAscan-SE ID: chrX.trna234) Gln (TTG) 72 bp Sc: 72.0 chrX:9091096-9091168(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Gln-TTG-3-1 (tRNAscan-SE ID: chrX.trna78) Gln (TTG) 72 bp Sc: 64.1 chrX:9091309-9091381(+)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCAGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-13 (tRNAscan-SE ID: chrX.trna233) Gln (TTG) 72 bp Sc: 72.0 chrX:9091556-9091628(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-12 (tRNAscan-SE ID: chrX.trna79) Ala (AGC) 72 bp Sc: 74.8 chrX:9237810-9237882(+)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-13 (tRNAscan-SE ID: chrX.trna80) Ala (AGC) 72 bp Sc: 74.8 chrX:9238863-9238935(+)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-iMet-CAT-1-8 (tRNAscan-SE ID: chrX.trna232) iMet (CAT) 72 bp Sc: 61.2 chrX:9373149-9373221(-)
+AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAACCACTCGCTGCTA
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-17 (tRNAscan-SE ID: chrX.trna231) Pro (TGG) 72 bp Sc: 75.2 chrX:9467728-9467800(-)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Val-AAC-2-10 (tRNAscan-SE ID: chrX.trna230) Val (AAC) 73 bp Sc: 76.6 chrX:9561087-9561160(-)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-14 (tRNAscan-SE ID: chrX.trna229) Ala (AGC) 72 bp Sc: 74.8 chrX:9622823-9622895(-)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-15 (tRNAscan-SE ID: chrX.trna228) Ala (AGC) 72 bp Sc: 74.8 chrX:9637851-9637923(-)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ala-TGC-1-8 (tRNAscan-SE ID: chrX.trna81) Ala (TGC) 72 bp Sc: 68.8 chrX:9743588-9743660(+)
+GGGGGTATAGCTCAGGGGTAGAGCGCTCGCTTTGCATGCGAGAAGTCTGGGGTTCGATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-16 (tRNAscan-SE ID: chrX.trna82) Ala (AGC) 72 bp Sc: 74.8 chrX:9743746-9743818(+)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Ile-TAT-1-4 (tRNAscan-SE ID: chrX.trna227) Ile (TAT) 85 bp Sc: 84.7 chrX:9829666-9829751(-)
+GCCCCGGTGGCCGAGCGGTCGAAGGCGTGAGACTTATGATCTCATTGGGTTAAACCAGTCGCGGGTTCGAATCCCGCCCGGGGCA
+>Caenorhabditis_elegans_tRNA-Arg-ACG-2-1 (tRNAscan-SE ID: chrX.trna226) Arg (ACG) 73 bp Sc: 71.6 chrX:10018424-10018497(-)
+GGCCGCgtggcgcaatggataacgcgtctgcctacggagcagaagattgtaggttcgaatcctaccgtggtcg
+>Caenorhabditis_elegans_tRNA-Ser-TGA-1-1 (tRNAscan-SE ID: chrX.trna83) Ser (TGA) 82 bp Sc: 84.9 chrX:10124497-10124579(+)
+GCTGCGATGTCCGAGTGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCGTAGGTTCAAATCCTGCTCGCAGCG
+>Caenorhabditis_elegans_tRNA-Arg-ACG-3-5 (tRNAscan-SE ID: chrX.trna84) Arg (ACG) 73 bp Sc: 68.7 chrX:10132677-10132750(+)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Arg-ACG-3-6 (tRNAscan-SE ID: chrX.trna225) Arg (ACG) 73 bp Sc: 68.7 chrX:10132970-10133043(-)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Arg-ACG-3-7 (tRNAscan-SE ID: chrX.trna85) Arg (ACG) 73 bp Sc: 68.7 chrX:10145155-10145228(+)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Arg-ACG-3-8 (tRNAscan-SE ID: chrX.trna224) Arg (ACG) 73 bp Sc: 68.7 chrX:10148648-10148721(-)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-12 (tRNAscan-SE ID: chrX.trna223) Glu (TTC) 72 bp Sc: 75.3 chrX:10667021-10667093(-)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-13 (tRNAscan-SE ID: chrX.trna86) Glu (TTC) 72 bp Sc: 75.3 chrX:10667592-10667664(+)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Arg-ACG-3-9 (tRNAscan-SE ID: chrX.trna222) Arg (ACG) 73 bp Sc: 68.7 chrX:10731988-10732061(-)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-14 (tRNAscan-SE ID: chrX.trna221) Glu (TTC) 72 bp Sc: 75.3 chrX:10821326-10821398(-)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-27 (tRNAscan-SE ID: chrX.trna87) Gly (TCC) 72 bp Sc: 71.7 chrX:10963827-10963899(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Leu-TAG-1-3 (tRNAscan-SE ID: chrX.trna88) Leu (TAG) 82 bp Sc: 75.3 chrX:11095672-11095754(+)
+GGTGAGATGGCCGAGTGGTCTAAGGCGCTGGTTTTAGGCACCAGTCCCTCCGGGGGCGTGGGTTCGAATCCCACTCTCATCA
+>Caenorhabditis_elegans_tRNA-Leu-AAG-3-7 (tRNAscan-SE ID: chrX.trna220) Leu (AAG) 82 bp Sc: 72.6 chrX:11162918-11163000(-)
+GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Leu-AAG-3-8 (tRNAscan-SE ID: chrX.trna219) Leu (AAG) 82 bp Sc: 72.6 chrX:11163357-11163439(-)
+GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Arg-ACG-3-10 (tRNAscan-SE ID: chrX.trna218) Arg (ACG) 73 bp Sc: 68.7 chrX:11252589-11252662(-)
+GGCCGCGTGGCGCAATGGATAACGCGTCTGCCTACGGAGCAGAAGATTGTAGGTTCGAATCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Asn-GTT-1-18 (tRNAscan-SE ID: chrX.trna89) Asn (GTT) 73 bp Sc: 73.5 chrX:11645682-11645755(+)
+GCTTCCGTGGCGCAATAGGCAGCGCGTTCGGCTGTTAACCGAAAGGTTGGTGGTTCGAGCCCACCCGGGAGCG
+>Caenorhabditis_elegans_tRNA-Leu-TAA-1-2 (tRNAscan-SE ID: chrX.trna217) Leu (TAA) 84 bp Sc: 77.4 chrX:11757830-11757914(-)
+AGCACGATGGCCGAGTGGTTAAGGCGTTGGACTTAAGTTCCAATGGTGGATAACACCTCGTGGGTTCGAACCCCACTCGTGCTA
+>Caenorhabditis_elegans_tRX-Arg-TCG-3-1 (tRNAscan-SE ID: chrX.trna216) Arg (TCG) 73 bp Sc: 45.2 chrX:11806587-11806660(-)
+GGTCGCGTCGCCTAATGGATAAGCCACCAGACTTCGAATCTGGGGATTACAGGTTCGATCCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-14 (tRNAscan-SE ID: chrX.trna215) Gln (TTG) 72 bp Sc: 72.0 chrX:11872240-11872312(-)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Gln-CTG-3-1 (tRNAscan-SE ID: chrX.trna90) Gln (CTG) 72 bp Sc: 61.0 chrX:11872505-11872577(+)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGTACTCTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGGACCT
+>Caenorhabditis_elegans_tRNA-Thr-CGT-6-1 (tRNAscan-SE ID: chrX.trna91) Thr (CGT) 72 bp Sc: 75.7 chrX:11933727-11933799(+)
+GCCCGTATAGCTCAGAGGCAGAGCGTCTGTCTCGTAAACAGAAGGTCGGCGGTTCAATCCCGCCTGTGGGCA
+>Caenorhabditis_elegans_tRNA-Thr-CGT-4-1 (tRNAscan-SE ID: chrX.trna214) Thr (CGT) 72 bp Sc: 76.0 chrX:11935079-11935151(-)
+GCCCGTATAGCTCAGTGGCAGAGCGTCTGTCTCGTAAACAGAAGGTCGGCGGTTCAATCCCGCCTGGGGGCA
+>Caenorhabditis_elegans_tRNA-His-GTG-2-4 (tRNAscan-SE ID: chrX.trna213) His (GTG) 72 bp Sc: 69.4 chrX:11993520-11993592(-)
+GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCCGCAGGCA
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-16 (tRNAscan-SE ID: chrX.trna212) Lys (CTT) 73 bp Sc: 85.9 chrX:12106146-12106219(-)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRX-Lys-CTT-6-4 (tRNAscan-SE ID: chrX.trna92) Lys (CTT) 62 bp Sc: 23.2 chrX:12166225-12166287(+)
+gtggtcgagtggtgaacgcattcgcctcttgagcaaaagtttgtgggttcggttcccacaca
+>Caenorhabditis_elegans_tRNA-Arg-TCG-2-4 (tRNAscan-SE ID: chrX.trna211) Arg (TCG) 73 bp Sc: 71.0 chrX:12337997-12338070(-)
+GGCCGCGTGGCCTAATGGATAAGGCACCAGACTTCGAATCTGGGGATTGCAGGTTCGAGTCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Leu-CAA-1-5 (tRNAscan-SE ID: chrX.trna210) Leu (CAA) 120 bp Sc: 74.2 chrX:12348006-12348126(-)
+GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCGAATCGCTTGCCTCAAGTTCGAGGTCAACTGGGTGTTCTGGTACTCGTATGGGTGCGTGGGTTCGAATCCCACTTCGTGCA
+>Caenorhabditis_elegans_tRNA-Glu-TTC-1-15 (tRNAscan-SE ID: chrX.trna209) Glu (TTC) 72 bp Sc: 75.3 chrX:12367641-12367713(-)
+TCCCATGTGGTCTAGTGGTTAGGATTCGTGGTTTTCACCCACGCGGCCCGGGTTCGATTCCCGGCATGGGAA
+>Caenorhabditis_elegans_tRNA-Ala-AGC-1-17 (tRNAscan-SE ID: chrX.trna208) Ala (AGC) 72 bp Sc: 74.8 chrX:12458175-12458247(-)
+GGGGGTATAGCTCAGTGGTAGAGCGCTCCCTTAGCATGGGAGAGGGCTGGGGTTCAATTCCCCATACCTCCA
+>Caenorhabditis_elegans_tRNA-Thr-TGT-1-8 (tRNAscan-SE ID: chrX.trna93) Thr (TGT) 72 bp Sc: 81.0 chrX:12563787-12563859(+)
+GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCCTGCGTGGGGGCA
+>Caenorhabditis_elegans_tRNA-Ile-TAT-2-3 (tRNAscan-SE ID: chrX.trna94) Ile (TAT) 84 bp Sc: 76.7 chrX:12661163-12661247(+)
+GCCCCATTGGCGCAGTCGGTTAGCGCGTGGTACTTATAGTTATAGGTCATGCCAAGGTCGCCAGTTCGAGCCTGGCATGGGGCA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-2-7 (tRNAscan-SE ID: chrX.trna95) Tyr (GTA) 84 bp Sc: 74.6 chrX:12665227-12665311(+)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGA
+>Caenorhabditis_elegans_tRNA-Val-AAC-2-11 (tRNAscan-SE ID: chrX.trna96) Val (AAC) 73 bp Sc: 76.6 chrX:12843687-12843760(+)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Pro-TGG-3-1 (tRNAscan-SE ID: chrX.trna207) Pro (TGG) 72 bp Sc: 66.7 chrX:12854839-12854911(-)
+GGCCGAATGGTCTATTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Ser-TGA-4-1 (tRNAscan-SE ID: chrX.trna97) Ser (TGA) 82 bp Sc: 81.8 chrX:12889939-12890021(+)
+GCAACGATGTCCGAGTGGTTAAGGAGATGGACTTGAAATCCATTGGGCTTTGCCCGCGTAGGTTCGATTCCTGCTCGTTGCG
+>Caenorhabditis_elegans_tRNA-Ala-CGC-1-1 (tRNAscan-SE ID: chrX.trna206) Ala (CGC) 72 bp Sc: 73.7 chrX:12890284-12890356(-)
+GGGGGCATAGCTCAGGGGTAGAGCGCTCGCTTCGCATGCGAGAAGTCCGGGGTTCAATTCCCCGTGCCTCCA
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-15 (tRNAscan-SE ID: chrX.trna98) Gln (TTG) 72 bp Sc: 72.0 chrX:12937700-12937772(+)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Gln-TTG-1-16 (tRNAscan-SE ID: chrX.trna99) Gln (TTG) 72 bp Sc: 72.0 chrX:12938181-12938253(+)
+GGTTCCATGGTGTAGCGGTTAGCACTCAGGACTTTGAATCCTGCGACCCGAGTTCAAATCTCGGTGGAACCT
+>Caenorhabditis_elegans_tRNA-Leu-AAG-3-9 (tRNAscan-SE ID: chrX.trna100) Leu (AAG) 82 bp Sc: 72.6 chrX:12942457-12942539(+)
+GGAGAGATGGCCGAGCGGTCTAAGGCGCTGGTTTAAGGCACCAGTCCCTTCGGGGGCGTGGGTTCGAATCCCACTCTCTTCA
+>Caenorhabditis_elegans_tRNA-Leu-CAG-2-3 (tRNAscan-SE ID: chrX.trna205) Leu (CAG) 84 bp Sc: 76.8 chrX:13038959-13039043(-)
+GCCGTTCTGGCCGAGTGGTCTAAGGCGCTGCGTTCAGGTCGCAGTCCTCTCCGGAGGGCGCAGGTTCGAATCCTGCGGACGGCA
+>Caenorhabditis_elegans_tRNA-Ser-CGA-1-3 (tRNAscan-SE ID: chrX.trna204) Ser (CGA) 82 bp Sc: 84.2 chrX:13046365-13046447(-)
+GCAGTCATGTCCGAGTGGTTAAGGAGTTTGACTCGAAATCAAATGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Ser-AGA-2-11 (tRNAscan-SE ID: chrX.trna101) Ser (AGA) 82 bp Sc: 81.6 chrX:13046577-13046659(+)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Gly-GCC-1-10 (tRNAscan-SE ID: chrX.trna203) Gly (GCC) 71 bp Sc: 77.2 chrX:13121260-13121331(-)
+gcatcggtggttcagtggtagaatgctcgcctgccacgcgggcggcccgggttcgattcccggtcgatgca
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-13 (tRNAscan-SE ID: chrX.trna102) Thr (AGT) 72 bp Sc: 85.3 chrX:13261202-13261274(+)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-2-8 (tRNAscan-SE ID: chrX.trna202) Tyr (GTA) 84 bp Sc: 74.6 chrX:13264682-13264766(-)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCGGGTATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGA
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-14 (tRNAscan-SE ID: chrX.trna201) Thr (AGT) 72 bp Sc: 85.3 chrX:13283636-13283708(-)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-5-1 (tRNAscan-SE ID: chrX.trna200) Tyr (GTA) 84 bp Sc: 68.8 chrX:13284765-13284849(-)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCACTGGTTCGAATCCGGTTGGACGGA
+>Caenorhabditis_elegans_tRNA-Thr-AGT-1-15 (tRNAscan-SE ID: chrX.trna103) Thr (AGT) 72 bp Sc: 85.3 chrX:13293191-13293263(+)
+GCCTCATTGGCTCAGTGGCAGAGCGTCTGTCTAGTAAACAGAAGGTCGCTGGTTCGATTCCAGCATGAGGCA
+>Caenorhabditis_elegans_tRNA-Val-TAC-3-2 (tRNAscan-SE ID: chrX.trna104) Val (TAC) 73 bp Sc: 77.2 chrX:13307033-13307106(+)
+GGTCCTATGGTGTAGTGGTTATCACGTCTGCTTTACACGCAGAAGATCGCCGGTTCGAACCCGGCTAGGACCT
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-18 (tRNAscan-SE ID: chrX.trna105) Pro (TGG) 72 bp Sc: 75.2 chrX:13308029-13308101(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-17 (tRNAscan-SE ID: chrX.trna199) Ile (AAT) 74 bp Sc: 86.9 chrX:13415119-13415193(-)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-18 (tRNAscan-SE ID: chrX.trna106) Ile (AAT) 74 bp Sc: 86.9 chrX:13435965-13436039(+)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Ser-GCT-2-1 (tRNAscan-SE ID: chrX.trna107) Ser (GCT) 82 bp Sc: 83.4 chrX:13442642-13442724(+)
+GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTGAGTTCGAATCTCATCTTGATCG
+>Caenorhabditis_elegans_tRNA-Leu-CAA-2-1 (tRNAscan-SE ID: chrX.trna198) Leu (CAA) 119 bp Sc: 72.2 chrX:13443385-13443504(-)
+GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCAATAGCTTGCTTCAAGTTCGAAGCCGATTGGGCGTTCTGGTACTCGTACGGGTGCGTGGGTTCGAATCCCACTTCGTGCA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-14 (tRNAscan-SE ID: chrX.trna108) Glu (CTC) 72 bp Sc: 77.9 chrX:13448676-13448748(+)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Ser-GCT-1-6 (tRNAscan-SE ID: chrX.trna197) Ser (GCT) 82 bp Sc: 84.4 chrX:13448872-13448954(-)
+GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTGAGTTCGAATCTCATCCTGATCG
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-19 (tRNAscan-SE ID: chrX.trna196) Pro (TGG) 72 bp Sc: 75.2 chrX:13511969-13512041(-)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Thr-TGT-1-9 (tRNAscan-SE ID: chrX.trna109) Thr (TGT) 72 bp Sc: 81.0 chrX:13653727-13653799(+)
+GCCCTTATAGCTCAGTGGTAGAGCGTTGGTCTTGTAAACCAAAGGTCCGTAGTTCAATCCTGCGTGGGGGCA
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-17 (tRNAscan-SE ID: chrX.trna195) Lys (CTT) 73 bp Sc: 85.9 chrX:13655916-13655989(-)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Leu-CAA-1-6 (tRNAscan-SE ID: chrX.trna110) Leu (CAA) 119 bp Sc: 74.2 chrX:13665554-13665673(+)
+GCACGGATGGCCGAGTGGTCTAAGGCGCCAGACTCAAGCGATTGCTTGCCTCAAGTACGAGGTCTCCTGGGTGTTCTGGTACTCGTATGGGTGCGTGGGTTCGAATCCCACTTCGTGCA
+>Caenorhabditis_elegans_tRNA-Lys-CTT-7-1 (tRNAscan-SE ID: chrX.trna194) Lys (CTT) 89 bp Sc: 71.5 chrX:13713638-13713727(-)
+GCCCGGTTAGCTCAGTCGCGAGTCGCGAGTCGCGGTAGAGCACCAGATTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-18 (tRNAscan-SE ID: chrX.trna111) Lys (CTT) 73 bp Sc: 85.9 chrX:13714887-13714960(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-5-1 (tRNAscan-SE ID: chrX.trna112) Lys (CTT) 73 bp Sc: 75.4 chrX:13716492-13716565(+)
+GCCTGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGTTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-19 (tRNAscan-SE ID: chrX.trna113) Lys (CTT) 73 bp Sc: 85.9 chrX:13717194-13717267(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-3-1 (tRNAscan-SE ID: chrX.trna114) Lys (CTT) 73 bp Sc: 79.6 chrX:13729904-13729977(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTCTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-20 (tRNAscan-SE ID: chrX.trna115) Lys (CTT) 73 bp Sc: 85.9 chrX:13730356-13730429(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-21 (tRNAscan-SE ID: chrX.trna116) Lys (CTT) 73 bp Sc: 85.9 chrX:13730777-13730850(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-22 (tRNAscan-SE ID: chrX.trna117) Lys (CTT) 73 bp Sc: 85.9 chrX:13781639-13781712(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-23 (tRNAscan-SE ID: chrX.trna118) Lys (CTT) 73 bp Sc: 85.9 chrX:13782248-13782321(+)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRX-Gly-TCC-3-1 (tRNAscan-SE ID: chrX.trna193) Gly (TCC) 73 bp Sc: 29.7 chrX:13886368-13886441(-)
+GACGTGTGTGGTCTAGTGGGTAAGGTGCGCGCCTTCCACCCACATGGTGCGGGTTCAATCCCCGCAGCGGTCA
+>Caenorhabditis_elegans_tRX-Gly-TCC-2-1 (tRNAscan-SE ID: chrX.trna119) Gly (TCC) 79 bp Sc: 30.8 chrX:14010245-14010324(+)
+GCATGTCGCGGTTTACCTGTGATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-15 (tRNAscan-SE ID: chrX.trna120) Glu (CTC) 72 bp Sc: 77.9 chrX:14015943-14016015(+)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRX-Lys-CTT-7-12 (tRNAscan-SE ID: chrX.trna121) Lys (CTT) 75 bp Sc: 20.2 chrX:14061671-14061746(+)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttta
+>Caenorhabditis_elegans_tRX-Lys-CTT-7-13 (tRNAscan-SE ID: chrX.trna192) Lys (CTT) 75 bp Sc: 20.2 chrX:14062438-14062513(-)
+ggttcggtggtcgagtggtgaacgcgttcgcctcttgagcagaagtttgtgggttcggttcccatacatggttta
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-13 (tRNAscan-SE ID: chrX.trna191) Lys (TTT) 73 bp Sc: 77.8 chrX:14063945-14064018(-)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-Arg-CCT-1-2 (tRNAscan-SE ID: chrX.trna122) Arg (CCT) 73 bp Sc: 69.7 chrX:14115690-14115763(+)
+GGCCGTGTGGCCTAATGGATAAGGCGTCGGTCTCCTAAACCGAAGACTGCAGGTTCGAGTCCTGCCTCGGTCG
+>Caenorhabditis_elegans_tRNA-His-GTG-2-5 (tRNAscan-SE ID: chrX.trna123) His (GTG) 72 bp Sc: 69.4 chrX:14135044-14135116(+)
+GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCCGCAGGCA
+>Caenorhabditis_elegans_tRNA-His-GTG-2-6 (tRNAscan-SE ID: chrX.trna190) His (GTG) 72 bp Sc: 69.4 chrX:14135307-14135379(-)
+GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCCGCAGGCA
+>Caenorhabditis_elegans_tRNA-His-GTG-2-7 (tRNAscan-SE ID: chrX.trna124) His (GTG) 72 bp Sc: 69.4 chrX:14135873-14135945(+)
+GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCCGCAGGCA
+>Caenorhabditis_elegans_tRNA-His-GTG-2-8 (tRNAscan-SE ID: chrX.trna189) His (GTG) 72 bp Sc: 69.4 chrX:14136123-14136195(-)
+GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCCGCAGGCA
+>Caenorhabditis_elegans_tRNA-His-GTG-2-9 (tRNAscan-SE ID: chrX.trna125) His (GTG) 72 bp Sc: 69.4 chrX:14136689-14136761(+)
+GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCCGCAGGCA
+>Caenorhabditis_elegans_tRNA-His-GTG-2-10 (tRNAscan-SE ID: chrX.trna188) His (GTG) 72 bp Sc: 69.4 chrX:14136938-14137010(-)
+GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCCGCAGGCA
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-18 (tRNAscan-SE ID: chrX.trna187) Asp (GTC) 72 bp Sc: 61.7 chrX:14162025-14162097(-)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Ser-AGA-1-2 (tRNAscan-SE ID: chrX.trna126) Ser (AGA) 82 bp Sc: 82.3 chrX:14162214-14162296(+)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTTTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Trp-CCA-2-1 (tRNAscan-SE ID: chrX.trna186) Trp (CCA) 72 bp Sc: 68.3 chrX:14228919-14228991(-)
+GACTGCTTGGCGCAATGGTAGCGCGTTCGACTCCAGATCGAAAGATTGGGCGTTCGATCCGCTCAGTGGTCA
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-20 (tRNAscan-SE ID: chrX.trna185) Pro (TGG) 72 bp Sc: 75.2 chrX:14437872-14437944(-)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-21 (tRNAscan-SE ID: chrX.trna127) Pro (TGG) 72 bp Sc: 75.2 chrX:14438101-14438173(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-24 (tRNAscan-SE ID: chrX.trna184) Lys (CTT) 73 bp Sc: 85.9 chrX:14478876-14478949(-)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRNA-Lys-CTT-6-1 (tRNAscan-SE ID: chrX.trna183) Lys (CTT) 81 bp Sc: 58.5 chrX:14486207-14486288(-)
+TAAAAGTAAAAATAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCTTAT
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-19 (tRNAscan-SE ID: chrX.trna128) Ile (AAT) 74 bp Sc: 86.9 chrX:14679159-14679233(+)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRNA-Cys-GCA-1-12 (tRNAscan-SE ID: chrX.trna129) Cys (GCA) 72 bp Sc: 74.0 chrX:14804876-14804948(+)
+GGGGGTATAGCTCAGTGGCAGAGCATTCGACTGCAGATCGAGAGGTCCCTGGTTCAACTCCGGGTGCCCCCT
+>Caenorhabditis_elegans_tRNA-Arg-TCT-3-2 (tRNAscan-SE ID: chrX.trna182) Arg (TCT) 73 bp Sc: 68.8 chrX:15146561-15146634(-)
+GGCCTTGTGGCCTAATGGATAAGGCGTCTGACTTCTAATCAGAAGATTGCAGGTTCGACCCCTGCCTGGGTCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-28 (tRNAscan-SE ID: chrX.trna181) Gly (TCC) 72 bp Sc: 71.7 chrX:15200816-15200888(-)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Gly-TCC-1-29 (tRNAscan-SE ID: chrX.trna130) Gly (TCC) 72 bp Sc: 71.7 chrX:15201006-15201078(+)
+GCGTTCGTGGTGTAATGGTCAGCATGGATGCCTTCCAAGCATTCGACGGGGGTTCGATTCCCCCCGAACGCA
+>Caenorhabditis_elegans_tRNA-Val-AAC-2-12 (tRNAscan-SE ID: chrX.trna131) Val (AAC) 73 bp Sc: 76.6 chrX:15236123-15236196(+)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Lys-CTT-1-25 (tRNAscan-SE ID: chrX.trna180) Lys (CTT) 73 bp Sc: 85.9 chrX:15241354-15241427(-)
+GCCCGGTTAGCTCAGTCGGTAGAGCACCAGACTCTTAATCTGGTTGTCGCGGGTTCGAGCCCCGCATTGGGCT
+>Caenorhabditis_elegans_tRX-Thr-CGT-3-1 (tRNAscan-SE ID: chrX.trna132) Thr (CGT) 74 bp Sc: 35.1 chrX:15248969-15249043(+)
+GCTGTTTACCTGTGCAGTGGCAGAGCGTCTGTCTCGTAAACAGAAGGTCGGCGGTTCAATCCCGCCTGGGGGCA
+>Caenorhabditis_elegans_tRNA-Ile-AAT-1-20 (tRNAscan-SE ID: chrX.trna133) Ile (AAT) 74 bp Sc: 86.9 chrX:15297470-15297544(+)
+GCCGCCATAGCTCAGTCGGTTAGAGCGTGGGTCTAATAAGCCCAAGGTCGCAGGTTCGACCCCTGCTGGCGGCA
+>Caenorhabditis_elegans_tRX-Ala-AGC-6-1 (tRNAscan-SE ID: chrX.trna134) Ala (AGC) 81 bp Sc: 20.3 chrX:15619433-15619514(+)
+TGCAAGGTGGCGCAACAGGTAGTGCGCGTAGCTAGCGTCCGAGAGGTCGCTGGTTCAATATCGCTCTCCAGCTCCATGCAG
+>Caenorhabditis_elegans_tRNA-Leu-CAG-1-2 (tRNAscan-SE ID: chrX.trna135) Leu (CAG) 84 bp Sc: 77.8 chrX:15742049-15742133(+)
+GCCGTTCTGGCCGAGTGGTCTAAGGCGCTGCGTTCAGGTCGCAGTCCTCTCAGGAGGGCGCAGGTTCGAACCCTGCGGACGGCA
+>Caenorhabditis_elegans_tRX-Pro-TGG-1-1 (tRNAscan-SE ID: chrX.trna179) Pro (TGG) 76 bp Sc: 44.5 chrX:15747802-15747878(-)
+GTTCAAAATCATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGATGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-TGG-8-1 (tRNAscan-SE ID: chrX.trna136) Pro (TGG) 71 bp Sc: 41.5 chrX:15748030-15748101(+)
+GGCCGAATGGTCTAGTGGTTTGATTCTCGCTTTGGGTGCGACAAGTCCCGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRX-Pro-TGG-3-1 (tRNAscan-SE ID: chrX.trna178) Pro (TGG) 72 bp Sc: 45.8 chrX:15748315-15748387(-)
+ACCTGTGTGGTTTTGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCA
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-22 (tRNAscan-SE ID: chrX.trna137) Pro (TGG) 72 bp Sc: 75.2 chrX:15751419-15751491(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Ser-AGA-4-1 (tRNAscan-SE ID: chrX.trna177) Ser (AGA) 82 bp Sc: 74.8 chrX:15770008-15770090(-)
+GCCGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Ser-CGA-2-2 (tRNAscan-SE ID: chrX.trna176) Ser (CGA) 82 bp Sc: 81.6 chrX:15773330-15773412(-)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTCGAAATCAATTGGGCTCTGCCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Ser-AGA-3-1 (tRNAscan-SE ID: chrX.trna138) Ser (AGA) 82 bp Sc: 75.1 chrX:15773526-15773608(+)
+GCAGTCATGTCCGAGTGGTTAAGGAGATTGACTAGAAATCAATTGGGCTCTGTCCGCGTAGGTTCGAATCCTGCTGACTGCG
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-23 (tRNAscan-SE ID: chrX.trna175) Pro (TGG) 72 bp Sc: 75.2 chrX:15796622-15796694(-)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Pro-TGG-1-24 (tRNAscan-SE ID: chrX.trna139) Pro (TGG) 72 bp Sc: 75.2 chrX:15796854-15796926(+)
+GGCCGAATGGTCTAGTGGTATGATTCTCGCTTTGGGTGCGAGAGGTCCCGGGTTCAATCCCCGGTTCGGCCC
+>Caenorhabditis_elegans_tRNA-Ser-TGA-2-2 (tRNAscan-SE ID: chrX.trna174) Ser (TGA) 82 bp Sc: 85.6 chrX:16042607-16042689(-)
+GCTGCGATGTCCGAGTGGTTAAGGAGTTGGACTTGAAATCCAATGGGCATTGCCCGCGTAGGTTCGAACCCTGCTCGCAGCG
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-2-9 (tRNAscan-SE ID: chrX.trna173) Tyr (GTA) 84 bp Sc: 74.6 chrX:16208262-16208346(-)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-2-10 (tRNAscan-SE ID: chrX.trna172) Tyr (GTA) 84 bp Sc: 74.6 chrX:16208824-16208908(-)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-2-11 (tRNAscan-SE ID: chrX.trna171) Tyr (GTA) 84 bp Sc: 74.6 chrX:16209227-16209311(-)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGA
+>Caenorhabditis_elegans_tRNA-Tyr-GTA-2-12 (tRNAscan-SE ID: chrX.trna170) Tyr (GTA) 84 bp Sc: 74.6 chrX:16209768-16209852(-)
+CCGTCGATAGCTCAGTTGGTAGAGCGGAGGACTGTAGAGTCAGCAGGTATCCTTAGGTCACTGGTTCGAATCCGGTTCGACGGA
+>Caenorhabditis_elegans_tRNA-Lys-TTT-1-14 (tRNAscan-SE ID: chrX.trna169) Lys (TTT) 73 bp Sc: 77.8 chrX:16217894-16217967(-)
+GCCTCCTTAGCTCAGTTGGTAGAGCGTGAGACTTTTAATCTTAAGGTCAGGGGTTCGAGTCCCCTAGGTGGCT
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-16 (tRNAscan-SE ID: chrX.trna168) Glu (CTC) 72 bp Sc: 77.9 chrX:16271295-16271367(-)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-4-1 (tRNAscan-SE ID: chrX.trna140) Glu (CTC) 72 bp Sc: 70.4 chrX:16273766-16273838(+)
+TCCGTTGTGGTCTAGTAGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-5-1 (tRNAscan-SE ID: chrX.trna141) Glu (CTC) 72 bp Sc: 56.8 chrX:16274497-16274569(+)
+TCCGTTGTTGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACAAAT
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-17 (tRNAscan-SE ID: chrX.trna167) Glu (CTC) 72 bp Sc: 77.9 chrX:16284322-16284394(-)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-18 (tRNAscan-SE ID: chrX.trna166) Glu (CTC) 72 bp Sc: 77.9 chrX:16285294-16285366(-)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Val-AAC-1-1 (tRNAscan-SE ID: chrX.trna142) Val (AAC) 73 bp Sc: 77.4 chrX:16298340-16298413(+)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGCGGTTCGATCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Val-AAC-1-2 (tRNAscan-SE ID: chrX.trna143) Val (AAC) 73 bp Sc: 77.4 chrX:16299392-16299465(+)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGCGGTTCGATCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Val-AAC-1-3 (tRNAscan-SE ID: chrX.trna144) Val (AAC) 73 bp Sc: 77.4 chrX:16300062-16300135(+)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGCGGTTCGATCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Val-AAC-1-4 (tRNAscan-SE ID: chrX.trna145) Val (AAC) 73 bp Sc: 77.4 chrX:16300588-16300661(+)
+GGTCTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGCGGTTCGATCCCGCCCGAGATCA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-19 (tRNAscan-SE ID: chrX.trna146) Glu (CTC) 72 bp Sc: 77.9 chrX:16378112-16378184(+)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-iMet-CAT-1-9 (tRNAscan-SE ID: chrX.trna147) iMet (CAT) 72 bp Sc: 61.2 chrX:16441145-16441217(+)
+AGCAGCGTGGCGCAGTGGAAGCGTGCTGGGCCCATAACCCAGAGGTCGGTGGATCGAAACCACTCGCTGCTA
+>Caenorhabditis_elegans_tRNA-Arg-TCG-4-1 (tRNAscan-SE ID: chrX.trna148) Arg (TCG) 73 bp Sc: 69.4 chrX:16461476-16461549(+)
+GGCCGCGTGGCCTAATGGATAAGGCATCAGACTTCGAATCTGGGGATTGCAGGTTCGATCCCTGCCGTGGTCG
+>Caenorhabditis_elegans_tRNA-Phe-GAA-4-2 (tRNAscan-SE ID: chrX.trna165) Phe (GAA) 73 bp Sc: 82.5 chrX:16503143-16503216(-)
+GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATCCTGGTTCGGGGCA
+>Caenorhabditis_elegans_tRNA-Phe-GAA-7-1 (tRNAscan-SE ID: chrX.trna149) Phe (GAA) 80 bp Sc: 46.5 chrX:16522761-16522841(+)
+ACCGCAAATCAACTGTGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATCCTGGTTCGGGGCA
+>Caenorhabditis_elegans_tRNA-Phe-GAA-4-3 (tRNAscan-SE ID: chrX.trna150) Phe (GAA) 73 bp Sc: 82.5 chrX:16523343-16523416(+)
+GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATCCTGGTTCGGGGCA
+>Caenorhabditis_elegans_tRNA-Phe-GAA-4-4 (tRNAscan-SE ID: chrX.trna151) Phe (GAA) 73 bp Sc: 82.5 chrX:16523922-16523995(+)
+GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATCCTGGTTCGGGGCA
+>Caenorhabditis_elegans_tRNA-Phe-GAA-4-5 (tRNAscan-SE ID: chrX.trna152) Phe (GAA) 73 bp Sc: 82.5 chrX:16551510-16551583(+)
+GCCTCGATAGCTCAGTTGGGAGAGCGTACGACTGAAGATCGTAAGGTCACCAGTTCGATCCTGGTTCGGGGCA
+>Caenorhabditis_elegans_tRNA-Glu-CTC-1-20 (tRNAscan-SE ID: chrX.trna153) Glu (CTC) 72 bp Sc: 77.9 chrX:16558941-16559013(+)
+TCCGTTGTGGTCTAGTGGTTAGGATTTATGGCTCTCACCCATAAGGCCGGGGTTCGATTCCCCGCAACGGAA
+>Caenorhabditis_elegans_tRNA-Val-CAC-1-4 (tRNAscan-SE ID: chrX.trna154) Val (CAC) 73 bp Sc: 80.7 chrX:16590394-16590467(+)
+GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTCACACGCAGAAGGTCGCCGGTTCGAACCCGGCCAGGACCT
+>Caenorhabditis_elegans_tRNA-Val-CAC-1-5 (tRNAscan-SE ID: chrX.trna164) Val (CAC) 73 bp Sc: 80.7 chrX:16590930-16591003(-)
+GGTCCTGTGGTGTAGTGGTTATCACGTCTGCTTCACACGCAGAAGGTCGCCGGTTCGAACCCGGCCAGGACCT
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-19 (tRNAscan-SE ID: chrX.trna163) Asp (GTC) 72 bp Sc: 61.7 chrX:16604719-16604791(-)
+TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCGGGTTCAATTCCCGGCCGGGGAG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-6-1 (tRNAscan-SE ID: chrX.trna162) Asp (GTC) 72 bp Sc: 52.1 chrX:16617891-16617963(-)
+TCCTCGGTAGTATAGTGGTGAGTATCCGCGTCTGTCACATGCGAGACCCTGGTTCAATTCCCGGCCGGGGAG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-20 (tRNAscan-SE ID: chrX.trna161) Asp (GTC) 72 bp Sc: 61.7 chrX:16618295-16618367(-)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-Asp-GTC-2-21 (tRNAscan-SE ID: chrX.trna160) Asp (GTC) 72 bp Sc: 61.7 chrX:16619332-16619404(-)
+TCCtcggtagtatagtggtgagtatccgcgtctgtcacatgcgagacccgggttcaattcccggccgGGGAG
+>Caenorhabditis_elegans_tRNA-His-GTG-2-11 (tRNAscan-SE ID: chrX.trna159) His (GTG) 72 bp Sc: 69.4 chrX:16634829-16634901(-)
+GCCTGCGTAGTATAGTGGTTAGTACTCCACGTTGTGGCCGTGGCGACGCTGGTTCGATTCCAGCCGCAGGCA
+>Caenorhabditis_elegans_tRNA-Ser-GCT-1-7 (tRNAscan-SE ID: chrX.trna158) Ser (GCT) 82 bp Sc: 84.4 chrX:16689984-16690066(-)
+GATCAGGTGGCCGAGTGGTTAAGGCGATGGACTGCTAATCCATTGGGGTTTCCCCGCGTGAGTTCGAATCTCATCCTGATCG
+>Caenorhabditis_elegans_tRNA-Gly-GCC-1-11 (tRNAscan-SE ID: chrX.trna157) Gly (GCC) 71 bp Sc: 77.2 chrX:16928270-16928341(-)
+gcatcggtggttcagtggtagaatgctcgcctgccacgcgggcggcccgggttcgattcccggtcgatgca
+>Caenorhabditis_elegans_tRNA-Val-AAC-4-1 (tRNAscan-SE ID: chrX.trna155) Val (AAC) 73 bp Sc: 73.3 chrX:17611288-17611361(+)
+GGTTTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCT
+>Caenorhabditis_elegans_tRNA-Val-AAC-3-2 (tRNAscan-SE ID: chrX.trna156) Val (AAC) 73 bp Sc: 75.2 chrX:17611502-17611575(-)
+GGTTTCGTGGTGTAGTGGTTATCACATCTGTCTAACACACAGAAGGTCGGTGGTTCGAGCCCGCCCGAGATCA
```

### Comparing `mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs_name_map.txt` & `mimseq-1.3.4/mimseq/data/ce11-eColitK/ce11-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11_eColitK.fa` & `mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11_eColitK.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa` & `mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11_eschColi-tRNAs.out` & `mimseq-1.3.4/mimseq/data/danRer11-eColitK/danRer11_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/danRer11-eColitK/filterList.txt` & `mimseq-1.3.4/mimseq/data/danRer11-eColitK/filterList.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/danRer11-eColitK/filtertRNAs.py` & `mimseq-1.3.4/mimseq/data/danRer11-eColitK/filtertRNAs.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6_eColitK-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6_eColitK-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6_eschColi-tRNAs.out` & `mimseq-1.3.4/mimseq/data/dm6-eColitK/dm6_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-tRNAs.out` & `mimseq-1.3.4/mimseq/data/dm6-tRNAs/dm6-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.out` & `mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.ss.sort` & `mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.ss.sort`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs_name_map.txt` & `mimseq-1.3.4/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/eschColi-tRNA_Lys/eschColi_K_12_MG1655-tRNAs.out` & `mimseq-1.3.4/mimseq/data/eschColi-tRNA_Lys/eschColi_K_12_MG1655-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/eschColi-tRNA_Lys/eschColi_modomics.fa` & `mimseq-1.3.4/mimseq/data/eschColi-tRNA_Lys/eschColi_modomics.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/README.txt` & `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.fa` & `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.tmp.fa` & `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.tmp.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-detailed.out` & `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered.fa` & `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered2.fa` & `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered2.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_name_map.txt` & `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_noChr.bed` & `mimseq-1.3.4/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_noChr.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg19-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.4/mimseq/data/hg19-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg19-eColitK/README.txt` & `mimseq-1.3.4/mimseq/data/hg19-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs-all.fa` & `mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs-detailed.out` & `mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs_name_map.txt` & `mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19_eschColi-tRNAs.out` & `mimseq-1.3.4/mimseq/data/hg19-eColitK/hg19_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19_eschColi-tRNAs.out` & `mimseq-1.3.4/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.4/mimseq/data/hg38-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK/README.txt` & `mimseq-1.3.4/mimseq/data/hg38-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs-all.fa` & `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs-detailed.out` & `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs-filtered.fa` & `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs-filtered.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs_name_map.txt` & `mimseq-1.3.4/mimseq/data/hg38-eColitK/hg38-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/FastaHeadersforMimseq.py` & `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/README.txt` & `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-all.fa` & `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-detailed.out` & `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-filtered.fa` & `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-filtered.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs_name_map.txt` & `mimseq-1.3.4/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm10-eColitK/mm10-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/mm10-eColitK/mm10-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm10-eColitK/mm10_eColitK-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/mm10-eColitK/mm10_eColitK-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm10-eColitK/mm10_eschColi-tRNAs.out` & `mimseq-1.3.4/mimseq/data/mm10-eColitK/mm10_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm10-tRNAs/mm10-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/mm10-tRNAs/mm10-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm10-tRNAs/mm10-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/mm10-tRNAs/mm10-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm10-tRNAs/mm10-tRNAs.out.filtered-noPseudo-noChrM` & `mimseq-1.3.4/mimseq/data/mm10-tRNAs/mm10-tRNAs.out.filtered-noPseudo-noChrM`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm39-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.4/mimseq/data/mm39-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm39-eColitK/README.txt` & `mimseq-1.3.4/mimseq/data/mm39-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs-all.fa` & `mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs-detailed.out` & `mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs-noeColi.fa` & `mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs-noeColi.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs_name_map.txt` & `mimseq-1.3.4/mimseq/data/mm39-eColitK/mm39-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/modomics` & `mimseq-1.3.4/mimseq/data/modomics`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/modomics_orig` & `mimseq-1.3.4/mimseq/data/modomics_orig`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/rn7-eColitK/README.txt` & `mimseq-1.3.4/mimseq/data/rn7-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-tRNAs-confidence-set.out` & `mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-tRNAs-confidence-set.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7_eColitK-tRNAs-confidence-set.out` & `mimseq-1.3.4/mimseq/data/rn7-eColitK/rn7_eColitK-tRNAs-confidence-set.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.out-noChrM` & `mimseq-1.3.4/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.out-noChrM`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-eColitK/Turk_2013_mitotRNAbounds_Tab1.bed` & `mimseq-1.3.4/mimseq/data/sacCer3-eColitK/Turk_2013_mitotRNAbounds_Tab1.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3_eschColi-tRNAs.out` & `mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3_eschColitK.fa` & `mimseq-1.3.4/mimseq/data/sacCer3-eColitK/sacCer3_eschColitK.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.out-noChrM` & `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.out-noChrM`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.ss.sort` & `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.ss.sort`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/README.txt` & `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/Turk_2013_mitotRNAbounds_Tab1.bed` & `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/Turk_2013_mitotRNAbounds_Tab1.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColi-tRNAs.out` & `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColitK.fa` & `mimseq-1.3.4/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColitK.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3_modOligos/sacCer3_eschColi-tRNAs.out` & `mimseq-1.3.4/mimseq/data/sacCer3_modOligos/sacCer3_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/sacCer3_modOligos/sacCer3_eschColitK.fa` & `mimseq-1.3.4/mimseq/data/sacCer3_modOligos/sacCer3_eschColitK.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.bed` & `mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.out.noChrM` & `mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.out.noChrM`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.ss.sort` & `mimseq-1.3.4/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.ss.sort`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/schiPomb-eColitK/schiPomb-mitotRNAs.fa` & `mimseq-1.3.4/mimseq/data/schiPomb-eColitK/schiPomb-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/schiPomb-eColitK/schiPomb_972H-tRNAs.fa` & `mimseq-1.3.4/mimseq/data/schiPomb-eColitK/schiPomb_972H-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/schiPomb-eColitK/schiPomb_eschColi-tRNAs.out` & `mimseq-1.3.4/mimseq/data/schiPomb-eColitK/schiPomb_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/data/tRNAmatureseq.cm` & `mimseq-1.3.4/mimseq/data/tRNAmatureseq.cm`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/deseq.R` & `mimseq-1.3.4/mimseq/deseq.R`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/getCoverage.py` & `mimseq-1.3.4/mimseq/getCoverage.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/mimseq.py` & `mimseq-1.3.4/mimseq/mimseq.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,16 +229,16 @@
 	###################
 
 	parser = argparse.ArgumentParser(description = 'Custom high-throughput tRNA sequencing alignment and quantification pipeline\
 		based on modification induced misincorporation cDNA synthesis.', add_help = True, usage = "%(prog)s [options] sample data")
 
 	inputs = parser.add_argument_group("Input files")
 	inputs.add_argument('-s','--species', metavar='species', required = not ('-t' in sys.argv or '--trnas' in sys.argv), dest = 'species', help = \
-		'Species being analyzed for which to load pre-packaged data files (prioritized over -t, -o and -m). Options are: Hsap, Hsap19, Mmus, Rnor, Scer, Spom, Dmel, Drer, Ecol, Atha', \
-		choices = ['Hsap', 'Hsap19','Ggor','Mmus','Rnor','Scer', 'Spom','Dmel', 'Drer', 'Ecol', 'Atha', 'HsapTCC', 'ScerMut'])
+		'Species being analyzed for which to load pre-packaged data files (prioritized over -t, -o and -m). Options are: Hsap, Hsap19, Mmus, Rnor, Scer, Spom, Dmel, Drer, Cele, Ecol, Atha', \
+		choices = ['Hsap', 'Hsap19','Ggor','Mmus','Rnor','Scer', 'Spom','Dmel', 'Drer', 'Cele', 'Ecol', 'Atha', 'HsapTCC', 'ScerMut'])
 	inputs.add_argument('-t', '--trnas', metavar='genomic tRNAs', required = False, dest = 'trnas', help = \
 		'Genomic tRNA fasta file, e.g. from gtRNAdb or tRNAscan-SE. Already avalable in data folder for a few model organisms.')
 	inputs.add_argument('-o', '--trnaout', metavar = 'tRNA out file', required = (not '--species' or '-s' in sys.argv) or ('-t' in sys.argv),
 		dest = 'trnaout', help = 'tRNA.out file generated by tRNAscan-SE (also may be available on gtRNAdb). Contains information about tRNA features, including introns.')
 	inputs.add_argument('-m', '--mito-trnas', metavar = 'mitochondrial tRNAs', required = False, dest = 'mito', \
 		help = 'Mitochondrial tRNA fasta file(s). Should be downloaded from mitotRNAdb for species of interest. Already available in data folder for a few model organisms.')
 	inputs.add_argument('-p', '--plastid-trnas', metavar = 'plastid tRNAs', required = False, dest = 'plastid', \
@@ -408,14 +408,18 @@
 					args.mito = ''
 				if args.species == 'Atha':
 					args.trnas = os.path.dirname(os.path.realpath(__file__)) + "/data/araTha1-eColitK/araTha1-tRNAs-all.fa"
 					args.trnaout = os.path.dirname(os.path.realpath(__file__)) + "/data/araTha1-eColitK/araTha1-tRNAs-detailed.out"
 					args.mito = os.path.dirname(os.path.realpath(__file__)) + "/data/araTha1-eColitK/araTha1-mitotRNAs.fa"
 					# plastid reference needed for A.thaliana
 					args.plastid = os.path.dirname(os.path.realpath(__file__)) + "/data/araTha1-eColitK/araTha1-plastidtRNAs.fa"
+				if args.species == 'Cele':
+					args.trnas = os.path.dirname(os.path.realpath(__file__)) + "/data/ce11-eColitK/ce11-tRNAs-all.fa"
+					args.trnaout = os.path.dirname(os.path.realpath(__file__)) + "/data/ce11-eColitK/ce11-tRNAs-detailed.out"
+					args.mito = os.path.dirname(os.path.realpath(__file__)) + "/data/ce11-eColitK/ce11-mitotRNAs.fa"
 			else:
 				args.species = args.trnas.split("/")[-1].split(".")[0]
 			mimseq(args.trnas, args.trnaout, args.name, args.species, args.out, args.cluster, args.cluster_id, args.cov_diff, \
 				args.posttrans, args.control_cond, args.threads, args.max_multi, args.snp_tolerance, \
 				args.keep_temp, args.cca, args.double_cca, args.min_cov, args.mismatches, args.remap, args.remap_mismatches, \
 				args.misinc_thresh, args.mito, args.plastid, args.pretrnas, args.local_mod, args.p_adj, args.crosstalks, args.sampledata)
```

### Comparing `mimseq-1.3.3/mimseq/mmQuant.py` & `mimseq-1.3.4/mimseq/mmQuant.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/modPlot.R` & `mimseq-1.3.4/mimseq/modPlot.R`

 * *Files 1% similar despite different names*

```diff
@@ -333,17 +333,17 @@
 
   temp_mods = merge(mods, context_info, by = c("isodecoder", "canon_pos"))
   temp_mods = temp_mods %>%
     group_by(isodecoder, canon_pos, bam, identity) %>%
     mutate(new_prop = proportion/sum(proportion))
   filter_proportions = temp_mods %>%
     group_by(isodecoder, canon_pos, bam, identity) %>%
-    filter((any(max(new_prop) > 0.95) &
+    filter((any(max(new_prop) > 0.97) &
               any(canon_pos != 34)) |
-             (any(max(new_prop) > 0.95) &
+             (any(max(new_prop) > 0.97) &
                 any(identity != 'A') &
                 any(canon_pos == 34) & any(type != "G")))
   sub_mods_agg = mods_agg[mods_agg$condition == i, ]
   sub_mods_pos = sub_mods_agg[sub_mods_agg$canon_pos %in% mod_sites, ]
   sub_mods_pos[which(sub_mods_pos$x > 1), "x"] = 1
   sub_mods_pos = merge(sub_mods_pos, context_info, by = c("isodecoder", "canon_pos"))
   sub_mods_pos = anti_join(sub_mods_pos,
@@ -416,20 +416,20 @@
                            by = c("isodecoder", "canon_pos"))
   sub_mods_aggtype$bam = sub(out, "", sub_mods_aggtype$bam)
   sub_mods_aggtype_cyt = sub_mods_aggtype[!grepl("mito", sub_mods_aggtype$isodecoder) &
                                           !grepl("plastid", sub_mods_aggtype$isodecoder) &
                                           !grepl("nmt", sub_mods_aggtype$isodecoder), ]
   # renormalise by sum of misinc at each site for each isodecoder in each bam file
   # this makes sum all misinc types = 1
-  # additionally filter all clusters at each pos where misinc of highest nucl > 0.95
+  # additionally filter all clusters at each pos where misinc of highest nucl > 0.97
   sub_mods_aggtype_cyt = sub_mods_aggtype_cyt %>%
     group_by(isodecoder, canon_pos, bam, identity) %>%
     mutate(new_prop = proportion/sum(proportion)) %>%
-    filter(any(max(new_prop) < 0.95) |
-             (any(max(new_prop) >= 0.95 &
+    filter(any(max(new_prop) < 0.97) |
+             (any(max(new_prop) >= 0.97 &
                     any(identity == 'A') &
                     any(canon_pos == 34) &
                     any(type == 'G'))))
   
   sub_mods_aggtype_cyt$canon_pos = factor(sub_mods_aggtype_cyt$canon_pos, 
                                           levels = c('9', '20', '20a','26','32','34','37','58'))
   color_num = length(unique(sub_mods_aggtype_cyt$bam)) + 1
@@ -471,15 +471,15 @@
   
   ggsave(paste(out, "mods/", paste(i, 'misincSignatures_downstreamContext.pdf', sep = '_'), sep = ''), signature_plot_downstream, height=10, width=14, useDingbats=FALSE)
   
   if (!is.na(mito_trnas)){
     sub_mods_aggtype_mito = sub_mods_aggtype[grepl("mito", sub_mods_aggtype$isodecoder) |
                                               grepl("plastid", sub_mods_aggtype$isodecoder) |
                                               grepl("nmt", sub_mods_aggtype$isodecoder), ]
-    sub_mods_aggtype_mito = sub_mods_aggtype_mito %>% group_by(isodecoder, canon_pos, bam) %>% mutate(new_prop = proportion/sum(proportion)) %>% filter(any(max(new_prop) < 0.95))
+    sub_mods_aggtype_mito = sub_mods_aggtype_mito %>% group_by(isodecoder, canon_pos, bam) %>% mutate(new_prop = proportion/sum(proportion)) %>% filter(any(max(new_prop) < 0.97))
     
     if(nrow(sub_mods_aggtype_mito) != 0) {
       # renormalise by sum of misinc at each site for each isodecoder in each bam file - this makes sum all misinc types = 1
       #sub_mods_aggtype_mito = aggregate(sub_mods_aggtype_mito$proportion, by = list(identity = sub_mods_aggtype_mito$identity, type = sub_mods_aggtype_mito$type, upstream = sub_mods_aggtype_mito$upstream, downstream = sub_mods_aggtype_mito$downstream, pos = sub_mods_aggtype_mito$pos, canon_pos=sub_mods_aggtype_mito$canon_pos), FUN = function(x) c(mean=mean(x), sd=sd(x)))
       #sub_mods_aggtype_mito = do.call("data.frame", sub_mods_aggtype_mito)
       sub_mods_aggtype_mito$canon_pos = factor(sub_mods_aggtype_mito$canon_pos, levels = c('9', '20', '20a', '26','32','34','37','58'))
```

### Comparing `mimseq-1.3.3/mimseq/modifications` & `mimseq-1.3.4/mimseq/modifications`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/splitClusters.py` & `mimseq-1.3.4/mimseq/splitClusters.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/ssAlign.py` & `mimseq-1.3.4/mimseq/ssAlign.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/tRNAmap.py` & `mimseq-1.3.4/mimseq/tRNAmap.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq/tRNAtools.py` & `mimseq-1.3.4/mimseq/tRNAtools.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.3/mimseq.egg-info/PKG-INFO` & `mimseq-1.3.4/mimseq.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: mimseq
-Version: 1.3.3
+Version: 1.3.4
 Summary: Custom high-throughput tRNA sequencing alignment and quantification pipeline based on modification induced misincorporation cDNA synthesis.
 Home-page: https://github.com/nedialkova-lab/mim-tRNAseq
 Author: Drew Behrens
 Author-email: abehrens@biochem.mpg.de
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `mimseq-1.3.3/mimseq.egg-info/SOURCES.txt` & `mimseq-1.3.4/mimseq.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,19 +45,22 @@
 mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.out
 mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.ss
 mimseq/data/araTha1-eColitK/araTha1-tRNAs.bed
 mimseq/data/araTha1-eColitK/araTha1-tRNAs.fa
 mimseq/data/araTha1-eColitK/araTha1-tRNAs_name_map.txt
 mimseq/data/araTha1-eColitK/convertPtRNAdbSearch.py
 mimseq/data/araTha1-eColitK/hg38README.txt
-mimseq/data/ce11-tRNAs/ce11-mitotRNAs.fa
-mimseq/data/ce11-tRNAs/ce11-tRNAs-detailed.out
-mimseq/data/ce11-tRNAs/ce11-tRNAs.bed
-mimseq/data/ce11-tRNAs/ce11-tRNAs.fa
-mimseq/data/ce11-tRNAs/ce11-tRNAs_name_map.txt
+mimseq/data/ce11-eColitK/FastaHeadersforMimseq.py
+mimseq/data/ce11-eColitK/README.txt
+mimseq/data/ce11-eColitK/ce11-mitotRNAs.fa
+mimseq/data/ce11-eColitK/ce11-tRNAs-all.fa
+mimseq/data/ce11-eColitK/ce11-tRNAs-all.tmp.fa
+mimseq/data/ce11-eColitK/ce11-tRNAs-detailed.out
+mimseq/data/ce11-eColitK/ce11-tRNAs.bed
+mimseq/data/ce11-eColitK/ce11-tRNAs_name_map.txt
 mimseq/data/danRer11-eColitK/README.txt
 mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa
 mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed
 mimseq/data/danRer11-eColitK/danRer11_eColitK.fa
 mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa
 mimseq/data/danRer11-eColitK/danRer11_eschColi-tRNAs.out
 mimseq/data/danRer11-eColitK/filterList.txt
```

### Comparing `mimseq-1.3.3/setup.py` & `mimseq-1.3.4/setup.py`

 * *Files identical despite different names*

