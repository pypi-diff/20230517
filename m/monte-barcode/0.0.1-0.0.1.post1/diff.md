# Comparing `tmp/monte-barcode-0.0.1.tar.gz` & `tmp/monte-barcode-0.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monte-barcode-0.0.1.tar", last modified: Wed May 17 20:13:26 2023, max compression
+gzip compressed data, was "monte-barcode-0.0.1.post1.tar", last modified: Wed May 17 21:45:06 2023, max compression
```

## Comparing `monte-barcode-0.0.1.tar` & `monte-barcode-0.0.1.post1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:13:26.419302 monte-barcode-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 20:13:15.000000 monte-barcode-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-05-17 20:13:26.419302 monte-barcode-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-05-17 20:13:15.000000 monte-barcode-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:13:26.419302 monte-barcode-0.0.1/monte_barcode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-05-17 20:13:26.000000 monte-barcode-0.0.1/monte_barcode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-17 20:13:26.000000 monte-barcode-0.0.1/monte_barcode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:13:26.000000 monte-barcode-0.0.1/monte_barcode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 20:13:26.000000 monte-barcode-0.0.1/monte_barcode.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 20:13:26.000000 monte-barcode-0.0.1/monte_barcode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 20:13:26.000000 monte-barcode-0.0.1/monte_barcode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:13:26.419302 monte-barcode-0.0.1/montebarcode/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 20:13:15.000000 monte-barcode-0.0.1/montebarcode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-05-17 20:13:15.000000 monte-barcode-0.0.1/montebarcode/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-17 20:13:15.000000 monte-barcode-0.0.1/montebarcode/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-17 20:13:15.000000 monte-barcode-0.0.1/montebarcode/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-17 20:13:15.000000 monte-barcode-0.0.1/montebarcode/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-17 20:13:15.000000 monte-barcode-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:13:26.419302 monte-barcode-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:13:26.419302 monte-barcode-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-17 20:13:15.000000 monte-barcode-0.0.1/test/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:45:06.274330 monte-barcode-0.0.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-05-17 21:45:06.274330 monte-barcode-0.0.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:45:06.274330 monte-barcode-0.0.1.post1/monte_barcode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-05-17 21:45:06.000000 monte-barcode-0.0.1.post1/monte_barcode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-17 21:45:06.000000 monte-barcode-0.0.1.post1/monte_barcode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:45:06.000000 monte-barcode-0.0.1.post1/monte_barcode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 21:45:06.000000 monte-barcode-0.0.1.post1/monte_barcode.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 21:45:06.000000 monte-barcode-0.0.1.post1/monte_barcode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 21:45:06.000000 monte-barcode-0.0.1.post1/monte_barcode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:45:06.274330 monte-barcode-0.0.1.post1/montebarcode/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/montebarcode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/montebarcode/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/montebarcode/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/montebarcode/codons.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/montebarcode/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/montebarcode/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:45:06.274330 monte-barcode-0.0.1.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:45:06.274330 monte-barcode-0.0.1.post1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/test/tests.py
```

### Comparing `monte-barcode-0.0.1/LICENSE` & `monte-barcode-0.0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `monte-barcode-0.0.1/PKG-INFO` & `monte-barcode-0.0.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monte-barcode
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: Generating sets of random DNA sequences optimized for use in high-throughput sequencing.
 Author-email: Eachan Johnson <eachan.johnson@crick.ac.uk>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,14 +36,17 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🔴🟢🔵⚫️ monte barcode
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/monte-barcode)
+![PyPI](https://img.shields.io/pypi/v/monte-barcode)
+
 Generating sets of random DNA sequences optimized for use in high-throughput sequencing.
 
 ## Installation
 
 ### The easy way
 
 Install the pre-compiled version from PyPI:
@@ -353,8 +356,8 @@
 (Counter({'homopolymer': 1, 'palindrome': 1}), 4, ['ATCGCG', 'GCCGAT'])
 >>> mb.make_checks(['AAAAT', 'CCCGGG', 'ATCGCG', 'GCCGAT'], n=1, checks=checks, quiet=True)
 (Counter({'homopolymer': 1, 'palindrome': 1}), 3, ['ATCGCG'])
 ```
 
 ### Documentation
 
-Full API documnetation is [here](https://monte-barcode.readthedocs.org).
+Full API documentation is [here](https://monte-barcode.readthedocs.org).
```

### Comparing `monte-barcode-0.0.1/README.md` & `monte-barcode-0.0.1.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # 🔴🟢🔵⚫️ monte barcode
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/monte-barcode)
+![PyPI](https://img.shields.io/pypi/v/monte-barcode)
+
 Generating sets of random DNA sequences optimized for use in high-throughput sequencing.
 
 ## Installation
 
 ### The easy way
 
 Install the pre-compiled version from PyPI:
@@ -313,8 +316,8 @@
 (Counter({'homopolymer': 1, 'palindrome': 1}), 4, ['ATCGCG', 'GCCGAT'])
 >>> mb.make_checks(['AAAAT', 'CCCGGG', 'ATCGCG', 'GCCGAT'], n=1, checks=checks, quiet=True)
 (Counter({'homopolymer': 1, 'palindrome': 1}), 3, ['ATCGCG'])
 ```
 
 ### Documentation
 
-Full API documnetation is [here](https://monte-barcode.readthedocs.org).
+Full API documentation is [here](https://monte-barcode.readthedocs.org).
```

### Comparing `monte-barcode-0.0.1/monte_barcode.egg-info/PKG-INFO` & `monte-barcode-0.0.1.post1/monte_barcode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monte-barcode
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: Generating sets of random DNA sequences optimized for use in high-throughput sequencing.
 Author-email: Eachan Johnson <eachan.johnson@crick.ac.uk>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,14 +36,17 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🔴🟢🔵⚫️ monte barcode
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/monte-barcode)
+![PyPI](https://img.shields.io/pypi/v/monte-barcode)
+
 Generating sets of random DNA sequences optimized for use in high-throughput sequencing.
 
 ## Installation
 
 ### The easy way
 
 Install the pre-compiled version from PyPI:
@@ -353,8 +356,8 @@
 (Counter({'homopolymer': 1, 'palindrome': 1}), 4, ['ATCGCG', 'GCCGAT'])
 >>> mb.make_checks(['AAAAT', 'CCCGGG', 'ATCGCG', 'GCCGAT'], n=1, checks=checks, quiet=True)
 (Counter({'homopolymer': 1, 'palindrome': 1}), 3, ['ATCGCG'])
 ```
 
 ### Documentation
 
-Full API documnetation is [here](https://monte-barcode.readthedocs.org).
+Full API documentation is [here](https://monte-barcode.readthedocs.org).
```

### Comparing `monte-barcode-0.0.1/montebarcode/checks.py` & `monte-barcode-0.0.1.post1/montebarcode/checks.py`

 * *Files identical despite different names*

### Comparing `monte-barcode-0.0.1/montebarcode/cli.py` & `monte-barcode-0.0.1.post1/montebarcode/cli.py`

 * *Files identical despite different names*

### Comparing `monte-barcode-0.0.1/montebarcode/generate.py` & `monte-barcode-0.0.1.post1/montebarcode/generate.py`

 * *Files identical despite different names*

### Comparing `monte-barcode-0.0.1/montebarcode/utils.py` & `monte-barcode-0.0.1.post1/montebarcode/utils.py`

 * *Files identical despite different names*

### Comparing `monte-barcode-0.0.1/pyproject.toml` & `monte-barcode-0.0.1.post1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "monte-barcode"
-version = "0.0.1"
+version = "0.0.1post1"
 authors = [
   { name="Eachan Johnson", email="eachan.johnson@crick.ac.uk" },
 ]
 description = "Generating sets of random DNA sequences optimized for use in high-throughput sequencing."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
@@ -35,12 +35,17 @@
 [project.urls]
 "Homepage" = "https://github.com/scbirlab/monte-barcode"
 "Bug Tracker" = "https://github.com/scbirlab/monte-barcode/issues"
 
 [project.scripts]  # Optional
 monte = "montebarcode.cli:main"
 
+[tool.setuptools]
+# If there are data files included in your packages that need to be
+# installed, specify them here.
+package-data = {"montebarcode" = ["*.yml"]}
+
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

