# Comparing `tmp/wgd-2.0.12.tar.gz` & `tmp/wgd-2.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wgd-2.0.12.tar", last modified: Tue May  9 09:30:37 2023, max compression
+gzip compressed data, was "dist/wgd-2.0.13.tar", last modified: Wed May 17 12:42:30 2023, max compression
```

## Comparing `wgd-2.0.12.tar` & `wgd-2.0.13.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-09 09:30:37.734892 wgd-2.0.12/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.12/LICENSE
--rwxrwxrwx   0 heche     (1000) heche     (1000)    27801 2023-05-09 09:30:37.734892 wgd-2.0.12/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)    27563 2023-05-08 19:59:05.000000 wgd-2.0.12/README.md
--rwxrwxrwx   0 heche     (1000) heche     (1000)    48998 2023-05-09 09:13:48.000000 wgd-2.0.12/cli.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-09 09:30:37.734892 wgd-2.0.12/setup.cfg
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1895 2023-05-09 09:30:13.000000 wgd-2.0.12/setup.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-09 09:30:37.712375 wgd-2.0.12/test/
--rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-05-08 19:45:47.000000 wgd-2.0.12/test/test_core.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-09 09:30:37.726938 wgd-2.0.12/wgd/
--rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.12/wgd/__init__.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.12/wgd/beast.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.12/wgd/cluster.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.12/wgd/codeml.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   134346 2023-05-08 19:45:47.000000 wgd-2.0.12/wgd/core.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.12/wgd/mcmctree.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.12/wgd/mix.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   103602 2023-05-08 19:45:47.000000 wgd-2.0.12/wgd/peak.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8513 2023-05-08 19:45:47.000000 wgd-2.0.12/wgd/syn.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    28648 2022-09-30 07:30:21.000000 wgd-2.0.12/wgd/utils.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    95007 2023-05-09 09:20:19.000000 wgd-2.0.12/wgd/viz.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-09 09:30:37.734023 wgd-2.0.12/wgd.egg-info/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    27801 2023-05-09 09:30:37.000000 wgd-2.0.12/wgd.egg-info/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)      369 2023-05-09 09:30:37.000000 wgd-2.0.12/wgd.egg-info/SOURCES.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-09 09:30:37.000000 wgd-2.0.12/wgd.egg-info/dependency_links.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       32 2023-05-09 09:30:37.000000 wgd-2.0.12/wgd.egg-info/entry_points.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)      740 2023-05-09 09:30:37.000000 wgd-2.0.12/wgd.egg-info/requires.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-05-09 09:30:37.000000 wgd-2.0.12/wgd.egg-info/top_level.txt
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-17 12:42:30.193328 wgd-2.0.13/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.13/LICENSE
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    34148 2023-05-17 12:42:30.195320 wgd-2.0.13/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    30341 2023-05-10 06:37:55.000000 wgd-2.0.13/README.md
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    48990 2023-05-11 09:03:45.000000 wgd-2.0.13/cli.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-17 12:42:30.196325 wgd-2.0.13/setup.cfg
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1895 2023-05-17 12:39:50.000000 wgd-2.0.13/setup.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-17 12:42:30.163813 wgd-2.0.13/test/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-05-08 19:45:47.000000 wgd-2.0.13/test/test_core.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-17 12:42:30.184322 wgd-2.0.13/wgd/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.13/wgd/__init__.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.13/wgd/beast.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.13/wgd/cluster.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.13/wgd/codeml.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   134351 2023-05-10 07:50:19.000000 wgd-2.0.13/wgd/core.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.13/wgd/mcmctree.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.13/wgd/mix.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   103647 2023-05-10 05:58:49.000000 wgd-2.0.13/wgd/peak.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     8513 2023-05-08 19:45:47.000000 wgd-2.0.13/wgd/syn.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    28648 2022-09-30 07:30:21.000000 wgd-2.0.13/wgd/utils.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    95109 2023-05-09 11:58:52.000000 wgd-2.0.13/wgd/viz.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-17 12:42:30.192319 wgd-2.0.13/wgd.egg-info/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    34148 2023-05-17 12:42:30.000000 wgd-2.0.13/wgd.egg-info/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      369 2023-05-17 12:42:30.000000 wgd-2.0.13/wgd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-17 12:42:30.000000 wgd-2.0.13/wgd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       51 2023-05-17 12:42:30.000000 wgd-2.0.13/wgd.egg-info/entry_points.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      740 2023-05-17 12:42:30.000000 wgd-2.0.13/wgd.egg-info/requires.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-05-17 12:42:30.000000 wgd-2.0.13/wgd.egg-info/top_level.txt
```

### Comparing `wgd-2.0.12/LICENSE` & `wgd-2.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `wgd-2.0.12/PKG-INFO` & `wgd-2.0.13/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: wgd
-Version: 2.0.12
-Summary: wgd
-Home-page: http://github.com/heche-psb/wgd
-Author: Hengchi Chen
-Author-email: heche@psb.vib-ugent.be
-License: GPL
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 
 # `wgd v2` : a suite tool of WGD inference and timing
 
 [![Build Status](https://app.travis-ci.com/heche-psb/wgd.svg?branch=phylodating)](https://travis-ci.com/heche-psb/wgd)
 
 **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
@@ -389,17 +378,61 @@
 First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
 
 ```
 wgd dmd Aquilegia_coerulea
 wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
 ```
 
-The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1.
+The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
+
+![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
+
+We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
+
+```
+wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+```
+
+As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
+
+![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
+
+The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
+
+![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
+
+The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
+
+A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
+
+![](data/Syndepth.svg)
+
+We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
+
+```
+wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+```
+
+The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
+
+![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
+
+Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
+
+```
+wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
+```
+
+The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
+
+![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
 
-![](data/Aquilegia_coerulea.tsv.ksd.svg)
+Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis.
 
 ## Citation
  
 Please cite us at https://doi.org/10.1093/bioinformatics/bty915
 
 ```
 Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
```

### Comparing `wgd-2.0.12/README.md` & `wgd-2.0.13/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,401 +1,456 @@
-<div align="center">
-
-# `wgd v2` : a suite tool of WGD inference and timing
-
-[![Build Status](https://app.travis-ci.com/heche-psb/wgd.svg?branch=phylodating)](https://travis-ci.com/heche-psb/wgd)
-
-**Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
-
-[**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
-
-[**Introduction**](#Introduction) | 
-[**Installation**](#Installation) | 
-[**Parameters**](#Parameters) | 
-[**Usage**](#Usage) | 
-[**Illustration**](#Illustration) |
-[**Citation**](#Citation)
-
-</div>
-
-`wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
-
-## Introduction
-
-Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
-
-The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
-
-## Installation
-
-The easiest way to install `wgd v2` is using PYPI
-
-```
-pip install wgd
-```
-
-To install `wgd v2` in a virtual environment, the following command lines could be used.
-
-```
-git clone <wgd repo>
-cd wgd
-virtualenv -p=python3 ENV (or python3 -m venv ENV)
-source ENV/bin/activate
-pip install -r requirements.txt
-pip install .
-```
-
-When met with permission problem in installation, please try the following command line.
-
-```
-pip install -e .
-```
-
-If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
-
-```
-export PATH="$PATH:~/.local/bin/wgd"
-```
-
-## Parameters
-
-There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
-
-The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
-```
-wgd dmd sequences (option)
---------------------------------------------------------------------------------
--o, --outdir, the output directory, default wgd_dmd
--t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
--c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
--I, --inflation, the inflation factor for MCL program, default 2.0
--e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
---to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
---cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
--f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
--ap, --anchorpoints, the anchor points data file, default None
--coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
--sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
--le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
--gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
--kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
--kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
--gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
--n, --nthreads, the number of threads to use, default 4
--oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
--oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
--gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
--tree, --tree_method, which gene tree inference program to invoke, default fasttree
--ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
--mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
--ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
--am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
--sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
--fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
--cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
--te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
--bs, --bins, the number of bins divided in gene length normalization, default 100
--np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
--nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
--bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
--bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
--bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
-```
-
-The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
-```
-wgd focus families sequences (option)
---------------------------------------------------------------------------------
--o, --outdir, the output directory, default wgd_focus
--t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
--n, --nthreads, the number of threads to use, default 4
---to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
---cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
---strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
--a, --aligner, which alignment program to use, default mafft
--tree, --tree_method, which gene tree inference program to invoke, default fasttree
--ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
---concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
---coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
--sp, --speciestree, species tree darafile for dating, default None
--d, --dating, which molecular dating program to use, default none
--ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
--ns, --nsites, the nsites information for r8s dating, default None
--ot, --outgroup, the outgroup information for r8s dating, default None
--pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
--am, --aamodel, which protein model to be used in mcmctree, default poisson
--ks, flag option, whether to initiate Ks analysis
---annotation, which annotation program to use, default none
---pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
--ed, --eggnogdata, the eggnog annotation datafile, default None
---pfam, which option to use for pfam annotation, default none
---dmnb, the diamond database for annotation, default None
---hmm, the HMM profile for annotation, default None
---evalue, the e-value cut-off for annotation, default 1e-10
---exepath, the path to the interproscan executable, default None
--f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
- -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
--cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
---beastlgjar, the path to beastLG.jar, default None
---beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
---protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
-```
-
-The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
-```
-wgd ksd families sequences (option)
---------------------------------------------------------------------------------
--o, --outdir, the output directory, default wgd_ksd
--t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
--n, --nthreads, the number of threads to use, default 4
---to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
---cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
---pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
---strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
--tree, --tree_method, which gene tree inference program to invoke, default fasttree
--sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
--sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
--rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
--or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
-```
-
-The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
-```
-wgd mix ks_datafile (option)
---------------------------------------------------------------------------------
--f, --filters, the cutoff alignment length, default 300
--r, --ks_range, the Ks range to be considered, default (0.005, 3)
--b, --bins, the number of bins in Ks distribution, default 50
--o, --outdir, the output directory, default wgd_mix
---method, which mixture model to use, default gmm
--n, --components, the range of the number of components to fit, default (1, 4)
--g, --gamma, the gamma parameter for bgmm models, default 0.001
--ni, --n_init, the number of k-means initializations, default 200
--mi, --max_iter, the maximum number of iterations, default 1000
-```
-
-The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
-```
-wgd peak ks_datafile (option)
---------------------------------------------------------------------------------
--ap, --anchorpoints, the anchor points datafile, default None
--sm, --segments, the segments datafile, default None
--le, --listelements, the listsegments datafile, default None 
--mp, --multipliconpairs, the multipliconpairs datafile, default None
--o, --outdir, the output directory, default wgd_peak
--af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
--r, --ksrange, range of Ks to be analyzed, default (0, 5)
--bw, --bin_width, bandwidth of Ks distribution, default 0.1
--ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
--m, --method, which mixture model to use, default gmm
---seed, random seed given to initialization, default 2352890
--ei, --em_iter, the number of EM iterations to perform, default 200
--ni, --n_init, the number of k-means initializations, default 200
--n, --components, the range of the number of components to fit, default (1, 4)
---boots, the number of bootstrap replicates of kde, default 200
---weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
--p, --plot, the plotting method to be used, default identical
--bm, --bw_method, the bandwidth method to be used, default silverman
---n_medoids, the number of medoids to fit, default 2
--km, --kdemethod, the kde method to be used, default scipy
---n_clusters, the number of clusters to plot Elbow loss function, default 5
---kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
--gd, --guide, the regime residing anchors, default: segment
--prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
--kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
--f, --family, the family to filter Ks upon, default None
---manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
--rh, --rel_height, the relative height at which the peak width is measured, default 0.4
---ci, the confidence level of log-normal distribution to date, default 95
---hdr, the highest densidy region (HDR) in a given distribution to date, default 95
---heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
--kc, --kscutoff, the Ks saturation cutoff in dating, default 5
-```
-
-The program `wgd syn` can realize the intra- and inter-specific synteny inference.
-```
-wgd syn families gffs (option)
---------------------------------------------------------------------------------
--ks, --ks_distribution, ks distribution datafile, default None
--o, --outdir, the output directory, default wgd_syn
--f, --feature, the feature for parsing gene IDs from GFF files, default gene
--a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
--ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
--ms, --maxsize, the maximum family size to include, default 200
--r, --ks_range, the Ks range in colored dotplot, default (0, 5)
---iadhore_options, the parameter setting in iadhore, default 
--ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
--mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
--kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-```
-
-The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
-```
-wgd viz (option)
---------------------------------------------------------------------------------
--d, --datafile, the Ks datafile, default None
--o, --outdir, the output directory, default wgd_viz
--sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
--gs, --gsmap, the gene name-species name map, default None
--sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
--pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
--rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
--or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
--iter, --em_iterations, the maximum EM iterations, default 200
--init, --em_initializations, the maximum EM initializations, default 200
--prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
--sm, --segments, the segments data file, default None
--ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
--ms, --maxsize, the maximum family size to include, default 200
--ap, --anchorpoints, the anchor points datafile, default None
--mt, --multiplicon, the multiplicons datafile, default None
--gt, --genetable, the gene table datafile, default None
--rh, --rel_height, the relative height at which the peak width is measured, default 0.4
--mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
--kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-```
-
-## Usage
-
-Here we provided the basic usage for each program.
-
-### wgd dmd
-
-**The delineation of whole paranome**
-```
-wgd dmd sequence
-``` 
-
-**The delineation of RBHs**
-```
-wgd dmd sequence1 sequence2
-```
-
-**The delineation of local MRBHs**
-```
-wgd dmd sequence1 sequence2 sequence3 -f sequence1
-```
-
-**The delineation of global MRBHs**
-```
-wgd dmd sequence1 sequence2 sequence3 -gm
-```
-
-**The delineation of orthogroups**
-```
-wgd dmd sequence1 sequence2 sequence3 -oi (option)
-```
-Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
-
-**The collinear coalescence inference of phylogeny**
-```
-wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
-```
-
-### wgd focus
-
-**The concatenation-based/coalescence-based phylogenetic inference**
-```
-wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
-```
-
-**The functional annotation of gene families**
-```
-wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
-```
-
-**The phylogenetic dating of WGDs**
-```
-wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
-```
-
-### wgd ksd
-
-**The construction of whole paranome *K*<sub>S</sub> age distribution**
-```
-wgd ksd families sequence
-```
-
-**The construction of orthologous *K*<sub>S</sub> age distribution**
-```
-wgd ksd families sequence1 sequence2
-```
-
-**The construction of *K*<sub>S</sub> age distribution with rate correction**
-```
-wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
-```
-
-### wgd mix
-
-**The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
-```
-wgd mix ksdata
-```
-
-### wgd peak
-
-**The search of crediable *K*<sub>S</sub> range used in WGD dating**
-```
-wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
-```
-Note that users can add the flag --heuristic to implement the heuristic search analysis
-
-### wgd syn
-
-**The intra-specific synteny inference**
-```
-wgd syn families gff
-```
-
-**The inter-specific synteny inference**
-```
-wgd syn families gff1 gff2
-```
-
-### wgd viz
-
-**The visualization of *K*<sub>S</sub> age distribution**
-```
-wgd viz -d ksdata
-```
-
-**The visualization of *K*<sub>S</sub> age distribution with rate correction**
-```
-wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
-```
-
-**The visualization of synteny**
-```
-wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
-```
-
-## Illustration
-
-We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
-
-The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
-
-First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
-
-```
-wgd dmd Aquilegia_coerulea
-wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
-```
-
-The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1.
-
-![](data/Aquilegia_coerulea.tsv.ksd.svg)
-
-## Citation
- 
-Please cite us at https://doi.org/10.1093/bioinformatics/bty915
-
-```
-Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
-
-Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
-```
-
-For citation of the tools used in wgd, please consult the documentation at
-https://wgd.readthedocs.io/en/latest/index.html#citation.
-
+Metadata-Version: 2.1
+Name: wgd
+Version: 2.0.13
+Summary: wgd
+Home-page: http://github.com/heche-psb/wgd
+Author: Hengchi Chen
+Author-email: heche@psb.vib-ugent.be
+License: GPL
+Description: <div align="center">
+        
+        # `wgd v2` : a suite tool of WGD inference and timing
+        
+        [![Build Status](https://app.travis-ci.com/heche-psb/wgd.svg?branch=phylodating)](https://travis-ci.com/heche-psb/wgd)
+        
+        **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
+        
+        [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
+        
+        [**Introduction**](#Introduction) | 
+        [**Installation**](#Installation) | 
+        [**Parameters**](#Parameters) | 
+        [**Usage**](#Usage) | 
+        [**Illustration**](#Illustration) |
+        [**Citation**](#Citation)
+        
+        </div>
+        
+        `wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
+        
+        ## Introduction
+        
+        Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
+        
+        The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
+        
+        ## Installation
+        
+        The easiest way to install `wgd v2` is using PYPI
+        
+        ```
+        pip install wgd
+        ```
+        
+        To install `wgd v2` in a virtual environment, the following command lines could be used.
+        
+        ```
+        git clone <wgd repo>
+        cd wgd
+        virtualenv -p=python3 ENV (or python3 -m venv ENV)
+        source ENV/bin/activate
+        pip install -r requirements.txt
+        pip install .
+        ```
+        
+        When met with permission problem in installation, please try the following command line.
+        
+        ```
+        pip install -e .
+        ```
+        
+        If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
+        
+        ```
+        export PATH="$PATH:~/.local/bin/wgd"
+        ```
+        
+        ## Parameters
+        
+        There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
+        
+        The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
+        ```
+        wgd dmd sequences (option)
+        --------------------------------------------------------------------------------
+        -o, --outdir, the output directory, default wgd_dmd
+        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+        -c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
+        -I, --inflation, the inflation factor for MCL program, default 2.0
+        -e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
+        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+        -f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
+        -ap, --anchorpoints, the anchor points data file, default None
+        -coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
+        -sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
+        -le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
+        -gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
+        -kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
+        -kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
+        -gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
+        -n, --nthreads, the number of threads to use, default 4
+        -oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
+        -oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
+        -gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
+        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
+        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+        -mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
+        -ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
+        -am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
+        -sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
+        -fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
+        -cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
+        -te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
+        -bs, --bins, the number of bins divided in gene length normalization, default 100
+        -np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
+        -nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
+        -bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
+        -bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
+        -bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
+        ```
+        
+        The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
+        ```
+        wgd focus families sequences (option)
+        --------------------------------------------------------------------------------
+        -o, --outdir, the output directory, default wgd_focus
+        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+        -n, --nthreads, the number of threads to use, default 4
+        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+        -a, --aligner, which alignment program to use, default mafft
+        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
+        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+        --concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
+        --coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
+        -sp, --speciestree, species tree darafile for dating, default None
+        -d, --dating, which molecular dating program to use, default none
+        -ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
+        -ns, --nsites, the nsites information for r8s dating, default None
+        -ot, --outgroup, the outgroup information for r8s dating, default None
+        -pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
+        -am, --aamodel, which protein model to be used in mcmctree, default poisson
+        -ks, flag option, whether to initiate Ks analysis
+        --annotation, which annotation program to use, default none
+        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+        -ed, --eggnogdata, the eggnog annotation datafile, default None
+        --pfam, which option to use for pfam annotation, default none
+        --dmnb, the diamond database for annotation, default None
+        --hmm, the HMM profile for annotation, default None
+        --evalue, the e-value cut-off for annotation, default 1e-10
+        --exepath, the path to the interproscan executable, default None
+        -f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
+         -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
+        -cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
+        --beastlgjar, the path to beastLG.jar, default None
+        --beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
+        --protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
+        ```
+        
+        The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
+        ```
+        wgd ksd families sequences (option)
+        --------------------------------------------------------------------------------
+        -o, --outdir, the output directory, default wgd_ksd
+        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+        -n, --nthreads, the number of threads to use, default 4
+        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
+        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+        ```
+        
+        The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
+        ```
+        wgd mix ks_datafile (option)
+        --------------------------------------------------------------------------------
+        -f, --filters, the cutoff alignment length, default 300
+        -r, --ks_range, the Ks range to be considered, default (0.005, 3)
+        -b, --bins, the number of bins in Ks distribution, default 50
+        -o, --outdir, the output directory, default wgd_mix
+        --method, which mixture model to use, default gmm
+        -n, --components, the range of the number of components to fit, default (1, 4)
+        -g, --gamma, the gamma parameter for bgmm models, default 0.001
+        -ni, --n_init, the number of k-means initializations, default 200
+        -mi, --max_iter, the maximum number of iterations, default 1000
+        ```
+        
+        The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
+        ```
+        wgd peak ks_datafile (option)
+        --------------------------------------------------------------------------------
+        -ap, --anchorpoints, the anchor points datafile, default None
+        -sm, --segments, the segments datafile, default None
+        -le, --listelements, the listsegments datafile, default None 
+        -mp, --multipliconpairs, the multipliconpairs datafile, default None
+        -o, --outdir, the output directory, default wgd_peak
+        -af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
+        -r, --ksrange, range of Ks to be analyzed, default (0, 5)
+        -bw, --bin_width, bandwidth of Ks distribution, default 0.1
+        -ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
+        -m, --method, which mixture model to use, default gmm
+        --seed, random seed given to initialization, default 2352890
+        -ei, --em_iter, the number of EM iterations to perform, default 200
+        -ni, --n_init, the number of k-means initializations, default 200
+        -n, --components, the range of the number of components to fit, default (1, 4)
+        --boots, the number of bootstrap replicates of kde, default 200
+        --weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
+        -p, --plot, the plotting method to be used, default identical
+        -bm, --bw_method, the bandwidth method to be used, default silverman
+        --n_medoids, the number of medoids to fit, default 2
+        -km, --kdemethod, the kde method to be used, default scipy
+        --n_clusters, the number of clusters to plot Elbow loss function, default 5
+        --kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
+        -gd, --guide, the regime residing anchors, default: segment
+        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+        -kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
+        -f, --family, the family to filter Ks upon, default None
+        --manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
+        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+        --ci, the confidence level of log-normal distribution to date, default 95
+        --hdr, the highest densidy region (HDR) in a given distribution to date, default 95
+        --heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
+        -kc, --kscutoff, the Ks saturation cutoff in dating, default 5
+        ```
+        
+        The program `wgd syn` can realize the intra- and inter-specific synteny inference.
+        ```
+        wgd syn families gffs (option)
+        --------------------------------------------------------------------------------
+        -ks, --ks_distribution, ks distribution datafile, default None
+        -o, --outdir, the output directory, default wgd_syn
+        -f, --feature, the feature for parsing gene IDs from GFF files, default gene
+        -a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
+        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+        -ms, --maxsize, the maximum family size to include, default 200
+        -r, --ks_range, the Ks range in colored dotplot, default (0, 5)
+        --iadhore_options, the parameter setting in iadhore, default 
+        -ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
+        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+        ```
+        
+        The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
+        ```
+        wgd viz (option)
+        --------------------------------------------------------------------------------
+        -d, --datafile, the Ks datafile, default None
+        -o, --outdir, the output directory, default wgd_viz
+        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+        -gs, --gsmap, the gene name-species name map, default None
+        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+        -pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
+        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+        -iter, --em_iterations, the maximum EM iterations, default 200
+        -init, --em_initializations, the maximum EM initializations, default 200
+        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+        -sm, --segments, the segments data file, default None
+        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+        -ms, --maxsize, the maximum family size to include, default 200
+        -ap, --anchorpoints, the anchor points datafile, default None
+        -mt, --multiplicon, the multiplicons datafile, default None
+        -gt, --genetable, the gene table datafile, default None
+        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+        ```
+        
+        ## Usage
+        
+        Here we provided the basic usage for each program.
+        
+        ### wgd dmd
+        
+        **The delineation of whole paranome**
+        ```
+        wgd dmd sequence
+        ``` 
+        
+        **The delineation of RBHs**
+        ```
+        wgd dmd sequence1 sequence2
+        ```
+        
+        **The delineation of local MRBHs**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -f sequence1
+        ```
+        
+        **The delineation of global MRBHs**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -gm
+        ```
+        
+        **The delineation of orthogroups**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -oi (option)
+        ```
+        Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
+        
+        **The collinear coalescence inference of phylogeny**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
+        ```
+        
+        ### wgd focus
+        
+        **The concatenation-based/coalescence-based phylogenetic inference**
+        ```
+        wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
+        ```
+        
+        **The functional annotation of gene families**
+        ```
+        wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
+        ```
+        
+        **The phylogenetic dating of WGDs**
+        ```
+        wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
+        ```
+        
+        ### wgd ksd
+        
+        **The construction of whole paranome *K*<sub>S</sub> age distribution**
+        ```
+        wgd ksd families sequence
+        ```
+        
+        **The construction of orthologous *K*<sub>S</sub> age distribution**
+        ```
+        wgd ksd families sequence1 sequence2
+        ```
+        
+        **The construction of *K*<sub>S</sub> age distribution with rate correction**
+        ```
+        wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
+        ```
+        
+        ### wgd mix
+        
+        **The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
+        ```
+        wgd mix ksdata
+        ```
+        
+        ### wgd peak
+        
+        **The search of crediable *K*<sub>S</sub> range used in WGD dating**
+        ```
+        wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
+        ```
+        Note that users can add the flag --heuristic to implement the heuristic search analysis
+        
+        ### wgd syn
+        
+        **The intra-specific synteny inference**
+        ```
+        wgd syn families gff
+        ```
+        
+        **The inter-specific synteny inference**
+        ```
+        wgd syn families gff1 gff2
+        ```
+        
+        ### wgd viz
+        
+        **The visualization of *K*<sub>S</sub> age distribution**
+        ```
+        wgd viz -d ksdata
+        ```
+        
+        **The visualization of *K*<sub>S</sub> age distribution with rate correction**
+        ```
+        wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
+        ```
+        
+        **The visualization of synteny**
+        ```
+        wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
+        ```
+        
+        ## Illustration
+        
+        We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
+        
+        The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
+        
+        First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
+        
+        ```
+        wgd dmd Aquilegia_coerulea
+        wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
+        ```
+        
+        The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
+        
+        ![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
+        
+        We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
+        
+        ```
+        wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+        ```
+        
+        As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
+        
+        ![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
+        
+        The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
+        
+        ![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
+        
+        The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
+        
+        ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
+        
+        A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
+        
+        ![](data/Syndepth.svg)
+        
+        We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
+        
+        ```
+        wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+        ```
+        
+        The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
+        
+        ![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
+        
+        Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
+        
+        ```
+        wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
+        ```
+        
+        The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
+        
+        ![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
+        
+        Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis.
+        
+        ## Citation
+         
+        Please cite us at https://doi.org/10.1093/bioinformatics/bty915
+        
+        ```
+        Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
+        
+        Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
+        ```
+        
+        For citation of the tools used in wgd, please consult the documentation at
+        https://wgd.readthedocs.io/en/latest/index.html#citation.
+        
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `wgd-2.0.12/cli.py` & `wgd-2.0.13/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -801,11 +801,11 @@
     logging.info("Writing component-wise probabilities to file")
     new_df = get_component_probabilities(df, best)
     new_df.round(5).to_csv(os.path.join(
             output_dir, "ks_{}.tsv".format(method)), sep="\t")
 
 
 if __name__ == '__main__':
-    start = time.time()
+    start = timer()
     cli()
-    end = time.time()
+    end = timer()
     logging.info("Total run time: {}s".format(int(end-start)))
```

### Comparing `wgd-2.0.12/setup.py` & `wgd-2.0.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='wgd',
-    version='2.0.12',
+    version='2.0.13',
     packages=['wgd'],
     url='http://github.com/heche-psb/wgd',
     license='GPL',
     author='Hengchi Chen',
     author_email='heche@psb.vib-ugent.be',
     description='wgd',
     long_description=long_description,
```

### Comparing `wgd-2.0.12/test/test_core.py` & `wgd-2.0.13/test/test_core.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.12/wgd/__init__.py` & `wgd-2.0.13/wgd/__init__.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.12/wgd/beast.py` & `wgd-2.0.13/wgd/beast.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.12/wgd/cluster.py` & `wgd-2.0.13/wgd/cluster.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.12/wgd/codeml.py` & `wgd-2.0.13/wgd/codeml.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.12/wgd/core.py` & `wgd-2.0.13/wgd/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1688,15 +1688,15 @@
         #for e in res: print(e.shape)
         #for j,e in zip(range(i, len(s)),res):
         #    print(type(e))
         #    print(e)
         #    s[i].dmd_hits[s[j].prefix] = e
         for j in range(i, len(s)): back_dmdhits(i,j,s,eval)
         s[i].rndmd_hit()
-    memory_reporter()
+    #memory_reporter()
     for i in range(1, len(s)):
         s[0].merge_dmd_hits(s[i])
         s[0].merge_seq(s[i])
     s[0].get_para_skip_dmd(inflation=inflation, eval=eval)
     prefix = s[0].prefix
     s[0].prefix = 'Orthologues'
     txtf = s[0].write_paranome(True)
@@ -1714,15 +1714,15 @@
     s0_orig = copy.deepcopy(s[0])
     if concat:
         sgidmaps = {}
         for x in s : sgidmaps.update(x.spgenemap())
         Concat_cdsf = concatcdss(sequences,outdir)
         ss = SequenceData(Concat_cdsf, out_path=outdir, tmp_path=tmpdir, to_stop=to_stop, cds=cds, cscore=cscore, threads=nthreads, bins=bins, normalizedpercent=normalizedpercent,nonormalization=nonormalization)
         logging.info("tmpdir = {} for {}".format(ss.tmp_path,ss.prefix))
-        memory_reporter()
+        #memory_reporter()
         ss.get_paranome(inflation=inflation, eval=eval, savememory = True,sgidmaps = sgidmaps)
         txtf = ss.write_paranome(True)
     #Concat_cdsf = concatcdss(sequences,outdir)
     #ss = SequenceData(Concat_cdsf, out_path=outdir, tmp_path=tmpdir, to_stop=to_stop, cds=cds, cscore=cscore)
     else: ss,txtf = ortho_infer_mul(s,nthreads,eval,inflation,False)
     #logging.info("tmpdir = {} for {}".format(ss.tmp_path,ss.prefix))
     #ss.get_paranome(inflation=inflation, eval=eval)
@@ -1997,15 +1997,15 @@
     frep = _mkdir(os.path.join(outdir,'Orthologues_Sequence_Representives'))
     fsog = _mkdir(os.path.join(outdir,'Orthologues_Single_Copy'))
     txt = pd.read_csv(txtf,header = None,index_col=0,sep='\t')
     y= lambda x: {j:sgmaps[j] for j in x}
     fams_df,counts_df,reps_df = [],[],[]
     sh = txt.shape[0]
     gsmaps = [y(txt.iloc[i,0].split(', ')) for i in range(sh)]
-    memory_reporter()
+    #memory_reporter()
     #Parallel(n_jobs=nthreads)(delayed(seqdict)(gsmaps[i],ss,i,ftmp) for i in range(sh))
     #for i in range(sh):
     #r = Parallel(n_jobs=nthreads,backend='multiprocessing',verbose=11,batch_size=1000)(delayed(first_tsv_genecounts)(gsmaps[i],slist,ss,msogcut) for i in range(sh))
     for i in range(sh):
         fam_df,count_df,rep_df = first_tsv_genecounts(gsmaps[i],slist,ss,msogcut)
         fams_df.append(fam_df)
         counts_df.append(count_df)
@@ -2035,15 +2035,15 @@
     fams_coc.to_csv(fname_fam,header = True,index =True,sep = '\t')
     counts_coc.to_csv(fname_count,header = True,index =True,sep = '\t')
     reps_coc.to_csv(fname_rep,header = True,index =True,sep = '\t')
     logging.info("In total {} orthologous families delineated".format(counts_coc.shape[0]))
     mu,mo,sg=(counts_coc[counts_coc['CopyType']==i].shape[0] for i in ['multi-copy','mostly single-copy','single-copy'])
     logging.info("with {0} multi-copy, {1} mostly single-copy, {2} single-copy".format(mu,mo,sg))
     Parallel(n_jobs=nthreads,backend='multiprocessing',verbose=11,batch_size=1000)(delayed(sgdict)(gsmaps[i],slist,ss,ftmp,frep,fsog,i,msogcut) for i in range(sh))
-    memory_reporter()
+    #memory_reporter()
     if getsog:
         fnest = _mkdir(os.path.join(outdir,'Orthologues_Nested_Single_Copy'))
         tree_famsf,tree_fams,nested_dfs,aln_fam_is = [],{},[],[]
         yc = lambda x: os.path.join(ftmp,'cds',"GF{:0>8}.cds".format(x+1))
         yp = lambda x: os.path.join(ftmp,'pep',"GF{:0>8}.pep".format(x+1))
         #yco = lambda x,y: counts_df[x].loc[0,y]
         yco = lambda x,y: counts_coc.loc["GF{:0>8}".format(x+1),y]
@@ -2057,15 +2057,15 @@
             nested_coc = pd.concat(nested_dfs,ignore_index=True).set_index('NestedSOG')
             nested_coc.to_csv(fname_nest,header = True,index =True,sep = '\t')
             logging.info("{} nested single-copy families delineated".format(nested_coc.shape[0]))
             nfs = list(nested_coc.index)
             nfs_count = {i:nfs.count(i) for i in set(nfs)}
             getnestedfasta(fnest,nested_coc,ss,nfs_count)
         else: logging.info("No nested single-copy families delineated")
-        memory_reporter()
+        #memory_reporter()
     if testsog: unbiasedsog(fsog,fams_coc,counts_coc,nthreads,s,outdir,eval,s0_orig)
 
 def get_sog_multiplicons(df,species_num):
     sp_counted = df.groupby(["multiplicon"])["genome"].aggregate(lambda x: len(set(x)))
     level = df.groupby(["multiplicon"])["genome"].aggregate(lambda x: len(x))
     FullCoverage_Multiplicons = sp_counted[sp_counted==species_num]
     RightLevel_Multiplicons = level[level==species_num]
```

### Comparing `wgd-2.0.12/wgd/mcmctree.py` & `wgd-2.0.13/wgd/mcmctree.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.12/wgd/mix.py` & `wgd-2.0.13/wgd/mix.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.12/wgd/peak.py` & `wgd-2.0.13/wgd/peak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1471,14 +1471,15 @@
 def add_seg(df,listelement,multipliconpairs,segment):
     #Here the df should be Ks 0-5 filter
     #It hasn't to be ap in listelement note that a same pair of syntelogs can be in different multiplicon
     mp = pd.read_csv(multipliconpairs, sep="\t", index_col=0)
     if len(mp.columns) == 5: mp = mp.drop(columns=['gene_y']).rename(columns = {'gene_x':'gene_y'}).rename(columns = {'Unnamed: 2':'gene_x'})
     mp = mp.loc[:,['multiplicon','gene_x','gene_y']]
     mp.loc[:,['pair']] = ["__".join(sorted([x,y])) for x,y in zip(list(mp['gene_x']),list(mp['gene_y']))]
+    mp = mp.drop_duplicates(subset=['pair'])
     mp.loc[:,['id']] = [i for i in range(mp.shape[0])]
     #mp= mp.drop_duplicates(subset=['pair']) #Here the same gene pair can be in different multiplicon
     df_seg = pd.read_csv(segment,header=0,index_col=None,sep='\t').rename(columns = {'id':'segment'}).loc[:,['segment','multiplicon']]
     df_le = pd.read_csv(listelement,header=0,index_col=0,sep='\t').merge(df_seg,on='segment').rename(columns = {'multiplicon':'multiplicon_x'}).loc[:,['segment','multiplicon_x','gene']]
     #mp_segment_pools = {mt:list(set(df_seg[df_seg['multiplicon']==mt]['segment'])) for mt in df_seg['multiplicon']}
     #segment_gene_pools = {sg:list(set(df_le[df_le['segment']==sg]['gene'])) for sg in df_le['segment']}
     df_mp_le = mp.merge(df_le,left_on='gene_x',right_on='gene')
```

### Comparing `wgd-2.0.12/wgd/syn.py` & `wgd-2.0.13/wgd/syn.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.12/wgd/utils.py` & `wgd-2.0.13/wgd/utils.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.12/wgd/viz.py` & `wgd-2.0.13/wgd/viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -712,30 +712,32 @@
     """
     Make a figure of node-weighted histograms for multiple distributions and
     variables. Returns the figure object.
     
     !!! note: Assumes the data frames are filtered as desired. 
     """
     ndists = len(args)
-    alphas = alphas or list(np.linspace(0.2, 1, ndists))
-    colors = colors or ['black'] * ndists 
+    #alphas = alphas or list(np.linspace(0.2, 1, ndists))
+    #colors = colors or ['black'] * ndists 
+    colors = ['gray','green'] if ndists == 2 else ['gray']
     # assemble panels
     keys = ["dS", "dS", "dN", "dN/dS"]
     np.seterr(divide='ignore')
     funs = [lambda x: x, np.log10, np.log10, np.log10]
     fig, axs = plt.subplots(2, 2)
-    for (c, a, dist) in zip(colors, alphas, args):
+    #for (c, a, dist) in zip(colors, alphas, args):
+    for (c, dist) in zip(colors, args):
         for ax, k, f in zip(axs.flatten(), keys, funs):
             w = node_weights(dist)
             x = f(dist[k])
             y = x[np.isfinite(x)]
             w = w[np.isfinite(x)]
-            if funs[0] == f: ax.hist(y, bins = np.arange(0, 5.1, 0.1), weights=w, color=c, alpha=a, rwidth=0.8)
-            if funs[1] == f or funs[2] == f: ax.hist(y, bins = np.arange(-4, 1.1, 0.1), weights=w, color=c, alpha=a, rwidth=0.8)
-            else: ax.hist(y, weights=w, color=c, alpha=a, rwidth=0.8,**kwargs)
+            if funs[0] == f: ax.hist(y, bins = np.arange(0, 5.1, 0.1), weights=w, color=c, alpha=1, rwidth=0.8)
+            if funs[1] == f or funs[2] == f: ax.hist(y, bins = np.arange(-4, 1.1, 0.1), weights=w, color=c, alpha=1, rwidth=0.8)
+            else: ax.hist(y, weights=w, color=c, alpha=1, rwidth=0.8,**kwargs)
             xlabel = _labels[k]
             if f == np.log10:
                 xlabel = "$\log_{10}" + xlabel[1:-1] + "$"
             ax.set_xlabel(xlabel)
     axs[0,0].set_ylabel(ylabel)
     axs[1,0].set_ylabel(ylabel)
     axs[0,0].set_xticks([0,1,2,3,4,5])
```

### Comparing `wgd-2.0.12/wgd.egg-info/PKG-INFO` & `wgd-2.0.13/wgd.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,412 +1,456 @@
 Metadata-Version: 2.1
 Name: wgd
-Version: 2.0.12
+Version: 2.0.13
 Summary: wgd
 Home-page: http://github.com/heche-psb/wgd
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
+Description: <div align="center">
+        
+        # `wgd v2` : a suite tool of WGD inference and timing
+        
+        [![Build Status](https://app.travis-ci.com/heche-psb/wgd.svg?branch=phylodating)](https://travis-ci.com/heche-psb/wgd)
+        
+        **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
+        
+        [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
+        
+        [**Introduction**](#Introduction) | 
+        [**Installation**](#Installation) | 
+        [**Parameters**](#Parameters) | 
+        [**Usage**](#Usage) | 
+        [**Illustration**](#Illustration) |
+        [**Citation**](#Citation)
+        
+        </div>
+        
+        `wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
+        
+        ## Introduction
+        
+        Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
+        
+        The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
+        
+        ## Installation
+        
+        The easiest way to install `wgd v2` is using PYPI
+        
+        ```
+        pip install wgd
+        ```
+        
+        To install `wgd v2` in a virtual environment, the following command lines could be used.
+        
+        ```
+        git clone <wgd repo>
+        cd wgd
+        virtualenv -p=python3 ENV (or python3 -m venv ENV)
+        source ENV/bin/activate
+        pip install -r requirements.txt
+        pip install .
+        ```
+        
+        When met with permission problem in installation, please try the following command line.
+        
+        ```
+        pip install -e .
+        ```
+        
+        If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
+        
+        ```
+        export PATH="$PATH:~/.local/bin/wgd"
+        ```
+        
+        ## Parameters
+        
+        There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
+        
+        The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
+        ```
+        wgd dmd sequences (option)
+        --------------------------------------------------------------------------------
+        -o, --outdir, the output directory, default wgd_dmd
+        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+        -c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
+        -I, --inflation, the inflation factor for MCL program, default 2.0
+        -e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
+        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+        -f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
+        -ap, --anchorpoints, the anchor points data file, default None
+        -coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
+        -sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
+        -le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
+        -gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
+        -kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
+        -kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
+        -gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
+        -n, --nthreads, the number of threads to use, default 4
+        -oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
+        -oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
+        -gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
+        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
+        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+        -mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
+        -ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
+        -am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
+        -sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
+        -fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
+        -cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
+        -te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
+        -bs, --bins, the number of bins divided in gene length normalization, default 100
+        -np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
+        -nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
+        -bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
+        -bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
+        -bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
+        ```
+        
+        The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
+        ```
+        wgd focus families sequences (option)
+        --------------------------------------------------------------------------------
+        -o, --outdir, the output directory, default wgd_focus
+        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+        -n, --nthreads, the number of threads to use, default 4
+        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+        -a, --aligner, which alignment program to use, default mafft
+        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
+        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+        --concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
+        --coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
+        -sp, --speciestree, species tree darafile for dating, default None
+        -d, --dating, which molecular dating program to use, default none
+        -ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
+        -ns, --nsites, the nsites information for r8s dating, default None
+        -ot, --outgroup, the outgroup information for r8s dating, default None
+        -pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
+        -am, --aamodel, which protein model to be used in mcmctree, default poisson
+        -ks, flag option, whether to initiate Ks analysis
+        --annotation, which annotation program to use, default none
+        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+        -ed, --eggnogdata, the eggnog annotation datafile, default None
+        --pfam, which option to use for pfam annotation, default none
+        --dmnb, the diamond database for annotation, default None
+        --hmm, the HMM profile for annotation, default None
+        --evalue, the e-value cut-off for annotation, default 1e-10
+        --exepath, the path to the interproscan executable, default None
+        -f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
+         -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
+        -cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
+        --beastlgjar, the path to beastLG.jar, default None
+        --beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
+        --protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
+        ```
+        
+        The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
+        ```
+        wgd ksd families sequences (option)
+        --------------------------------------------------------------------------------
+        -o, --outdir, the output directory, default wgd_ksd
+        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+        -n, --nthreads, the number of threads to use, default 4
+        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
+        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+        ```
+        
+        The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
+        ```
+        wgd mix ks_datafile (option)
+        --------------------------------------------------------------------------------
+        -f, --filters, the cutoff alignment length, default 300
+        -r, --ks_range, the Ks range to be considered, default (0.005, 3)
+        -b, --bins, the number of bins in Ks distribution, default 50
+        -o, --outdir, the output directory, default wgd_mix
+        --method, which mixture model to use, default gmm
+        -n, --components, the range of the number of components to fit, default (1, 4)
+        -g, --gamma, the gamma parameter for bgmm models, default 0.001
+        -ni, --n_init, the number of k-means initializations, default 200
+        -mi, --max_iter, the maximum number of iterations, default 1000
+        ```
+        
+        The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
+        ```
+        wgd peak ks_datafile (option)
+        --------------------------------------------------------------------------------
+        -ap, --anchorpoints, the anchor points datafile, default None
+        -sm, --segments, the segments datafile, default None
+        -le, --listelements, the listsegments datafile, default None 
+        -mp, --multipliconpairs, the multipliconpairs datafile, default None
+        -o, --outdir, the output directory, default wgd_peak
+        -af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
+        -r, --ksrange, range of Ks to be analyzed, default (0, 5)
+        -bw, --bin_width, bandwidth of Ks distribution, default 0.1
+        -ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
+        -m, --method, which mixture model to use, default gmm
+        --seed, random seed given to initialization, default 2352890
+        -ei, --em_iter, the number of EM iterations to perform, default 200
+        -ni, --n_init, the number of k-means initializations, default 200
+        -n, --components, the range of the number of components to fit, default (1, 4)
+        --boots, the number of bootstrap replicates of kde, default 200
+        --weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
+        -p, --plot, the plotting method to be used, default identical
+        -bm, --bw_method, the bandwidth method to be used, default silverman
+        --n_medoids, the number of medoids to fit, default 2
+        -km, --kdemethod, the kde method to be used, default scipy
+        --n_clusters, the number of clusters to plot Elbow loss function, default 5
+        --kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
+        -gd, --guide, the regime residing anchors, default: segment
+        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+        -kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
+        -f, --family, the family to filter Ks upon, default None
+        --manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
+        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+        --ci, the confidence level of log-normal distribution to date, default 95
+        --hdr, the highest densidy region (HDR) in a given distribution to date, default 95
+        --heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
+        -kc, --kscutoff, the Ks saturation cutoff in dating, default 5
+        ```
+        
+        The program `wgd syn` can realize the intra- and inter-specific synteny inference.
+        ```
+        wgd syn families gffs (option)
+        --------------------------------------------------------------------------------
+        -ks, --ks_distribution, ks distribution datafile, default None
+        -o, --outdir, the output directory, default wgd_syn
+        -f, --feature, the feature for parsing gene IDs from GFF files, default gene
+        -a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
+        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+        -ms, --maxsize, the maximum family size to include, default 200
+        -r, --ks_range, the Ks range in colored dotplot, default (0, 5)
+        --iadhore_options, the parameter setting in iadhore, default 
+        -ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
+        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+        ```
+        
+        The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
+        ```
+        wgd viz (option)
+        --------------------------------------------------------------------------------
+        -d, --datafile, the Ks datafile, default None
+        -o, --outdir, the output directory, default wgd_viz
+        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+        -gs, --gsmap, the gene name-species name map, default None
+        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+        -pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
+        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+        -iter, --em_iterations, the maximum EM iterations, default 200
+        -init, --em_initializations, the maximum EM initializations, default 200
+        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+        -sm, --segments, the segments data file, default None
+        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+        -ms, --maxsize, the maximum family size to include, default 200
+        -ap, --anchorpoints, the anchor points datafile, default None
+        -mt, --multiplicon, the multiplicons datafile, default None
+        -gt, --genetable, the gene table datafile, default None
+        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+        ```
+        
+        ## Usage
+        
+        Here we provided the basic usage for each program.
+        
+        ### wgd dmd
+        
+        **The delineation of whole paranome**
+        ```
+        wgd dmd sequence
+        ``` 
+        
+        **The delineation of RBHs**
+        ```
+        wgd dmd sequence1 sequence2
+        ```
+        
+        **The delineation of local MRBHs**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -f sequence1
+        ```
+        
+        **The delineation of global MRBHs**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -gm
+        ```
+        
+        **The delineation of orthogroups**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -oi (option)
+        ```
+        Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
+        
+        **The collinear coalescence inference of phylogeny**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
+        ```
+        
+        ### wgd focus
+        
+        **The concatenation-based/coalescence-based phylogenetic inference**
+        ```
+        wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
+        ```
+        
+        **The functional annotation of gene families**
+        ```
+        wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
+        ```
+        
+        **The phylogenetic dating of WGDs**
+        ```
+        wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
+        ```
+        
+        ### wgd ksd
+        
+        **The construction of whole paranome *K*<sub>S</sub> age distribution**
+        ```
+        wgd ksd families sequence
+        ```
+        
+        **The construction of orthologous *K*<sub>S</sub> age distribution**
+        ```
+        wgd ksd families sequence1 sequence2
+        ```
+        
+        **The construction of *K*<sub>S</sub> age distribution with rate correction**
+        ```
+        wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
+        ```
+        
+        ### wgd mix
+        
+        **The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
+        ```
+        wgd mix ksdata
+        ```
+        
+        ### wgd peak
+        
+        **The search of crediable *K*<sub>S</sub> range used in WGD dating**
+        ```
+        wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
+        ```
+        Note that users can add the flag --heuristic to implement the heuristic search analysis
+        
+        ### wgd syn
+        
+        **The intra-specific synteny inference**
+        ```
+        wgd syn families gff
+        ```
+        
+        **The inter-specific synteny inference**
+        ```
+        wgd syn families gff1 gff2
+        ```
+        
+        ### wgd viz
+        
+        **The visualization of *K*<sub>S</sub> age distribution**
+        ```
+        wgd viz -d ksdata
+        ```
+        
+        **The visualization of *K*<sub>S</sub> age distribution with rate correction**
+        ```
+        wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
+        ```
+        
+        **The visualization of synteny**
+        ```
+        wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
+        ```
+        
+        ## Illustration
+        
+        We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
+        
+        The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
+        
+        First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
+        
+        ```
+        wgd dmd Aquilegia_coerulea
+        wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
+        ```
+        
+        The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
+        
+        ![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
+        
+        We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
+        
+        ```
+        wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+        ```
+        
+        As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
+        
+        ![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
+        
+        The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
+        
+        ![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
+        
+        The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
+        
+        ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
+        
+        A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
+        
+        ![](data/Syndepth.svg)
+        
+        We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
+        
+        ```
+        wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+        ```
+        
+        The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
+        
+        ![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
+        
+        Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
+        
+        ```
+        wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
+        ```
+        
+        The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
+        
+        ![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
+        
+        Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis.
+        
+        ## Citation
+         
+        Please cite us at https://doi.org/10.1093/bioinformatics/bty915
+        
+        ```
+        Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
+        
+        Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
+        ```
+        
+        For citation of the tools used in wgd, please consult the documentation at
+        https://wgd.readthedocs.io/en/latest/index.html#citation.
+        
+        
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div align="center">
-
-# `wgd v2` : a suite tool of WGD inference and timing
-
-[![Build Status](https://app.travis-ci.com/heche-psb/wgd.svg?branch=phylodating)](https://travis-ci.com/heche-psb/wgd)
-
-**Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
-
-[**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
-
-[**Introduction**](#Introduction) | 
-[**Installation**](#Installation) | 
-[**Parameters**](#Parameters) | 
-[**Usage**](#Usage) | 
-[**Illustration**](#Illustration) |
-[**Citation**](#Citation)
-
-</div>
-
-`wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
-
-## Introduction
-
-Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
-
-The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
-
-## Installation
-
-The easiest way to install `wgd v2` is using PYPI
-
-```
-pip install wgd
-```
-
-To install `wgd v2` in a virtual environment, the following command lines could be used.
-
-```
-git clone <wgd repo>
-cd wgd
-virtualenv -p=python3 ENV (or python3 -m venv ENV)
-source ENV/bin/activate
-pip install -r requirements.txt
-pip install .
-```
-
-When met with permission problem in installation, please try the following command line.
-
-```
-pip install -e .
-```
-
-If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
-
-```
-export PATH="$PATH:~/.local/bin/wgd"
-```
-
-## Parameters
-
-There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
-
-The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
-```
-wgd dmd sequences (option)
---------------------------------------------------------------------------------
--o, --outdir, the output directory, default wgd_dmd
--t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
--c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
--I, --inflation, the inflation factor for MCL program, default 2.0
--e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
---to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
---cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
--f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
--ap, --anchorpoints, the anchor points data file, default None
--coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
--sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
--le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
--gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
--kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
--kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
--gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
--n, --nthreads, the number of threads to use, default 4
--oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
--oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
--gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
--tree, --tree_method, which gene tree inference program to invoke, default fasttree
--ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
--mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
--ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
--am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
--sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
--fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
--cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
--te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
--bs, --bins, the number of bins divided in gene length normalization, default 100
--np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
--nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
--bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
--bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
--bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
-```
-
-The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
-```
-wgd focus families sequences (option)
---------------------------------------------------------------------------------
--o, --outdir, the output directory, default wgd_focus
--t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
--n, --nthreads, the number of threads to use, default 4
---to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
---cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
---strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
--a, --aligner, which alignment program to use, default mafft
--tree, --tree_method, which gene tree inference program to invoke, default fasttree
--ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
---concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
---coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
--sp, --speciestree, species tree darafile for dating, default None
--d, --dating, which molecular dating program to use, default none
--ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
--ns, --nsites, the nsites information for r8s dating, default None
--ot, --outgroup, the outgroup information for r8s dating, default None
--pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
--am, --aamodel, which protein model to be used in mcmctree, default poisson
--ks, flag option, whether to initiate Ks analysis
---annotation, which annotation program to use, default none
---pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
--ed, --eggnogdata, the eggnog annotation datafile, default None
---pfam, which option to use for pfam annotation, default none
---dmnb, the diamond database for annotation, default None
---hmm, the HMM profile for annotation, default None
---evalue, the e-value cut-off for annotation, default 1e-10
---exepath, the path to the interproscan executable, default None
--f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
- -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
--cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
---beastlgjar, the path to beastLG.jar, default None
---beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
---protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
-```
-
-The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
-```
-wgd ksd families sequences (option)
---------------------------------------------------------------------------------
--o, --outdir, the output directory, default wgd_ksd
--t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
--n, --nthreads, the number of threads to use, default 4
---to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
---cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
---pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
---strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
--tree, --tree_method, which gene tree inference program to invoke, default fasttree
--sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
--sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
--rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
--or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
-```
-
-The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
-```
-wgd mix ks_datafile (option)
---------------------------------------------------------------------------------
--f, --filters, the cutoff alignment length, default 300
--r, --ks_range, the Ks range to be considered, default (0.005, 3)
--b, --bins, the number of bins in Ks distribution, default 50
--o, --outdir, the output directory, default wgd_mix
---method, which mixture model to use, default gmm
--n, --components, the range of the number of components to fit, default (1, 4)
--g, --gamma, the gamma parameter for bgmm models, default 0.001
--ni, --n_init, the number of k-means initializations, default 200
--mi, --max_iter, the maximum number of iterations, default 1000
-```
-
-The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
-```
-wgd peak ks_datafile (option)
---------------------------------------------------------------------------------
--ap, --anchorpoints, the anchor points datafile, default None
--sm, --segments, the segments datafile, default None
--le, --listelements, the listsegments datafile, default None 
--mp, --multipliconpairs, the multipliconpairs datafile, default None
--o, --outdir, the output directory, default wgd_peak
--af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
--r, --ksrange, range of Ks to be analyzed, default (0, 5)
--bw, --bin_width, bandwidth of Ks distribution, default 0.1
--ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
--m, --method, which mixture model to use, default gmm
---seed, random seed given to initialization, default 2352890
--ei, --em_iter, the number of EM iterations to perform, default 200
--ni, --n_init, the number of k-means initializations, default 200
--n, --components, the range of the number of components to fit, default (1, 4)
---boots, the number of bootstrap replicates of kde, default 200
---weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
--p, --plot, the plotting method to be used, default identical
--bm, --bw_method, the bandwidth method to be used, default silverman
---n_medoids, the number of medoids to fit, default 2
--km, --kdemethod, the kde method to be used, default scipy
---n_clusters, the number of clusters to plot Elbow loss function, default 5
---kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
--gd, --guide, the regime residing anchors, default: segment
--prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
--kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
--f, --family, the family to filter Ks upon, default None
---manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
--rh, --rel_height, the relative height at which the peak width is measured, default 0.4
---ci, the confidence level of log-normal distribution to date, default 95
---hdr, the highest densidy region (HDR) in a given distribution to date, default 95
---heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
--kc, --kscutoff, the Ks saturation cutoff in dating, default 5
-```
-
-The program `wgd syn` can realize the intra- and inter-specific synteny inference.
-```
-wgd syn families gffs (option)
---------------------------------------------------------------------------------
--ks, --ks_distribution, ks distribution datafile, default None
--o, --outdir, the output directory, default wgd_syn
--f, --feature, the feature for parsing gene IDs from GFF files, default gene
--a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
--ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
--ms, --maxsize, the maximum family size to include, default 200
--r, --ks_range, the Ks range in colored dotplot, default (0, 5)
---iadhore_options, the parameter setting in iadhore, default 
--ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
--mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
--kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-```
-
-The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
-```
-wgd viz (option)
---------------------------------------------------------------------------------
--d, --datafile, the Ks datafile, default None
--o, --outdir, the output directory, default wgd_viz
--sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
--gs, --gsmap, the gene name-species name map, default None
--sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
--pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
--rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
--or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
--iter, --em_iterations, the maximum EM iterations, default 200
--init, --em_initializations, the maximum EM initializations, default 200
--prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
--sm, --segments, the segments data file, default None
--ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
--ms, --maxsize, the maximum family size to include, default 200
--ap, --anchorpoints, the anchor points datafile, default None
--mt, --multiplicon, the multiplicons datafile, default None
--gt, --genetable, the gene table datafile, default None
--rh, --rel_height, the relative height at which the peak width is measured, default 0.4
--mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
--kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-```
-
-## Usage
-
-Here we provided the basic usage for each program.
-
-### wgd dmd
-
-**The delineation of whole paranome**
-```
-wgd dmd sequence
-``` 
-
-**The delineation of RBHs**
-```
-wgd dmd sequence1 sequence2
-```
-
-**The delineation of local MRBHs**
-```
-wgd dmd sequence1 sequence2 sequence3 -f sequence1
-```
-
-**The delineation of global MRBHs**
-```
-wgd dmd sequence1 sequence2 sequence3 -gm
-```
-
-**The delineation of orthogroups**
-```
-wgd dmd sequence1 sequence2 sequence3 -oi (option)
-```
-Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
-
-**The collinear coalescence inference of phylogeny**
-```
-wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
-```
-
-### wgd focus
-
-**The concatenation-based/coalescence-based phylogenetic inference**
-```
-wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
-```
-
-**The functional annotation of gene families**
-```
-wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
-```
-
-**The phylogenetic dating of WGDs**
-```
-wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
-```
-
-### wgd ksd
-
-**The construction of whole paranome *K*<sub>S</sub> age distribution**
-```
-wgd ksd families sequence
-```
-
-**The construction of orthologous *K*<sub>S</sub> age distribution**
-```
-wgd ksd families sequence1 sequence2
-```
-
-**The construction of *K*<sub>S</sub> age distribution with rate correction**
-```
-wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
-```
-
-### wgd mix
-
-**The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
-```
-wgd mix ksdata
-```
-
-### wgd peak
-
-**The search of crediable *K*<sub>S</sub> range used in WGD dating**
-```
-wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
-```
-Note that users can add the flag --heuristic to implement the heuristic search analysis
-
-### wgd syn
-
-**The intra-specific synteny inference**
-```
-wgd syn families gff
-```
-
-**The inter-specific synteny inference**
-```
-wgd syn families gff1 gff2
-```
-
-### wgd viz
-
-**The visualization of *K*<sub>S</sub> age distribution**
-```
-wgd viz -d ksdata
-```
-
-**The visualization of *K*<sub>S</sub> age distribution with rate correction**
-```
-wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
-```
-
-**The visualization of synteny**
-```
-wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
-```
-
-## Illustration
-
-We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
-
-The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
-
-First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
-
-```
-wgd dmd Aquilegia_coerulea
-wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
-```
-
-The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1.
-
-![](data/Aquilegia_coerulea.tsv.ksd.svg)
-
-## Citation
- 
-Please cite us at https://doi.org/10.1093/bioinformatics/bty915
-
-```
-Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
-
-Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
-```
-
-For citation of the tools used in wgd, please consult the documentation at
-https://wgd.readthedocs.io/en/latest/index.html#citation.
-
```

### Comparing `wgd-2.0.12/wgd.egg-info/requires.txt` & `wgd-2.0.13/wgd.egg-info/requires.txt`

 * *Files identical despite different names*

