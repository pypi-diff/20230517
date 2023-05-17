# Comparing `tmp/sequana_nanomerge-1.1.0.tar.gz` & `tmp/sequana_nanomerge-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_nanomerge-1.1.0.tar", last modified: Fri May 12 09:47:21 2023, max compression
+gzip compressed data, was "dist/sequana_nanomerge-1.2.0.tar", last modified: Wed May 17 08:52:26 2023, max compression
```

## Comparing `sequana_nanomerge-1.1.0.tar` & `sequana_nanomerge-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7966 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5383 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7966 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13153 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/dag.png
--rw-r--r--   0 runner    (1001) docker     (122)     4538 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5191 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/nanomerge.rules
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3557 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8119 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5520 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8119 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    13153 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/dag.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4538 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5661 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/nanomerge.rules
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3557 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/setup.py
```

### Comparing `sequana_nanomerge-1.1.0/PKG-INFO` & `sequana_nanomerge-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequana_nanomerge
-Version: 1.1.0
+Version: 1.2.0
 Summary: Merge barcoded or non barcoded fastq files generated by Nanopore runs
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -153,14 +153,16 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        1.2.0     * handle large promethium run by using find+cat instead of just cat
+                    to cope with very large number of input files.
         1.1.0     * add subsample option and set to 1,000,000 reads to handle large 
                     runs such as promethion
         1.0.1     * CSV can now handle sample or samplename column name in samplesheet.
                   * Fix the pyco file paths, update requirements and doc
         1.0.0     Stable release ready for production
         0.0.1     **First release.**
         ========= ====================================================================
```

### Comparing `sequana_nanomerge-1.1.0/README.rst` & `sequana_nanomerge-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,16 @@
 
 Changelog
 ~~~~~~~~~
 
 ========= ====================================================================
 Version   Description
 ========= ====================================================================
+1.2.0     * handle large promethium run by using find+cat instead of just cat
+            to cope with very large number of input files.
 1.1.0     * add subsample option and set to 1,000,000 reads to handle large 
             runs such as promethion
 1.0.1     * CSV can now handle sample or samplename column name in samplesheet.
           * Fix the pyco file paths, update requirements and doc
 1.0.0     Stable release ready for production
 0.0.1     **First release.**
 ========= ====================================================================
```

### Comparing `sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/PKG-INFO` & `sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequana-nanomerge
-Version: 1.1.0
+Version: 1.2.0
 Summary: Merge barcoded or non barcoded fastq files generated by Nanopore runs
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -153,14 +153,16 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        1.2.0     * handle large promethium run by using find+cat instead of just cat
+                    to cope with very large number of input files.
         1.1.0     * add subsample option and set to 1,000,000 reads to handle large 
                     runs such as promethion
         1.0.1     * CSV can now handle sample or samplename column name in samplesheet.
                   * Fix the pyco file paths, update requirements and doc
         1.0.0     Stable release ready for production
         0.0.1     **First release.**
         ========= ====================================================================
```

### Comparing `sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/SOURCES.txt` & `sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/config.yaml` & `sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/dag.png` & `sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/main.py` & `sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/main.py`

 * *Files identical despite different names*

### Comparing `sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/nanomerge.rules` & `sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/nanomerge.rules`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,21 @@
     if samples.barcoded:
         barcode = samples.get_barcode_from_sample(wildcards.sample)
         filenames = list((input_directory / barcode).glob("*.fastq.gz"))
     else:
         filenames = list((input_directory).glob(input_pattern))
     return filenames
 
+def get_input_directory(wildcards):
+    if samples.barcoded:
+        barcode = samples.get_barcode_from_sample(wildcards.sample)
+        return input_directory / barcode
+    else:
+        return input_directory
+
 
 if config["summary"]:
     rule pyco:
         input:
             config['summary']
         output:
             "pyco/pyco.html"
@@ -116,17 +123,19 @@
 
 
 rule merge:
     input:
         get_input_merge
     output:
         "./{project}/{sample}.fastq.gz"
+    params:
+        indir=get_input_directory
     shell:
         """
-        cat {input} > {output}
+        find {params.indir} -type f -name "*fastq.gz" -exec cat {{}} + > {output}
         """
 
 
 rule rulegraph:
     input:
         workflow.snakefile
     output:
@@ -164,15 +173,15 @@
 
         dirs = ",".join([f'<a href="{x}/">{x}</a>' for x in samples.get_projects()])
         if config['summary']:
             with open("pyco/pyco.html", "r") as fout:
                 pycodata = fout.read()
                 pycodata = '<div class="columns">' + pycodata.split('<div class="columns">')[-1].replace("</div>\n</body>\n</html>","")
 
-            s = SummaryModule2(data, f"Your data are available in {dirs} directories" + pycodata)
+            s = SummaryModule2(data, f"""Your data are available in {dirs} directories. Please see the summary plots here below (if sequence summary was provided), generated with <a href="https://github.com/a-slide/pycoQC">pycoQC</a> software.""" + pycodata)
         else:
             s = SummaryModule2(data, f"no summary found. Please checkout the sub directories {dirs}. They should contain your final fastq files for each project.")
 
 # ======================================================================================== rulegraph
 
 
 onsuccess:
```

### Comparing `sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/schema.yaml` & `sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/schema.yaml`

 * *Files identical despite different names*

### Comparing `sequana_nanomerge-1.1.0/setup.py` & `sequana_nanomerge-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # handle sequana git link
 with open("requirements.txt", encoding='utf-8') as fh:
     requirements = [req.rstrip() if not req.startswith("git+") else req.rstrip().split("egg=")[-1] for req in fh]
 
 
 _MAJOR               = 1
-_MINOR               = 1
+_MINOR               = 2
 _MICRO               = 0
 version = f"{_MAJOR}.{_MINOR}.{_MICRO}"
 release = f"{_MAJOR}.{_MINOR}"
 
 
 metainfo = {
     'authors': {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
```

