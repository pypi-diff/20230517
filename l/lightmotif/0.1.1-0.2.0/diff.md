# Comparing `tmp/lightmotif-0.1.1.tar.gz` & `tmp/lightmotif-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightmotif-0.1.1.tar", last modified: Thu May  4 01:38:59 2023, max compression
+gzip compressed data, was "lightmotif-0.2.0.tar", last modified: Wed May 17 14:53:14 2023, max compression
```

## Comparing `lightmotif-0.1.1.tar` & `lightmotif-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.253166 lightmotif-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-04 01:38:54.000000 lightmotif-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-04 01:38:54.000000 lightmotif-0.1.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-04 01:38:54.000000 lightmotif-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-05-04 01:38:59.253166 lightmotif-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-05-04 01:38:54.000000 lightmotif-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif/benches/
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/benches/ecoli.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.253166 lightmotif-0.1.1/lightmotif/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/abc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/dense.rs
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/err.rs
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/pli.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/pwm.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/seq.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.253166 lightmotif-0.1.1/lightmotif/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/tests/dna.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif-py/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif-py/lightmotif/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif-py/lightmotif/arch/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/arch/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/arch/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif-py/lightmotif/avx2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/avx2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif-py/lightmotif/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/tests/test_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/tests/unittest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-05-04 01:38:59.000000 lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 01:38:59.000000 lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 01:38:59.000000 lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 01:38:59.000000 lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 01:38:59.000000 lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-04 01:38:59.000000 lightmotif-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-04 01:38:59.253166 lightmotif-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-04 01:38:54.000000 lightmotif-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-17 14:53:09.000000 lightmotif-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-17 14:53:09.000000 lightmotif-0.2.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-17 14:53:09.000000 lightmotif-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-17 14:53:13.997680 lightmotif-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-05-17 14:53:09.000000 lightmotif-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.993680 lightmotif-0.2.0/lightmotif/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif/benches/
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/benches/ecoli.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/abc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/dense.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/err.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/num.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif/src/pli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif/src/pli/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/platform/avx2.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/platform/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/platform/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/platform/neon.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/platform/sse2.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/scores.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pwm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/seq.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/tests/dna.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif-py/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif-py/lightmotif/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/lightmotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/lightmotif/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif-py/lightmotif/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/lightmotif/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/lightmotif/tests/test_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/lightmotif/tests/unittest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-17 14:53:13.000000 lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-17 14:53:13.000000 lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:53:13.000000 lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 14:53:13.000000 lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:53:13.000000 lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 14:53:13.000000 lightmotif-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 14:53:13.997680 lightmotif-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-17 14:53:09.000000 lightmotif-0.2.0/setup.py
```

### Comparing `lightmotif-0.1.1/COPYING` & `lightmotif-0.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.1/PKG-INFO` & `lightmotif-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightmotif
-Version: 0.1.1
+Version: 0.2.0
 Summary: PyO3 bindings and Python interface to lightmotif, a library for platform-accelerated biological motif scanning using position weight matrices.
 Home-page: https://github.com/althonos/lightmotif
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/lightmotif/issues
 Project-URL: Changelog, https://github.com/althonos/lightmotif/blob/master/CHANGELOG.md
@@ -74,14 +74,15 @@
 - Compile-time definition of alphabets and matrix dimensions.
 - Sequence symbol encoding for fast table look-ups, as implemented in
   HMMER[\[1\]](#ref1) or MEME[\[2\]](#ref2)
 - Striped sequence matrices to process several positions in parallel,
   inspired by Michael Farrar[\[3\]](#ref3).
 - Vectorized matrix row look-up using `permute` instructions of [AVX2](https://fr.wikipedia.org/wiki/Advanced_Vector_Extensions).
 
+*This is the Python version, there is a [Rust crate](https://crates.io/crates/lightmotif) available as well.*
 
 ## 🔧 Installing
 
 `lightmotif` can be installed directly from [PyPI](https://pypi.org/project/lightmotif/),
 which hosts some pre-built wheels for most mainstream platforms, as well as the 
 code required to compile from source with Rust:
 ```console
@@ -129,17 +130,16 @@
 Benchmarks use the [MX000001](https://www.prodoric.de/matrix/MX000001.html)
 motif from [PRODORIC](https://www.prodoric.de/)[\[4\]](#ref4), and the
 [complete genome](https://www.ncbi.nlm.nih.gov/nuccore/U00096) of an
 *Escherichia coli K12* strain. 
 *Benchmarks were run on a [i7-10710U CPU](https://ark.intel.com/content/www/us/en/ark/products/196448/intel-core-i7-10710u-processor-12m-cache-up-to-4-70-ghz.html) running @1.10GHz, compiled with `--target-cpu=native`*.
 
 ```console
-lightmotif (avx2):      26,528,740 ns/iter (+/- 14,817,953) = 166.9 MiB/s
-lightmotif (generic):  654,599,309 ns/iter (+/- 81,292,868) =   6.8 MiB/s
-Bio.motifs:            526,309,061 ns/iter (+/- 45,603,991) =   8.4 MiB/s
+lightmotif (avx2):      9,125,495 ns/iter    (+/- 6,392,241) = 485.1 MiB/s
+Bio.motifs:           284,696,651 ns/iter    (+/- 6,454,945) =  15.5 MiB/s
 ```
 
 
 ## 💭 Feedback
 
 ### ⚠️ Issue Tracker
```

### Comparing `lightmotif-0.1.1/README.md` & `lightmotif-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/lightmotif/)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/lightmotif/)
 [![GitHub issues](https://img.shields.io/github/issues/althonos/lightmotif.svg?style=flat-square&maxAge=600)](https://github.com/althonos/lightmotif/issues)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/lightmotif/blob/master/CHANGELOG.md)
 
 ## 🗺️ Overview
 
-[Motif](https://en.wikipedia.org/wiki/Sequence_motif) scanning with 
+[Motif](https://en.wikipedia.org/wiki/Sequence_motif) scanning with
 [position weight matrices](https://en.wikipedia.org/wiki/Position_weight_matrix)
-(also known as position-specific scoring matrices) is a robust method for 
-identifying motifs of fixed length inside a 
-[biological sequence](https://en.wikipedia.org/wiki/Sequence_(biology)). They can be 
-used to identify [transcription factor](https://en.wikipedia.org/wiki/Transcription_factor) 
-[binding sites in DNA](https://en.wikipedia.org/wiki/DNA_binding_site), 
-or [protease](https://en.wikipedia.org/wiki/Protease) [cleavage](https://en.wikipedia.org/wiki/Proteolysis) site in [polypeptides](https://en.wikipedia.org/wiki/Proteolysis). 
+(also known as position-specific scoring matrices) is a robust method for
+identifying motifs of fixed length inside a
+[biological sequence](https://en.wikipedia.org/wiki/Sequence_(biology)). They can be
+used to identify [transcription factor](https://en.wikipedia.org/wiki/Transcription_factor)
+[binding sites in DNA](https://en.wikipedia.org/wiki/DNA_binding_site),
+or [protease](https://en.wikipedia.org/wiki/Protease) [cleavage](https://en.wikipedia.org/wiki/Proteolysis) site in [polypeptides](https://en.wikipedia.org/wiki/Proteolysis).
 Position weight matrices are often viewed as [sequence logos](https://en.wikipedia.org/wiki/Sequence_logo):
 
 [![MX000274.svg](https://raw.githubusercontent.com/althonos/lightmotif/main/docs/_static/prodoric_logo_mx000274.svg)](https://www.prodoric.de/matrix/MX000274.html)
 
 The `lightmotif` library provides a Rust crate to run very efficient
 searches for a motif encoded in a position weight matrix. The position
 scanning combines several techniques to allow high-throughput processing
@@ -34,72 +34,81 @@
 - Compile-time definition of alphabets and matrix dimensions.
 - Sequence symbol encoding for fast table look-ups, as implemented in
   HMMER[\[1\]](#ref1) or MEME[\[2\]](#ref2)
 - Striped sequence matrices to process several positions in parallel,
   inspired by Michael Farrar[\[3\]](#ref3).
 - Vectorized matrix row look-up using `permute` instructions of [AVX2](https://fr.wikipedia.org/wiki/Advanced_Vector_Extensions).
 
+*This is the Rust version, there is a [Python package](https://pypi.org/project/lightmotif) available as well.*
+
 ## 💡 Example
 
 ```rust
 use lightmotif::*;
+use typenum::U32;
 
 // Create a count matrix from an iterable of motif sequences
-let counts = CountMatrix::<Dna, {Dna::K}>::from_sequences(&[
+let counts = CountMatrix::<Dna>::from_sequences(&[
     EncodedSequence::encode("GTTGACCTTATCAAC").unwrap(),
     EncodedSequence::encode("GTTGATCCAGTCAAC").unwrap(),
 ]).unwrap();
 
 // Create a PSSM with 0.1 pseudocounts and uniform background frequencies.
 let pssm = counts.to_freq(0.1).to_scoring(None);
 
 // Encode the target sequence into a striped matrix
 let seq = "ATGTCCCAACAACGATACCCCGAGCCCATCGCCGTCATCGGCTCGGCATGCAGATTCCCAGGCG";
-let encoded = EncodedSequence::<Dna>::encode(seq).unwrap();
-let mut striped = encoded.to_striped::<32>();
+let encoded = EncodedSequence::encode(seq).unwrap();
+let mut striped = encoded.to_striped::<U32>();
 striped.configure(&pssm);
 
-// Use a pipeline to compute scores for every position of the matrix
-let scores = Pipeline::<Dna, f32>::score(&striped, &pssm);
+// Use a pipeline to compute scores for every position of the matrix.
+let pli = Pipeline::generic();
+let scores = pli.score(&striped, &pssm);
 
 // Scores can be extracted into a Vec<f32>, or indexed directly.
 let v = scores.to_vec();
 assert_eq!(scores[0], -23.07094);
 assert_eq!(v[0], -23.07094);
+
+// The highest scoring position can be searched with a pipeline as well.
+let best = pli.best_position(&scores).unwrap();
+assert_eq!(best, 18);
+
 ```
 
-To use the AVX2 implementation, simply create a `Pipeline<_, __m256>` instead
-of the `Pipeline<_, f32>`. This is only supported when the library is compiled
-with the `avx2` target feature, but it can be easily configured with Rust's
-`#[cfg]` attribute.
+Not specifying a vector type will cause the `Pipeline` to use the best
+vector type available based on the selected target features. To explicitly
+use the AVX2, SSSE3, or generic implementation, use `Pipeline<Dna, __m256i>`,
+`Pipeline<Dna, __m128i>`, or `Pipeline<Dna, u8>` respectively.
 
 ## ⏱️ Benchmarks
 
 Both benchmarks use the [MX000001](https://www.prodoric.de/matrix/MX000001.html)
 motif from [PRODORIC](https://www.prodoric.de/)[\[4\]](#ref4), and the
 [complete genome](https://www.ncbi.nlm.nih.gov/nuccore/U00096) of an
-*Escherichia coli K12* strain. 
+*Escherichia coli K12* strain.
 *Benchmarks were run on a [i7-10710U CPU](https://ark.intel.com/content/www/us/en/ark/products/196448/intel-core-i7-10710u-processor-12m-cache-up-to-4-70-ghz.html) running @1.10GHz, compiled with `--target-cpu=native`*.
 
 - Score every position of the genome with the motif weight matrix:
   ```console
   running 3 tests
-  test bench_avx2    ... bench:  13,053,752 ns/iter (+/- 45,411) = 355 MB/s
-  test bench_ssse3   ... bench:  37,203,277 ns/iter (+/- 2,416,572) = 124 MB/s
-  test bench_generic ... bench: 314,682,807 ns/iter (+/- 1,072,174) = 14 MB/s
+  test bench_avx2    ... bench:   6,948,169 ns/iter (+/- 16,477) = 668 MB/s
+  test bench_ssse3   ... bench:  29,079,674 ns/iter (+/- 875,880) = 159 MB/s
+  test bench_generic ... bench: 331,656,134 ns/iter (+/- 5,310,490) = 13 MB/s
   ```
 
 - Find the highest-scoring position for a motif in a 10kb sequence
   (compared to the PSSM algorithm implemented in
   [`bio::pattern_matching::pssm`](https://docs.rs/bio/1.1.0/bio/pattern_matching/pssm/index.html)):
   ```console
-  test bench_avx2    ... bench:      46,390 ns/iter (+/- 115) = 215 MB/s
-  test bench_ssse3   ... bench:      97,691 ns/iter (+/- 2,720) = 102 MB/s
-  test bench_generic ... bench:     740,305 ns/iter (+/- 2,527) = 13 MB/s
-  test bench_bio     ... bench:   1,575,504 ns/iter (+/- 2,799) = 6 MB/s
+  test bench_avx2    ... bench:      49,259 ns/iter (+/- 1,489) = 203 MB/s
+  test bench_bio     ... bench:   1,440,705 ns/iter (+/- 5,291) = 6 MB/s
+  test bench_generic ... bench:     706,361 ns/iter (+/- 1,726) = 14 MB/s
+  test bench_sssee   ... bench:      94,152 ns/iter (+/- 36) = 106 MB/s
   ```
 
 
 ## 💭 Feedback
 
 ### ⚠️ Issue Tracker
```

### Comparing `lightmotif-0.1.1/lightmotif/README.md` & `lightmotif-0.2.0/lightmotif/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/lightmotif/)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/lightmotif/)
 [![GitHub issues](https://img.shields.io/github/issues/althonos/lightmotif.svg?style=flat-square&maxAge=600)](https://github.com/althonos/lightmotif/issues)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/lightmotif/blob/master/CHANGELOG.md)
 
 ## 🗺️ Overview
 
-[Motif](https://en.wikipedia.org/wiki/Sequence_motif) scanning with 
+[Motif](https://en.wikipedia.org/wiki/Sequence_motif) scanning with
 [position weight matrices](https://en.wikipedia.org/wiki/Position_weight_matrix)
-(also known as position-specific scoring matrices) is a robust method for 
-identifying motifs of fixed length inside a 
-[biological sequence](https://en.wikipedia.org/wiki/Sequence_(biology)). They can be 
-used to identify [transcription factor](https://en.wikipedia.org/wiki/Transcription_factor) 
-[binding sites in DNA](https://en.wikipedia.org/wiki/DNA_binding_site), 
-or [protease](https://en.wikipedia.org/wiki/Protease) [cleavage](https://en.wikipedia.org/wiki/Proteolysis) site in [polypeptides](https://en.wikipedia.org/wiki/Proteolysis). 
+(also known as position-specific scoring matrices) is a robust method for
+identifying motifs of fixed length inside a
+[biological sequence](https://en.wikipedia.org/wiki/Sequence_(biology)). They can be
+used to identify [transcription factor](https://en.wikipedia.org/wiki/Transcription_factor)
+[binding sites in DNA](https://en.wikipedia.org/wiki/DNA_binding_site),
+or [protease](https://en.wikipedia.org/wiki/Protease) [cleavage](https://en.wikipedia.org/wiki/Proteolysis) site in [polypeptides](https://en.wikipedia.org/wiki/Proteolysis).
 Position weight matrices are often viewed as [sequence logos](https://en.wikipedia.org/wiki/Sequence_logo):
 
 [![MX000274.svg](https://raw.githubusercontent.com/althonos/lightmotif/main/docs/_static/prodoric_logo_mx000274.svg)](https://www.prodoric.de/matrix/MX000274.html)
 
 The `lightmotif` library provides a Rust crate to run very efficient
 searches for a motif encoded in a position weight matrix. The position
 scanning combines several techniques to allow high-throughput processing
@@ -34,72 +34,81 @@
 - Compile-time definition of alphabets and matrix dimensions.
 - Sequence symbol encoding for fast table look-ups, as implemented in
   HMMER[\[1\]](#ref1) or MEME[\[2\]](#ref2)
 - Striped sequence matrices to process several positions in parallel,
   inspired by Michael Farrar[\[3\]](#ref3).
 - Vectorized matrix row look-up using `permute` instructions of [AVX2](https://fr.wikipedia.org/wiki/Advanced_Vector_Extensions).
 
+*This is the Rust version, there is a [Python package](https://pypi.org/project/lightmotif) available as well.*
+
 ## 💡 Example
 
 ```rust
 use lightmotif::*;
+use typenum::U32;
 
 // Create a count matrix from an iterable of motif sequences
-let counts = CountMatrix::<Dna, {Dna::K}>::from_sequences(&[
+let counts = CountMatrix::<Dna>::from_sequences(&[
     EncodedSequence::encode("GTTGACCTTATCAAC").unwrap(),
     EncodedSequence::encode("GTTGATCCAGTCAAC").unwrap(),
 ]).unwrap();
 
 // Create a PSSM with 0.1 pseudocounts and uniform background frequencies.
 let pssm = counts.to_freq(0.1).to_scoring(None);
 
 // Encode the target sequence into a striped matrix
 let seq = "ATGTCCCAACAACGATACCCCGAGCCCATCGCCGTCATCGGCTCGGCATGCAGATTCCCAGGCG";
-let encoded = EncodedSequence::<Dna>::encode(seq).unwrap();
-let mut striped = encoded.to_striped::<32>();
+let encoded = EncodedSequence::encode(seq).unwrap();
+let mut striped = encoded.to_striped::<U32>();
 striped.configure(&pssm);
 
-// Use a pipeline to compute scores for every position of the matrix
-let scores = Pipeline::<Dna, f32>::score(&striped, &pssm);
+// Use a pipeline to compute scores for every position of the matrix.
+let pli = Pipeline::generic();
+let scores = pli.score(&striped, &pssm);
 
 // Scores can be extracted into a Vec<f32>, or indexed directly.
 let v = scores.to_vec();
 assert_eq!(scores[0], -23.07094);
 assert_eq!(v[0], -23.07094);
+
+// The highest scoring position can be searched with a pipeline as well.
+let best = pli.best_position(&scores).unwrap();
+assert_eq!(best, 18);
+
 ```
 
-To use the AVX2 implementation, simply create a `Pipeline<_, __m256>` instead
-of the `Pipeline<_, f32>`. This is only supported when the library is compiled
-with the `avx2` target feature, but it can be easily configured with Rust's
-`#[cfg]` attribute.
+Not specifying a vector type will cause the `Pipeline` to use the best
+vector type available based on the selected target features. To explicitly
+use the AVX2, SSSE3, or generic implementation, use `Pipeline<Dna, __m256i>`,
+`Pipeline<Dna, __m128i>`, or `Pipeline<Dna, u8>` respectively.
 
 ## ⏱️ Benchmarks
 
 Both benchmarks use the [MX000001](https://www.prodoric.de/matrix/MX000001.html)
 motif from [PRODORIC](https://www.prodoric.de/)[\[4\]](#ref4), and the
 [complete genome](https://www.ncbi.nlm.nih.gov/nuccore/U00096) of an
-*Escherichia coli K12* strain. 
+*Escherichia coli K12* strain.
 *Benchmarks were run on a [i7-10710U CPU](https://ark.intel.com/content/www/us/en/ark/products/196448/intel-core-i7-10710u-processor-12m-cache-up-to-4-70-ghz.html) running @1.10GHz, compiled with `--target-cpu=native`*.
 
 - Score every position of the genome with the motif weight matrix:
   ```console
   running 3 tests
-  test bench_avx2    ... bench:  13,053,752 ns/iter (+/- 45,411) = 355 MB/s
-  test bench_ssse3   ... bench:  37,203,277 ns/iter (+/- 2,416,572) = 124 MB/s
-  test bench_generic ... bench: 314,682,807 ns/iter (+/- 1,072,174) = 14 MB/s
+  test bench_avx2    ... bench:   6,948,169 ns/iter (+/- 16,477) = 668 MB/s
+  test bench_ssse3   ... bench:  29,079,674 ns/iter (+/- 875,880) = 159 MB/s
+  test bench_generic ... bench: 331,656,134 ns/iter (+/- 5,310,490) = 13 MB/s
   ```
 
 - Find the highest-scoring position for a motif in a 10kb sequence
   (compared to the PSSM algorithm implemented in
   [`bio::pattern_matching::pssm`](https://docs.rs/bio/1.1.0/bio/pattern_matching/pssm/index.html)):
   ```console
-  test bench_avx2    ... bench:      46,390 ns/iter (+/- 115) = 215 MB/s
-  test bench_ssse3   ... bench:      97,691 ns/iter (+/- 2,720) = 102 MB/s
-  test bench_generic ... bench:     740,305 ns/iter (+/- 2,527) = 13 MB/s
-  test bench_bio     ... bench:   1,575,504 ns/iter (+/- 2,799) = 6 MB/s
+  test bench_avx2    ... bench:      49,259 ns/iter (+/- 1,489) = 203 MB/s
+  test bench_bio     ... bench:   1,440,705 ns/iter (+/- 5,291) = 6 MB/s
+  test bench_generic ... bench:     706,361 ns/iter (+/- 1,726) = 14 MB/s
+  test bench_sssee   ... bench:      94,152 ns/iter (+/- 36) = 106 MB/s
   ```
 
 
 ## 💭 Feedback
 
 ### ⚠️ Issue Tracker
```

### Comparing `lightmotif-0.1.1/lightmotif/src/abc.rs` & `lightmotif-0.2.0/lightmotif/src/seq.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,238 +1,226 @@
-use std::fmt::Debug;
+//! Linear and striped storage for alphabet-encoded sequences.
 
-use super::err::InvalidData;
+use std::fmt::Display;
+use std::fmt::Formatter;
+use std::fmt::Result as FmtResult;
+use std::str::FromStr;
+
+use typenum::marker_traits::NonZero;
+use typenum::marker_traits::Unsigned;
+
+use super::abc::Alphabet;
+use super::abc::Symbol;
+use super::dense::DenseMatrix;
 use super::err::InvalidSymbol;
+use super::num::StrictlyPositive;
+use super::pwm::ScoringMatrix;
 
-// --- Symbol ------------------------------------------------------------------
+// --- EncodedSequence ---------------------------------------------------------
 
-/// Common traits for a biological symbol.
-pub trait Symbol: Default + Sized + Copy {
-    /// View this symbol as a zero-based index.
-    fn as_index(&self) -> usize;
-    /// View this symbol as a string character.
-    fn as_char(&self) -> char;
-    /// Parse a string character into a symbol.
-    fn from_char(c: char) -> Result<Self, InvalidSymbol>;
-}
-
-/// A deoxyribonucleotide.
-#[derive(Clone, Copy, PartialEq, Debug)]
-#[repr(u8)]
-pub enum Nucleotide {
-    /// Adenine.
-    A = 0,
-    /// Cytosine.
-    C = 1,
-    /// Thymine.
-    T = 2,
-    /// Guanine.
-    G = 3,
-    /// Unknown base.
-    N = 4,
+/// A biological sequence encoded with an alphabet.
+#[derive(Clone, Debug)]
+pub struct EncodedSequence<A: Alphabet> {
+    alphabet: std::marker::PhantomData<A>,
+    data: Vec<A::Symbol>,
 }
 
-impl Symbol for Nucleotide {
-    fn as_index(&self) -> usize {
-        *self as usize
+impl<A: Alphabet> EncodedSequence<A> {
+    /// Create a new encoded sequence.
+    pub fn new(data: Vec<A::Symbol>) -> Self {
+        Self {
+            data,
+            alphabet: std::marker::PhantomData,
+        }
     }
 
-    fn as_char(&self) -> char {
-        match self {
-            Nucleotide::A => 'A',
-            Nucleotide::C => 'C',
-            Nucleotide::T => 'T',
-            Nucleotide::G => 'G',
-            Nucleotide::N => 'N',
+    /// Create a new encoded sequence from a textual representation.
+    pub fn encode(sequence: &str) -> Result<Self, InvalidSymbol> {
+        sequence
+            .chars()
+            .map(A::Symbol::from_char)
+            .collect::<Result<_, _>>()
+            .map(Self::new)
+    }
+
+    /// Return the number of symbols in the sequence.
+    #[inline]
+    pub fn len(&self) -> usize {
+        self.data.len()
+    }
+
+    /// Iterate over the symbols in the sequence.
+    #[inline]
+    pub fn iter(&self) -> impl IntoIterator<Item = &A::Symbol> {
+        self.data.iter()
+    }
+
+    /// Convert the encoded sequence to a striped matrix.
+    pub fn to_striped<C: Unsigned + NonZero>(&self) -> StripedSequence<A, C> {
+        let length = self.data.len();
+        let n = (length + (C::USIZE - 1)) / C::USIZE;
+        let mut data = DenseMatrix::new(n);
+        for (i, &x) in self.data.iter().enumerate() {
+            data[i % n][i / n] = x;
+        }
+        StripedSequence {
+            alphabet: std::marker::PhantomData,
+            data,
+            length,
+            wrap: 0,
         }
     }
 
-    fn from_char(c: char) -> Result<Self, InvalidSymbol> {
-        match c {
-            'A' => Ok(Nucleotide::A),
-            'C' => Ok(Nucleotide::C),
-            'T' => Ok(Nucleotide::T),
-            'G' => Ok(Nucleotide::G),
-            'N' => Ok(Nucleotide::N),
-            _ => Err(InvalidSymbol(c)),
+    /// Convert the encoded sequence back to its textual representation.
+    pub fn to_string(&self) -> String {
+        let mut s = String::with_capacity(self.len());
+        for c in self.data.iter() {
+            s.push(c.as_char());
         }
+        s
     }
 }
 
-impl From<Nucleotide> for char {
-    fn from(n: Nucleotide) -> char {
-        n.as_char()
+impl<A: Alphabet> AsRef<EncodedSequence<A>> for EncodedSequence<A> {
+    fn as_ref(&self) -> &Self {
+        self
     }
 }
 
-impl Default for Nucleotide {
-    fn default() -> Nucleotide {
-        Nucleotide::N
+impl<A: Alphabet> AsRef<[<A as Alphabet>::Symbol]> for EncodedSequence<A> {
+    fn as_ref(&self) -> &[<A as Alphabet>::Symbol] {
+        self.data.as_slice()
     }
 }
 
-// --- Alphabet ----------------------------------------------------------------
-
-/// Common traits for a biological alphabet.
-pub trait Alphabet: Debug + Copy + Default + 'static {
-    type Symbol: Symbol;
-    const K: usize;
+impl<A: Alphabet> Display for EncodedSequence<A> {
+    fn fmt(&self, f: &mut Formatter) -> FmtResult {
+        for c in self.data.iter() {
+            write!(f, "{}", c.as_char())?;
+        }
+        Ok(())
+    }
+}
 
-    /// Get the default symbol for this alphabet.
-    fn default_symbol() -> Self::Symbol {
-        Default::default()
+impl<A: Alphabet> FromStr for EncodedSequence<A> {
+    type Err = InvalidSymbol;
+    fn from_str(seq: &str) -> Result<Self, Self::Err> {
+        Self::encode(seq)
     }
 }
 
-/// The standard DNA alphabet composed of 4 deoxyribonucleotides and a wildcard.
-#[derive(Default, Debug, Clone, Copy)]
-pub struct Dna;
+impl<'a, A: Alphabet> IntoIterator for &'a EncodedSequence<A> {
+    type Item = &'a A::Symbol;
+    type IntoIter = std::slice::Iter<'a, A::Symbol>;
 
-impl Alphabet for Dna {
-    type Symbol = Nucleotide;
-    const K: usize = 5;
+    fn into_iter(self) -> Self::IntoIter {
+        self.data.iter()
+    }
 }
 
-// --- Background --------------------------------------------------------------
+// --- StripedSequence ---------------------------------------------------------
 
-/// The background frequencies for an alphabet.
+/// An encoded sequence stored in a striped matrix with a fixed column count.
 #[derive(Clone, Debug)]
-pub struct Background<A: Alphabet, const K: usize> {
-    frequencies: [f32; K],
+pub struct StripedSequence<A: Alphabet, C: StrictlyPositive> {
     alphabet: std::marker::PhantomData<A>,
+    pub length: usize,
+    pub wrap: usize,
+    pub data: DenseMatrix<A::Symbol, C>,
 }
 
-impl<A: Alphabet, const K: usize> Background<A, K> {
-    /// Create a new background with the given frequencies.
-    ///
-    /// The array must contain valid frequencies, i.e. real numbers between
-    /// zero and one that sum to one.
-    pub fn new(frequencies: [f32; K]) -> Result<Self, InvalidData> {
-        let mut sum = 0.0;
-        for &f in frequencies.iter() {
-            if f < 0.0 || f > 1.0 {
-                return Err(InvalidData);
-            }
-            sum += f;
-        }
-        if sum != 1.0 {
-            return Err(InvalidData);
+impl<A: Alphabet, C: StrictlyPositive> StripedSequence<A, C> {
+    /// Create a new striped sequence from a textual representation.
+    pub fn encode(sequence: &str) -> Result<Self, InvalidSymbol> {
+        let length = sequence.len();
+        let n = (length + (C::USIZE - 1)) / C::USIZE;
+        let mut data = DenseMatrix::new(n);
+        for (i, x) in sequence.chars().enumerate() {
+            data[i % n][i / n] = A::Symbol::from_char(x)?;
         }
-        Ok(Self {
-            frequencies,
+        Ok(StripedSequence {
             alphabet: std::marker::PhantomData,
+            data,
+            length,
+            wrap: 0,
         })
     }
 
-    /// Create a new background with uniform frequencies.
-    ///
-    /// The non-default symbols from the alphabet `A` will be initialized
-    /// with a frequency of `1/(K-1)`, while the default symbol will remain
-    /// with a zero frequency.
-    ///
-    /// # Note
-    /// The `Default` implementation for `Background` uses uniform frequencies.
-    ///
-    /// # Example
-    /// ```
-    /// # use lightmotif::*;
-    /// let bg = Background::<Dna, { Dna::K }>::uniform();
-    /// assert_eq!(bg.frequencies(), &[0.25, 0.25, 0.25, 0.25, 0.0]);
-    /// ```
-    pub fn uniform() -> Self {
-        let mut frequencies = [0.0; K];
-        for i in 0..K {
-            if i != A::default_symbol().as_index() {
-                frequencies[i] = 1.0 / ((K - 1) as f32);
-            }
-        }
-        Self {
-            frequencies,
-            alphabet: std::marker::PhantomData,
+    /// Reconfigure the striped sequence for searching with a motif.
+    pub fn configure(&mut self, motif: &ScoringMatrix<A>) {
+        if motif.len() > 0 {
+            self.configure_wrap(motif.len() - 1);
         }
     }
 
-    /// A reference to the raw background frequencies.
-    pub fn frequencies(&self) -> &[f32; K] {
-        &self.frequencies
-    }
-}
-
-impl<A: Alphabet, const K: usize> AsRef<[f32; K]> for Background<A, K> {
-    fn as_ref(&self) -> &[f32; K] {
-        &self.frequencies
-    }
-}
-
-impl<A: Alphabet, const K: usize> Default for Background<A, K> {
-    fn default() -> Self {
-        Self::uniform()
-    }
-}
-
-// --- Pseudocounts ------------------------------------------------------------
-
-/// A structure for storing the pseudocounts over an alphabet.
-#[derive(Clone, Debug)]
-pub struct Pseudocounts<A: Alphabet, const K: usize> {
-    alphabet: std::marker::PhantomData<A>,
-    counts: [f32; K],
-}
-
-impl<A: Alphabet, const K: usize> Pseudocounts<A, K> {
-    pub fn counts(&self) -> &[f32; K] {
-        &self.counts
-    }
-}
-
-impl<A: Alphabet, const K: usize> Default for Pseudocounts<A, K> {
-    fn default() -> Self {
-        Self::from([0.0; K])
-    }
-}
-
-impl<A: Alphabet, const K: usize> From<[f32; K]> for Pseudocounts<A, K> {
-    fn from(counts: [f32; K]) -> Self {
-        Self {
-            alphabet: std::marker::PhantomData,
-            counts,
+    /// Add wrap-around rows for a motif of length `m`.
+    pub fn configure_wrap(&mut self, m: usize) {
+        if m > self.wrap {
+            let rows = self.data.rows() - self.wrap;
+            self.data.resize(self.data.rows() + m - self.wrap);
+            for i in 0..m {
+                for j in 0..C::USIZE - 1 {
+                    self.data[rows + i][j] = self.data[i][j + 1];
+                }
+            }
+            self.wrap = m;
         }
     }
 }
 
-impl<A: Alphabet, const K: usize> From<f32> for Pseudocounts<A, K> {
-    fn from(count: f32) -> Self {
-        let mut counts: [f32; K] = [0.0; K];
-        for i in 0..K {
-            if i != A::default_symbol().as_index() {
-                counts[i] = count;
-            }
-        }
-        Self {
-            counts,
-            alphabet: std::marker::PhantomData,
-        }
+impl<A: Alphabet, C: StrictlyPositive> AsRef<StripedSequence<A, C>> for StripedSequence<A, C> {
+    fn as_ref(&self) -> &Self {
+        self
     }
 }
 
-impl<A: Alphabet, const K: usize> AsRef<[f32; K]> for Pseudocounts<A, K> {
-    fn as_ref(&self) -> &[f32; K] {
-        &self.counts
+impl<A: Alphabet, C: StrictlyPositive> From<EncodedSequence<A>> for StripedSequence<A, C> {
+    fn from(encoded: EncodedSequence<A>) -> Self {
+        encoded.to_striped()
     }
 }
 
-impl<A: Alphabet, const K: usize> AsMut<[f32; K]> for Pseudocounts<A, K> {
-    fn as_mut(&mut self) -> &mut [f32; K] {
-        &mut self.counts
+impl<A: Alphabet, C: StrictlyPositive> FromStr for StripedSequence<A, C> {
+    type Err = InvalidSymbol;
+    fn from_str(seq: &str) -> Result<Self, Self::Err> {
+        Self::encode(seq)
     }
 }
 
 #[cfg(test)]
 mod test {
+    use typenum::consts::U2;
+    use typenum::consts::U4;
+
     use super::*;
 
+    use crate::abc::Dna;
+    use crate::abc::Nucleotide::*;
+
+    #[test]
+    fn test_stripe() {
+        let seq = EncodedSequence::<Dna>::from_str("ATGCA").unwrap();
+        let striped = seq.to_striped::<U4>();
+        assert_eq!(striped.data.rows(), 2);
+        assert_eq!(&striped.data[0], &[A, G, A, N]);
+        assert_eq!(&striped.data[1], &[T, C, N, N]);
+
+        let striped = seq.to_striped::<U2>();
+        assert_eq!(striped.data.rows(), 3);
+        assert_eq!(&striped.data[0], &[A, C,]);
+        assert_eq!(&striped.data[1], &[T, A,]);
+        assert_eq!(&striped.data[2], &[G, N,]);
+    }
+
     #[test]
-    fn test_background_new() {
-        assert!(Background::<Dna, { Dna::K }>::new([0.3, 0.2, 0.2, 0.3, 0.0]).is_ok());
-        assert!(Background::<Dna, { Dna::K }>::new([0.1, 0.1, 0.1, 0.1, 0.0]).is_err());
+    fn test_configure_wrap() {
+        let seq = EncodedSequence::<Dna>::from_str("ATGCA").unwrap();
+        let mut striped = seq.to_striped::<U4>();
+
+        striped.configure_wrap(2);
+        assert_eq!(striped.data.rows(), 4);
+        assert_eq!(&striped.data[0], &[A, G, A, N]);
+        assert_eq!(&striped.data[1], &[T, C, N, N]);
+        assert_eq!(&striped.data[2], &[G, A, N, N]);
+        assert_eq!(&striped.data[3], &[C, N, N, N]);
     }
 }
```

### Comparing `lightmotif-0.1.1/lightmotif/src/dense.rs` & `lightmotif-0.2.0/lightmotif/src/dense.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,85 @@
+//! Dense matrix storage with automatic memory alignment.
+
+use std::iter::ExactSizeIterator;
+use std::iter::FusedIterator;
 use std::ops::Index;
 use std::ops::IndexMut;
 use std::ptr::NonNull;
 
-use std::iter::ExactSizeIterator;
-use std::iter::FusedIterator;
+use typenum::marker_traits::Unsigned;
 
 // --- DenseMatrix -------------------------------------------------------------
 
 /// An aligned dense matrix of with a constant number of columns.
 #[derive(Debug, Clone)]
-pub struct DenseMatrix<T: Default + Copy, const C: usize = 32> {
+pub struct DenseMatrix<T: Default + Copy, C: Unsigned> {
     data: Vec<T>,
     indices: Vec<usize>,
+    _columns: std::marker::PhantomData<C>,
 }
 
-impl<T: Default + Copy, const C: usize> DenseMatrix<T, C> {
+impl<T: Default + Copy, C: Unsigned> DenseMatrix<T, C> {
     /// Create a new matrix with the given number of rows.
     pub fn new(rows: usize) -> Self {
         let data = Vec::new();
         let indices = Vec::new();
-        let mut matrix = Self { data, indices };
+        let mut matrix = Self {
+            data,
+            indices,
+            _columns: std::marker::PhantomData,
+        };
         matrix.resize(rows);
         matrix
     }
 
+    /// Create a new *uninitialized* matrix with the given number of rows.
+    pub unsafe fn uninitialized(rows: usize) -> Self {
+        // alway over-allocate columns to avoid alignment issues.
+        let c = C::USIZE.next_power_of_two();
+
+        // NOTE: this is unsafe but given that we require `T` to be
+        //       copy, this should be fine, as `Copy` prevents the
+        //       type to be `Dorp` as well.
+        // reserve the vector without initializing the data
+        let mut data = Vec::with_capacity((rows + 1) * c);
+        data.set_len((rows + 1) * c);
+
+        // compute offset to aligned memory
+        let mut offset = 0;
+        while data[offset..].as_ptr() as usize % c > 0 {
+            offset += 1
+        }
+
+        // record indices to each rows
+        let indices = (0..rows).map(|i| offset + i * c).collect();
+
+        Self {
+            data,
+            indices,
+            _columns: std::marker::PhantomData,
+        }
+    }
+
     /// The number of columns of the matrix.
     #[inline]
     pub const fn columns(&self) -> usize {
-        C
+        C::USIZE
     }
 
     /// The number of rows of the matrix.
     #[inline]
     pub fn rows(&self) -> usize {
         self.indices.len()
     }
 
     /// Change the number of rows of the matrix.
     pub fn resize(&mut self, rows: usize) {
         // alway over-allocate columns to avoid alignment issues.
-        let c = C.next_power_of_two();
+        let c = C::USIZE.next_power_of_two();
 
         //
         let previous_rows = self.rows();
         let previous_offset = if self.rows() == 0 { 0 } else { self.indices[0] };
 
         // allocate data block
         self.data.resize_with((rows + 1) * c, T::default);
@@ -78,146 +114,166 @@
     /// Returns an iterator that allows modifying each row.
     #[inline]
     pub fn iter_mut(&mut self) -> IterMut<'_, T, C> {
         IterMut::new(self)
     }
 }
 
-impl<T: Default + Copy, const C: usize> Index<usize> for DenseMatrix<T, C> {
+impl<T: Default + Copy, C: Unsigned> Index<usize> for DenseMatrix<T, C> {
     type Output = [T];
     #[inline]
     fn index(&self, index: usize) -> &Self::Output {
         let row = self.indices[index];
-        &self.data[row..row + C]
+        &self.data[row..row + C::USIZE]
     }
 }
 
-impl<T: Default + Copy, const C: usize> IndexMut<usize> for DenseMatrix<T, C> {
+impl<T: Default + Copy, C: Unsigned> IndexMut<usize> for DenseMatrix<T, C> {
     #[inline]
     fn index_mut(&mut self, index: usize) -> &mut Self::Output {
         let row = self.indices[index];
-        &mut self.data[row..row + C]
+        &mut self.data[row..row + C::USIZE]
     }
 }
 
-impl<'a, T: Default + Copy, const C: usize> IntoIterator for &'a DenseMatrix<T, C> {
+impl<'a, T: Default + Copy, C: Unsigned> IntoIterator for &'a DenseMatrix<T, C> {
     type Item = &'a [T];
     type IntoIter = Iter<'a, T, C>;
     fn into_iter(self) -> Self::IntoIter {
         Iter::new(self)
     }
 }
 
-impl<'a, T: Default + Copy, const C: usize> IntoIterator for &'a mut DenseMatrix<T, C> {
+impl<'a, T: Default + Copy, C: Unsigned> IntoIterator for &'a mut DenseMatrix<T, C> {
     type Item = &'a mut [T];
     type IntoIter = IterMut<'a, T, C>;
     fn into_iter(self) -> Self::IntoIter {
         IterMut::new(self)
     }
 }
 
 // --- Iter --------------------------------------------------------------------
 
-pub struct Iter<'a, T, const C: usize>
+pub struct Iter<'a, T, C>
 where
     T: 'a + Default + Copy,
+    C: Unsigned,
 {
     indices: std::slice::Iter<'a, usize>,
     data: std::ptr::NonNull<T>,
+    _columns: std::marker::PhantomData<C>,
 }
 
-impl<'a, T, const C: usize> Iter<'a, T, C>
+impl<'a, T, C> Iter<'a, T, C>
 where
     T: 'a + Default + Copy,
+    C: Unsigned,
 {
     fn new(matrix: &'a DenseMatrix<T, C>) -> Self {
         let indices = matrix.indices.iter();
         let data = unsafe { NonNull::new_unchecked(matrix.data.as_ptr() as *mut T) };
-        Self { indices, data }
+        Self {
+            indices,
+            data,
+            _columns: std::marker::PhantomData,
+        }
     }
 
     fn get(&mut self, i: usize) -> &'a [T] {
-        unsafe { std::slice::from_raw_parts(self.data.as_ptr().add(i), C) }
+        unsafe { std::slice::from_raw_parts(self.data.as_ptr().add(i), C::USIZE) }
     }
 }
 
 // --- IterMut -----------------------------------------------------------------
 
-pub struct IterMut<'a, T, const C: usize>
+pub struct IterMut<'a, T, C>
 where
     T: 'a + Default + Copy,
+    C: Unsigned,
 {
     indices: std::slice::Iter<'a, usize>,
     data: std::ptr::NonNull<T>,
+    _columns: std::marker::PhantomData<C>,
 }
 
-impl<'a, T, const C: usize> IterMut<'a, T, C>
+impl<'a, T, C> IterMut<'a, T, C>
 where
     T: 'a + Default + Copy,
+    C: Unsigned,
 {
     fn new(matrix: &'a mut DenseMatrix<T, C>) -> Self {
         let indices = matrix.indices.iter();
         let data = unsafe { NonNull::new_unchecked(matrix.data.as_mut_ptr()) };
-        Self { indices, data }
+        Self {
+            indices,
+            data,
+            _columns: std::marker::PhantomData,
+        }
     }
 
     fn get(&mut self, i: usize) -> &'a mut [T] {
-        unsafe { std::slice::from_raw_parts_mut(self.data.as_ptr().add(i), C) }
+        unsafe { std::slice::from_raw_parts_mut(self.data.as_ptr().add(i), C::USIZE) }
     }
 }
 
 // --- iterator ----------------------------------------------------------------
 
 macro_rules! iterator {
     ($t:ident, $T:ident, $($item:tt)*) => {
-        impl<'a, $T, const C: usize> Iterator for $t<'a, $T, C>
+        impl<'a, $T, C> Iterator for $t<'a, $T, C>
         where
             $T: Default + Copy,
+            C: Unsigned,
         {
             type Item = &'a $($item)*;
             fn next(&mut self) -> Option<Self::Item> {
                 self.indices.next().map(|&i| self.get(i))
             }
         }
 
-        impl<'a, $T, const C: usize> ExactSizeIterator for $t<'a, $T, C>
+        impl<'a, $T, C> ExactSizeIterator for $t<'a, $T, C>
         where
             $T: Default + Copy,
+            C: Unsigned,
         {
             fn len(&self) -> usize {
                 self.indices.len()
             }
         }
 
-        impl<'a, $T, const C: usize> FusedIterator for $t<'a, $T, C>
+        impl<'a, $T, C> FusedIterator for $t<'a, $T, C>
         where
-            $T: Default + Copy
+            $T: Default + Copy,
+            C: Unsigned,
         {}
 
-        impl<'a, $T, const C: usize> DoubleEndedIterator for $t<'a, $T, C>
+        impl<'a, $T, C> DoubleEndedIterator for $t<'a, $T, C>
         where
-            $T: Default + Copy
+            $T: Default + Copy,
+            C: Unsigned,
         {
             fn next_back(&mut self) -> Option<Self::Item> {
                 self.indices.next_back().map(|&i| self.get(i))
             }
         }
     };
 }
 
 iterator!(Iter, T, [T]);
 iterator!(IterMut, T, mut [T]);
 
 #[cfg(test)]
 mod test {
+    use typenum::consts::U32;
+
     use super::*;
 
     #[test]
     fn test_resize() {
-        let mut dense = DenseMatrix::<u64, 32>::new(4);
+        let mut dense = DenseMatrix::<u64, U32>::new(4);
 
         for i in 0..4 {
             dense[i][0] = (i + 1) as u64;
         }
         assert_eq!(dense[0][0], 1);
         assert_eq!(dense[1][0], 2);
         assert_eq!(dense[2][0], 3);
@@ -237,15 +293,15 @@
         assert_eq!(dense[2][0], 3);
         assert_eq!(dense[3][0], 4);
         assert_eq!(dense[0].as_ptr() as usize % 4, 0);
     }
 
     #[test]
     fn test_iter_mut() {
-        let mut dense = DenseMatrix::<u64, 32>::new(4);
+        let mut dense = DenseMatrix::<u64, U32>::new(4);
         for i in 0..4 {
             dense[i][0] = (i + 1) as u64;
         }
         assert_eq!(dense[0][0], 1);
         assert_eq!(dense[1][0], 2);
         assert_eq!(dense[2][0], 3);
         assert_eq!(dense[3][0], 4);
```

### Comparing `lightmotif-0.1.1/lightmotif/src/err.rs` & `lightmotif-0.2.0/lightmotif/src/err.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+//! Error traits for failible operations in the library.
+
 use std::error::Error;
 use std::fmt::Display;
 use std::fmt::Error as FmtError;
 use std::fmt::Formatter;
 
 /// The given character is not a valid symbol.
 #[derive(Clone, Debug)]
@@ -22,7 +24,19 @@
 impl Display for InvalidData {
     fn fmt(&self, f: &mut Formatter<'_>) -> Result<(), FmtError> {
         f.write_str("invalid data found")
     }
 }
 
 impl Error for InvalidData {}
+
+/// The requested backend is unsupported on the host platform.
+#[derive(Debug, Clone)]
+pub struct UnsupportedBackend;
+
+impl Display for UnsupportedBackend {
+    fn fmt(&self, f: &mut Formatter<'_>) -> Result<(), FmtError> {
+        f.write_str("unsupported backend for the host platform")
+    }
+}
+
+impl Error for UnsupportedBackend {}
```

### Comparing `lightmotif-0.1.1/lightmotif/src/pwm.rs` & `lightmotif-0.2.0/lightmotif/src/pwm.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,49 @@
+//! Storage types for the different stages of a PSSM construction.
+
+use typenum::marker_traits::Unsigned;
+
 use super::abc::Alphabet;
 use super::abc::Background;
+use super::abc::ComplementableAlphabet;
 use super::abc::Pseudocounts;
 use super::abc::Symbol;
 use super::dense::DenseMatrix;
 use super::err::InvalidData;
 use super::seq::EncodedSequence;
 
 // --- CountMatrix -------------------------------------------------------------
 
 /// A matrix storing symbol occurences at each position.
 #[derive(Clone, Debug)]
-pub struct CountMatrix<A: Alphabet, const K: usize> {
+pub struct CountMatrix<A: Alphabet> {
     /// The alphabet of the count matrix.
     alphabet: std::marker::PhantomData<A>,
     /// The actual counts for each position of the motif.
-    data: DenseMatrix<u32, K>,
+    data: DenseMatrix<u32, A::K>,
     /// The number of sequences from which this count matrix was obtained.
     #[allow(unused)]
     n: u32,
 }
 
-impl<A: Alphabet, const K: usize> CountMatrix<A, K> {
+impl<A: Alphabet> CountMatrix<A> {
     /// Create a new count matrix without checking the contents.
-    fn new_unchecked(data: DenseMatrix<u32, K>, n: u32) -> Self {
+    fn new_unchecked(data: DenseMatrix<u32, A::K>, n: u32) -> Self {
         Self {
             alphabet: std::marker::PhantomData,
             n,
             data,
         }
     }
 
     /// Create a new count matrix from the given data.
     ///
     /// The matrix must contain count data, for sequences of the same
     /// length, i.e. rows should all sum to the same value.
-    pub fn new(data: DenseMatrix<u32, K>) -> Result<Self, InvalidData> {
+    pub fn new(data: DenseMatrix<u32, A::K>) -> Result<Self, InvalidData> {
         // Empty matrices contain valid data.
         if data.rows() == 0 {
             return Ok(Self::new_unchecked(data, 0));
         }
         // Check row sums.
         let n = data.iter().map(|row| row.iter().sum()).max().unwrap();
         Ok(Self::new_unchecked(data, n))
@@ -72,193 +77,234 @@
         match data {
             None => Ok(Self::new_unchecked(DenseMatrix::new(0), n)),
             Some(matrix) => Ok(Self::new_unchecked(matrix, n)),
         }
     }
 
     /// Build a probability matrix from this count matrix using pseudo-counts.
-    pub fn to_freq<P>(&self, pseudo: P) -> FrequencyMatrix<A, K>
+    pub fn to_freq<P>(&self, pseudo: P) -> FrequencyMatrix<A>
     where
-        P: Into<Pseudocounts<A, K>>,
+        P: Into<Pseudocounts<A>>,
     {
         let p = pseudo.into();
         let mut probas = DenseMatrix::new(self.data.rows());
         for i in 0..self.data.rows() {
             let src = &self.data[i];
             let dst = &mut probas[i];
             for (j, &x) in src.iter().enumerate() {
-                dst[j] = x as f32 + p.counts()[j] as f32;
+                dst[j] = x as f32 + p.counts()[j];
             }
             let s: f32 = dst.iter().sum();
             for x in dst.iter_mut() {
                 *x /= s;
             }
         }
-        FrequencyMatrix {
-            alphabet: std::marker::PhantomData,
-            data: probas,
-        }
+        FrequencyMatrix::new_unchecked(probas)
     }
 
     /// The raw counts from the count matrix.
     #[inline]
-    pub fn counts(&self) -> &DenseMatrix<u32, K> {
+    pub fn counts(&self) -> &DenseMatrix<u32, A::K> {
         &self.data
     }
 }
 
-impl<A: Alphabet, const K: usize> AsRef<DenseMatrix<u32, K>> for CountMatrix<A, K> {
-    fn as_ref(&self) -> &DenseMatrix<u32, K> {
+impl<A: ComplementableAlphabet> CountMatrix<A> {
+    /// Get the reverse-complement of this count matrix.
+    pub fn reverse_complement(&self) -> Self {
+        let mut data = DenseMatrix::new(self.data.rows());
+        for (i, row) in self.data.iter().rev().enumerate() {
+            for &s in A::symbols() {
+                data[i][s.as_index()] = row[A::complement(s).as_index()];
+            }
+        }
+        Self::new_unchecked(data, self.n)
+    }
+}
+
+impl<A: Alphabet> AsRef<DenseMatrix<u32, A::K>> for CountMatrix<A> {
+    fn as_ref(&self) -> &DenseMatrix<u32, A::K> {
         &self.data
     }
 }
 
-impl<A: Alphabet, const K: usize> FromIterator<EncodedSequence<A>>
-    for Result<CountMatrix<A, K>, InvalidData>
-{
+impl<A: Alphabet> FromIterator<EncodedSequence<A>> for Result<CountMatrix<A>, InvalidData> {
     fn from_iter<I>(iter: I) -> Self
     where
         I: IntoIterator<Item = EncodedSequence<A>>,
     {
         CountMatrix::from_sequences(iter)
     }
 }
 
 // --- FrequencyMatrix ---------------------------------------------------------
 
 /// A matrix storing symbol frequencies at each position.
 #[derive(Clone, Debug)]
-pub struct FrequencyMatrix<A: Alphabet, const K: usize> {
+pub struct FrequencyMatrix<A: Alphabet> {
     alphabet: std::marker::PhantomData<A>,
-    data: DenseMatrix<f32, K>,
+    data: DenseMatrix<f32, A::K>,
 }
 
-impl<A: Alphabet, const K: usize> FrequencyMatrix<A, K> {
+impl<A: Alphabet> FrequencyMatrix<A> {
+    /// Create a new frequency matrix without checking the contents.
+    fn new_unchecked(data: DenseMatrix<f32, A::K>) -> Self {
+        Self {
+            alphabet: std::marker::PhantomData,
+            data,
+        }
+    }
+
     /// Convert to a weight matrix using the given background frequencies.
-    pub fn to_weight<B>(&self, background: B) -> WeightMatrix<A, K>
+    pub fn to_weight<B>(&self, background: B) -> WeightMatrix<A>
     where
-        B: Into<Option<Background<A, K>>>,
+        B: Into<Option<Background<A>>>,
     {
         let bg = background.into().unwrap_or_default();
         let mut weight = DenseMatrix::new(self.data.rows());
         for (src, dst) in self.data.iter().zip(weight.iter_mut()) {
             for (j, (&x, &f)) in src.iter().zip(bg.frequencies()).enumerate() {
                 dst[j] = x / f;
             }
         }
-        WeightMatrix {
-            background: bg,
-            data: weight,
-        }
+        WeightMatrix::new_unchecked(bg, weight)
     }
 
     /// Convert to a scoring matrix using the given background frequencies.
-    pub fn to_scoring<B>(&self, background: B) -> ScoringMatrix<A, K>
+    pub fn to_scoring<B>(&self, background: B) -> ScoringMatrix<A>
     where
-        B: Into<Option<Background<A, K>>>,
+        B: Into<Option<Background<A>>>,
     {
         let bg = background.into().unwrap_or_default();
-        let mut weight = DenseMatrix::new(self.data.rows());
-        for (src, dst) in self.data.iter().zip(weight.iter_mut()) {
+        let mut scores = DenseMatrix::new(self.data.rows());
+        for (src, dst) in self.data.iter().zip(scores.iter_mut()) {
             for (j, (&x, &f)) in src.iter().zip(bg.frequencies()).enumerate() {
                 dst[j] = (x / f).log2();
             }
         }
-        ScoringMatrix {
-            background: bg,
-            data: weight,
-        }
+        ScoringMatrix::new_unchecked(bg, scores)
     }
 }
 
-impl<A: Alphabet, const K: usize> AsRef<DenseMatrix<f32, K>> for FrequencyMatrix<A, K> {
-    fn as_ref(&self) -> &DenseMatrix<f32, K> {
+impl<A: Alphabet> AsRef<DenseMatrix<f32, A::K>> for FrequencyMatrix<A> {
+    fn as_ref(&self) -> &DenseMatrix<f32, A::K> {
         &self.data
     }
 }
 
+impl<A: ComplementableAlphabet> FrequencyMatrix<A> {
+    /// Get the reverse-complement of this count matrix.
+    pub fn reverse_complement(&self) -> Self {
+        let mut data = DenseMatrix::new(self.data.rows());
+        for (i, row) in self.data.iter().rev().enumerate() {
+            for &s in A::symbols() {
+                data[i][s.as_index()] = row[A::complement(s).as_index()];
+            }
+        }
+        Self::new_unchecked(data)
+    }
+}
+
 // --- WeightMatrix ------------------------------------------------------------
 
 /// A matrix storing odds ratio of symbol occurences at each position.
 #[derive(Clone, Debug)]
-pub struct WeightMatrix<A: Alphabet, const K: usize> {
-    background: Background<A, K>,
-    data: DenseMatrix<f32, K>,
+pub struct WeightMatrix<A: Alphabet> {
+    background: Background<A>,
+    data: DenseMatrix<f32, A::K>,
 }
 
-impl<A: Alphabet, const K: usize> WeightMatrix<A, K> {
+impl<A: Alphabet> WeightMatrix<A> {
+    /// Create a new weight matrix without checking the contents.
+    fn new_unchecked(background: Background<A>, data: DenseMatrix<f32, A::K>) -> Self {
+        Self { background, data }
+    }
+
     /// The length of the motif encoded in this weight matrix.
     #[inline]
     pub fn len(&self) -> usize {
         self.data.rows()
     }
 
     /// The log-likelihoods of the position weight matrix.
     #[inline]
-    pub fn weights(&self) -> &DenseMatrix<f32, K> {
+    pub fn weights(&self) -> &DenseMatrix<f32, A::K> {
         &self.data
     }
 
     /// The background frequencies of the position weight matrix.
     #[inline]
-    pub fn background(&self) -> &Background<A, K> {
+    pub fn background(&self) -> &Background<A> {
         &self.background
     }
 
     /// Rescale this weight matrix with a different background.
     pub fn rescale<B>(&self, background: B) -> Self
     where
-        B: Into<Option<Background<A, K>>>,
+        B: Into<Option<Background<A>>>,
     {
         let b = background.into().unwrap_or_default();
         if b.frequencies() != self.background.frequencies() {
             let old_freqs = self.background.frequencies();
             let new_freqs = b.frequencies();
             let mut data = self.data.clone();
             for row in data.iter_mut() {
-                for j in 0..K {
+                for j in 0..A::K::USIZE {
                     row[j] *= old_freqs[j] / new_freqs[j];
                 }
             }
             Self {
                 data,
                 background: b,
             }
         } else {
             self.clone()
         }
     }
 
     /// Get a position-specific scoring matrix from this position weight matrix.
-    pub fn to_scoring(&self) -> ScoringMatrix<A, K> {
+    pub fn to_scoring(&self) -> ScoringMatrix<A> {
         let background = self.background.clone();
         let mut data = self.data.clone();
         for row in data.iter_mut() {
             for item in row.iter_mut() {
                 *item = item.log2();
             }
         }
-        ScoringMatrix { background, data }
+        ScoringMatrix::new_unchecked(background, data)
     }
 }
 
-impl<A: Alphabet, const K: usize> AsRef<WeightMatrix<A, K>> for WeightMatrix<A, K> {
+impl<A: ComplementableAlphabet> WeightMatrix<A> {
+    /// Get the reverse-complement of this count matrix.
+    pub fn reverse_complement(&self) -> Self {
+        let mut data = DenseMatrix::new(self.data.rows());
+        for (i, row) in self.data.iter().rev().enumerate() {
+            for &s in A::symbols() {
+                data[i][s.as_index()] = row[A::complement(s).as_index()];
+            }
+        }
+        Self::new_unchecked(self.background.clone(), data)
+    }
+}
+
+impl<A: Alphabet> AsRef<WeightMatrix<A>> for WeightMatrix<A> {
     fn as_ref(&self) -> &Self {
-        &self
+        self
     }
 }
 
-impl<A: Alphabet, const K: usize> AsRef<DenseMatrix<f32, K>> for WeightMatrix<A, K> {
-    fn as_ref(&self) -> &DenseMatrix<f32, K> {
+impl<A: Alphabet> AsRef<DenseMatrix<f32, A::K>> for WeightMatrix<A> {
+    fn as_ref(&self) -> &DenseMatrix<f32, A::K> {
         &self.data
     }
 }
 
-impl<A: Alphabet, const K: usize> From<ScoringMatrix<A, K>> for WeightMatrix<A, K> {
-    fn from(pwm: ScoringMatrix<A, K>) -> Self {
+impl<A: Alphabet> From<ScoringMatrix<A>> for WeightMatrix<A> {
+    fn from(pwm: ScoringMatrix<A>) -> Self {
         let background = pwm.background;
         let mut data = pwm.data;
         for row in data.iter_mut() {
             for item in row.iter_mut() {
                 *item = 2f32.powf(*item);
             }
         }
@@ -266,53 +312,71 @@
     }
 }
 
 // --- ScoringMatrix -----------------------------------------------------------
 
 /// A matrix storing odds ratio of symbol occurences at each position.
 #[derive(Clone, Debug)]
-pub struct ScoringMatrix<A: Alphabet, const K: usize> {
-    background: Background<A, K>,
-    data: DenseMatrix<f32, K>,
+pub struct ScoringMatrix<A: Alphabet> {
+    background: Background<A>,
+    data: DenseMatrix<f32, A::K>,
 }
 
-impl<A: Alphabet, const K: usize> ScoringMatrix<A, K> {
+impl<A: ComplementableAlphabet> ScoringMatrix<A> {
+    /// Get the reverse-complement of this count matrix.
+    pub fn reverse_complement(&self) -> Self {
+        let mut data = DenseMatrix::new(self.data.rows());
+        for (i, row) in self.data.iter().rev().enumerate() {
+            for &s in A::symbols() {
+                data[i][s.as_index()] = row[A::complement(s).as_index()];
+            }
+        }
+        Self::new_unchecked(self.background.clone(), data)
+    }
+}
+
+impl<A: Alphabet> ScoringMatrix<A> {
+    /// Create a new scoring matrix without checking the contents.
+    fn new_unchecked(background: Background<A>, data: DenseMatrix<f32, A::K>) -> Self {
+        Self { background, data }
+    }
+
     /// The length of the motif encoded in this scoring matrix.
     #[inline]
     pub fn len(&self) -> usize {
         self.data.rows()
     }
 
     /// The log-likelihoods of the position weight matrix.
     #[inline]
-    pub fn weights(&self) -> &DenseMatrix<f32, K> {
+    pub fn weights(&self) -> &DenseMatrix<f32, A::K> {
         &self.data
     }
 
     /// The background frequencies of the position weight matrix.
     #[inline]
-    pub fn background(&self) -> &Background<A, K> {
+    pub fn background(&self) -> &Background<A> {
         &self.background
     }
 }
 
-impl<A: Alphabet, const K: usize> AsRef<ScoringMatrix<A, K>> for ScoringMatrix<A, K> {
+impl<A: Alphabet> AsRef<ScoringMatrix<A>> for ScoringMatrix<A> {
     fn as_ref(&self) -> &Self {
-        &self
+        self
     }
 }
 
-impl<A: Alphabet, const K: usize> AsRef<DenseMatrix<f32, K>> for ScoringMatrix<A, K> {
-    fn as_ref(&self) -> &DenseMatrix<f32, K> {
+impl<A: Alphabet> AsRef<DenseMatrix<f32, A::K>> for ScoringMatrix<A> {
+    fn as_ref(&self) -> &DenseMatrix<f32, A::K> {
         &self.data
     }
 }
 
-impl<A: Alphabet, const K: usize> From<WeightMatrix<A, K>> for ScoringMatrix<A, K> {
-    fn from(pwm: WeightMatrix<A, K>) -> Self {
+impl<A: Alphabet> From<WeightMatrix<A>> for ScoringMatrix<A> {
+    fn from(pwm: WeightMatrix<A>) -> Self {
         let background = pwm.background;
         let mut data = pwm.data;
         for row in data.iter_mut() {
             for item in row.iter_mut() {
                 *item = item.log2();
             }
         }
```

### Comparing `lightmotif-0.1.1/lightmotif/tests/dna.rs` & `lightmotif-0.2.0/lightmotif/tests/dna.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 extern crate lightmotif;
+extern crate typenum;
 
-#[cfg(target_feature = "ssse3")]
-use std::arch::x86_64::__m128;
-#[cfg(target_feature = "avx2")]
-use std::arch::x86_64::__m256;
-use std::str::FromStr;
-
-use lightmotif::Alphabet;
-use lightmotif::CountMatrix;
-use lightmotif::Dna;
-use lightmotif::EncodedSequence;
-use lightmotif::Pipeline;
-use lightmotif::Score;
+use lightmotif::abc::Dna;
+use lightmotif::num::StrictlyPositive;
+use lightmotif::num::U1;
+use lightmotif::num::U16;
+use lightmotif::num::U32;
+use lightmotif::pli::BestPosition;
+use lightmotif::pli::Pipeline;
+use lightmotif::pli::Score;
+use lightmotif::pwm::CountMatrix;
+use lightmotif::seq::EncodedSequence;
+use lightmotif::seq::StripedSequence;
 
-const SEQUENCE: &'static str = "ATGTCCCAACAACGATACCCCGAGCCCATCGCCGTCATCGGCTCGGCATGCAGATTCCCAGGCG";
-const PATTERNS: &[&'static str] = &["GTTGACCTTATCAAC", "GTTGATCCAGTCAAC"];
+const SEQUENCE: &str = "ATGTCCCAACAACGATACCCCGAGCCCATCGCCGTCATCGGCTCGGCATGCAGATTCCCAGGCG";
+const PATTERNS: &[&str] = &["GTTGACCTTATCAAC", "GTTGATCCAGTCAAC"];
 
 // scores computed with Bio.motifs
 #[rustfmt::skip]
 const EXPECTED: &[f32] = &[
     -23.07094  , -18.678621 , -15.219191 , -17.745737 , 
     -18.678621 , -23.07094  , -17.745737 , -19.611507 , 
     -27.463257 , -29.989803 , -14.286304 , -26.53037  , 
@@ -30,109 +30,112 @@
     -8.961102  , -26.53037  , -27.463257 , -14.286304 , 
     -15.219191 , -26.53037  , -23.07094  , -18.678621 ,
     -14.286304 , -18.678621 , -26.53037  , -16.152077 , 
     -17.745737 , -18.678621 , -17.745737 , -14.286304 , 
     -30.922688 , -18.678621 
 ];
 
-#[test]
-fn test_score_generic() {
-    let encoded = EncodedSequence::<Dna>::from_str(SEQUENCE).unwrap();
-    let mut striped = encoded.to_striped::<2>();
+fn test_score<C: StrictlyPositive, P: Score<Dna, C>>(pli: &P) {
+    let mut striped = StripedSequence::<Dna, C>::encode(SEQUENCE).unwrap();
 
-    let cm = CountMatrix::<Dna, { Dna::K }>::from_sequences(
-        PATTERNS
-            .iter()
-            .map(|x| EncodedSequence::from_str(x).unwrap()),
+    let cm = CountMatrix::<Dna>::from_sequences(
+        PATTERNS.iter().map(|x| EncodedSequence::encode(x).unwrap()),
     )
     .unwrap();
-    let pbm = cm.to_freq([0.1, 0.1, 0.1, 0.1, 0.0]);
+    let pbm = cm.to_freq(0.1);
     let pwm = pbm.to_weight(None);
     let pssm = pwm.into();
 
     striped.configure(&pssm);
-    let result = Pipeline::<Dna, f32>::score(&striped, &pssm);
+    let result = pli.score(&striped, &pssm);
     let scores = result.to_vec();
 
     assert_eq!(scores.len(), EXPECTED.len());
     for i in 0..scores.len() {
         assert!(
             (scores[i] - EXPECTED[i]).abs() < 1e-5,
             "{} != {} at position {}",
             scores[i],
             EXPECTED[i],
             i
         );
     }
 }
 
-#[cfg(target_feature = "ssse3")]
-#[test]
-fn test_score_ssse3() {
-    let encoded = EncodedSequence::<Dna>::from_str(SEQUENCE).unwrap();
-    let mut striped = encoded.to_striped();
-
-    let cm = CountMatrix::from_sequences(
-        PATTERNS
-            .iter()
-            .map(|x| EncodedSequence::from_str(x).unwrap()),
+fn test_best_position<C: StrictlyPositive, P: Score<Dna, C> + BestPosition<C>>(pli: &P) {
+    let mut striped = StripedSequence::<Dna, C>::encode(SEQUENCE).unwrap();
+
+    let cm = CountMatrix::<Dna>::from_sequences(
+        PATTERNS.iter().map(|x| EncodedSequence::encode(x).unwrap()),
     )
     .unwrap();
-    let pbm = cm.to_freq([0.1, 0.1, 0.1, 0.1, 0.0]);
+    let pbm = cm.to_freq(0.1);
     let pwm = pbm.to_weight(None);
     let pssm = pwm.into();
 
     striped.configure(&pssm);
-    let result = Pipeline::<_, __m128>::score(&striped, &pssm);
+    let result = pli.score(&striped, &pssm);
+    assert_eq!(pli.best_position(&result), Some(18));
+}
 
-    // for i in 0..result.data.rows() {
-    //     println!("i={} {:?}", i, &result.data[i]);
-    // }
+#[test]
+fn test_score_generic() {
+    let pli = Pipeline::generic();
+    test_score::<U32, _>(&pli);
+    test_score::<U1, _>(&pli);
+}
 
-    let scores = result.to_vec();
-    assert_eq!(scores.len(), EXPECTED.len());
-    for i in 0..EXPECTED.len() {
-        assert!(
-            (scores[i] - EXPECTED[i]).abs() < 1e-5,
-            "{} != {} at position {}",
-            scores[i],
-            EXPECTED[i],
-            i
-        );
-    }
+#[test]
+fn test_best_position_generic() {
+    let pli = Pipeline::generic();
+    test_best_position::<U32, _>(&pli);
+    test_best_position::<U1, _>(&pli);
+}
+
+#[cfg(target_feature = "sse2")]
+#[test]
+fn test_score_sse2() {
+    let pli = Pipeline::sse2().unwrap();
+    test_score::<U16, _>(&pli);
+}
+
+#[cfg(target_feature = "sse2")]
+#[test]
+fn test_best_position_sse2() {
+    let pli = Pipeline::sse2().unwrap();
+    test_best_position::<U16, _>(&pli);
+}
+
+#[cfg(target_feature = "sse2")]
+#[test]
+fn test_score_sse2_32() {
+    let pli = Pipeline::sse2().unwrap();
+    test_score::<U32, _>(&pli);
 }
 
 #[cfg(target_feature = "avx2")]
 #[test]
 fn test_score_avx2() {
-    let encoded = EncodedSequence::<Dna>::from_str(SEQUENCE).unwrap();
-    let mut striped = encoded.to_striped::<{ std::mem::size_of::<__m256>() }>();
-
-    let cm = CountMatrix::<Dna, { Dna::K }>::from_sequences(
-        PATTERNS
-            .iter()
-            .map(|x| EncodedSequence::from_str(x).unwrap()),
-    )
-    .unwrap();
-    let pbm = cm.to_freq([0.1, 0.1, 0.1, 0.1, 0.0]);
-    let pwm = pbm.to_weight(None);
-    let pssm = pwm.into();
+    let pli = Pipeline::avx2().unwrap();
+    test_score(&pli);
+}
 
-    striped.configure(&pssm);
-    let result = Pipeline::<_, __m256>::score(&striped, &pssm);
-    let scores = result.to_vec();
+#[cfg(target_feature = "avx2")]
+#[test]
+fn test_best_position_avx2() {
+    let pli = Pipeline::avx2().unwrap();
+    test_best_position(&pli);
+}
 
-    // for i in 0..result.data.rows() {
-    //     println!("{:?}", &result.data[i]);
-    // }
+#[cfg(target_feature = "neon")]
+#[test]
+fn test_score_neon() {
+    let pli = Pipeline::neon().unwrap();
+    test_score::<U16, _>(&pli);
+}
 
-    assert_eq!(scores.len(), EXPECTED.len());
-    for i in 0..EXPECTED.len() {
-        assert!(
-            (scores[i] - EXPECTED[i]).abs() < 1e-5,
-            "{} != {} at position {}",
-            scores[i],
-            EXPECTED[i],
-            i
-        );
-    }
+#[cfg(target_feature = "neon")]
+#[test]
+fn test_best_position_neon() {
+    let pli = Pipeline::neon().unwrap();
+    test_best_position::<U16, _>(&pli);
 }
```

### Comparing `lightmotif-0.1.1/lightmotif-py/Cargo.toml` & `lightmotif-0.2.0/lightmotif-py/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "lightmotif-py"
-version = "0.1.1"
+version = "0.2.0"
 authors = ["Martin Larralde <martin.larralde@embl.de>"]
 edition = "2021"
 license = "MIT"
 description = "PyO3 bindings and Python interface to the lightmotif crate."
 repository = "https://github.com/althonos/lightmotif"
 homepage = "https://github.com/althonos/lightmotif"
 readme = "README.md"
@@ -13,17 +13,18 @@
 
 [lib]
 crate-type = ["cdylib", "rlib"]
 path = "lightmotif/lib.rs"
 
 [dependencies.lightmotif]
 path = "../lightmotif"
-version = "0.1.1"
+version = "0.2.0"
 [dependencies]
 pyo3 = "0.18.3"
+generic-array = "0.14"
 
 [features]
 default = []
 built = []
 extension-module = ["pyo3/extension-module"]
 nightly = ["pyo3/nightly"]
```

### Comparing `lightmotif-0.1.1/lightmotif-py/README.md` & `lightmotif-0.2.0/lightmotif-py/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 - Compile-time definition of alphabets and matrix dimensions.
 - Sequence symbol encoding for fast table look-ups, as implemented in
   HMMER[\[1\]](#ref1) or MEME[\[2\]](#ref2)
 - Striped sequence matrices to process several positions in parallel,
   inspired by Michael Farrar[\[3\]](#ref3).
 - Vectorized matrix row look-up using `permute` instructions of [AVX2](https://fr.wikipedia.org/wiki/Advanced_Vector_Extensions).
 
+*This is the Python version, there is a [Rust crate](https://crates.io/crates/lightmotif) available as well.*
 
 ## 🔧 Installing
 
 `lightmotif` can be installed directly from [PyPI](https://pypi.org/project/lightmotif/),
 which hosts some pre-built wheels for most mainstream platforms, as well as the 
 code required to compile from source with Rust:
 ```console
@@ -94,17 +95,16 @@
 Benchmarks use the [MX000001](https://www.prodoric.de/matrix/MX000001.html)
 motif from [PRODORIC](https://www.prodoric.de/)[\[4\]](#ref4), and the
 [complete genome](https://www.ncbi.nlm.nih.gov/nuccore/U00096) of an
 *Escherichia coli K12* strain. 
 *Benchmarks were run on a [i7-10710U CPU](https://ark.intel.com/content/www/us/en/ark/products/196448/intel-core-i7-10710u-processor-12m-cache-up-to-4-70-ghz.html) running @1.10GHz, compiled with `--target-cpu=native`*.
 
 ```console
-lightmotif (avx2):      26,528,740 ns/iter (+/- 14,817,953) = 166.9 MiB/s
-lightmotif (generic):  654,599,309 ns/iter (+/- 81,292,868) =   6.8 MiB/s
-Bio.motifs:            526,309,061 ns/iter (+/- 45,603,991) =   8.4 MiB/s
+lightmotif (avx2):      9,125,495 ns/iter    (+/- 6,392,241) = 485.1 MiB/s
+Bio.motifs:           284,696,651 ns/iter    (+/- 6,454,945) =  15.5 MiB/s
 ```
 
 
 ## 💭 Feedback
 
 ### ⚠️ Issue Tracker
```

### Comparing `lightmotif-0.1.1/lightmotif-py/lightmotif/lib.rs` & `lightmotif-0.2.0/lightmotif-py/lightmotif/lib.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,89 @@
 #![doc = include_str!("../README.md")]
 
+extern crate generic_array;
 extern crate lightmotif;
 extern crate pyo3;
 
-#[cfg(target_feature = "avx2")]
-use std::arch::x86_64::__m256;
-#[cfg(any(target_arch = "x86", target_arch = "x86_64"))]
-use std::arch::x86_64::__m256i;
-
-use lightmotif as lm;
-use lightmotif::Alphabet;
-use lightmotif::Pipeline;
-use lightmotif::Score;
-use lightmotif::Symbol;
+use lightmotif::abc::Symbol;
+use lightmotif::num::Unsigned;
+use lightmotif::pli::platform::Backend;
+use lightmotif::pli::Pipeline;
+use lightmotif::pli::Score;
 
 use pyo3::exceptions::PyBufferError;
 use pyo3::exceptions::PyIndexError;
-use pyo3::exceptions::PyRuntimeError;
 use pyo3::exceptions::PyTypeError;
 use pyo3::exceptions::PyValueError;
 use pyo3::ffi::Py_ssize_t;
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
 use pyo3::types::PyString;
 use pyo3::AsPyPointer;
 
+use generic_array::GenericArray;
+
 // --- Compile-time constants --------------------------------------------------
 
+#[cfg(any(target_arch = "arm", target_arch = "aarch64"))]
+type C = <lightmotif::pli::platform::Neon as Backend>::LANES;
 #[cfg(any(target_arch = "x86", target_arch = "x86_64"))]
-const C: usize = std::mem::size_of::<__m256i>();
-#[cfg(not(any(target_arch = "x86", target_arch = "x86_64")))]
-const C: usize = 1;
+type C = <lightmotif::pli::platform::Avx2 as Backend>::LANES;
+#[cfg(not(any(
+    target_arch = "x86",
+    target_arch = "x86_64",
+    target_arch = "arm",
+    target_arch = "aarch64",
+)))]
+type C = typenum::consts::U1;
 
 // --- Helpers -----------------------------------------------------------------
 
-fn dict_to_alphabet_array<'py, A: lm::Alphabet, const K: usize>(
+fn dict_to_alphabet_array<'py, A: lightmotif::Alphabet>(
     d: &'py PyDict,
-) -> PyResult<[f32; K]> {
-    let mut p = [0.0; K];
+) -> PyResult<GenericArray<f32, A::K>> {
+    let mut p = std::iter::repeat(0.0)
+        .take(A::K::USIZE)
+        .collect::<GenericArray<f32, A::K>>();
     for (k, v) in d.iter() {
         let s = k.extract::<&PyString>()?.to_str()?;
         if s.len() != 1 {
             return Err(PyValueError::new_err((
                 "Invalid key for pseudocount:",
                 s.to_string(),
             )));
         }
         let x = s.chars().next().unwrap();
-        let symbol = <A as lm::Alphabet>::Symbol::from_char(x)
+        let symbol = <A as lightmotif::Alphabet>::Symbol::from_char(x)
             .map_err(|_| PyValueError::new_err(("Invalid key for pseudocount:", x)))?;
         let value = v.extract::<f32>()?;
         p[symbol.as_index()] = value;
     }
     Ok(p)
 }
 
 // --- EncodedSequence ---------------------------------------------------------
 
 #[pyclass(module = "lightmotif.lib")]
 #[derive(Clone, Debug)]
 pub struct EncodedSequence {
-    data: lm::EncodedSequence<lm::Dna>,
+    data: lightmotif::seq::EncodedSequence<lightmotif::Dna>,
 }
 
 #[pymethods]
 impl EncodedSequence {
     /// Encode a sequence with the given alphabet.
     #[new]
     pub fn __init__(sequence: &PyString) -> PyResult<PyClassInitializer<Self>> {
         let seq = sequence.to_str()?;
-        let data = lm::EncodedSequence::encode(&seq).map_err(|lm::InvalidSymbol(x)| {
-            PyValueError::new_err(format!("Invalid symbol in input: {}", x))
-        })?;
+        let data = lightmotif::EncodedSequence::encode(&seq).map_err(
+            |lightmotif::err::InvalidSymbol(x)| {
+                PyValueError::new_err(format!("Invalid symbol in input: {}", x))
+            },
+        )?;
         Ok(EncodedSequence { data }.into())
     }
 
     /// Create a copy of this sequence.
     pub fn copy(&self) -> EncodedSequence {
         self.clone()
     }
@@ -89,135 +97,144 @@
 }
 
 // --- StripedSequence ---------------------------------------------------------
 
 #[pyclass(module = "lightmotif.lib")]
 #[derive(Clone, Debug)]
 pub struct StripedSequence {
-    data: lm::StripedSequence<lm::Dna, C>,
+    data: lightmotif::seq::StripedSequence<lightmotif::Dna, C>,
 }
 
 // --- CountMatrix -------------------------------------------------------------
 
 #[pyclass(module = "lightmotif.lib")]
 #[derive(Clone, Debug)]
 pub struct CountMatrix {
-    data: lm::CountMatrix<lm::Dna, { lm::Dna::K }>,
+    data: lightmotif::CountMatrix<lightmotif::Dna>,
 }
 
 #[pymethods]
 impl CountMatrix {
     pub fn normalize(&self, pseudocount: Option<PyObject>) -> PyResult<WeightMatrix> {
         let pseudo = Python::with_gil(|py| {
             if let Some(obj) = pseudocount {
                 if let Ok(x) = obj.extract::<f32>(py) {
-                    Ok(lm::Pseudocounts::from(x))
+                    Ok(lightmotif::abc::Pseudocounts::from(x))
                 } else if let Ok(d) = obj.extract::<&PyDict>(py) {
-                    let p = dict_to_alphabet_array::<lm::Dna, { lm::Dna::K }>(d)?;
-                    Ok(lm::Pseudocounts::from(p))
+                    let p = dict_to_alphabet_array::<lightmotif::Dna>(d)?;
+                    Ok(lightmotif::abc::Pseudocounts::from(p))
                 } else {
                     Err(PyTypeError::new_err("Invalid type for pseudocount"))
                 }
             } else {
-                Ok(lm::Pseudocounts::default())
+                Ok(lightmotif::abc::Pseudocounts::default())
             }
         })?;
         let data = self.data.to_freq(pseudo).to_weight(None);
         Ok(WeightMatrix { data })
     }
 }
 
-impl From<lm::CountMatrix<lm::Dna, { lm::Dna::K }>> for CountMatrix {
-    fn from(data: lm::CountMatrix<lm::Dna, { lm::Dna::K }>) -> Self {
+impl From<lightmotif::CountMatrix<lightmotif::Dna>> for CountMatrix {
+    fn from(data: lightmotif::CountMatrix<lightmotif::Dna>) -> Self {
         Self { data }
     }
 }
 
 // --- FrequencyMatrix ---------------------------------------------------------
 
 #[pyclass(module = "lightmotif.lib")]
 #[derive(Clone, Debug)]
 pub struct WeightMatrix {
-    data: lm::WeightMatrix<lm::Dna, { lm::Dna::K }>,
+    data: lightmotif::pwm::WeightMatrix<lightmotif::Dna>,
 }
 
 #[pymethods]
 impl WeightMatrix {
     pub fn log_odds(&self, background: Option<PyObject>) -> PyResult<ScoringMatrix> {
         // extract the background from the method argument
         let bg = Python::with_gil(|py| {
             if let Some(obj) = background {
                 if let Ok(d) = obj.extract::<&PyDict>(py) {
-                    let p = dict_to_alphabet_array::<lm::Dna, { lm::Dna::K }>(d)?;
-                    lm::Background::new(p)
+                    let p = dict_to_alphabet_array::<lightmotif::Dna>(d)?;
+                    lightmotif::abc::Background::new(p)
                         .map_err(|_| PyValueError::new_err("Invalid background frequencies"))
                 } else {
                     Err(PyTypeError::new_err("Invalid type for pseudocount"))
                 }
             } else {
-                Ok(lm::Background::uniform())
+                Ok(lightmotif::abc::Background::uniform())
             }
         })?;
         // rescale if backgrounds do not match
         let pwm = match bg.frequencies() != self.data.background().frequencies() {
             false => self.data.rescale(bg),
             true => self.data.clone(),
         };
         Ok(ScoringMatrix { data: pwm.into() })
     }
 }
 
-impl From<lm::WeightMatrix<lm::Dna, { lm::Dna::K }>> for WeightMatrix {
-    fn from(data: lm::WeightMatrix<lm::Dna, { lm::Dna::K }>) -> Self {
+impl From<lightmotif::WeightMatrix<lightmotif::Dna>> for WeightMatrix {
+    fn from(data: lightmotif::WeightMatrix<lightmotif::Dna>) -> Self {
         Self { data }
     }
 }
 
 // --- ScoringMatrix -----------------------------------------------------------
 
 #[pyclass(module = "lightmotif.lib")]
 #[derive(Clone, Debug)]
 pub struct ScoringMatrix {
-    data: lm::ScoringMatrix<lm::Dna, { lm::Dna::K }>,
+    data: lightmotif::ScoringMatrix<lightmotif::Dna>,
 }
 
 #[pymethods]
 impl ScoringMatrix {
     /// Return the PSSM score for all positions of the given sequence.
     pub fn calculate(
         slf: PyRef<'_, Self>,
         sequence: &mut StripedSequence,
     ) -> PyResult<StripedScores> {
         let pssm = &slf.data;
-        sequence.data.configure(pssm);
+        let seq = &mut sequence.data;
+        seq.configure(pssm);
 
         let scores = slf.py().allow_threads(|| {
-            #[cfg(target_feature = "avx2")]
-            if std::is_x86_feature_detected!("avx2") {
-                return Pipeline::<lm::Dna, __m256>::score(&sequence.data, pssm);
+            #[cfg(any(target_arch = "x86", target_arch = "x86_64"))]
+            if let Ok(pli) = Pipeline::avx2() {
+                return pli.score(seq, pssm);
+            }
+            #[cfg(any(target_arch = "x86", target_arch = "x86_64"))]
+            if let Ok(pli) = Pipeline::sse2() {
+                return pli.score(seq, pssm);
+            }
+            #[cfg(any(target_arch = "arm", target_arch = "aarch64"))]
+            if let Ok(pli) = Pipeline::neon() {
+                return pli.score(seq, pssm);
             }
-            Pipeline::<lm::Dna, f32>::score(&sequence.data, pssm)
+            Pipeline::generic().score(seq, pssm)
         });
 
         Ok(StripedScores::from(scores))
     }
 }
 
-impl From<lm::ScoringMatrix<lm::Dna, { lm::Dna::K }>> for ScoringMatrix {
-    fn from(data: lm::ScoringMatrix<lm::Dna, { lm::Dna::K }>) -> Self {
+impl From<lightmotif::ScoringMatrix<lightmotif::Dna>> for ScoringMatrix {
+    fn from(data: lightmotif::ScoringMatrix<lightmotif::Dna>) -> Self {
         Self { data }
     }
 }
 
 // --- Scores ------------------------------------------------------------------
 
 #[pyclass(module = "lightmotif.lib")]
 #[derive(Clone, Debug)]
 pub struct StripedScores {
-    scores: lm::StripedScores<C>,
+    scores: lightmotif::pli::StripedScores<C>,
     shape: [Py_ssize_t; 2],
     strides: [Py_ssize_t; 2],
 }
 
 #[pymethods]
 impl StripedScores {
     fn __len__(&self) -> usize {
@@ -263,16 +280,16 @@
         (*view).suboffsets = std::ptr::null_mut();
         (*view).internal = std::ptr::null_mut();
 
         Ok(())
     }
 }
 
-impl From<lm::StripedScores<C>> for StripedScores {
-    fn from(mut scores: lm::StripedScores<C>) -> Self {
+impl From<lightmotif::pli::StripedScores<C>> for StripedScores {
+    fn from(mut scores: lightmotif::pli::StripedScores<C>) -> Self {
         // extract the matrix shape
         let cols = scores.matrix().columns();
         let rows = scores.matrix().rows();
         // record the matrix shape as a Fortran buffer
         let shape = [cols as Py_ssize_t, rows as Py_ssize_t];
         let strides = [
             std::mem::size_of::<f32>() as Py_ssize_t,
@@ -306,61 +323,70 @@
     pwm: Py<WeightMatrix>,
     #[pyo3(get)]
     pssm: Py<ScoringMatrix>,
 }
 
 // --- Module ------------------------------------------------------------------
 
+/// Create a new motif from an iterable of sequences.
 #[pyfunction]
-fn create<'py>(sequences: &'py PyAny) -> PyResult<Motif> {
+pub fn create<'py>(sequences: &'py PyAny) -> PyResult<Motif> {
     let py = sequences.py();
 
     let mut encoded = Vec::new();
     for seq in sequences.iter()? {
         let s = seq?.extract::<&PyString>()?.to_str()?;
         let x = py
-            .allow_threads(|| lm::EncodedSequence::encode(&s))
+            .allow_threads(|| lightmotif::EncodedSequence::encode(&s))
             .map_err(|_| PyValueError::new_err("Invalid symbol in sequence"))?;
         encoded.push(x);
     }
 
-    let data = lm::CountMatrix::from_sequences(encoded)
+    let data = lightmotif::CountMatrix::from_sequences(encoded)
         .map_err(|_| PyValueError::new_err("Inconsistent sequence length"))?;
     let weights = data.to_freq(0.0).to_weight(None);
     let scoring = weights.to_scoring();
 
     Ok(Motif {
         counts: Py::new(py, CountMatrix::from(data))?,
         pwm: Py::new(py, WeightMatrix::from(weights))?,
         pssm: Py::new(py, ScoringMatrix::from(scoring))?,
     })
 }
 
+/// Encode and stripe a text sequence.
+#[pyfunction]
+pub fn stripe<'py>(sequence: &'py PyAny) -> PyResult<StripedSequence> {
+    let py = sequence.py();
+    let s = sequence.extract::<&PyString>()?;
+    let encoded = EncodedSequence::__init__(s).and_then(|e| Py::new(py, e))?;
+    let striped = encoded.borrow(py).stripe();
+    Ok(striped)
+}
+
 /// PyO3 bindings to ``lightmotif``, a library for fast PWM motif scanning.
 ///
 /// The API is similar to the `Bio.motifs` module from Biopython on purpose.
 #[pymodule]
 #[pyo3(name = "lib")]
-pub fn init(py: Python, m: &PyModule) -> PyResult<()> {
+pub fn init(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add("__package__", "lightmotif")?;
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
     m.add("__author__", env!("CARGO_PKG_AUTHORS").replace(':', "\n"))?;
 
+    #[cfg(any(target_arch = "x86", target_arch = "x86_64"))]
+    m.add("AVX2_SUPPORTED", std::is_x86_feature_detected!("avx2"))?;
+    #[cfg(not(any(target_arch = "x86", target_arch = "x86_64")))]
+    m.add("AVX2_SUPPORTED", false)?;
+
     m.add_class::<EncodedSequence>()?;
     m.add_class::<StripedSequence>()?;
 
     m.add_class::<CountMatrix>()?;
     m.add_class::<WeightMatrix>()?;
     m.add_class::<ScoringMatrix>()?;
 
     m.add_function(wrap_pyfunction!(create, m)?)?;
-
-    // If compiled in AVX2 mode, check that AVX2 is supported by the CPU
-    #[cfg(target_feature = "avx2")]
-    if !std::is_x86_feature_detected!("avx2") {
-        return Err(PyRuntimeError::new_err(
-            "Importing AVX2 extension on machine without AVX2 support",
-        ));
-    }
+    m.add_function(wrap_pyfunction!(stripe, m)?)?;
 
     Ok(())
 }
```

### Comparing `lightmotif-0.1.1/lightmotif-py/lightmotif/tests/test_dna.py` & `lightmotif-0.2.0/lightmotif-py/lightmotif/tests/test_dna.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,12 @@
 
 class TestDNAMotif(unittest.TestCase):
     def test_calculate(self):
         motif = lightmotif.create(["GTTGACCTTATCAAC", "GTTGATCCAGTCAAC"])
         frequencies = motif.counts.normalize(0.1)
         pssm = frequencies.log_odds()
 
-        seq = lightmotif.EncodedSequence(SEQUENCE)
-        striped = seq.stripe()
-
-        scores = pssm.calculate(striped)
+        seq = lightmotif.stripe(SEQUENCE)
+        scores = pssm.calculate(seq)
         self.assertEqual(len(scores), len(EXPECTED))
         for x, y in zip(scores, EXPECTED):
             self.assertAlmostEqual(x, y, places=5)
```

### Comparing `lightmotif-0.1.1/lightmotif-py/lightmotif/tests/unittest.rs` & `lightmotif-0.2.0/lightmotif-py/lightmotif/tests/unittest.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/PKG-INFO` & `lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightmotif
-Version: 0.1.1
+Version: 0.2.0
 Summary: PyO3 bindings and Python interface to lightmotif, a library for platform-accelerated biological motif scanning using position weight matrices.
 Home-page: https://github.com/althonos/lightmotif
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/lightmotif/issues
 Project-URL: Changelog, https://github.com/althonos/lightmotif/blob/master/CHANGELOG.md
@@ -74,14 +74,15 @@
 - Compile-time definition of alphabets and matrix dimensions.
 - Sequence symbol encoding for fast table look-ups, as implemented in
   HMMER[\[1\]](#ref1) or MEME[\[2\]](#ref2)
 - Striped sequence matrices to process several positions in parallel,
   inspired by Michael Farrar[\[3\]](#ref3).
 - Vectorized matrix row look-up using `permute` instructions of [AVX2](https://fr.wikipedia.org/wiki/Advanced_Vector_Extensions).
 
+*This is the Python version, there is a [Rust crate](https://crates.io/crates/lightmotif) available as well.*
 
 ## 🔧 Installing
 
 `lightmotif` can be installed directly from [PyPI](https://pypi.org/project/lightmotif/),
 which hosts some pre-built wheels for most mainstream platforms, as well as the 
 code required to compile from source with Rust:
 ```console
@@ -129,17 +130,16 @@
 Benchmarks use the [MX000001](https://www.prodoric.de/matrix/MX000001.html)
 motif from [PRODORIC](https://www.prodoric.de/)[\[4\]](#ref4), and the
 [complete genome](https://www.ncbi.nlm.nih.gov/nuccore/U00096) of an
 *Escherichia coli K12* strain. 
 *Benchmarks were run on a [i7-10710U CPU](https://ark.intel.com/content/www/us/en/ark/products/196448/intel-core-i7-10710u-processor-12m-cache-up-to-4-70-ghz.html) running @1.10GHz, compiled with `--target-cpu=native`*.
 
 ```console
-lightmotif (avx2):      26,528,740 ns/iter (+/- 14,817,953) = 166.9 MiB/s
-lightmotif (generic):  654,599,309 ns/iter (+/- 81,292,868) =   6.8 MiB/s
-Bio.motifs:            526,309,061 ns/iter (+/- 45,603,991) =   8.4 MiB/s
+lightmotif (avx2):      9,125,495 ns/iter    (+/- 6,392,241) = 485.1 MiB/s
+Bio.motifs:           284,696,651 ns/iter    (+/- 6,454,945) =  15.5 MiB/s
 ```
 
 
 ## 💭 Feedback
 
 ### ⚠️ Issue Tracker
```

### Comparing `lightmotif-0.1.1/setup.cfg` & `lightmotif-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 	Builds = https://github.com/althonos/lightmotif/actions/
 	PyPI = https://pypi.org/project/lightmotif
 
 [options]
 zip_safe = true
 packages = 
 	lightmotif
-	lightmotif.avx2
 	lightmotif.tests
 test_suite = lightmotif.tests
 python_requires = >=3.7
 setup_requires = 
 	setuptools >=39.2
 	setuptools-rust >=1.0
```

### Comparing `lightmotif-0.1.1/setup.py` & `lightmotif-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -114,54 +114,32 @@
 
     def build_extension(self, ext, target):
         with patch_env("RUSTFLAGS", " ".join(ext.rustc_flags)):
             return _build_rust.build_extension(self, ext, target)
 
     def get_dylib_ext_path(self, ext, module_name):
         ext_path = _build_rust.get_dylib_ext_path(self, ext, module_name)
-        # if self.inplace:
-        #     base = os.path.basename(ext_path)
-        #     folder = os.path.dirname(os.path.realpath(__file__))
-        #     prefix = os.path.sep.join(ext.name.split(".")[:-1])
-        #     ext_path = os.path.join(folder, prefix, base)
+        if self.inplace:
+            package_dir = self.distribution.package_dir['']
+            base = os.path.basename(ext_path)
+            folder = os.path.dirname(os.path.realpath(__file__))
+            prefix = os.path.sep.join(ext.name.split(".")[:-1])
+            ext_path = os.path.join(folder, package_dir, prefix, base)
         return ext_path
 
 
 # --- Setup ---------------------------------------------------------------------
 
-
-RUST_EXTENSIONS = [
-    rust.RustExtension(
-        "lightmotif.arch",
-        path=os.path.join("lightmotif-py", "lightmotif", "arch", "Cargo.toml"),
-        binding=rust.Binding.PyO3,
-        strip=rust.Strip.Debug,
-        features=["extension-module"],
-    ),
-    rust.RustExtension(
-        "lightmotif.lib",
-        path=os.path.join("lightmotif-py", "Cargo.toml"),
-        binding=rust.Binding.PyO3,
-        strip=rust.Strip.Debug,
-        features=["extension-module"],
-    ),
-]
-
-if re.match("(x86_64)|(x86)|(AMD64|amd64)|(^i.86$)", MACHINE):
-    RUST_EXTENSIONS.append(
+setuptools.setup(
+    setup_requires=["setuptools", "setuptools_rust"],
+    cmdclass=dict(sdist=sdist, build_rust=build_rust),
+    package_dir={"": "lightmotif-py"},
+    rust_extensions=[
         rust.RustExtension(
-            "lightmotif.avx2.lib",
+            "lightmotif.lib",
             path=os.path.join("lightmotif-py", "Cargo.toml"),
             binding=rust.Binding.PyO3,
             strip=rust.Strip.Debug,
             features=["extension-module"],
-            rustc_flags=["-Ctarget-feature=+avx2"],
-            optional=True,
         ),
-    )
-
-setuptools.setup(
-    setup_requires=["setuptools", "setuptools_rust"],
-    cmdclass=dict(sdist=sdist, build_rust=build_rust),
-    package_dir={"": "lightmotif-py"},
-    rust_extensions=RUST_EXTENSIONS,
+    ],
 )
```

