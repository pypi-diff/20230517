# Comparing `tmp/sequana_demultiplex-1.2.1.tar.gz` & `tmp/sequana_demultiplex-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_demultiplex-1.2.1.tar", last modified: Fri Aug 12 06:10:08 2022, max compression
+gzip compressed data, was "dist/sequana_demultiplex-1.3.0.tar", last modified: Wed May 17 12:04:29 2023, max compression
```

## Comparing `sequana_demultiplex-1.2.1.tar` & `sequana_demultiplex-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11523 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8730 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/sequana_demultiplex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11523 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/sequana_demultiplex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/sequana_demultiplex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/sequana_demultiplex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/sequana_demultiplex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/sequana_demultiplex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/sequana_demultiplex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/sequana_demultiplex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/sequana_pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    17354 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/dag.png
--rw-r--r--   0 runner    (1001) docker     (121)     7096 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/demultiplex.rules
--rw-r--r--   0 runner    (1001) docker     (121)     8732 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/logo.png
--rwxr-xr-x   0 runner    (1001) docker     (121)     8427 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/main.py
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2937 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 06:10:08.000000 sequana_demultiplex-1.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/test/test_check_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-08-12 06:10:06.000000 sequana_demultiplex-1.2.1/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    12131 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9282 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    12131 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      745 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    17354 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/dag.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7372 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/demultiplex.rules
+-rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/logo.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8427 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/test/test_check_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/test/test_main.py
```

### Comparing `sequana_demultiplex-1.2.1/PKG-INFO` & `sequana_demultiplex-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 1.2
 Name: sequana_demultiplex
-Version: 1.2.1
+Version: 1.3.0
 Summary: Pipeline that runs bcl2fastq and creates additional plots within a Snakemake workflow
 Home-page: https://github.com/sequana/
 Author: cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
 Description: 
         .. image:: https://badge.fury.io/py/sequana-demultiplex.svg
              :target: https://pypi.python.org/pypi/sequana_demultiplex
         
-        .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
-            :target: http://joss.theoj.org/papers/10.21105/joss.00352
-            :alt: JOSS (journal of open source software) DOI
-        
         .. image:: https://github.com/sequana/demultiplex/actions/workflows/main.yml/badge.svg
            :target: https://github.com/sequana/demultiplex/actions/workflows/main.yml
         
+        .. image:: https://coveralls.io/repos/github/sequana/demultiplex/badge.svg?branch=main
+            :target: https://coveralls.io/github/sequana/demultiplex?branch=main
+        
+        .. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+            :target: https://pypi.python.org/pypi/sequana
+            :alt: Python 3.8 | 3.9 | 3.10
+        
+        .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+           :target: http://joss.theoj.org/papers/10.21105/joss.00352
+           :alt: JOSS (journal of open source software) DOI
         
         This is is the **demultiplex** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
         
         :Overview: Runs bcl2fastq on raw BCL data and creates plots to ease the QC validation
-        :Input: A valid Illumina base calling directory
+        :Input: A valid Illumina base calling directory and sample sheet file
         :Output: An HTML report, a set of PNG files and the expected FastQ files
         :Status: production
         :Wiki: https://github.com/sequana/demultiplex/wiki
         :Documentation: This README file, the Wiki from the github repository (link above) and https://sequana.readthedocs.io
         :Citation: Cokelaer et al, (2017), 'Sequana': a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI https://doi:10.21105/joss.00352
         
         
@@ -74,15 +80,15 @@
         ~~~~~~~~~~~~
         
         This pipeline requires the following third-party tool(s):
         
         - bcl2fastq 2.20.0
         
         This software has an end-user license agreement (EULA). Given the EULA details
-        of this software, it cannot be distributed by us but only by Illumina.
+        of this software, it cannot be distributed according to ` Illumina license <https://support.illumina.com/content/dam/illumina-support/documents/downloads/software/bcl2fastq/bcl2fastq2-v2-20-eula.pdf>`_
         Therefore, you should install it yourself. On cluster facility, you may ask to
         your system administator. For instance::
         
             module load bcl2fastq/2.20.0
         
         For the same reason you cannot find it on community such as bioconda or docker (aug 2020).
         
@@ -116,14 +122,15 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= =======================================================================
         Version   Description
         ========= =======================================================================
+        1.3.0     * use latest sequana-wrappers to benefit and graphivz apptainer
         1.2.1     * Update CI action and use new sequana_pipetools v0.9.0
         1.2.0     * stable release with cleanup of the setup and README
         1.1.3     * add the --mars-seq option that fills the config automatically
         1.1.2     * fix the none_and_force merging strategy option
         1.1.1     * fix a regression bug
         1.1.0     * Uses new sequana-wrappers repository
         1.0.5     * Fix regression bug to cope with new snakemake API
```

### Comparing `sequana_demultiplex-1.2.1/README.rst` & `sequana_demultiplex-1.3.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 
 .. image:: https://badge.fury.io/py/sequana-demultiplex.svg
      :target: https://pypi.python.org/pypi/sequana_demultiplex
 
-.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
-    :target: http://joss.theoj.org/papers/10.21105/joss.00352
-    :alt: JOSS (journal of open source software) DOI
-
 .. image:: https://github.com/sequana/demultiplex/actions/workflows/main.yml/badge.svg
    :target: https://github.com/sequana/demultiplex/actions/workflows/main.yml
 
+.. image:: https://coveralls.io/repos/github/sequana/demultiplex/badge.svg?branch=main
+    :target: https://coveralls.io/github/sequana/demultiplex?branch=main
+
+.. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+    :target: https://pypi.python.org/pypi/sequana
+    :alt: Python 3.8 | 3.9 | 3.10
+
+.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+   :target: http://joss.theoj.org/papers/10.21105/joss.00352
+   :alt: JOSS (journal of open source software) DOI
 
 This is is the **demultiplex** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
 
 :Overview: Runs bcl2fastq on raw BCL data and creates plots to ease the QC validation
-:Input: A valid Illumina base calling directory
+:Input: A valid Illumina base calling directory and sample sheet file
 :Output: An HTML report, a set of PNG files and the expected FastQ files
 :Status: production
 :Wiki: https://github.com/sequana/demultiplex/wiki
 :Documentation: This README file, the Wiki from the github repository (link above) and https://sequana.readthedocs.io
 :Citation: Cokelaer et al, (2017), 'Sequana': a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI https://doi:10.21105/joss.00352
 
 
@@ -64,15 +70,15 @@
 ~~~~~~~~~~~~
 
 This pipeline requires the following third-party tool(s):
 
 - bcl2fastq 2.20.0
 
 This software has an end-user license agreement (EULA). Given the EULA details
-of this software, it cannot be distributed by us but only by Illumina.
+of this software, it cannot be distributed according to ` Illumina license <https://support.illumina.com/content/dam/illumina-support/documents/downloads/software/bcl2fastq/bcl2fastq2-v2-20-eula.pdf>`_
 Therefore, you should install it yourself. On cluster facility, you may ask to
 your system administator. For instance::
 
     module load bcl2fastq/2.20.0
 
 For the same reason you cannot find it on community such as bioconda or docker (aug 2020).
 
@@ -106,14 +112,15 @@
 
 Changelog
 ~~~~~~~~~
 
 ========= =======================================================================
 Version   Description
 ========= =======================================================================
+1.3.0     * use latest sequana-wrappers to benefit and graphivz apptainer
 1.2.1     * Update CI action and use new sequana_pipetools v0.9.0
 1.2.0     * stable release with cleanup of the setup and README
 1.1.3     * add the --mars-seq option that fills the config automatically
 1.1.2     * fix the none_and_force merging strategy option
 1.1.1     * fix a regression bug
 1.1.0     * Uses new sequana-wrappers repository
 1.0.5     * Fix regression bug to cope with new snakemake API
```

### Comparing `sequana_demultiplex-1.2.1/sequana_demultiplex.egg-info/PKG-INFO` & `sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 1.2
 Name: sequana-demultiplex
-Version: 1.2.1
+Version: 1.3.0
 Summary: Pipeline that runs bcl2fastq and creates additional plots within a Snakemake workflow
 Home-page: https://github.com/sequana/
 Author: cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
 Description: 
         .. image:: https://badge.fury.io/py/sequana-demultiplex.svg
              :target: https://pypi.python.org/pypi/sequana_demultiplex
         
-        .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
-            :target: http://joss.theoj.org/papers/10.21105/joss.00352
-            :alt: JOSS (journal of open source software) DOI
-        
         .. image:: https://github.com/sequana/demultiplex/actions/workflows/main.yml/badge.svg
            :target: https://github.com/sequana/demultiplex/actions/workflows/main.yml
         
+        .. image:: https://coveralls.io/repos/github/sequana/demultiplex/badge.svg?branch=main
+            :target: https://coveralls.io/github/sequana/demultiplex?branch=main
+        
+        .. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+            :target: https://pypi.python.org/pypi/sequana
+            :alt: Python 3.8 | 3.9 | 3.10
+        
+        .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+           :target: http://joss.theoj.org/papers/10.21105/joss.00352
+           :alt: JOSS (journal of open source software) DOI
         
         This is is the **demultiplex** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
         
         :Overview: Runs bcl2fastq on raw BCL data and creates plots to ease the QC validation
-        :Input: A valid Illumina base calling directory
+        :Input: A valid Illumina base calling directory and sample sheet file
         :Output: An HTML report, a set of PNG files and the expected FastQ files
         :Status: production
         :Wiki: https://github.com/sequana/demultiplex/wiki
         :Documentation: This README file, the Wiki from the github repository (link above) and https://sequana.readthedocs.io
         :Citation: Cokelaer et al, (2017), 'Sequana': a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI https://doi:10.21105/joss.00352
         
         
@@ -74,15 +80,15 @@
         ~~~~~~~~~~~~
         
         This pipeline requires the following third-party tool(s):
         
         - bcl2fastq 2.20.0
         
         This software has an end-user license agreement (EULA). Given the EULA details
-        of this software, it cannot be distributed by us but only by Illumina.
+        of this software, it cannot be distributed according to ` Illumina license <https://support.illumina.com/content/dam/illumina-support/documents/downloads/software/bcl2fastq/bcl2fastq2-v2-20-eula.pdf>`_
         Therefore, you should install it yourself. On cluster facility, you may ask to
         your system administator. For instance::
         
             module load bcl2fastq/2.20.0
         
         For the same reason you cannot find it on community such as bioconda or docker (aug 2020).
         
@@ -116,14 +122,15 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= =======================================================================
         Version   Description
         ========= =======================================================================
+        1.3.0     * use latest sequana-wrappers to benefit and graphivz apptainer
         1.2.1     * Update CI action and use new sequana_pipetools v0.9.0
         1.2.0     * stable release with cleanup of the setup and README
         1.1.3     * add the --mars-seq option that fills the config automatically
         1.1.2     * fix the none_and_force merging strategy option
         1.1.1     * fix a regression bug
         1.1.0     * Uses new sequana-wrappers repository
         1.0.5     * Fix regression bug to cope with new snakemake API
```

### Comparing `sequana_demultiplex-1.2.1/sequana_demultiplex.egg-info/SOURCES.txt` & `sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/config.yaml` & `sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,20 @@
 #   intensities are expected to be found in input_directory/Data/Intensities
 #   Base call data are to be found in input_directory/Data/Intensities/BaseCalls
 #
 #   if merge_all_lanes is set to True, merged all lanes. This must be used with
 #   NextSeq sequencers for instance.
 #
 general:
-  input_directory: 
+  input_directory:
+
+
+apptainers:
+  graphviz: "https://zenodo.org/record/7928262/files/graphviz_7.0.5.img"
+
 
 ###################################################################################
 #
 #
 #
 # --ignore_missing_bcls: interpret missing *.bcl files as no call (N)
 # --no-bgzf-compression: turn off BGZF compression for FASTQ files
```

### Comparing `sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/dag.png` & `sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/demultiplex.rules` & `sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/demultiplex.rules`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 
 # do not overwrite the snakemake logger !
 from sequana import logger as log
 
 # This must be defined before the include
 configfile: "config.yaml"
 
+sequana_wrapper_branch = "main"
+
+
 # A convenient manager
 manager = PipelineManagerDirectory("demultiplex", config)
 
 
 samplesheet = config['bcl2fastq']['samplesheet_file'].strip()
 
 
@@ -72,38 +75,38 @@
     input: "Stats/Stats.json"
     output:
         csv= "undetermined_barcodes.csv",
         csv20= "undetermined_barcodes_20.csv",
         png= "barcodes.png"
     run:
         from sequana.demultiplex import StatsFile
+        from pylab import savefig
+        import pandas as pd
+
         s = StatsFile(input[0])
         df = s.plot_unknown_barcodes()
-        from pylab import savefig
         savefig(output.png, dpi=200)
         df.to_csv(output.csv20)
 
         # df contains the best 20 undetermined barcode, let us save all of them
         # for the users.
         ub = s.data['UnknownBarcodes']
-        import pandas as pd
         df = pd.DataFrame({x['Lane']:x['Barcodes'] for x in ub})
         df.columns = ["Lane {}".format(x) for x in df.columns]
         df.to_csv(output.csv)
 
 
 rule check_samplesheet:
     input: config['bcl2fastq']['samplesheet_file']
     output: temp("ss.log")
     shell:
         """
         sequana samplesheet --check {input[0]} 2> {output[0]}
         """
 
-
 rule bcl2fastq:
     input:
         valid_samplesheet="ss.log",
         samplesheet=config['bcl2fastq']['samplesheet_file']
     output:
         "Stats/Stats.json",
     params:
@@ -116,15 +119,14 @@
     threads: config['bcl2fastq']['threads']
     resources:
        **config['bcl2fastq']['resources']
     wrapper:
         "main/wrappers/bcl2fastq"
 
 
-
 rule plot_barplot_samples:
     input:  "Stats/Stats.json"
     output:
         barplot="samples.png"
     run:
         from sequana.demultiplex import StatsFile
         s = StatsFile(input[0])
@@ -141,22 +143,35 @@
         s = StatsFile(input[0])
         s.barplot_summary(filename=output.barplot)
         # save summary at the end because barplot output is not set.
         s.to_summary_reads(output.summary)
 
 
 rule rulegraph:
-    input: manager.snakefile
+    input:
+        workflow.snakefile
     output:
-        svg = ".sequana/rulegraph.svg"
+        "rulegraph/rulegraph.dot"
     params:
         mapper = {},
         configname = "config.yaml"
     wrapper:
-        "main/wrappers/rulegraph"
+        f"{sequana_wrapper_branch}/wrappers/rulegraph"
+
+
+rule dot2svg:
+    input:
+        "rulegraph/rulegraph.dot"
+    output:
+        ".sequana/rulegraph.svg"
+    container:
+        config['apptainers']['graphviz']
+    shell:
+        """dot -Tsvg {input} -o {output}"""
+
 
 localrules: rulegraph, check_samplesheet
 
 
 onsuccess:
     shell("chmod -R g+w .")
     manager.teardown()
```

### Comparing `sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/logo.png` & `sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/logo.png`

 * *Files identical despite different names*

### Comparing `sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/main.py` & `sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/main.py`

 * *Files identical despite different names*

### Comparing `sequana_demultiplex-1.2.1/sequana_pipelines/demultiplex/schema.yaml` & `sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/schema.yaml`

 * *Files identical despite different names*

### Comparing `sequana_demultiplex-1.2.1/setup.py` & `sequana_demultiplex-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from setuptools import setup, find_namespace_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
-import subprocess
 
 _MAJOR               = 1
-_MINOR               = 2
-_MICRO               = 1
+_MINOR               = 3
+_MICRO               = 0
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 metainfo = {
     'authors': {"main": ("cokelaer", "thomas.cokelaer@pasteur.fr")},
     'version': version,
     'license' : 'new BSD',
@@ -63,13 +62,12 @@
         '': ['*.yaml', "*.rules", "*.json", "requirements.txt", "*png", "*yml", "*smk"]
         },
 
     zip_safe=False,
 
     entry_points = {'console_scripts':[
         'sequana_demultiplex=sequana_pipelines.demultiplex.main:main',
-        'sequana_fix_samplesheet=sequana_pipelines.demultiplex.fix_samplesheet:main',
-        'sequana_check_samplesheet=sequana_pipelines.demultiplex.check_samplesheet:main']
+        ]
     }
 
 )
```

### Comparing `sequana_demultiplex-1.2.1/test/test_check_samplesheet.py` & `sequana_demultiplex-1.3.0/test/test_check_samplesheet.py`

 * *Files identical despite different names*

### Comparing `sequana_demultiplex-1.2.1/test/test_main.py` & `sequana_demultiplex-1.3.0/test/test_main.py`

 * *Files identical despite different names*

