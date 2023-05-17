# Comparing `tmp/commonnexus-1.2.0.tar.gz` & `tmp/commonnexus-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonnexus-1.2.0.tar", last modified: Wed Mar 15 06:29:57 2023, max compression
+gzip compressed data, was "commonnexus-1.3.0.tar", last modified: Wed May 17 06:36:13 2023, max compression
```

## Comparing `commonnexus-1.2.0.tar` & `commonnexus-1.3.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-03-15 06:29:57.858458 commonnexus-1.2.0/
--rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2023-02-08 09:11:27.000000 commonnexus-1.2.0/LICENSE
--rw-rw-r--   0 robert    (1000) robert    (1000)     4646 2023-03-15 06:29:57.858458 commonnexus-1.2.0/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)     3106 2023-03-14 06:35:07.000000 commonnexus-1.2.0/README.md
--rw-rw-r--   0 robert    (1000) robert    (1000)     2428 2023-03-15 06:29:57.858458 commonnexus-1.2.0/setup.cfg
--rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2023-02-08 09:14:01.000000 commonnexus-1.2.0/setup.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-03-15 06:29:57.858458 commonnexus-1.2.0/src/
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-03-15 06:29:57.858458 commonnexus-1.2.0/src/commonnexus/
--rw-rw-r--   0 robert    (1000) robert    (1000)      121 2023-03-15 06:28:37.000000 commonnexus-1.2.0/src/commonnexus/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     4361 2023-03-04 14:48:53.000000 commonnexus-1.2.0/src/commonnexus/__main__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      189 2023-02-08 10:31:55.000000 commonnexus-1.2.0/src/commonnexus/_compat.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-03-15 06:29:57.858458 commonnexus-1.2.0/src/commonnexus/blocks/
--rw-rw-r--   0 robert    (1000) robert    (1000)      602 2023-03-05 14:33:36.000000 commonnexus-1.2.0/src/commonnexus/blocks/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    11215 2023-02-14 14:50:23.000000 commonnexus-1.2.0/src/commonnexus/blocks/assumptions.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     7979 2023-03-08 10:40:36.000000 commonnexus-1.2.0/src/commonnexus/blocks/base.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    57499 2023-03-13 15:54:49.000000 commonnexus-1.2.0/src/commonnexus/blocks/characters.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     7365 2023-02-16 11:10:00.000000 commonnexus-1.2.0/src/commonnexus/blocks/codons.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    15853 2023-03-08 09:06:05.000000 commonnexus-1.2.0/src/commonnexus/blocks/distances.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     8333 2023-03-13 07:11:10.000000 commonnexus-1.2.0/src/commonnexus/blocks/notes.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     7699 2023-02-14 12:01:40.000000 commonnexus-1.2.0/src/commonnexus/blocks/sets.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3040 2023-03-07 08:22:00.000000 commonnexus-1.2.0/src/commonnexus/blocks/taxa.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    16947 2023-03-14 16:03:53.000000 commonnexus-1.2.0/src/commonnexus/blocks/trees.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2240 2023-02-16 11:10:00.000000 commonnexus-1.2.0/src/commonnexus/blocks/unaligned.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3710 2023-03-13 14:04:48.000000 commonnexus-1.2.0/src/commonnexus/cli_util.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     4318 2023-03-08 10:24:09.000000 commonnexus-1.2.0/src/commonnexus/command.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-03-15 06:29:57.858458 commonnexus-1.2.0/src/commonnexus/commands/
--rw-rw-r--   0 robert    (1000) robert    (1000)        0 2023-03-02 07:16:22.000000 commonnexus-1.2.0/src/commonnexus/commands/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     5977 2023-03-10 08:48:03.000000 commonnexus-1.2.0/src/commonnexus/commands/characters.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      530 2023-03-02 09:45:35.000000 commonnexus-1.2.0/src/commonnexus/commands/combine.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      316 2023-03-04 14:51:27.000000 commonnexus-1.2.0/src/commonnexus/commands/help.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      349 2023-03-06 11:27:02.000000 commonnexus-1.2.0/src/commonnexus/commands/normalise.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     1201 2023-03-10 11:18:14.000000 commonnexus-1.2.0/src/commonnexus/commands/split.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     8705 2023-03-13 14:05:09.000000 commonnexus-1.2.0/src/commonnexus/commands/taxa.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3174 2023-03-13 14:15:33.000000 commonnexus-1.2.0/src/commonnexus/commands/trees.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    17585 2023-03-10 14:17:53.000000 commonnexus-1.2.0/src/commonnexus/nexus.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    11459 2023-03-08 14:41:35.000000 commonnexus-1.2.0/src/commonnexus/tokenizer.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-03-15 06:29:57.858458 commonnexus-1.2.0/src/commonnexus/tools/
--rw-rw-r--   0 robert    (1000) robert    (1000)      213 2023-03-02 07:36:37.000000 commonnexus-1.2.0/src/commonnexus/tools/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3061 2023-03-07 09:13:58.000000 commonnexus-1.2.0/src/commonnexus/tools/combine.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    11492 2023-03-10 08:40:51.000000 commonnexus-1.2.0/src/commonnexus/tools/matrix.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     4137 2023-03-09 12:21:29.000000 commonnexus-1.2.0/src/commonnexus/tools/normalise.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      168 2023-02-16 08:50:17.000000 commonnexus-1.2.0/src/commonnexus/util.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-03-15 06:29:57.858458 commonnexus-1.2.0/src/commonnexus.egg-info/
--rw-rw-r--   0 robert    (1000) robert    (1000)     4646 2023-03-15 06:29:57.000000 commonnexus-1.2.0/src/commonnexus.egg-info/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)     1316 2023-03-15 06:29:57.000000 commonnexus-1.2.0/src/commonnexus.egg-info/SOURCES.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-03-15 06:29:57.000000 commonnexus-1.2.0/src/commonnexus.egg-info/dependency_links.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)       58 2023-03-15 06:29:57.000000 commonnexus-1.2.0/src/commonnexus.egg-info/entry_points.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-02-08 09:38:01.000000 commonnexus-1.2.0/src/commonnexus.egg-info/not-zip-safe
--rw-rw-r--   0 robert    (1000) robert    (1000)      220 2023-03-15 06:29:57.000000 commonnexus-1.2.0/src/commonnexus.egg-info/requires.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)       12 2023-03-15 06:29:57.000000 commonnexus-1.2.0/src/commonnexus.egg-info/top_level.txt
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2023-02-08 09:11:27.000000 commonnexus-1.3.0/LICENSE
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4659 2023-05-17 06:36:13.753529 commonnexus-1.3.0/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3106 2023-03-14 06:35:07.000000 commonnexus-1.3.0/README.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2441 2023-05-17 06:36:13.753529 commonnexus-1.3.0/setup.cfg
+-rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2023-02-08 09:14:01.000000 commonnexus-1.3.0/setup.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/src/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/src/commonnexus/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      121 2023-05-17 06:35:26.000000 commonnexus-1.3.0/src/commonnexus/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4361 2023-03-04 14:48:53.000000 commonnexus-1.3.0/src/commonnexus/__main__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      189 2023-03-15 10:02:49.000000 commonnexus-1.3.0/src/commonnexus/_compat.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/src/commonnexus/blocks/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      602 2023-03-05 14:33:36.000000 commonnexus-1.3.0/src/commonnexus/blocks/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11215 2023-02-14 14:50:23.000000 commonnexus-1.3.0/src/commonnexus/blocks/assumptions.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     7979 2023-03-08 10:40:36.000000 commonnexus-1.3.0/src/commonnexus/blocks/base.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    57499 2023-03-13 15:54:49.000000 commonnexus-1.3.0/src/commonnexus/blocks/characters.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     7365 2023-02-16 11:10:00.000000 commonnexus-1.3.0/src/commonnexus/blocks/codons.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    15853 2023-03-08 09:06:05.000000 commonnexus-1.3.0/src/commonnexus/blocks/distances.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     8333 2023-03-13 07:11:10.000000 commonnexus-1.3.0/src/commonnexus/blocks/notes.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     7699 2023-02-14 12:01:40.000000 commonnexus-1.3.0/src/commonnexus/blocks/sets.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3040 2023-03-07 08:22:00.000000 commonnexus-1.3.0/src/commonnexus/blocks/taxa.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    17067 2023-05-15 14:44:35.000000 commonnexus-1.3.0/src/commonnexus/blocks/trees.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2240 2023-02-16 11:10:00.000000 commonnexus-1.3.0/src/commonnexus/blocks/unaligned.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3710 2023-03-13 14:04:48.000000 commonnexus-1.3.0/src/commonnexus/cli_util.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4318 2023-03-08 10:24:09.000000 commonnexus-1.3.0/src/commonnexus/command.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/src/commonnexus/commands/
+-rw-rw-r--   0 robert    (1000) robert    (1000)        0 2023-03-02 07:16:22.000000 commonnexus-1.3.0/src/commonnexus/commands/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     5977 2023-03-10 08:48:03.000000 commonnexus-1.3.0/src/commonnexus/commands/characters.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      530 2023-03-02 09:45:35.000000 commonnexus-1.3.0/src/commonnexus/commands/combine.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      316 2023-03-04 14:51:27.000000 commonnexus-1.3.0/src/commonnexus/commands/help.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      349 2023-03-06 11:27:02.000000 commonnexus-1.3.0/src/commonnexus/commands/normalise.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1201 2023-03-10 11:18:14.000000 commonnexus-1.3.0/src/commonnexus/commands/split.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     8705 2023-03-13 14:05:09.000000 commonnexus-1.3.0/src/commonnexus/commands/taxa.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3174 2023-03-13 14:15:33.000000 commonnexus-1.3.0/src/commonnexus/commands/trees.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    17585 2023-03-10 14:17:53.000000 commonnexus-1.3.0/src/commonnexus/nexus.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11459 2023-03-08 14:41:35.000000 commonnexus-1.3.0/src/commonnexus/tokenizer.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/src/commonnexus/tools/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      213 2023-03-02 07:36:37.000000 commonnexus-1.3.0/src/commonnexus/tools/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3061 2023-03-07 09:13:58.000000 commonnexus-1.3.0/src/commonnexus/tools/combine.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11492 2023-03-10 08:40:51.000000 commonnexus-1.3.0/src/commonnexus/tools/matrix.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4137 2023-03-09 12:21:29.000000 commonnexus-1.3.0/src/commonnexus/tools/normalise.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      168 2023-02-16 08:50:17.000000 commonnexus-1.3.0/src/commonnexus/util.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/src/commonnexus.egg-info/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4659 2023-05-17 06:36:13.000000 commonnexus-1.3.0/src/commonnexus.egg-info/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1316 2023-05-17 06:36:13.000000 commonnexus-1.3.0/src/commonnexus.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-05-17 06:36:13.000000 commonnexus-1.3.0/src/commonnexus.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       58 2023-05-17 06:36:13.000000 commonnexus-1.3.0/src/commonnexus.egg-info/entry_points.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-02-08 09:38:01.000000 commonnexus-1.3.0/src/commonnexus.egg-info/not-zip-safe
+-rw-rw-r--   0 robert    (1000) robert    (1000)      220 2023-05-17 06:36:13.000000 commonnexus-1.3.0/src/commonnexus.egg-info/requires.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       12 2023-05-17 06:36:13.000000 commonnexus-1.3.0/src/commonnexus.egg-info/top_level.txt
```

### Comparing `commonnexus-1.2.0/LICENSE` & `commonnexus-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/PKG-INFO` & `commonnexus-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: commonnexus
-Version: 1.2.0
+Version: 1.3.0
 Summary: A nexus (phylogenetics) file reader and writer (.nex, .trees)
 Home-page: https://github.com/dlce-eva/commonnexus
 Author: Robert Forkel
 Author-email: robert_forkel@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/dlce-eva/commonnexus/issues
 Keywords: phylogenetics nexus newick paup splitstree
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `commonnexus-1.2.0/README.md` & `commonnexus-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/setup.cfg` & `commonnexus-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [metadata]
 name = commonnexus
-version = 1.2.0
+version = 1.3.0
 author = Robert Forkel
 author_email = robert_forkel@eva.mpg.de
 description = A nexus (phylogenetics) file reader and writer (.nex, .trees)
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = phylogenetics nexus newick paup splitstree
 license = Apache 2.0
 license_files = LICENSE
 url = https://github.com/dlce-eva/commonnexus
 project_urls = 
 	Bug Tracker = https://github.com/dlce-eva/commonnexus/issues
 platforms = any
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Natural Language :: English
 	Operating System :: OS Independent
 	Environment :: Console
 	License :: OSI Approved :: Apache Software License
 	Topic :: Scientific/Engineering
```

### Comparing `commonnexus-1.2.0/src/commonnexus/__main__.py` & `commonnexus-1.3.0/src/commonnexus/__main__.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/blocks/__init__.py` & `commonnexus-1.3.0/src/commonnexus/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/blocks/assumptions.py` & `commonnexus-1.3.0/src/commonnexus/blocks/assumptions.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/blocks/base.py` & `commonnexus-1.3.0/src/commonnexus/blocks/base.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/blocks/characters.py` & `commonnexus-1.3.0/src/commonnexus/blocks/characters.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/blocks/codons.py` & `commonnexus-1.3.0/src/commonnexus/blocks/codons.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/blocks/distances.py` & `commonnexus-1.3.0/src/commonnexus/blocks/distances.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/blocks/notes.py` & `commonnexus-1.3.0/src/commonnexus/blocks/notes.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/blocks/sets.py` & `commonnexus-1.3.0/src/commonnexus/blocks/sets.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/blocks/taxa.py` & `commonnexus-1.3.0/src/commonnexus/blocks/taxa.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/blocks/trees.py` & `commonnexus-1.3.0/src/commonnexus/blocks/trees.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,14 +321,26 @@
                         'TRANSLATE command **after** TREE command', log=log, level='warning')
                 else:
                     with_translate = True
             else:
                 tree_seen = True
         return valid
 
+    @cached_property
+    def translate_mapping(self):
+        mapping = {}
+        if 'TRANSLATE' in self.commands:
+            mapping.update(self.TRANSLATE.mapping)
+        if 'TAXA' in self.linked_blocks:
+            mapping.update({
+                str(k): v for k, v in self.linked_blocks['TAXA'].TAXLABELS.labels.items()})
+        elif self.nexus.TAXA and self.nexus.TAXA.TAXLABELS:
+            mapping.update({str(k): v for k, v in self.nexus.TAXA.TAXLABELS.labels.items()})
+        return mapping
+
     def translate(self, tree: typing.Union[Tree, newick.Node]) -> newick.Node:
         """
         Translate a tree according to the mapping TREES TRANSLATE.
 
         :return: A Newick node where the node labels have been translated to valid taxon labels.
 
         .. note::
@@ -346,26 +358,18 @@
                 ...         tree.name,
                 ...         untranslated.TREES.translate(tree).newick,
                 ...         rooted=tree.rooted))
                 >>> untranslated.replace_block(
                 ...     untranslated.TREES, [('TREE', tree) for tree in trees])
                 >>> path.write_text(str(untranslated))
         """
-        mapping = {}
-        if 'TRANSLATE' in self.commands:
-            mapping.update(self.TRANSLATE.mapping)
-        if 'TAXA' in self.linked_blocks:
-            mapping.update({
-                str(k): v for k, v in self.linked_blocks['TAXA'].TAXLABELS.labels.items()})
-        elif self.nexus.TAXA and self.nexus.TAXA.TAXLABELS:
-            mapping.update({str(k): v for k, v in self.nexus.TAXA.TAXLABELS.labels.items()})
-
-        res = (tree.newick if isinstance(tree, Tree) else tree).rename(auto_quote=True, **mapping)
+        res = (tree.newick if isinstance(tree, Tree) else tree).rename(
+            auto_quote=True, **self.translate_mapping)
         if not set(n.unquoted_name for n in res.walk() if n.name and n.is_leaf).issubset(
-                mapping.values()):
+                self.translate_mapping.values()):
             warnings.warn('un-translatable leaf nodes!')
         return res
 
     @classmethod
     def from_data(cls,
                   *tree_specs: typing.Iterable[TreeSpec],
                   **translate_labels: typing.Dict[str, str]) -> 'Trees':
```

### Comparing `commonnexus-1.2.0/src/commonnexus/blocks/unaligned.py` & `commonnexus-1.3.0/src/commonnexus/blocks/unaligned.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/cli_util.py` & `commonnexus-1.3.0/src/commonnexus/cli_util.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/command.py` & `commonnexus-1.3.0/src/commonnexus/command.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/commands/characters.py` & `commonnexus-1.3.0/src/commonnexus/commands/characters.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/commands/combine.py` & `commonnexus-1.3.0/src/commonnexus/commands/combine.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/commands/split.py` & `commonnexus-1.3.0/src/commonnexus/commands/split.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/commands/taxa.py` & `commonnexus-1.3.0/src/commonnexus/commands/taxa.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/commands/trees.py` & `commonnexus-1.3.0/src/commonnexus/commands/trees.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/nexus.py` & `commonnexus-1.3.0/src/commonnexus/nexus.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/tokenizer.py` & `commonnexus-1.3.0/src/commonnexus/tokenizer.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/tools/combine.py` & `commonnexus-1.3.0/src/commonnexus/tools/combine.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/tools/matrix.py` & `commonnexus-1.3.0/src/commonnexus/tools/matrix.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus/tools/normalise.py` & `commonnexus-1.3.0/src/commonnexus/tools/normalise.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.2.0/src/commonnexus.egg-info/PKG-INFO` & `commonnexus-1.3.0/src/commonnexus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: commonnexus
-Version: 1.2.0
+Version: 1.3.0
 Summary: A nexus (phylogenetics) file reader and writer (.nex, .trees)
 Home-page: https://github.com/dlce-eva/commonnexus
 Author: Robert Forkel
 Author-email: robert_forkel@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/dlce-eva/commonnexus/issues
 Keywords: phylogenetics nexus newick paup splitstree
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `commonnexus-1.2.0/src/commonnexus.egg-info/SOURCES.txt` & `commonnexus-1.3.0/src/commonnexus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

