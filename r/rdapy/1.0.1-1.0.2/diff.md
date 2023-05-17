# Comparing `tmp/rdapy-1.0.1.tar.gz` & `tmp/rdapy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdapy-1.0.1.tar", last modified: Wed May 17 16:05:38 2023, max compression
+gzip compressed data, was "rdapy-1.0.2.tar", last modified: Wed May 17 16:14:11 2023, max compression
```

## Comparing `rdapy-1.0.1.tar` & `rdapy-1.0.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.809479 rdapy-1.0.1/
--rw-r--r--   0 alecramsay   (501) staff       (20)     1067 2023-05-15 21:02:16.000000 rdapy-1.0.1/LICENSE
--rw-r--r--   0 alecramsay   (501) staff       (20)     1519 2023-05-17 16:05:38.809342 rdapy-1.0.1/PKG-INFO
--rw-r--r--   0 alecramsay   (501) staff       (20)      940 2023-05-17 15:57:58.000000 rdapy-1.0.1/README.md
--rw-r--r--   0 alecramsay   (501) staff       (20)      576 2023-05-17 16:05:24.000000 rdapy-1.0.1/pyproject.toml
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.802790 rdapy-1.0.1/rdapy/
--rw-r--r--   0 alecramsay   (501) staff       (20)     1250 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/__init__.py
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.804192 rdapy-1.0.1/rdapy/compactness/
--rw-r--r--   0 alecramsay   (501) staff       (20)      128 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/__init__.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     1351 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/compactness.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     7701 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/features.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     2651 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/kiwysi.py
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.805011 rdapy-1.0.1/rdapy/compactness/pypoly/
--rw-r--r--   0 alecramsay   (501) staff       (20)      360 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/pypoly/__init__.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     2299 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/pypoly/miniumareaboundingrectangle.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     3605 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/pypoly/polygonattributes.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     3357 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/pypoly/polygoncoordinates.py
--rw-r--r--   0 alecramsay   (501) staff       (20)      684 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/pypoly/project.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     4916 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/compactness/pypoly/smallestenclosingcircle.py
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.805290 rdapy-1.0.1/rdapy/equal/
--rw-r--r--   0 alecramsay   (501) staff       (20)       69 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/equal/__init__.py
--rw-r--r--   0 alecramsay   (501) staff       (20)      300 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/equal/population.py
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.805809 rdapy-1.0.1/rdapy/graph/
--rw-r--r--   0 alecramsay   (501) staff       (20)      117 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/graph/__init__.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     1132 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/graph/connected.py
--rw-r--r--   0 alecramsay   (501) staff       (20)       98 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/graph/constants.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     1429 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/graph/embedded.py
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.806752 rdapy-1.0.1/rdapy/partisan/
--rw-r--r--   0 alecramsay   (501) staff       (20)      145 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/__init__.py
--rwxr-xr-x   0 alecramsay   (501) staff       (20)     8599 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/bias.py
--rw-r--r--   0 alecramsay   (501) staff       (20)       83 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/constants.py
--rwxr-xr-x   0 alecramsay   (501) staff       (20)     4532 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/method.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     3571 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/partisan.py
--rwxr-xr-x   0 alecramsay   (501) staff       (20)     3165 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/responsiveness.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     1420 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/partisan/utils.py
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.807128 rdapy-1.0.1/rdapy/splitting/
--rw-r--r--   0 alecramsay   (501) staff       (20)      268 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/splitting/__init__.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     1362 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/splitting/coi.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     7959 2023-05-15 21:02:16.000000 rdapy-1.0.1/rdapy/splitting/county.py
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.803644 rdapy-1.0.1/rdapy.egg-info/
--rw-r--r--   0 alecramsay   (501) staff       (20)     1519 2023-05-17 16:05:38.000000 rdapy-1.0.1/rdapy.egg-info/PKG-INFO
--rw-r--r--   0 alecramsay   (501) staff       (20)     1360 2023-05-17 16:05:38.000000 rdapy-1.0.1/rdapy.egg-info/SOURCES.txt
--rw-r--r--   0 alecramsay   (501) staff       (20)        1 2023-05-17 16:05:38.000000 rdapy-1.0.1/rdapy.egg-info/dependency_links.txt
--rw-r--r--   0 alecramsay   (501) staff       (20)        1 2023-05-17 14:22:22.000000 rdapy-1.0.1/rdapy.egg-info/not-zip-safe
--rw-r--r--   0 alecramsay   (501) staff       (20)      161 2023-05-17 16:05:38.000000 rdapy-1.0.1/rdapy.egg-info/requires.txt
--rw-r--r--   0 alecramsay   (501) staff       (20)       16 2023-05-17 16:05:38.000000 rdapy-1.0.1/rdapy.egg-info/top_level.txt
--rw-r--r--   0 alecramsay   (501) staff       (20)       38 2023-05-17 16:05:38.809532 rdapy-1.0.1/setup.cfg
--rw-r--r--   0 alecramsay   (501) staff       (20)      839 2023-05-17 16:02:31.000000 rdapy-1.0.1/setup.py
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.808638 rdapy-1.0.1/test/
--rw-r--r--   0 alecramsay   (501) staff       (20)      982 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_bias.py
--rw-r--r--   0 alecramsay   (501) staff       (20)      593 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_coi_splitting.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     1518 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_compactness.py
--rw-r--r--   0 alecramsay   (501) staff       (20)    20846 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_county_splitting.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     4689 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_graph.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     1987 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_kiwysi.py
--rw-r--r--   0 alecramsay   (501) staff       (20)    29281 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_method.py
--rw-r--r--   0 alecramsay   (501) staff       (20)    32227 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_partisan.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     1315 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_population.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     3073 2023-05-15 21:02:16.000000 rdapy-1.0.1/test/test_responsiveness.py
-drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:05:38.809170 rdapy-1.0.1/testutils/
--rw-r--r--   0 alecramsay   (501) staff       (20)      156 2023-05-15 21:02:17.000000 rdapy-1.0.1/testutils/__init__.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     1194 2023-05-15 21:02:17.000000 rdapy-1.0.1/testutils/compactness.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     1652 2023-05-15 21:02:17.000000 rdapy-1.0.1/testutils/equal.py
--rw-r--r--   0 alecramsay   (501) staff       (20)     6371 2023-05-15 21:02:17.000000 rdapy-1.0.1/testutils/readwrite.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:14:11.426640 rdapy-1.0.2/
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1067 2023-05-15 21:02:16.000000 rdapy-1.0.2/LICENSE
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1519 2023-05-17 16:14:11.426500 rdapy-1.0.2/PKG-INFO
+-rw-r--r--   0 alecramsay   (501) staff       (20)      940 2023-05-17 15:57:58.000000 rdapy-1.0.2/README.md
+-rw-r--r--   0 alecramsay   (501) staff       (20)      576 2023-05-17 16:13:29.000000 rdapy-1.0.2/pyproject.toml
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:14:11.420043 rdapy-1.0.2/rdapy/
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1250 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/__init__.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:14:11.421390 rdapy-1.0.2/rdapy/compactness/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      128 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/compactness/__init__.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1351 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/compactness/compactness.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     7701 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/compactness/features.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     2651 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/compactness/kiwysi.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:14:11.422272 rdapy-1.0.2/rdapy/compactness/pypoly/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      360 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/compactness/pypoly/__init__.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     2299 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/compactness/pypoly/miniumareaboundingrectangle.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     3605 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/compactness/pypoly/polygonattributes.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     3357 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/compactness/pypoly/polygoncoordinates.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)      684 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/compactness/pypoly/project.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     4916 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/compactness/pypoly/smallestenclosingcircle.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:14:11.422589 rdapy-1.0.2/rdapy/equal/
+-rw-r--r--   0 alecramsay   (501) staff       (20)       69 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/equal/__init__.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)      300 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/equal/population.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:14:11.423119 rdapy-1.0.2/rdapy/graph/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      117 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/graph/__init__.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1132 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/graph/connected.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)       98 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/graph/constants.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1429 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/graph/embedded.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:14:11.424032 rdapy-1.0.2/rdapy/partisan/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      145 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/partisan/__init__.py
+-rwxr-xr-x   0 alecramsay   (501) staff       (20)     8599 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/partisan/bias.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)       83 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/partisan/constants.py
+-rwxr-xr-x   0 alecramsay   (501) staff       (20)     4532 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/partisan/method.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     3571 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/partisan/partisan.py
+-rwxr-xr-x   0 alecramsay   (501) staff       (20)     3165 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/partisan/responsiveness.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1420 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/partisan/utils.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:14:11.424443 rdapy-1.0.2/rdapy/splitting/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      268 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/splitting/__init__.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1362 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/splitting/coi.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     7959 2023-05-15 21:02:16.000000 rdapy-1.0.2/rdapy/splitting/county.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:14:11.420836 rdapy-1.0.2/rdapy.egg-info/
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1519 2023-05-17 16:14:11.000000 rdapy-1.0.2/rdapy.egg-info/PKG-INFO
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1360 2023-05-17 16:14:11.000000 rdapy-1.0.2/rdapy.egg-info/SOURCES.txt
+-rw-r--r--   0 alecramsay   (501) staff       (20)        1 2023-05-17 16:14:11.000000 rdapy-1.0.2/rdapy.egg-info/dependency_links.txt
+-rw-r--r--   0 alecramsay   (501) staff       (20)        1 2023-05-17 14:22:22.000000 rdapy-1.0.2/rdapy.egg-info/not-zip-safe
+-rw-r--r--   0 alecramsay   (501) staff       (20)      161 2023-05-17 16:14:11.000000 rdapy-1.0.2/rdapy.egg-info/requires.txt
+-rw-r--r--   0 alecramsay   (501) staff       (20)        6 2023-05-17 16:14:11.000000 rdapy-1.0.2/rdapy.egg-info/top_level.txt
+-rw-r--r--   0 alecramsay   (501) staff       (20)       38 2023-05-17 16:14:11.426686 rdapy-1.0.2/setup.cfg
+-rw-r--r--   0 alecramsay   (501) staff       (20)      952 2023-05-17 16:13:44.000000 rdapy-1.0.2/setup.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:14:11.425821 rdapy-1.0.2/test/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      982 2023-05-15 21:02:16.000000 rdapy-1.0.2/test/test_bias.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)      593 2023-05-15 21:02:16.000000 rdapy-1.0.2/test/test_coi_splitting.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1518 2023-05-15 21:02:16.000000 rdapy-1.0.2/test/test_compactness.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)    20846 2023-05-15 21:02:16.000000 rdapy-1.0.2/test/test_county_splitting.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     4689 2023-05-15 21:02:16.000000 rdapy-1.0.2/test/test_graph.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1987 2023-05-15 21:02:16.000000 rdapy-1.0.2/test/test_kiwysi.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)    29281 2023-05-15 21:02:16.000000 rdapy-1.0.2/test/test_method.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)    32227 2023-05-15 21:02:16.000000 rdapy-1.0.2/test/test_partisan.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1315 2023-05-15 21:02:16.000000 rdapy-1.0.2/test/test_population.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     3073 2023-05-15 21:02:16.000000 rdapy-1.0.2/test/test_responsiveness.py
+drwxr-xr-x   0 alecramsay   (501) staff       (20)        0 2023-05-17 16:14:11.426323 rdapy-1.0.2/testutils/
+-rw-r--r--   0 alecramsay   (501) staff       (20)      156 2023-05-15 21:02:17.000000 rdapy-1.0.2/testutils/__init__.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1194 2023-05-15 21:02:17.000000 rdapy-1.0.2/testutils/compactness.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     1652 2023-05-15 21:02:17.000000 rdapy-1.0.2/testutils/equal.py
+-rw-r--r--   0 alecramsay   (501) staff       (20)     6371 2023-05-15 21:02:17.000000 rdapy-1.0.2/testutils/readwrite.py
```

### Comparing `rdapy-1.0.1/LICENSE` & `rdapy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/PKG-INFO` & `rdapy-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdapy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Redistricting analytics in Python
 Home-page: https://github.com/dra2020/rdapy
 Author: alecramsay
 Author-email: Alec Ramsay <alec@davesredistricting.org>
 License: MIT
 Project-URL: Homepage, https://github.com/dra2020/rdapy
 Project-URL: Bug Tracker, https://github.com/dra2020/rdapy/issues
```

### Comparing `rdapy-1.0.1/README.md` & `rdapy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/pyproject.toml` & `rdapy-1.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rdapy"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Alec Ramsay", email="alec@davesredistricting.org" },
 ]
 description = "Redistricting analytics in Python"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `rdapy-1.0.1/rdapy/__init__.py` & `rdapy-1.0.2/rdapy/__init__.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/compactness/compactness.py` & `rdapy-1.0.2/rdapy/compactness/compactness.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/compactness/features.py` & `rdapy-1.0.2/rdapy/compactness/features.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/compactness/kiwysi.py` & `rdapy-1.0.2/rdapy/compactness/kiwysi.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/compactness/pypoly/miniumareaboundingrectangle.py` & `rdapy-1.0.2/rdapy/compactness/pypoly/miniumareaboundingrectangle.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/compactness/pypoly/polygonattributes.py` & `rdapy-1.0.2/rdapy/compactness/pypoly/polygonattributes.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/compactness/pypoly/polygoncoordinates.py` & `rdapy-1.0.2/rdapy/compactness/pypoly/polygoncoordinates.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/compactness/pypoly/project.py` & `rdapy-1.0.2/rdapy/compactness/pypoly/project.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/compactness/pypoly/smallestenclosingcircle.py` & `rdapy-1.0.2/rdapy/compactness/pypoly/smallestenclosingcircle.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/graph/connected.py` & `rdapy-1.0.2/rdapy/graph/connected.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/graph/embedded.py` & `rdapy-1.0.2/rdapy/graph/embedded.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/partisan/bias.py` & `rdapy-1.0.2/rdapy/partisan/bias.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/partisan/method.py` & `rdapy-1.0.2/rdapy/partisan/method.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/partisan/partisan.py` & `rdapy-1.0.2/rdapy/partisan/partisan.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/partisan/responsiveness.py` & `rdapy-1.0.2/rdapy/partisan/responsiveness.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/partisan/utils.py` & `rdapy-1.0.2/rdapy/partisan/utils.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/splitting/coi.py` & `rdapy-1.0.2/rdapy/splitting/coi.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy/splitting/county.py` & `rdapy-1.0.2/rdapy/splitting/county.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/rdapy.egg-info/PKG-INFO` & `rdapy-1.0.2/rdapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdapy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Redistricting analytics in Python
 Home-page: https://github.com/dra2020/rdapy
 Author: alecramsay
 Author-email: Alec Ramsay <alec@davesredistricting.org>
 License: MIT
 Project-URL: Homepage, https://github.com/dra2020/rdapy
 Project-URL: Bug Tracker, https://github.com/dra2020/rdapy/issues
```

### Comparing `rdapy-1.0.1/rdapy.egg-info/SOURCES.txt` & `rdapy-1.0.2/rdapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/setup.py` & `rdapy-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,22 +3,28 @@
 """
 python setup.py register
 python setup.py register sdist upload
 """
 
 setup(
     name="rdapy",
-    version="1.0",
+    version="1.0.2",
     description="Redistricting analytics in Python",
     url="https://github.com/dra2020/rdapy",
     author="alecramsay",
     author_email="alec@davesredistricting.org",
     license="MIT",
-    packages=find_packages(),
-    # packages=["rdapy"],
+    packages=[
+        "rdapy",
+        "rdapy.compactness",
+        "rdapy.equal",
+        "rdapy.graph",
+        "rdapy.partisan",
+        "rdapy.splitting",
+    ],
     install_requires=[
         "attrs",
         "certifi",
         "click",
         "click-plugins",
         "cligj",
         "exceptiongroup",
```

### Comparing `rdapy-1.0.1/test/test_bias.py` & `rdapy-1.0.2/test/test_bias.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/test/test_coi_splitting.py` & `rdapy-1.0.2/test/test_coi_splitting.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/test/test_compactness.py` & `rdapy-1.0.2/test/test_compactness.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/test/test_county_splitting.py` & `rdapy-1.0.2/test/test_county_splitting.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/test/test_graph.py` & `rdapy-1.0.2/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/test/test_kiwysi.py` & `rdapy-1.0.2/test/test_kiwysi.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/test/test_method.py` & `rdapy-1.0.2/test/test_method.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/test/test_partisan.py` & `rdapy-1.0.2/test/test_partisan.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/test/test_population.py` & `rdapy-1.0.2/test/test_population.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/test/test_responsiveness.py` & `rdapy-1.0.2/test/test_responsiveness.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/testutils/compactness.py` & `rdapy-1.0.2/testutils/compactness.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/testutils/equal.py` & `rdapy-1.0.2/testutils/equal.py`

 * *Files identical despite different names*

### Comparing `rdapy-1.0.1/testutils/readwrite.py` & `rdapy-1.0.2/testutils/readwrite.py`

 * *Files identical despite different names*

