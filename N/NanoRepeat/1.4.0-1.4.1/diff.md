# Comparing `tmp/NanoRepeat-1.4.0.tar.gz` & `tmp/NanoRepeat-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NanoRepeat-1.4.0.tar", last modified: Wed May 10 09:43:11 2023, max compression
+gzip compressed data, was "NanoRepeat-1.4.1.tar", last modified: Wed May 17 15:32:35 2023, max compression
```

## Comparing `NanoRepeat-1.4.0.tar` & `NanoRepeat-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-10 09:43:11.899855 NanoRepeat-1.4.0/
--rw-r--r--   0 fangli    (1002) fangli    (1002)     1097 2023-05-09 10:40:15.000000 NanoRepeat-1.4.0/LICENSE
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    15342 2023-05-10 09:43:11.895855 NanoRepeat-1.4.0/PKG-INFO
--rw-r--r--   0 fangli    (1002) fangli    (1002)    15007 2023-05-10 09:30:58.000000 NanoRepeat-1.4.0/README.md
--rw-rw-r--   0 fangli    (1002) fangli    (1002)       38 2023-05-10 09:43:11.899855 NanoRepeat-1.4.0/setup.cfg
--rw-rw-r--   0 fangli    (1002) fangli    (1002)      803 2023-05-10 09:42:54.000000 NanoRepeat-1.4.0/setup.py
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-10 09:43:11.891855 NanoRepeat-1.4.0/src/
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-10 09:43:11.895855 NanoRepeat-1.4.0/src/NanoRepeat/
--rw-rw-r--   0 fangli    (1002) fangli    (1002)      186 2023-05-10 09:10:19.000000 NanoRepeat-1.4.0/src/NanoRepeat/__init__.py
--rwxr-xr-x   0 fangli    (1002) fangli    (1002)    36428 2023-05-10 09:09:17.000000 NanoRepeat-1.4.0/src/NanoRepeat/nanoRepeat-joint.py
--rwxr-xr-x   0 fangli    (1002) fangli    (1002)    10798 2023-05-10 09:04:29.000000 NanoRepeat-1.4.0/src/NanoRepeat/nanoRepeat.py
--rw-r--r--   0 fangli    (1002) fangli    (1002)    29923 2023-05-10 06:31:20.000000 NanoRepeat-1.4.0/src/NanoRepeat/nanoRepeat_bam.py
--rw-r--r--   0 fangli    (1002) fangli    (1002)     3074 2023-05-09 10:33:30.000000 NanoRepeat-1.4.0/src/NanoRepeat/paf.py
--rw-r--r--   0 fangli    (1002) fangli    (1002)     4442 2023-05-09 07:44:26.000000 NanoRepeat-1.4.0/src/NanoRepeat/repeat_region.py
--rw-r--r--   0 fangli    (1002) fangli    (1002)    31071 2023-05-09 10:33:41.000000 NanoRepeat-1.4.0/src/NanoRepeat/split_alleles.py
--rw-r--r--   0 fangli    (1002) fangli    (1002)    16165 2023-05-10 08:44:43.000000 NanoRepeat-1.4.0/src/NanoRepeat/tk.py
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-10 09:43:11.895855 NanoRepeat-1.4.0/src/NanoRepeat.egg-info/
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    15342 2023-05-10 09:43:11.000000 NanoRepeat-1.4.0/src/NanoRepeat.egg-info/PKG-INFO
--rw-rw-r--   0 fangli    (1002) fangli    (1002)      446 2023-05-10 09:43:11.000000 NanoRepeat-1.4.0/src/NanoRepeat.egg-info/SOURCES.txt
--rw-rw-r--   0 fangli    (1002) fangli    (1002)        1 2023-05-10 09:43:11.000000 NanoRepeat-1.4.0/src/NanoRepeat.egg-info/dependency_links.txt
--rw-rw-r--   0 fangli    (1002) fangli    (1002)       53 2023-05-10 09:43:11.000000 NanoRepeat-1.4.0/src/NanoRepeat.egg-info/requires.txt
--rw-rw-r--   0 fangli    (1002) fangli    (1002)       11 2023-05-10 09:43:11.000000 NanoRepeat-1.4.0/src/NanoRepeat.egg-info/top_level.txt
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-17 15:32:35.224437 NanoRepeat-1.4.1/
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)     1097 2023-05-11 08:33:58.000000 NanoRepeat-1.4.1/LICENSE
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    16293 2023-05-17 15:32:35.224437 NanoRepeat-1.4.1/PKG-INFO
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    15958 2023-05-17 14:33:11.000000 NanoRepeat-1.4.1/README.md
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)       38 2023-05-17 15:32:35.224437 NanoRepeat-1.4.1/setup.cfg
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)      803 2023-05-17 15:31:55.000000 NanoRepeat-1.4.1/setup.py
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-17 15:32:35.220437 NanoRepeat-1.4.1/src/
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-17 15:32:35.224437 NanoRepeat-1.4.1/src/NanoRepeat/
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)      186 2023-05-11 08:33:58.000000 NanoRepeat-1.4.1/src/NanoRepeat/__init__.py
+-rwxrwxr-x   0 fangli    (1002) fangli    (1002)    36432 2023-05-13 06:07:32.000000 NanoRepeat-1.4.1/src/NanoRepeat/nanoRepeat-joint.py
+-rwxrwxr-x   0 fangli    (1002) fangli    (1002)    10986 2023-05-17 12:43:34.000000 NanoRepeat-1.4.1/src/NanoRepeat/nanoRepeat.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    30089 2023-05-17 13:59:27.000000 NanoRepeat-1.4.1/src/NanoRepeat/nanoRepeat_bam.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)     3078 2023-05-13 06:08:14.000000 NanoRepeat-1.4.1/src/NanoRepeat/paf.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)     4446 2023-05-13 06:08:18.000000 NanoRepeat-1.4.1/src/NanoRepeat/repeat_region.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    31135 2023-05-14 07:24:25.000000 NanoRepeat-1.4.1/src/NanoRepeat/split_alleles.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    16195 2023-05-17 13:58:21.000000 NanoRepeat-1.4.1/src/NanoRepeat/tk.py
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-17 15:32:35.224437 NanoRepeat-1.4.1/src/NanoRepeat.egg-info/
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    16293 2023-05-17 15:32:35.000000 NanoRepeat-1.4.1/src/NanoRepeat.egg-info/PKG-INFO
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)      446 2023-05-17 15:32:35.000000 NanoRepeat-1.4.1/src/NanoRepeat.egg-info/SOURCES.txt
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)        1 2023-05-17 15:32:35.000000 NanoRepeat-1.4.1/src/NanoRepeat.egg-info/dependency_links.txt
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)       53 2023-05-17 15:32:35.000000 NanoRepeat-1.4.1/src/NanoRepeat.egg-info/requires.txt
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)       11 2023-05-17 15:32:35.000000 NanoRepeat-1.4.1/src/NanoRepeat.egg-info/top_level.txt
```

### Comparing `NanoRepeat-1.4.0/LICENSE` & `NanoRepeat-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.4.0/PKG-INFO` & `NanoRepeat-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,11 @@
-Metadata-Version: 2.1
-Name: NanoRepeat
-Version: 1.4.0
-Summary: NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data
-Home-page: https://github.com/WGLab/NanoRepeat
-Author: Li Fang, Kai Wang
-Author-email: fangli9@sysu.edu.cn
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7024485.svg)](https://doi.org/10.5281/zenodo.7024485)
+[![PyPI version](https://badge.fury.io/py/NanoRepeat.svg)](https://badge.fury.io/py/NanoRepeat)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7919607.svg)](https://doi.org/10.5281/zenodo.7919607)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
   - [Regular use cases](#regular-use-cases)
   - [Joint quantification of two adjacent repeats](#joint_quantification)
@@ -24,30 +14,37 @@
 - [Contact Us](#contact-us)
 
 ## Installation
 
 #### Prerequisites:
 
 1. [Python](https://www.python.org/downloads/) (version >= 3.8)
-2. [Minimap2](https://github.com/lh3/minimap2) (version >= 2.8)
-3. [Samtools](https://github.com/samtools/samtools.git) (version >= 1.3)
+2. [Minimap2](https://github.com/lh3/minimap2) (version >= 2.22)
+3. [Samtools](https://github.com/samtools/samtools.git) (version >= 1.13)
 
-You may alreadly have `minimap2` and `samtools` if you performed analysis of Oxford Nanopore sequencing data. You can use `which minimap2` and `which samtools` to check the full path to the two executable files.
+You may alreadly have `minimap2` and `samtools` if you performed analysis of Oxford Nanopore sequencing data. You can use `which minimap2` and `which samtools` to check the full path to the two executable files. Please note that `minimap2` should be v2.22 or later. 
+
+Once you installed the above tools, you can use the following commands to install NanoRepeat (we recommend creating an new conda environment to avoid dependency issues):
 
-Once you installed the above tools, you can use the following commands to install NanoRepeat:
-```
-pip install NanoRepeat
-```
-or
 ```
+conda create -n nanorepeat python=3.8
+conda activate nanorepeat
 git clone https://github.com/WGLab/NanoRepeat.git
 cd NanoRepeat
 pip install .
 ```
 
+If you want to install a stable version from Python Package Index (PyPI): 
+
+```
+conda create -n nanorepeat python=3.8
+conda activate nanorepeat
+pip install NanoRepeat
+```
+
 ## Usage
 
 ### Regular use cases
 
 NanoRepeat can quantify STRs from targeted sequencing or whole-genome sequencing data. We will demonstrate the usage of NanoRepeat using an example data set, which can be downloaded using the following commands. 
 
 ```
@@ -68,25 +65,28 @@
 
 You can use the following command to run NanoRepeat: 
 
 ```
 nanoRepeat.py \
     -i path/to/NanoRepeat_v1.3_example_data/HG002/hg002_Q20.20210805_3flowcells.hs37d5.example_regions.bam \
     -t bam \
+    -d ont_q20 \
     -r path/to/NanoRepeat_v1.3_example_data/HG002/GRCh37_chr1.fasta \
     -b path/to/NanoRepeat_v1.3_example_data/HG002/HG002_GRCh37_example_regions.bed \
     -c 4 \
     --samtools path/to/samtools \
     --minimap2 path/to/minimap2 \
     -o ./nanorepeat_output/HG002
 ```
 
 `-i` specifies the input file, which can be in `fasta`, `fastq` or `bam` format. In this case our input file is `hg002_Q20.20210805_3flowcells.hs37d5.example_regions.bam`. It is a subset of an Oxford Nanopore whole-genome sequencing dataset of the [NIST/GIAB HG002 (GM24385/NA24385)](https://catalog.coriell.org/0/Sections/Search/Sample_Detail.aspx?Ref=NA24385&Product=DNA) genome. The sequencing data was from the [Oxford Nanopore Technologies Benchmark Datasets](https://registry.opendata.aws/ont-open-data/) and reads from 15 example STR regions in `chr1` were extracted. These regions were selected because they overlap with the [HG002 SV benchmark set](https://ftp-trace.ncbi.nlm.nih.gov/giab/ftp/data/AshkenazimTrio/analysis/NIST_SVs_Integration_v0.6/HG002_SVs_Tier1_v0.6.vcf.gz) and are heterozygous (i.e., two alleles have different repeat sizes). 
 
-`-t` specifies the input file type. There are three valid values: bam, fastq or fasta. In this case the input file is in a bam file. 
+`-t` specifies the input file type. There are four valid values: bam, cram, fastq or fasta. In this case the input file is in a bam file. 
+
+`-d` specifies the data type. There are five valid values: `ont_q20`, `ont_sup`, `ont`, `hifi`, and `clr`. `ont_q20` is for Oxford Nanopore sequencing with Q20+ chemistry. `ont_sup` is for Oxford Nanopore sequencing with R9 flowcells and basecalled in super accuracy mode. `ont` is for Oxford Nanopore sequencing with R9 flowcells and basecalled in fast mode or high accuracy mode. `hifi` is for PacBio HiFi/CCS reads. `clr` is for PacBio Continuous Long Reads (CLR) reads. Default value: `ont`.
 
 `-r` specifies the reference genome file in `FASTA` format. In this case, `GRCh37_chr1.fasta` is chr1 of the GRCh37/hg19 reference genome. We used GRCh37 instead of GRCh38 because the HG002 SV benchmark set is based on GRCh37. 
 
 `-b` specifies the information of the tandem repeat regions that you are interested in. It is a tab-delimited text file in BED format. There are four required columns: `chromosome`, `start_position`, `end_position`, `repeat_unit_sequence`. In our case, `HG002_GRCh37_example_regions.bed` contains 15 STR regions in chr1 of GRCh37. The first 5 rows of the `HG002_GRCh37_example_regions.bed` are shown below. 
 
 | 1 | 4599903  | 4599930   | TTTAG   |
 |---|----------|-----------|---------|
```

### Comparing `NanoRepeat-1.4.0/README.md` & `NanoRepeat-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,22 @@
+Metadata-Version: 2.1
+Name: NanoRepeat
+Version: 1.4.1
+Summary: NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data
+Home-page: https://github.com/WGLab/NanoRepeat
+Author: Li Fang, Kai Wang
+Author-email: fangli9@sysu.edu.cn
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7024485.svg)](https://doi.org/10.5281/zenodo.7024485)
+[![PyPI version](https://badge.fury.io/py/NanoRepeat.svg)](https://badge.fury.io/py/NanoRepeat)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7919607.svg)](https://doi.org/10.5281/zenodo.7919607)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
   - [Regular use cases](#regular-use-cases)
   - [Joint quantification of two adjacent repeats](#joint_quantification)
@@ -13,30 +25,37 @@
 - [Contact Us](#contact-us)
 
 ## Installation
 
 #### Prerequisites:
 
 1. [Python](https://www.python.org/downloads/) (version >= 3.8)
-2. [Minimap2](https://github.com/lh3/minimap2) (version >= 2.8)
-3. [Samtools](https://github.com/samtools/samtools.git) (version >= 1.3)
+2. [Minimap2](https://github.com/lh3/minimap2) (version >= 2.22)
+3. [Samtools](https://github.com/samtools/samtools.git) (version >= 1.13)
 
-You may alreadly have `minimap2` and `samtools` if you performed analysis of Oxford Nanopore sequencing data. You can use `which minimap2` and `which samtools` to check the full path to the two executable files.
+You may alreadly have `minimap2` and `samtools` if you performed analysis of Oxford Nanopore sequencing data. You can use `which minimap2` and `which samtools` to check the full path to the two executable files. Please note that `minimap2` should be v2.22 or later. 
+
+Once you installed the above tools, you can use the following commands to install NanoRepeat (we recommend creating an new conda environment to avoid dependency issues):
 
-Once you installed the above tools, you can use the following commands to install NanoRepeat:
-```
-pip install NanoRepeat
-```
-or
 ```
+conda create -n nanorepeat python=3.8
+conda activate nanorepeat
 git clone https://github.com/WGLab/NanoRepeat.git
 cd NanoRepeat
 pip install .
 ```
 
+If you want to install a stable version from Python Package Index (PyPI): 
+
+```
+conda create -n nanorepeat python=3.8
+conda activate nanorepeat
+pip install NanoRepeat
+```
+
 ## Usage
 
 ### Regular use cases
 
 NanoRepeat can quantify STRs from targeted sequencing or whole-genome sequencing data. We will demonstrate the usage of NanoRepeat using an example data set, which can be downloaded using the following commands. 
 
 ```
@@ -57,25 +76,28 @@
 
 You can use the following command to run NanoRepeat: 
 
 ```
 nanoRepeat.py \
     -i path/to/NanoRepeat_v1.3_example_data/HG002/hg002_Q20.20210805_3flowcells.hs37d5.example_regions.bam \
     -t bam \
+    -d ont_q20 \
     -r path/to/NanoRepeat_v1.3_example_data/HG002/GRCh37_chr1.fasta \
     -b path/to/NanoRepeat_v1.3_example_data/HG002/HG002_GRCh37_example_regions.bed \
     -c 4 \
     --samtools path/to/samtools \
     --minimap2 path/to/minimap2 \
     -o ./nanorepeat_output/HG002
 ```
 
 `-i` specifies the input file, which can be in `fasta`, `fastq` or `bam` format. In this case our input file is `hg002_Q20.20210805_3flowcells.hs37d5.example_regions.bam`. It is a subset of an Oxford Nanopore whole-genome sequencing dataset of the [NIST/GIAB HG002 (GM24385/NA24385)](https://catalog.coriell.org/0/Sections/Search/Sample_Detail.aspx?Ref=NA24385&Product=DNA) genome. The sequencing data was from the [Oxford Nanopore Technologies Benchmark Datasets](https://registry.opendata.aws/ont-open-data/) and reads from 15 example STR regions in `chr1` were extracted. These regions were selected because they overlap with the [HG002 SV benchmark set](https://ftp-trace.ncbi.nlm.nih.gov/giab/ftp/data/AshkenazimTrio/analysis/NIST_SVs_Integration_v0.6/HG002_SVs_Tier1_v0.6.vcf.gz) and are heterozygous (i.e., two alleles have different repeat sizes). 
 
-`-t` specifies the input file type. There are three valid values: bam, fastq or fasta. In this case the input file is in a bam file. 
+`-t` specifies the input file type. There are four valid values: bam, cram, fastq or fasta. In this case the input file is in a bam file. 
+
+`-d` specifies the data type. There are five valid values: `ont_q20`, `ont_sup`, `ont`, `hifi`, and `clr`. `ont_q20` is for Oxford Nanopore sequencing with Q20+ chemistry. `ont_sup` is for Oxford Nanopore sequencing with R9 flowcells and basecalled in super accuracy mode. `ont` is for Oxford Nanopore sequencing with R9 flowcells and basecalled in fast mode or high accuracy mode. `hifi` is for PacBio HiFi/CCS reads. `clr` is for PacBio Continuous Long Reads (CLR) reads. Default value: `ont`.
 
 `-r` specifies the reference genome file in `FASTA` format. In this case, `GRCh37_chr1.fasta` is chr1 of the GRCh37/hg19 reference genome. We used GRCh37 instead of GRCh38 because the HG002 SV benchmark set is based on GRCh37. 
 
 `-b` specifies the information of the tandem repeat regions that you are interested in. It is a tab-delimited text file in BED format. There are four required columns: `chromosome`, `start_position`, `end_position`, `repeat_unit_sequence`. In our case, `HG002_GRCh37_example_regions.bed` contains 15 STR regions in chr1 of GRCh37. The first 5 rows of the `HG002_GRCh37_example_regions.bed` are shown below. 
 
 | 1 | 4599903  | 4599930   | TTTAG   |
 |---|----------|-----------|---------|
```

### Comparing `NanoRepeat-1.4.0/setup.py` & `NanoRepeat-1.4.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
     
 setup(
     name='NanoRepeat',
-    version='1.4.0',
+    version='1.4.1',
     description='NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data',
     long_description = readme,
     long_description_content_type = 'text/markdown',
     url='https://github.com/WGLab/NanoRepeat',
     author='Li Fang, Kai Wang',
     author_email='fangli9@sysu.edu.cn',
     license='MIT',
```

### Comparing `NanoRepeat-1.4.0/src/NanoRepeat/nanoRepeat-joint.py` & `NanoRepeat-1.4.1/src/NanoRepeat/nanoRepeat-joint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 
 '''
-Copyright (c) 2020- Children's Hospital of Philadelphia
+Copyright (c) 2020-2023 Children's Hospital of Philadelphia
 Author: Li Fang (fangli2718@gmail.com)
               
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
```

### Comparing `NanoRepeat-1.4.0/src/NanoRepeat/nanoRepeat.py` & `NanoRepeat-1.4.1/src/NanoRepeat/nanoRepeat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 '''
-Copyright (c) 2020- Children's Hospital of Philadelphia
+Copyright (c) 2020-2023 Children's Hospital of Philadelphia
 Author: Li Fang (fangli2718@gmail.com)
               
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
@@ -108,45 +108,47 @@
     examples += f'\t{program} -i input.bam   -t bam -d ont_sup -r hg38.fasta -b hg38.repeats.bed -c 4 -o prefix/of/output/files\n\n'
     examples += f'\t# For ONT Q20+ reads\n'
     examples += f'\t{program} -i input.bam   -t bam -d ont_q20 -r hg38.fasta -b hg38.repeats.bed -c 4 -o prefix/of/output/files\n\n'
     examples += f'\t# For PacBio HiFi reads:\n'
     examples += f'\t{program} -i input.bam   -t bam -d hifi    -r hg38.fasta -b hg38.repeats.bed -c 4 -o prefix/of/output/files\n\n'
     examples += f'\t# For PacBio CLR reads:\n'
     examples += f'\t{program} -i input.bam   -t bam -d clr     -r hg38.fasta -b hg38.repeats.bed -c 4 -o prefix/of/output/files\n\n'
+    
     examples += f'\nContact: Li Fang (fangli9@sysu.edu.cn)\n'
     
     parser = argparse.ArgumentParser(prog = program, description=f'NanoRepeat: short tandem repeat (STR) quantification from Nanopore long-read sequencing', epilog=examples, formatter_class=RawTextHelpFormatter)
 
     # required
     parser.add_argument('-i', '--input', required = True, metavar = 'input_file', type = str, help = '(required) path to input file (supported format: sorted_bam, fastq or fasta)')
-    parser.add_argument('-t', '--type', required = True, metavar = 'input_type', type = str, help = '(required) input file type (valid values: bam, fastq or fasta)')
+    parser.add_argument('-t', '--type', required = True, metavar = 'input_file_type', type = str, help = '(required) input file type (valid values: bam, cram, fastq or fasta)')
     parser.add_argument('-r', '--ref_fasta', required = True, metavar = 'ref.fasta',   type = str, help = '(required) path to reference genome sequence in FASTA format')
     
     parser.add_argument('-b', '--repeat_region_bed', required = True, metavar = 'repeat_regions.bed', type = str, help = '(required) path to the repeat region file (tab delimited text file with 4 columns: chrom start end repeat_unit_seq. Positions start from 0. Start position is self-inclusive but end position is NOT self-inclusive)')
     parser.add_argument('-o', '--out_prefix', required = True, metavar = 'path/to/out_dir/prefix_of_file_names',   type = str, help = '(required) prefix of output files')
     
     # optional
     parser.add_argument('-d', '--data_type', required = False, metavar = 'data_type',  type = str, default = 'ont', help = '(required) sequencing data type. Should be one of the following: ont, ont_sup, ont_q20, clr, hifi')
     parser.add_argument('-c', '--num_cpu', required = False, metavar = 'INT',   type = int, default = 1,  help ='(optional) number of CPU cores (default: 1)')
     parser.add_argument('--samtools', required = False, metavar = 'path/to/samtools',  type = str, default = 'samtools', help ='(optional) path to samtools (default: using environment default)')
     parser.add_argument('--minimap2', required = False, metavar = 'path/to/minimap2',  type = str, default = 'minimap2', help ='(optional) path to minimap2 (default: using environment default)')
     parser.add_argument('--ploidy',   required = False, metavar = 'INT', type = int, default = 2,  help ='(optional) ploidy of the sample (default: 2)')
     parser.add_argument('--anchor_len', required = False, metavar = 'INT', type = int, default = 1000, help ='(optional) length of up/downstream sequence to help identify the repeat region (default: 1000 bp, increase this value if the 1000 bp up/downstream sequences are also repeat)')
     parser.add_argument('--max_mutual_overlap', required = False, metavar = 'FLOAT',  type = float, default = 0.15,  help = 'max mutual overlap of two alleles in terms of repeat size distribution (default value: 0.1). If the Gaussian distribution of two alleles have more overlap than this value, the two alleles will be merged into one allele.')
     parser.add_argument('--remove_noisy_reads', required = False, action='store_true', help = 'remove noisy components when there are more components than ploidy')
+    parser.add_argument('--save_temp_files', required = False, action='store_true', help = 'save temporary alignment files')
     parser.add_argument('--max_num_components', required = False, metavar = 'INT',  type = int, default = -1,  help = 'max number of components for the Gaussian mixture model (default value: ploidy + 20). Some noisy reads and outlier reads may form a component. Therefore the number of components is usually larger than ploidy. If your sample have too many outlier reads, you can increase this number.')
     
     if len(sys.argv) < 2 or sys.argv[1] in ['help', 'h', '-help', 'usage']:
         input_args = parser.parse_args(['--help'])
     else:
         input_args = parser.parse_args()
 
     input_args.type = input_args.type.lower()
     
-    if input_args.type not in ['bam', 'fastq', 'fasta']:
+    if input_args.type not in ['bam', 'cram', 'fastq', 'fasta']:
         tk.eprint(f'ERROR! unknown input type: {input_args.type} valid values are: bam, fastq, fasta')
         sys.exit(1)
     
     if input_args.data_type not in ['ont', 'ont_sup', 'ont_q20', 'clr', 'hifi']:
         tk.eprint(f'ERROR! data_type should be one of the following: ont, ont_sup, clr, hifi\n')
         tk.eprint(f'ont:     Oxford Nanopore sequencing, NOT Super Accuracy mode\n')
         tk.eprint(f'ont_sup: Oxford Nanopore sequencing, Super Accuracy mode\n')
@@ -187,18 +189,18 @@
 
     os.makedirs(out_dir, exist_ok=True)
 
     if input_args.type == 'fastq':
         preprocess_fastq(input_args)
     elif input_args.type == 'fasta':
         preprocess_fastq(input_args)
-    elif input_args.type == 'bam':
+    elif input_args.type == 'bam' or input_args.type == 'cram':
         nanoRepeat_bam.nanoRepeat_bam(input_args, input_args.input)
     else:
-        tk.eprint(f'ERROR! Unknown input type: {input_args.type} valid values are: bam, fastq, fasta')
+        tk.eprint(f'ERROR! Unknown input type: {input_args.type} valid values are: bam, cram, fastq, fasta')
         sys.exit(1)
     
     return
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `NanoRepeat-1.4.0/src/NanoRepeat/nanoRepeat_bam.py` & `NanoRepeat-1.4.1/src/NanoRepeat/nanoRepeat_bam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 '''
-Copyright (c) 2020- Children's Hospital of Philadelphia
+Copyright (c) 2020-2023 Children's Hospital of Philadelphia
 Author: Li Fang (fangli2718@gmail.com)
               
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
@@ -148,17 +148,17 @@
     ref_check_paf_file   = os.path.join(temp_out_dir, 'ref_aligned_to_pure_repeats.paf')
     mid_ref_seq_file     = os.path.join(temp_out_dir, 'mid_ref_seq.fasta')
     pure_repeat_seq_file = os.path.join(temp_out_dir, 'pure_repeat_seq.fasta')
 
     write_seq_to_fasta(f'mid_ref_seq_{repeat_region_location}', mid_ref_seq, mid_ref_seq_file)
     write_seq_to_fasta('pure_repeat_seq', pure_repeat_seq, pure_repeat_seq_file)
 
-    score_parameters = '-A1 -B4 -O6,26 -E2,1 -z30' 
-    cmd = f'{minimap2} {score_parameters} -k3 -w2 -m3 -n1 -s3 -f 10000 --cs  {pure_repeat_seq_file} {mid_ref_seq_file} > {ref_check_paf_file} 2> /dev/null'
-    tk.eprint(f'NOTICE: Running command: {cmd}')
+    score_parameters = '-x ava-ont -z30 -k3 -w2 -m1 -n2 -s10'
+
+    cmd = f'{minimap2} {score_parameters} -f 0 --cs  {pure_repeat_seq_file} {mid_ref_seq_file} > {ref_check_paf_file}'
     tk.run_system_cmd(cmd)
 
     ref_check_paf_f = open(ref_check_paf_file, 'r')
     lines = list(ref_check_paf_f)
     ref_check_paf_f.close()
 
     paf_list = []
@@ -352,16 +352,15 @@
     template_fasta_fp.write('%s\n' % right_template_seq)
     template_fasta_fp.close()
 
     anchor_locations_paf_file = os.path.join(repeat_region.temp_out_dir, 'anchor_locations.paf')
     repeat_region.temp_file_list.append(anchor_locations_paf_file)
 
     preset = tk.get_preset_for_minimap2(data_type)
-    cmd = f'{minimap2} -c -t {num_cpu} {preset} {template_fasta_file} {repeat_region.region_fq_file} > {anchor_locations_paf_file} 2> /dev/null'
-    tk.eprint(f'NOTICE: Running command: {cmd}')
+    cmd = f'{minimap2} -c -t {num_cpu} {preset} {template_fasta_file} {repeat_region.region_fq_file} > {anchor_locations_paf_file}'
     tk.run_system_cmd(cmd)
 
     find_anchor_locations_from_paf(repeat_region, anchor_locations_paf_file)
     
     return
 
 def make_core_seq_fastq(repeat_region: RepeatRegion):
@@ -432,17 +431,15 @@
     round1_fasta_f.write(f'{repeat_region.left_anchor_seq}{repeat_region.repeat_unit_seq * template_repeat_size}\n')
     round1_fasta_f.close()
 
     round1_paf_file = os.path.join(repeat_region.temp_out_dir, 'round1.paf')
     repeat_region.temp_file_list.append(round1_paf_file)
     
     preset = tk.get_preset_for_minimap2(data_type)
-    cmd = f'{minimap2} -c -t {num_cpu} {preset} {round1_fasta_file} {repeat_region.core_seq_fq_file} > {round1_paf_file} 2> /dev/null'
-    
-    tk.eprint(f'NOTICE: Running command: {cmd}')
+    cmd = f'{minimap2} -c -t {num_cpu} {preset} -f 0.0 {round1_fasta_file} {repeat_region.core_seq_fq_file} > {round1_paf_file}'
     tk.run_system_cmd(cmd)
     round1_paf_f = open(round1_paf_file, 'r')
     lines = list(round1_paf_f)
     round1_paf_f.close()
 
     for line in lines:
         col_list = line.strip().split('\t')
@@ -536,15 +533,15 @@
 
     template_fasta_fp.close()
 
     round3_paf_file = os.path.join(repeat_region.temp_out_dir, 'round3.paf')
     repeat_region.temp_file_list.append(round3_paf_file)
 
     preset = tk.get_preset_for_minimap2(data_type)
-    cmd = f'{minimap2} {preset} -N 100 -c --eqx -t {num_cpu} {template_fasta_file} {repeat_region.core_seq_fq_file} > {round3_paf_file} 2> /dev/null'
+    cmd = f'{minimap2} {preset} -f 0.0 -N 100 -c --eqx -t {num_cpu} {template_fasta_file} {repeat_region.core_seq_fq_file} > {round3_paf_file}'
     tk.run_system_cmd(cmd)
 
     round3_estimation_from_paf(repeat_region, round3_paf_file)
     
     return
 
 def remove_noisy_reads_1d(allele_list, ploidy):
@@ -609,15 +606,14 @@
     allele_list.sort(key = lambda allele:allele.gmm_mean1)
 
     readinfo_dict = create_readinfo_dict_from_allele_list(allele_list, dimension)
 
     tk.eprint('NOTICE: Writing phasing results...')
     output_phasing_results_1d(allele_list, repeat_region.to_unique_id(), repeat_region.out_prefix)
     
-    tk.eprint('NOTICE: Writing to output fastq files...')
     output_phased_fastq(in_fastq_file, readinfo_dict, best_n_components, out_prefix)
 
     tk.eprint('NOTICE: Writing summary file...')
     output_summary_file_1d(allele_list, repeat_region.to_unique_id(), num_removed_reads, out_prefix)
 
     tk.eprint('NOTICE: Plotting figures...')
     plot_repeat_counts_1d(readinfo_dict, allele_list, repeat_region.to_unique_id(), out_prefix)
@@ -631,34 +627,43 @@
 
     repeat_region.temp_out_dir = temp_out_dir
     repeat_region.out_prefix = f'{input_args.out_prefix}.{repeat_region.to_outfile_prefix()}'
     repeat_region.anchor_len = input_args.anchor_len
 
     # extract reads from bam file
     repeat_region.region_fq_file = os.path.join(temp_out_dir, f'{repeat_region.to_outfile_prefix()}.fastq')
-    cmd = f'{input_args.samtools} view -h {in_bam_file} {repeat_region.to_invertal(flank_dist=10)} | {input_args.samtools} fastq - > {repeat_region.region_fq_file} 2> /dev/null'
+    region_bam_file = f'{repeat_region.out_prefix}.sorted.bam'
+    cmd = f'{input_args.samtools} view --reference {input_args.ref_fasta} -hb {in_bam_file} {repeat_region.to_invertal(flank_dist=repeat_region.anchor_len)} > {region_bam_file}'
+    tk.run_system_cmd(cmd)
+    
+    cmd = f'{input_args.samtools} index {region_bam_file}'
+    tk.run_system_cmd(cmd)
+    
+    cmd = f'{input_args.samtools} fastq {region_bam_file} > {repeat_region.region_fq_file}'
     tk.run_system_cmd(cmd)
 
     fastq_file_size = os.path.getsize(repeat_region.region_fq_file)
     if fastq_file_size == 0:
         tk.eprint(f'WARNING! No reads were found in repeat region: {repeat_region.to_outfile_prefix()}')
-        shutil.rmtree(repeat_region.temp_out_dir)
+        if input_args.save_temp_files == False: 
+            shutil.rmtree(repeat_region.temp_out_dir)
         return
 
     # extract ref sequence
     extract_ref_sequence(ref_fasta_dict, repeat_region)
     
     refine_repeat_region_in_ref(input_args.minimap2, repeat_region)
     
     if repeat_region.ref_has_issue == True: 
-        shutil.rmtree(repeat_region.temp_out_dir)
+        if input_args.save_temp_files == False: 
+            shutil.rmtree(repeat_region.temp_out_dir)
         return
     
     tk.eprint('NOTICE: Step 1: finding anchor location in reads')
-    status = find_anchor_locations_in_reads(input_args.minimap2, input_args.data_type, repeat_region, input_args.num_cpu)
+    find_anchor_locations_in_reads(input_args.minimap2, input_args.data_type, repeat_region, input_args.num_cpu)
     tk.eprint('NOTICE: Step 1 finished')
 
     # make core sequence fastq
     make_core_seq_fastq(repeat_region)
 
     tk.eprint('NOTICE: Step 2: round 1 and round 2 estimation')
     round1_and_round2_estimation(input_args.minimap2, input_args.data_type, repeat_region, input_args.num_cpu)
@@ -670,28 +675,29 @@
 
     tk.eprint('NOTICE: Writing to repeat size file...')
     output_repeat_size_1d(repeat_region)
 
     tk.eprint('NOTICE: Step 4: phasing reads using GMM')
     split_allele_using_gmm_1d(repeat_region, input_args.ploidy, error_rate, input_args.max_mutual_overlap, input_args.max_num_components, input_args.remove_noisy_reads)
     
-    shutil.rmtree(repeat_region.temp_out_dir)
+    if input_args.save_temp_files == False:
+        shutil.rmtree(repeat_region.temp_out_dir)
 
     return
 
 def nanoRepeat_bam (input_args, in_bam_file:string):
     
     # ont, ont_sup, ont_q20, clr, hifi
 
     if input_args.data_type == 'ont' or 'clr':
-        error_rate = 0.14
-    elif input_args.data_type == 'ont_sup':
         error_rate = 0.07
-    elif input_args.data_type == 'ont_q20':
+    elif input_args.data_type == 'ont_sup':
         error_rate = 0.04
+    elif input_args.data_type == 'ont_q20':
+        error_rate = 0.03
     elif input_args.data_type == 'hifi':
         error_rate = 0.02
     else:
         tk.eprint(f'ERROR! unknown data type: {input_args.data_type}')
         sys.exit(1)
     
     tk.eprint(f'NOTICE: Reading repeat region file: {input_args.repeat_region_bed}')
```

### Comparing `NanoRepeat-1.4.0/src/NanoRepeat/paf.py` & `NanoRepeat-1.4.1/src/NanoRepeat/paf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 '''
-Copyright (c) 2020- Children's Hospital of Philadelphia
+Copyright (c) 2020-2023 Children's Hospital of Philadelphia
 Author: Li Fang (fangli2718@gmail.com)
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
```

### Comparing `NanoRepeat-1.4.0/src/NanoRepeat/repeat_region.py` & `NanoRepeat-1.4.1/src/NanoRepeat/repeat_region.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 '''
-Copyright (c) 2020- Children's Hospital of Philadelphias
+Copyright (c) 2020-2023 Children's Hospital of Philadelphias
 Author: Li Fang (fangli2718@gmail.com)
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
```

### Comparing `NanoRepeat-1.4.0/src/NanoRepeat/split_alleles.py` & `NanoRepeat-1.4.1/src/NanoRepeat/split_alleles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 '''
-Copyright (c) 2020- Children's Hospital of Philadelphia
+Copyright (c) 2020-2023 Children's Hospital of Philadelphia
 Author: Li Fang (fangli2718@gmail.com)
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
@@ -21,14 +21,15 @@
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 '''
 
+import os
 import sys
 import random
 import numpy as np
 from sklearn.mixture import GaussianMixture
 from scipy.stats import norm
 import math
 import gzip
@@ -69,18 +70,17 @@
         self.readname = readname
         self.label = -1
         self.repeat_size1 = -1
         self.repeat_size2 = -1
         self.confidence = 1
 
 def simulate_reads(read_repeat_count_list, error_rate):
-    min_std = 1.0
     simulated_read_repeat_count_list = read_repeat_count_list * 100
     for i in range(0, len(simulated_read_repeat_count_list)):
-        std = min_std + 1.25 * error_rate/3.0 * simulated_read_repeat_count_list[i]
+        std = error_rate * (10 + simulated_read_repeat_count_list[i])
         random_error = random.gauss(0, std)
         simulated_read_repeat_count_list[i] += random_error
     return simulated_read_repeat_count_list
 
 def interval_has_overlap(interval1, interval2):
     start = min(interval1[1], interval2[1])
     end = max(interval1[0], interval2[0])
@@ -457,19 +457,19 @@
 
     return
 
 def output_summary_file_1d(allele_list, repeat_id, num_removed_reads, out_prefix):
 
     num_alleles = len(allele_list)
     out_summray_file = out_prefix + '.summary.txt'
+    filebasename = os.path.split(out_summray_file)[1]
     out_summray_f = open(out_summray_file, 'w')
-    summary_info  = f'Repeat_Region={repeat_id}'
+    summary_info  = f'Summary_file={filebasename}\tRepeat_Region={repeat_id}'
     summary_info += f'\tMethod=GMM'
     summary_info += f'\tNum_Alleles={num_alleles}'
-
     summary_info += f'\tNum_Removed_Reads={num_removed_reads}'
 
     for label in range(0, num_alleles):
         allele_id = label + 1
         summary_info += f'\tAllele{allele_id}_Num_Reads={allele_list[label].num_reads}'
         summary_info += f'\tAllele{allele_id}_Repeat_Size={allele_list[label].repeat1_median_size}'
```

### Comparing `NanoRepeat-1.4.0/src/NanoRepeat/tk.py` & `NanoRepeat-1.4.1/src/NanoRepeat/tk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 '''
-Copyright (c) 2020- Children's Hospital of Philadelphia
+Copyright (c) 2020-2023 Children's Hospital of Philadelphia
 Author: Li Fang (fangli2718@gmail.com)
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
@@ -92,15 +92,14 @@
     if os.path.exists(out_file) == False or os.path.getsize(out_file) == 0:
         return False
     else:
         return True
 
 def eprint(message):
     sys.stderr.write('[' + datetime.now().strftime(TimeFormat) + '] ' + message + '\n')
-
     return
 
 def get_file_prefix(input_file):
 
     return os.path.splitext(os.path.split(input_file)[1])[0]
 
 ### FASTQ/FASTA ###
@@ -499,21 +498,21 @@
     read_error = ReadError(num_match, num_mismatch, num_ins, num_del, align_score)
     return read_error
 
 def get_preset_for_minimap2(data_type):
     if data_type == 'ont':
         preset = ' -x map-ont '
     elif data_type == 'ont_sup':
-        preset = ' -x map-ont -A 2 -B 6 '
+        preset = ' -x map-ont '
     elif data_type == 'ont_q20':
-        preset = ' -x map-ont -A 2 -B 8 '
+        preset = ' -x map-ont '
     elif data_type == 'clr':
-        preset = ' -x map-pb '
+        preset = ' -x map-ont '
     elif data_type == 'hifi':
-        preset = ' -x map-hifi '
+        preset = ' -x map-ont '
     else:
         eprint(f'ERROR: Unknown data type: {data_type}\n')
         sys.exit(1)
     
     return preset
 
 minimap2_mid_para   = ' -k 5 -w 3 -n 1 -m 10 -s 40 '
@@ -523,15 +522,15 @@
 def switch_two_numbers(a, b):
     return b, a
 
 def switch_two_objects(a, b):
     return b, a
 
 def run_system_cmd(cmd):
-
+    eprint(f'NOTICE: Running command: {cmd}')  
     ret = os.system(cmd)
     if ret != 0: 
         eprint('ERROR: Failed to run command: %s' % cmd)
         eprint('Return value is: %d' % ret)
         sys.exit()
     return
```

### Comparing `NanoRepeat-1.4.0/src/NanoRepeat.egg-info/PKG-INFO` & `NanoRepeat-1.4.1/src/NanoRepeat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: NanoRepeat
-Version: 1.4.0
+Version: 1.4.1
 Summary: NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data
 Home-page: https://github.com/WGLab/NanoRepeat
 Author: Li Fang, Kai Wang
 Author-email: fangli9@sysu.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7024485.svg)](https://doi.org/10.5281/zenodo.7024485)
+[![PyPI version](https://badge.fury.io/py/NanoRepeat.svg)](https://badge.fury.io/py/NanoRepeat)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7919607.svg)](https://doi.org/10.5281/zenodo.7919607)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
   - [Regular use cases](#regular-use-cases)
   - [Joint quantification of two adjacent repeats](#joint_quantification)
@@ -24,30 +25,37 @@
 - [Contact Us](#contact-us)
 
 ## Installation
 
 #### Prerequisites:
 
 1. [Python](https://www.python.org/downloads/) (version >= 3.8)
-2. [Minimap2](https://github.com/lh3/minimap2) (version >= 2.8)
-3. [Samtools](https://github.com/samtools/samtools.git) (version >= 1.3)
+2. [Minimap2](https://github.com/lh3/minimap2) (version >= 2.22)
+3. [Samtools](https://github.com/samtools/samtools.git) (version >= 1.13)
 
-You may alreadly have `minimap2` and `samtools` if you performed analysis of Oxford Nanopore sequencing data. You can use `which minimap2` and `which samtools` to check the full path to the two executable files.
+You may alreadly have `minimap2` and `samtools` if you performed analysis of Oxford Nanopore sequencing data. You can use `which minimap2` and `which samtools` to check the full path to the two executable files. Please note that `minimap2` should be v2.22 or later. 
+
+Once you installed the above tools, you can use the following commands to install NanoRepeat (we recommend creating an new conda environment to avoid dependency issues):
 
-Once you installed the above tools, you can use the following commands to install NanoRepeat:
-```
-pip install NanoRepeat
-```
-or
 ```
+conda create -n nanorepeat python=3.8
+conda activate nanorepeat
 git clone https://github.com/WGLab/NanoRepeat.git
 cd NanoRepeat
 pip install .
 ```
 
+If you want to install a stable version from Python Package Index (PyPI): 
+
+```
+conda create -n nanorepeat python=3.8
+conda activate nanorepeat
+pip install NanoRepeat
+```
+
 ## Usage
 
 ### Regular use cases
 
 NanoRepeat can quantify STRs from targeted sequencing or whole-genome sequencing data. We will demonstrate the usage of NanoRepeat using an example data set, which can be downloaded using the following commands. 
 
 ```
@@ -68,25 +76,28 @@
 
 You can use the following command to run NanoRepeat: 
 
 ```
 nanoRepeat.py \
     -i path/to/NanoRepeat_v1.3_example_data/HG002/hg002_Q20.20210805_3flowcells.hs37d5.example_regions.bam \
     -t bam \
+    -d ont_q20 \
     -r path/to/NanoRepeat_v1.3_example_data/HG002/GRCh37_chr1.fasta \
     -b path/to/NanoRepeat_v1.3_example_data/HG002/HG002_GRCh37_example_regions.bed \
     -c 4 \
     --samtools path/to/samtools \
     --minimap2 path/to/minimap2 \
     -o ./nanorepeat_output/HG002
 ```
 
 `-i` specifies the input file, which can be in `fasta`, `fastq` or `bam` format. In this case our input file is `hg002_Q20.20210805_3flowcells.hs37d5.example_regions.bam`. It is a subset of an Oxford Nanopore whole-genome sequencing dataset of the [NIST/GIAB HG002 (GM24385/NA24385)](https://catalog.coriell.org/0/Sections/Search/Sample_Detail.aspx?Ref=NA24385&Product=DNA) genome. The sequencing data was from the [Oxford Nanopore Technologies Benchmark Datasets](https://registry.opendata.aws/ont-open-data/) and reads from 15 example STR regions in `chr1` were extracted. These regions were selected because they overlap with the [HG002 SV benchmark set](https://ftp-trace.ncbi.nlm.nih.gov/giab/ftp/data/AshkenazimTrio/analysis/NIST_SVs_Integration_v0.6/HG002_SVs_Tier1_v0.6.vcf.gz) and are heterozygous (i.e., two alleles have different repeat sizes). 
 
-`-t` specifies the input file type. There are three valid values: bam, fastq or fasta. In this case the input file is in a bam file. 
+`-t` specifies the input file type. There are four valid values: bam, cram, fastq or fasta. In this case the input file is in a bam file. 
+
+`-d` specifies the data type. There are five valid values: `ont_q20`, `ont_sup`, `ont`, `hifi`, and `clr`. `ont_q20` is for Oxford Nanopore sequencing with Q20+ chemistry. `ont_sup` is for Oxford Nanopore sequencing with R9 flowcells and basecalled in super accuracy mode. `ont` is for Oxford Nanopore sequencing with R9 flowcells and basecalled in fast mode or high accuracy mode. `hifi` is for PacBio HiFi/CCS reads. `clr` is for PacBio Continuous Long Reads (CLR) reads. Default value: `ont`.
 
 `-r` specifies the reference genome file in `FASTA` format. In this case, `GRCh37_chr1.fasta` is chr1 of the GRCh37/hg19 reference genome. We used GRCh37 instead of GRCh38 because the HG002 SV benchmark set is based on GRCh37. 
 
 `-b` specifies the information of the tandem repeat regions that you are interested in. It is a tab-delimited text file in BED format. There are four required columns: `chromosome`, `start_position`, `end_position`, `repeat_unit_sequence`. In our case, `HG002_GRCh37_example_regions.bed` contains 15 STR regions in chr1 of GRCh37. The first 5 rows of the `HG002_GRCh37_example_regions.bed` are shown below. 
 
 | 1 | 4599903  | 4599930   | TTTAG   |
 |---|----------|-----------|---------|
```

