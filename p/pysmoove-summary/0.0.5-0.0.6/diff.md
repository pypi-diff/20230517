# Comparing `tmp/pysmoove_summary-0.0.5.tar.gz` & `tmp/pysmoove_summary-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmoove_summary-0.0.5.tar", last modified: Mon Apr  4 19:54:09 2022, max compression
+gzip compressed data, was "pysmoove_summary-0.0.6.tar", last modified: Wed May 17 19:33:03 2023, max compression
```

## Comparing `pysmoove_summary-0.0.5.tar` & `pysmoove_summary-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2022-04-04 19:54:09.229088 pysmoove_summary-0.0.5/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1059 2022-04-04 19:41:02.000000 pysmoove_summary-0.0.5/LICENSE
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      572 2022-04-04 19:54:09.228618 pysmoove_summary-0.0.5/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       83 2022-04-04 19:41:02.000000 pysmoove_summary-0.0.5/README.md
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2022-04-04 19:54:09.224777 pysmoove_summary-0.0.5/pysmoove_summary/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       68 2022-04-04 19:41:02.000000 pysmoove_summary-0.0.5/pysmoove_summary/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3003 2022-04-04 19:52:41.000000 pysmoove_summary-0.0.5/pysmoove_summary/pysmoove_summary.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2022-04-04 19:54:09.227921 pysmoove_summary-0.0.5/pysmoove_summary.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      572 2022-04-04 19:54:09.000000 pysmoove_summary-0.0.5/pysmoove_summary.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      334 2022-04-04 19:54:09.000000 pysmoove_summary-0.0.5/pysmoove_summary.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2022-04-04 19:54:09.000000 pysmoove_summary-0.0.5/pysmoove_summary.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2022-04-04 19:54:09.000000 pysmoove_summary-0.0.5/pysmoove_summary.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       15 2022-04-04 19:54:09.000000 pysmoove_summary-0.0.5/pysmoove_summary.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       17 2022-04-04 19:54:09.000000 pysmoove_summary-0.0.5/pysmoove_summary.egg-info/top_level.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2022-04-04 19:54:09.229202 pysmoove_summary-0.0.5/setup.cfg
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      848 2022-04-04 19:52:46.000000 pysmoove_summary-0.0.5/setup.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-05-17 19:33:03.320797 pysmoove_summary-0.0.6/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1059 2022-04-04 19:41:02.000000 pysmoove_summary-0.0.6/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      535 2023-05-17 19:33:03.320462 pysmoove_summary-0.0.6/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       83 2022-04-04 19:41:02.000000 pysmoove_summary-0.0.6/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-05-17 19:33:03.317542 pysmoove_summary-0.0.6/pysmoove_summary/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       68 2022-04-04 19:41:02.000000 pysmoove_summary-0.0.6/pysmoove_summary/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5027 2022-05-18 00:59:06.000000 pysmoove_summary-0.0.6/pysmoove_summary/correlated_phenotypes.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4320 2023-05-17 19:27:36.000000 pysmoove_summary-0.0.6/pysmoove_summary/correlated_phenotypes_3rdseq.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1207 2022-05-18 00:42:08.000000 pysmoove_summary-0.0.6/pysmoove_summary/parse_phenotypes.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      776 2023-05-17 19:27:36.000000 pysmoove_summary-0.0.6/pysmoove_summary/parse_phenotypes_3rdseq.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3051 2023-05-17 19:31:00.000000 pysmoove_summary-0.0.6/pysmoove_summary/pysmoove_summary.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-05-17 19:33:03.320019 pysmoove_summary-0.0.6/pysmoove_summary.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      535 2023-05-17 19:33:03.000000 pysmoove_summary-0.0.6/pysmoove_summary.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      506 2023-05-17 19:33:03.000000 pysmoove_summary-0.0.6/pysmoove_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-05-17 19:33:03.000000 pysmoove_summary-0.0.6/pysmoove_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       76 2023-05-17 19:33:03.000000 pysmoove_summary-0.0.6/pysmoove_summary.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       15 2023-05-17 19:33:03.000000 pysmoove_summary-0.0.6/pysmoove_summary.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       17 2023-05-17 19:33:03.000000 pysmoove_summary-0.0.6/pysmoove_summary.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-05-17 19:33:03.320879 pysmoove_summary-0.0.6/setup.cfg
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      848 2023-05-17 19:32:45.000000 pysmoove_summary-0.0.6/setup.py
```

### Comparing `pysmoove_summary-0.0.5/LICENSE` & `pysmoove_summary-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmoove_summary-0.0.5/PKG-INFO` & `pysmoove_summary-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: pysmoove_summary
-Version: 0.0.5
+Version: 0.0.6
 Summary: Summarize pysmoove SV calling VCF results in a BED-like format
 Home-page: https://gitlab.com/salk-tm/pysmoove_summary
 Author: Anthony Aylward
 Author-email: aaylward@salk.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysmoove-summary
 
 Summarize pysmoove SV calling VCF results in a BED-like format
-
-
```

### Comparing `pysmoove_summary-0.0.5/pysmoove_summary/pysmoove_summary.py` & `pysmoove_summary-0.0.6/pysmoove_summary/pysmoove_summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     parser = ArgumentParser(description='generate summary BED from VCF of SVs')
     parser.add_argument('vcf', metavar='<vcf>', help='VCF containing SVs')
     parser.add_argument('--dhffc-del', metavar='<float>', type=float,
         default=DHFFC_DEL, help=f'filter out deletions with DHFFC above this value [{DHFFC_DEL}]')
     parser.add_argument('--dhffc-dup', metavar='<float>', type=float,
         default=DHFFC_DUP, help=f'filter out duplications with DHFFC below this value [{DHFFC_DUP}]')
     parser.add_argument('--mshq', metavar='<float>', type=float,
-        default=MSHQ, help=f'filter out hets with MSHQ below this value [{MSHQ}]')
+        help=f'filter out hets with MSHQ below this value. A recommendation is 3.0')
     parser.add_argument('--header', action='store_true',
         help='include a header in output')
     parser.add_argument('--sv-only', action='store_true',
         help='show SVs only, no SNPs or small INDELs')
     return parser.parse_args()
 
 def main():
@@ -46,17 +46,18 @@
             continue
         if rec.info['SVTYPE'] == 'DEL':
             if all(rec.samples[s]['DHFFC'] > args.dhffc_del for s in samples):
                 continue
         if rec.info['SVTYPE'] == 'DUP':
             if all(rec.samples[s]['DHFFC'] < args.dhffc_dup for s in samples):
                 continue
-        if '0/1' in genotypes:
-            if rec.info['MSHQ'] < args.mshq:
-                continue
+        if args.mshq is not None:
+            if '0/1' in genotypes:
+                if rec.info['MSHQ'] < args.mshq:
+                    continue
         genes = tuple(g.split('|')[0] for g in rec.info.get('smoove_gene', ())
                         if g.split('|')[1].startswith('gene'))
         if len(genes) == 0:
             genes = ('NA',)
         elif len(genes) > 4:
             genes = ('MANY',)
         print(rec.contig, rec.pos-1, rec.stop, rec.info['SVTYPE'],
```

### Comparing `pysmoove_summary-0.0.5/pysmoove_summary.egg-info/PKG-INFO` & `pysmoove_summary-0.0.6/pysmoove_summary.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: pysmoove-summary
-Version: 0.0.5
+Version: 0.0.6
 Summary: Summarize pysmoove SV calling VCF results in a BED-like format
 Home-page: https://gitlab.com/salk-tm/pysmoove_summary
 Author: Anthony Aylward
 Author-email: aaylward@salk.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysmoove-summary
 
 Summarize pysmoove SV calling VCF results in a BED-like format
-
-
```

### Comparing `pysmoove_summary-0.0.5/setup.py` & `pysmoove_summary-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pysmoove_summary',
-    version='0.0.5',
+    version='0.0.6',
     author='Anthony Aylward',
     author_email='aaylward@salk.edu',
     description='Summarize pysmoove SV calling VCF results in a BED-like format',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://gitlab.com/salk-tm/pysmoove_summary',
     packages=setuptools.find_packages(),
```

