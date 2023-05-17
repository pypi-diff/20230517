# Comparing `tmp/sequana_fastqc-1.6.1.tar.gz` & `tmp/sequana_fastqc-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_fastqc-1.6.1.tar", last modified: Wed Nov  2 09:58:58 2022, max compression
+gzip compressed data, was "dist/sequana_fastqc-1.7.0.tar", last modified: Wed May 17 11:26:40 2023, max compression
```

## Comparing `sequana_fastqc-1.6.1.tar` & `sequana_fastqc-1.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 09:58:58.000000 sequana_fastqc-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-11-02 09:58:49.000000 sequana_fastqc-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10294 2022-11-02 09:58:58.000000 sequana_fastqc-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7596 2022-11-02 09:58:49.000000 sequana_fastqc-1.6.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-02 09:58:49.000000 sequana_fastqc-1.6.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 09:58:58.000000 sequana_fastqc-1.6.1/sequana_fastqc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10294 2022-11-02 09:58:58.000000 sequana_fastqc-1.6.1/sequana_fastqc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-11-02 09:58:58.000000 sequana_fastqc-1.6.1/sequana_fastqc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 09:58:58.000000 sequana_fastqc-1.6.1/sequana_fastqc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-02 09:58:58.000000 sequana_fastqc-1.6.1/sequana_fastqc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 09:58:58.000000 sequana_fastqc-1.6.1/sequana_fastqc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-02 09:58:58.000000 sequana_fastqc-1.6.1/sequana_fastqc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-02 09:58:58.000000 sequana_fastqc-1.6.1/sequana_fastqc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 09:58:58.000000 sequana_fastqc-1.6.1/sequana_pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 09:58:58.000000 sequana_fastqc-1.6.1/sequana_pipelines/fastqc/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-11-02 09:58:49.000000 sequana_fastqc-1.6.1/sequana_pipelines/fastqc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-11-02 09:58:49.000000 sequana_fastqc-1.6.1/sequana_pipelines/fastqc/config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    12071 2022-11-02 09:58:49.000000 sequana_fastqc-1.6.1/sequana_pipelines/fastqc/dag.png
--rw-r--r--   0 runner    (1001) docker     (121)    12948 2022-11-02 09:58:49.000000 sequana_fastqc-1.6.1/sequana_pipelines/fastqc/fastqc.rules
--rw-r--r--   0 runner    (1001) docker     (121)    75082 2022-11-02 09:58:49.000000 sequana_fastqc-1.6.1/sequana_pipelines/fastqc/logo.png
--rwxr-xr-x   0 runner    (1001) docker     (121)     4157 2022-11-02 09:58:49.000000 sequana_fastqc-1.6.1/sequana_pipelines/fastqc/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5303 2022-11-02 09:58:49.000000 sequana_fastqc-1.6.1/sequana_pipelines/fastqc/multiqc_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-02 09:58:49.000000 sequana_fastqc-1.6.1/sequana_pipelines/fastqc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1580 2022-11-02 09:58:49.000000 sequana_fastqc-1.6.1/sequana_pipelines/fastqc/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-02 09:58:58.000000 sequana_fastqc-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-11-02 09:58:49.000000 sequana_fastqc-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 11:26:40.000000 sequana_fastqc-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-17 11:26:36.000000 sequana_fastqc-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10435 2023-05-17 11:26:40.000000 sequana_fastqc-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7721 2023-05-17 11:26:36.000000 sequana_fastqc-1.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-17 11:26:36.000000 sequana_fastqc-1.7.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 11:26:40.000000 sequana_fastqc-1.7.0/sequana_fastqc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10435 2023-05-17 11:26:39.000000 sequana_fastqc-1.7.0/sequana_fastqc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2023-05-17 11:26:40.000000 sequana_fastqc-1.7.0/sequana_fastqc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 11:26:39.000000 sequana_fastqc-1.7.0/sequana_fastqc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-17 11:26:39.000000 sequana_fastqc-1.7.0/sequana_fastqc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 11:26:39.000000 sequana_fastqc-1.7.0/sequana_fastqc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-17 11:26:39.000000 sequana_fastqc-1.7.0/sequana_fastqc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-17 11:26:39.000000 sequana_fastqc-1.7.0/sequana_fastqc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 11:26:40.000000 sequana_fastqc-1.7.0/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 11:26:40.000000 sequana_fastqc-1.7.0/sequana_pipelines/fastqc/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-17 11:26:36.000000 sequana_fastqc-1.7.0/sequana_pipelines/fastqc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-05-17 11:26:36.000000 sequana_fastqc-1.7.0/sequana_pipelines/fastqc/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    12071 2023-05-17 11:26:36.000000 sequana_fastqc-1.7.0/sequana_pipelines/fastqc/dag.png
+-rw-r--r--   0 runner    (1001) docker     (122)    13336 2023-05-17 11:26:36.000000 sequana_fastqc-1.7.0/sequana_pipelines/fastqc/fastqc.rules
+-rw-r--r--   0 runner    (1001) docker     (122)    75082 2023-05-17 11:26:36.000000 sequana_fastqc-1.7.0/sequana_pipelines/fastqc/logo.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4157 2023-05-17 11:26:36.000000 sequana_fastqc-1.7.0/sequana_pipelines/fastqc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5303 2023-05-17 11:26:36.000000 sequana_fastqc-1.7.0/sequana_pipelines/fastqc/multiqc_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-17 11:26:36.000000 sequana_fastqc-1.7.0/sequana_pipelines/fastqc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-05-17 11:26:36.000000 sequana_fastqc-1.7.0/sequana_pipelines/fastqc/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-05-17 11:26:40.000000 sequana_fastqc-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-05-17 11:26:36.000000 sequana_fastqc-1.7.0/setup.py
```

### Comparing `sequana_fastqc-1.6.1/PKG-INFO` & `sequana_fastqc-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequana_fastqc
-Version: 1.6.1
+Version: 1.7.0
 Summary: A fastqc pipeline from sequana project.
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -138,14 +138,16 @@
         to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
         
         Changelog
         ~~~~~~~~~
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        1.7.0     * Use new rulegraph wrapper and new graphviz apptainer
+        1.6.2     * slight refactorisation to use rulegraph wrapper
         1.6.1     * pin sequana version to 1.4.4 to force usage of new fastqc module
                     to fix falco. Updated config documentation.
         1.6.0     * Fixed falco output error and use singularity containers
         1.5.0     * removed modules completely.
         1.4.2     * simplified pipeline (suppress setup and use existing wrapper)
         1.4.1     * simplified pipeline with wrappers/rules
         1.4.0     * This version uses sequana 0.12.0 and new sequana-wrappers
```

### Comparing `sequana_fastqc-1.6.1/README.rst` & `sequana_fastqc-1.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,16 @@
 to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
 
 Changelog
 ~~~~~~~~~
 ========= ====================================================================
 Version   Description
 ========= ====================================================================
+1.7.0     * Use new rulegraph wrapper and new graphviz apptainer
+1.6.2     * slight refactorisation to use rulegraph wrapper
 1.6.1     * pin sequana version to 1.4.4 to force usage of new fastqc module
             to fix falco. Updated config documentation.
 1.6.0     * Fixed falco output error and use singularity containers
 1.5.0     * removed modules completely.
 1.4.2     * simplified pipeline (suppress setup and use existing wrapper)
 1.4.1     * simplified pipeline with wrappers/rules
 1.4.0     * This version uses sequana 0.12.0 and new sequana-wrappers
```

### Comparing `sequana_fastqc-1.6.1/sequana_fastqc.egg-info/PKG-INFO` & `sequana_fastqc-1.7.0/sequana_fastqc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequana-fastqc
-Version: 1.6.1
+Version: 1.7.0
 Summary: A fastqc pipeline from sequana project.
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -138,14 +138,16 @@
         to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
         
         Changelog
         ~~~~~~~~~
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        1.7.0     * Use new rulegraph wrapper and new graphviz apptainer
+        1.6.2     * slight refactorisation to use rulegraph wrapper
         1.6.1     * pin sequana version to 1.4.4 to force usage of new fastqc module
                     to fix falco. Updated config documentation.
         1.6.0     * Fixed falco output error and use singularity containers
         1.5.0     * removed modules completely.
         1.4.2     * simplified pipeline (suppress setup and use existing wrapper)
         1.4.1     * simplified pipeline with wrappers/rules
         1.4.0     * This version uses sequana 0.12.0 and new sequana-wrappers
```

### Comparing `sequana_fastqc-1.6.1/sequana_fastqc.egg-info/SOURCES.txt` & `sequana_fastqc-1.7.0/sequana_fastqc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sequana_fastqc-1.6.1/sequana_pipelines/fastqc/config.yaml` & `sequana_fastqc-1.7.0/sequana_pipelines/fastqc/config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -14,20 +14,26 @@
 
 # See sequana_pipetools.readthedocs.io for details about these 2 options
 # common prefixes are removed. addition prefixes may be removed here
 #extra_prefixes_to_strip = []
 # in special cases, sample names can be extracted with a pattern
 #sample_pattern: '{sample}.fastq.gz'
 
+
+apptainers:
+    falco: "https://zenodo.org/record/7014954/files/falco_1.0.0.img"
+    fastqc: "https://zenodo.org/record/7923780/files/fastqc_0.12.1.img"
+    graphviz: "https://zenodo.org/record/7928262/files/graphviz_7.0.5.img"
+
+
 ##############################################################################
 # general section
 #
 # Choose one of the standard method to perform QC of your fastq data
 #
-# method_choice__ = ['fastqc', 'falco']
 general:
     method_choice: fastqc
 
 ##############################################################################
 # FastQC section
 #
 # :Parameters:
```

### Comparing `sequana_fastqc-1.6.1/sequana_pipelines/fastqc/dag.png` & `sequana_fastqc-1.7.0/sequana_pipelines/fastqc/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_fastqc-1.6.1/sequana_pipelines/fastqc/fastqc.rules` & `sequana_fastqc-1.7.0/sequana_pipelines/fastqc/fastqc.rules`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 
 from sequana.utils.datatables_js import DataTable
 from sequana.utils.tree import HTMLDirectory
 
 from sequana_pipetools import PipelineManager
 from sequana_pipetools import snaketools as sm
 
-# This must be defined before the include
+
 configfile: "config.yaml"
 
 manager = PipelineManager("fastqc", config)
 
+sequana_wrapper_branch = "main"
+
 # This is just for information. Not used in the pipeline but only for HTML rpeort
 # do we have illumina paired data with tag _R1_ ?
 R1 = [1 for x in manager.samples.values() if "_R1_" in x.split("/")[-1]]
 R2 = [1 for x in manager.samples.values() if "_R2_" in x.split("/")[-1]]
 
 PAIRED = False
 if len(R1) == len(R2) and len(R1) != 0:
@@ -63,50 +65,54 @@
 
 if 'general' in config and 'method_choice' in config['general'] and \
     config['general']['method_choice'] == 'falco':
 
     METHOD = "falco"
 
     rule falco:
-        input: manager.getrawdata()
-        output: "samples/{sample}/summary.txt"
+        input:
+            manager.getrawdata()
+        output:
+            "samples/{sample}/summary.txt"
         log:
             "samples/{sample}/falco.log"
         threads:
             config['falco']['threads']
         params:
             options=config['falco']['options'],
             working_directory="samples/{sample}"
         container:
-            "https://zenodo.org/record/7014954/files/falco_1.0.0.img"
+            config['apptainers']['falco']
         resources:
             **config['falco']['resources']
         wrapper:
-            "main/wrappers/falco"
+            f"{sequana_wrapper_branch}/wrappers/falco"
     __multiqc__input = expand("samples/{sample}/summary.txt", sample=manager.samples)
 
 else:
     METHOD = "fastqc"
 
     rule fastqc:
-        input: manager.getrawdata()
-        output: "samples/{sample}/fastqc.done"
+        input:
+            manager.getrawdata()
+        output:
+            "samples/{sample}/fastqc.done"
         log:
             "samples/{sample}/fastqc.log"
         threads:
             config['fastqc']['threads']
         params:
             options=config['fastqc']['options'],
             working_directory="samples/{sample}"
         resources:
             **config['fastqc']['resources']
         container:
-            "https://zenodo.org/record/7015004/files/fastqc_0.11.9-py3.img"
+            config['apptainers']['fastqc']
         wrapper:
-            "main/wrappers/fastqc"
+            f"{sequana_wrapper_branch}/wrappers/fastqc"
     __multiqc__input = expand("samples/{sample}/fastqc.done", sample=manager.samples)
 
 
 # define a list of files for the md5sum
 allfiles = []
 for k,v in manager.samples.items():
     if isinstance(v, str):
@@ -166,19 +172,36 @@
            "multiqc/multiqc.log"
         resources:
             **config["multiqc"]["resources"]
         wrapper:
            "main/wrappers/multiqc"
 
 
-# ====================================================================== rulegraph 
-sequana_rulegraph_mapper = {}
-if config['multiqc']['do']:
-    sequana_rulegraph_mapper["multiqc"] = "../multiqc/multiqc_report.html"
-include: sm.modules['rulegraph']
+# ====================================================================== rulegraph
+
+rule rulegraph:
+    input: str(manager.snakefile)
+    output:
+        svg = "rulegraph/rulegraph.dot"
+    params:
+        mapper = {"multiqc": "../multiqc/multiqc_report.html"} if config['multiqc']['do'] else {},
+        configname = "config.yaml"
+    wrapper:
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
 
 
 rule plotting_and_stats:
     input: expand("samples/{sample}/" + f"{METHOD}.log", sample=manager.samples)
     output: "outputs/summary.png", "outputs/summary.json"
     resources:
         **config["multiqc"]["resources"]
```

### Comparing `sequana_fastqc-1.6.1/sequana_pipelines/fastqc/logo.png` & `sequana_fastqc-1.7.0/sequana_pipelines/fastqc/logo.png`

 * *Files identical despite different names*

### Comparing `sequana_fastqc-1.6.1/sequana_pipelines/fastqc/main.py` & `sequana_fastqc-1.7.0/sequana_pipelines/fastqc/main.py`

 * *Files identical despite different names*

### Comparing `sequana_fastqc-1.6.1/sequana_pipelines/fastqc/multiqc_config.yaml` & `sequana_fastqc-1.7.0/sequana_pipelines/fastqc/multiqc_config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_fastqc-1.6.1/sequana_pipelines/fastqc/schema.yaml` & `sequana_fastqc-1.7.0/sequana_pipelines/fastqc/schema.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,17 @@
                 required: False
             "threads":
                 type: int
                 required: True
             "resources":
                 type: any
                 required: true
+    "apptainers":
+        type: any
+
 
     "multiqc":
         type: map
         mapping:
             "do":
               type: bool
             "options":
```

### Comparing `sequana_fastqc-1.6.1/setup.py` & `sequana_fastqc-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_namespace_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 import subprocess
 
 _MAJOR               = 1
-_MINOR               = 6
-_MICRO               = 1
+_MINOR               = 7
+_MICRO               = 0
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 metainfo = {
     'authors': {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
     'version': version,
     'license' : 'new BSD',
```

