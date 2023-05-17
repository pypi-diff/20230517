# Comparing `tmp/portfolyo-0.5.1.tar.gz` & `tmp/portfolyo-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolyo-0.5.1.tar", last modified: Sat Apr 29 17:06:08 2023, max compression
+gzip compressed data, was "portfolyo-0.5.2.tar", last modified: Wed May 17 09:21:02 2023, max compression
```

## Comparing `portfolyo-0.5.1.tar` & `portfolyo-0.5.2.tar`

### file list

```diff
@@ -1,82 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.361255 portfolyo-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-29 17:05:54.000000 portfolyo-0.5.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-29 17:05:54.000000 portfolyo-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-29 17:06:08.361255 portfolyo-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-29 17:05:54.000000 portfolyo-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.361255 portfolyo-0.5.1/portfolyo/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 17:06:08.361255 portfolyo-0.5.1/portfolyo/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.349255 portfolyo-0.5.1/portfolyo/core/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/extendpandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.349255 portfolyo-0.5.1/portfolyo/core/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/mixins/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/mixins/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/mixins/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/ndframelike.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.357255 portfolyo-0.5.1/portfolyo/core/pfline/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/enable_arithmatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/flat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/flat_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/interop.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfline/nested_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.357255 portfolyo-0.5.1/portfolyo/core/pfstate/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfstate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfstate/enable_arithmatic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfstate/pfstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/pfstate/pfstate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/core/suppresswarnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.357255 portfolyo-0.5.1/portfolyo/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/dev/develop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/dev/mockup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.357255 portfolyo-0.5.1/portfolyo/prices/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/prices/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/prices/hedge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/prices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.357255 portfolyo-0.5.1/portfolyo/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.361255 portfolyo-0.5.1/portfolyo/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/ceil.py
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/changefreq.py
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/changeyear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/floor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/freq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/isboundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/leftandright.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/peakperiod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/right.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/righttoleft.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/round.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/standardize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/tzone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/unitdefinitions.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/tools/wavg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.361255 portfolyo-0.5.1/portfolyo/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/visualize/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/visualize/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-04-29 17:05:54.000000 portfolyo-0.5.1/portfolyo/visualize/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:08.345255 portfolyo-0.5.1/portfolyo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-29 17:06:08.000000 portfolyo-0.5.1/portfolyo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-29 17:06:08.000000 portfolyo-0.5.1/portfolyo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:06:08.000000 portfolyo-0.5.1/portfolyo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:06:08.000000 portfolyo-0.5.1/portfolyo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-29 17:06:08.000000 portfolyo-0.5.1/portfolyo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 17:06:08.000000 portfolyo-0.5.1/portfolyo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-29 17:05:54.000000 portfolyo-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-29 17:06:08.361255 portfolyo-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-29 17:05:54.000000 portfolyo-0.5.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-29 17:05:54.000000 portfolyo-0.5.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.838975 portfolyo-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-17 09:20:48.000000 portfolyo-0.5.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-17 09:20:48.000000 portfolyo-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-17 09:21:02.838975 portfolyo-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-17 09:20:48.000000 portfolyo-0.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.842975 portfolyo-0.5.2/portfolyo/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-17 09:21:02.842975 portfolyo-0.5.2/portfolyo/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.830975 portfolyo-0.5.2/portfolyo/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/extendpandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.830975 portfolyo-0.5.2/portfolyo/core/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/mixins/excelclipboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/mixins/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/mixins/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/ndframelike.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.834975 portfolyo-0.5.2/portfolyo/core/pfline/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/arithmatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/children.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18958 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/dataframeexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/developernotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/flat_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/flat_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/nested_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/nested_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/prices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.834975 portfolyo-0.5.2/portfolyo/core/pfstate/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfstate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfstate/arithmatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfstate/pfstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfstate/pfstate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/suppresswarnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.834975 portfolyo-0.5.2/portfolyo/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/dev/develop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/dev/mockup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.834975 portfolyo-0.5.2/portfolyo/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16678 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/prices/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/prices/hedge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/prices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.834975 portfolyo-0.5.2/portfolyo/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.838975 portfolyo-0.5.2/portfolyo/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/changefreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/changeyear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/floor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/freq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/isboundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/leftandright.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/peakperiod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/right.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/righttoleft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/round.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/standardize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/tzone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/unitdefinitions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/wavg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.838975 portfolyo-0.5.2/portfolyo/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/visualize/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/visualize/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/visualize/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.830975 portfolyo-0.5.2/portfolyo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-17 09:21:02.000000 portfolyo-0.5.2/portfolyo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-17 09:21:02.000000 portfolyo-0.5.2/portfolyo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:21:02.000000 portfolyo-0.5.2/portfolyo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:21:02.000000 portfolyo-0.5.2/portfolyo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-17 09:21:02.000000 portfolyo-0.5.2/portfolyo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 09:21:02.000000 portfolyo-0.5.2/portfolyo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-17 09:20:48.000000 portfolyo-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-17 09:21:02.838975 portfolyo-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-17 09:20:48.000000 portfolyo-0.5.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-17 09:20:49.000000 portfolyo-0.5.2/versioneer.py
```

### Comparing `portfolyo-0.5.1/LICENCE` & `portfolyo-0.5.2/LICENCE`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/PKG-INFO` & `portfolyo-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolyo
-Version: 0.5.1
+Version: 0.5.2
 Summary: Analysing and manipulating timeseries related to power and gas offtake portfolios.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENCE
 
 portfolyo
```

### Comparing `portfolyo-0.5.1/README.rst` & `portfolyo-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/__init__.py` & `portfolyo-0.5.2/portfolyo/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Package to analyse and manipulate timeseries related to power and gas offtake portfolios."""
 
 
 from . import _version, dev, tools
 from .core import extendpandas  # extend functionalty of pandas
 from .core import suppresswarnings
 from .core.mixins.plot import plot_pfstates
-from .core.pfline import FlatPfLine, Kind, NestedPfLine, PfLine
+from .core.pfline import Kind, PfLine, Structure, create
 from .core.pfstate import PfState
 from .prices.hedge import hedge
 from .prices.utils import is_peak_hour
 from .tools.changeyear import characterize_index, map_frame_to_year
 from .tools.freq import FREQUENCIES
 from .tools.standardize import frame as standardize
 from .tools.tzone import force_agnostic, force_aware
```

### Comparing `portfolyo-0.5.1/portfolyo/core/mixins/other.py` & `portfolyo-0.5.2/portfolyo/core/mixins/excelclipboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 Module with mixins, to add other output-methods to PfLine and PfState classes.
 """
 
 from __future__ import annotations
+
+import functools
 from typing import TYPE_CHECKING, Union
+
 import pandas as pd
-import functools
 
 if TYPE_CHECKING:  # needed to avoid circular imports
-    from ..pfstate import PfState
     from ..pfline import PfLine
+    from ..pfstate import PfState
 
 
-def _prepare_df(pfl_or_pfs: Union[PfLine, PfState]) -> pd.DataFrame:
+def prepare_df(pfl_or_pfs: Union[PfLine, PfState]) -> pd.DataFrame:
     """Prepare dataframe so it can easily be saved to excel or copied to clipboard."""
-    return pfl_or_pfs.df(flatten=False).pint.dequantify().tz_localize(None)
+    return pfl_or_pfs.dataframe().pint.dequantify().tz_localize(None)
 
 
-class OtherOutput:  # for both PfLine and PfState
+class ExcelClipboardOutput:  # for both PfLine and PfState
     @functools.wraps(pd.DataFrame.to_clipboard)
     def to_clipboard(self: Union[PfLine, PfState], *args, **kwargs) -> None:
-        _prepare_df(self).to_clipboard(*args, **kwargs)
+        prepare_df(self).to_clipboard(*args, **kwargs)
 
     @functools.wraps(pd.DataFrame.to_excel)
     def to_excel(self: Union[PfLine, PfState], *args, **kwargs) -> None:
-        _prepare_df(self).to_excel(*args, *kwargs)
+        prepare_df(self).to_excel(*args, *kwargs)
```

### Comparing `portfolyo-0.5.1/portfolyo/core/mixins/plot.py` & `portfolyo-0.5.2/portfolyo/core/mixins/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,14 @@
     sharey = axesgroups[:, 2]
     for ax1, ax2 in zip(sharey[1:], sharey[:-1]):
         ax1.sharey(ax2)
 
     # TODO: resample all to have same index (frequency and length).
 
     for i, ((pfname, pfs), axes) in enumerate(zip(dic.items(), axesgroups)):
-
         # If freq is MS or longer: use categorical axes. Plot volumes in MWh.
         # If freq is D or shorter: use time axes. Plot volumes in MW.
         is_category = tools.freq.shortest(pfs.index.freq, "MS") == "MS"
 
         # Portfolio name.
         axes[0].text(
             0,
```

### Comparing `portfolyo-0.5.1/portfolyo/core/mixins/text.py` & `portfolyo-0.5.2/portfolyo/core/mixins/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,16 +134,16 @@
         out.append(tree["10"] + txtline)
     return out
 
 
 def _flatdatablock(pfl: PfLine, cols: Iterable[str], num_of_ts: int) -> Iterable[str]:
     """The timestamps and data to be shown in a block, next to the tree."""
     # Obtain dataframe with index = timestamp as string and columns = one or more of 'qwpr'.
-    df = pfl.df(cols, flatten=True)
-    # . reduce number of timestamps to increase speed of conversion to strings.
+    df = pfl.df[list(cols)]
+    # . (roughly) reduce number of timestamps to increase speed of conversion to strings.
     if len(df.index) > num_of_ts * 2:
         df = pd.concat([df.iloc[:num_of_ts, :], df.iloc[-num_of_ts:, :]], axis=0)
     # . turn values into strings.
     df = _df_with_strvalues(df)
     # . turn index into strings and reduce to wanted number of datapoints
     df = _df_with_strindex(df, num_of_ts)
     # . column withs
@@ -190,15 +190,15 @@
 
 
 def pfs_as_string(pfs: PfState, num_of_ts: int, color: bool) -> str:
     lines = ["PfState object."]
     lines.extend(_index_info(pfs.index))
     spaces = " " * (MAX_DEPTH + 5)
     lines.extend([spaces + txtline for txtline in _dataheader("wqpr")])
-    lines.extend(_nestedtree("offtake", pfs.offtakevolume, "wqpr", num_of_ts))
+    lines.extend(_nestedtree("offtake", pfs.offtakevolume, "wq", num_of_ts))
     lines.extend(_nestedtree("pnl_cost", pfs.pnl_cost, "wqpr", num_of_ts))
     txt = "\n".join(lines)
     return txt if color else _remove_color(txt)
 
 
 class PfLineText:
     def __repr__(self):
```

### Comparing `portfolyo-0.5.1/portfolyo/core/pfline/base.py` & `portfolyo-0.5.2/portfolyo/core/pfline/classes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,192 +1,141 @@
-"""
-Abstract Base Class for PfLine.
-"""
-
 from __future__ import annotations
 
-from abc import abstractmethod
-from enum import Enum
-from typing import TYPE_CHECKING, Iterable, Union
+import abc
+import dataclasses
+from typing import Any, Callable, Dict, Iterable, Mapping, Union  # noqa
 
+import numpy as np
 import pandas as pd
 
 from ... import tools
-from ...prices import convert, hedge
-from ...prices.utils import duration_bpo
-from ..mixins import OtherOutput, PfLinePlot, PfLineText
-
-# from . import flat, multi, interop  #<-- moved to end of file
+from ..mixins import ExcelClipboardOutput, PfLinePlot, PfLineText
 from ..ndframelike import NDFrameLike
+from . import (
+    create,
+    dataframeexport,
+    decorators,
+    flat_methods,
+    nested_methods,
+    prices,
+    children,
+)
+from .arithmatic import PfLineArithmatic
+from .enums import Kind, Structure
+
+
+def constructor(structure: Structure, kind: Kind) -> type:
+    """Return reference to class constructor."""
+    classmatrix = {
+        (Structure.FLAT, Kind.VOLUME): FlatVolumePfLine,
+        (Structure.FLAT, Kind.PRICE): FlatPricePfLine,
+        (Structure.FLAT, Kind.REVENUE): FlatRevenuePfLine,
+        (Structure.FLAT, Kind.COMPLETE): FlatCompletePfLine,
+        (Structure.NESTED, Kind.VOLUME): NestedVolumePfLine,
+        (Structure.NESTED, Kind.PRICE): NestedPricePfLine,
+        (Structure.NESTED, Kind.REVENUE): NestedRevenuePfLine,
+        (Structure.NESTED, Kind.COMPLETE): NestedCompletePfLine,
+    }
+    return classmatrix.get((structure, kind))
+
+
+# When creating a PfLine (or FlatPfLine or NestedPfLine) instance directly (i.e., with
+# PfLine(data)), the code actually creates, initialises, and returns one of its
+# subclasses. Normally, this would causes python to finally call the subclass' __init__
+# method once more, using the original data as input, undoing the previous
+# initialisation. To prevent this, use decorate the subclass with this decorator.
+def dont_init_twice(Class):
+    """Decorator for PfLine descendents, to allow PfLine to return a child instance."""
+    original_init = Class.__init__
+    Class._initialized = False
+
+    def wrapped_init(self, *args, **kwargs):
+        if not self._initialized:
+            object.__setattr__(self, "_initialized", True)
+            original_init(self, *args, **kwargs)
 
-# Developer notes: we would like to be able to handle 2 cases with volume AND financial
-# information. We would like to...
-# ... handle the situation where, for some timestamp, the volume q == 0 but the revenue
-#   r != 0, because this occasionally arises for the sourced volume, e.g. after buying
-#   and selling the same volume at unequal price. So: we want to be able to store q and r.
-# ... keep price information even if the volume q == 0, because at a later time this price
-#   might still be needed, e.g. if a perfect hedge becomes unperfect. So: we want to be
-#   able to store q and p.
-# Both cases can be catered to. The first as a 'FlatPfLine', where the timeseries for
-# q and r are used in the instance creation. The price is not defined at the timestamp in
-# the example, but can be calculated for other timestamps, and downsampling is also still
-# possble.
-# The second is a bit more complex. It is possible as a 'NestedPfLine'. This has then 2
-# 'FlatPfLine' instances as its children: one made from each of the timeseries for q
-# and p.
-
-
-if TYPE_CHECKING:
-    from .flat import FlatPfLine  # noqa
-    from .nested import NestedPfLine  # noqa
-
-
-class Kind(Enum):
-    """Enumerate what kind of information (which dimensions) is present in a PfLine."""
-
-    # abbreviation, available columns, summable (pfl1 + pfl2) columns
-    VOLUME = "vol", "wq", "q"
-    PRICE = "pri", "p", "p"
-    REVENUE = "rev", "r", "r"
-    COMPLETE = "all", "wqpr", "qr"
-
-    @classmethod
-    def _missing_(cls, val):
-        for member in cls:
-            if member.value[0] == val:
-                return member
+    Class.__init__ = wrapped_init
 
-    @property
-    def available(self):
-        return tuple(self.value[1])
+    return Class
 
-    @property
-    def summable(self):
-        return tuple(self.value[2])
 
-    def __repr__(self):
-        return f"<{self.value[0]}>"
+def series_property_raising_typeerror(what: str) -> Callable[[PfLine], pd.Series]:
+    @property
+    def get_series(self) -> pd.Series:
+        raise TypeError(f"This portfolio line does not contain {what} information.")
 
-    def __str__(self):
-        return self.value[0]
+    return get_series
 
 
-class PfLine(NDFrameLike, PfLineText, PfLinePlot, OtherOutput):
+class PfLine(
+    NDFrameLike, PfLineText, PfLinePlot, ExcelClipboardOutput, PfLineArithmatic
+):
     """Class to hold a related energy timeseries. This can be volume data (with q
     [MWh] and w [MW]), price data (with p [Eur/MWh]), revenue data (with r [Eur]), or
     a combination of all.
     """
 
-    def __new__(cls, data=None):
+    def __new__(cls, data=None, *args, **kwargs):
         if cls is not PfLine:
-            # User actually called a descendent class.
+            # User actually called one of its descendents. Just move along
             return super().__new__(cls)
 
-        # User actually called PfLine().
-
-        elif isinstance(data, PfLine):
-            # Data is already a valid instance and can directly be used.
-            return data
-
-        # User called PfLine and data must be processed by a descendent's __init__
-
-        errors = {}
-        for subcls in [flat.FlatPfLine, nested.NestedPfLine]:
-            # Try passing data to subclasses to see if they can handle it.
-            try:
-                return subcls(data)
-            except (ValueError, TypeError, KeyError) as e:
-                errors[subcls] = e
-                pass
-        errormsg = "\n".join(f"- {c.__name__}: {e.args[0]}" for c, e in errors.items())
-        raise ValueError(
-            f"Cannot create flat or nested PfLine, with the following reasons:\n{errormsg}"
-        )
+        # User did indeed call PfLine and data must be processed by a descendent's __init__
+        return create.pfline(data)
 
-    # Additional abstract methods to be implemented by descendents.
+    def __post_init__(self):
+        err = f"Expected columns {self.kind.available}, received {self.df.columns}."
+        assert set(self.df.columns) == set(self.kind.available), err
 
     @property
-    @abstractmethod
-    def kind(self) -> Kind:
-        """Kind of data that is stored in the instance."""
-        ...
+    def index(self) -> pd.DatetimeIndex:
+        """Index of the data, containing the left-bound timestamps of the delivery periods."""
+        return self.df.index
 
-    @property
-    @abstractmethod
-    def w(self) -> pd.Series:
-        """(Flattened) power timeseries in [MW]."""
+    @abc.abstractproperty
+    def w(self) -> pd.Series:  # override if applicable
+        """Return (flat) volume timeseries in [MW]."""
         ...
 
-    @property
-    @abstractmethod
-    def q(self) -> pd.Series:
-        """(Flattened) energy timeseries in [MWh]."""
+    @abc.abstractproperty
+    def q(self) -> pd.Series:  # override if applicable
+        """Return (flat) volume timeseries in [MWh]."""
         ...
 
-    @property
-    @abstractmethod
-    def p(self) -> pd.Series:
-        """(Flattened) price timeseries in [Eur/MWh]."""
+    @abc.abstractproperty
+    def p(self) -> pd.Series:  # override if applicable
+        """Return (flat) price timeseries in [Eur/MWh]."""
         ...
 
-    @property
-    @abstractmethod
-    def r(self) -> pd.Series:
-        """(Flattened) revenue timeseries in [Eur]."""
+    @abc.abstractproperty
+    def r(self) -> pd.Series:  # override if applicable
+        """Return (flat) revenue timeseries in [Eur]."""
         ...
 
-    @abstractmethod
-    def df(
-        self, cols: Iterable[str] = None, flatten: bool = True, has_units: bool = False
-    ) -> pd.DataFrame:
-        """DataFrame for portfolio line in default units.
-
-        Parameters
-        ----------
-        cols : str, optional (default: all that are available)
-            The columns (w, q, p, r) to include in the dataframe.
-        flatten : bool, optional (default: True)
-            - If True, include only aggregated timeseries (4 or less; 1 per dimension).
-            - If False, include all children and their (intermediate and final)
-              aggregations.
-        has_units : bool, optional (default: True)
-            - If True, return dataframe with ``pint`` units. (The unit can be extracted
-              as a column level with ``.pint.dequantify()``).
-            - If False, return dataframe with float values.
-
-        Returns
-        -------
-        pd.DataFrame
-        """
-        ...
-
-    @property
-    @abstractmethod
-    def volume(self) -> FlatPfLine:
-        """Return (flattened) volume-only PfLine."""
+    @abc.abstractproperty
+    def volume(self) -> PfLine:  # override if applicable
+        """Return volume-only PfLine."""
         ...
 
-    @property
-    @abstractmethod
-    def price(self) -> FlatPfLine:
-        """Return (flattened) price-only PfLine."""
+    @abc.abstractproperty
+    def price(self) -> PfLine:  # override if applicable
+        """Return price-only PfLine."""
         ...
 
-    @property
-    @abstractmethod
-    def revenue(self) -> FlatPfLine:
-        """Return (flattened) revenue-only PfLine."""
+    @abc.abstractproperty
+    def revenue(self) -> PfLine:  # override if applicable
+        """Return revenue-only PfLine"""
         ...
 
-    @abstractmethod
-    def flatten(self) -> FlatPfLine:
-        """Return flat instance, i.e., without children."""
+    @abc.abstractmethod
+    def flatten(self) -> PfLine:
+        """Return flattened instance, i.e., without children."""
         ...
 
-    @abstractmethod
+    @abc.abstractmethod
     def map_to_year(self, year: int, holiday_country: str = None) -> PfLine:
         """Transfer the data to a hypothetical other year.
 
         Parameters
         ----------
         year : int
             Year to transfer the data to.
@@ -197,165 +146,57 @@
 
         Returns
         -------
         PfLine
 
         Notes
         -----
-        Useful for daily data and shorter. Copies over the data but takes weekdays (and
-        holidays) target year into consideration. See ``portfolyo.map_frame_as_year()``
+        Useful for daily (and shorter) data. Copies over the data but takes weekdays (and
+        holidays) of target year into consideration. See ``portfolyo.map_frame_as_year()``
         for more information.
         Inaccurate for monthly data and longer, because we only have one value per month,
         and can therefore not take different number of holidays/weekends (i.e., offpeak
         hours) into consideration.
         """
         ...
 
-    @abstractmethod
-    def __bool__(self) -> bool:
-        """Return True if object (i.e., its children) contains any non-zero data."""
-        ...
-
-    # Dunder methods.
-
-    @abstractmethod
-    def __getitem__(self, *args, **kwargs):  # Get child
-        ...
-
-    # Implemented directly here.
-
-    # Class should be immutable; remove __setitem__ and __delitem__
-    def __setitem__(self, *args, **kwargs):
-        raise TypeError("PfLine instances are immutable.")
-
-    def __delitem__(self, *args, **kwargs):
-        raise TypeError("PfLine instances are immutable.")
-
-    def _set_col_val(
-        self, col: str, val: Union[pd.Series, float, int, tools.unit.Q_]
-    ) -> FlatPfLine:
-        """Set or update a timeseries and return the modified instance."""
-
-        if self.kind is Kind.COMPLETE:
-            raise ValueError(
-                "Cannot set column value when ``.kind`` is Kind.COMPLETE. First select "
-                "the data you wish to keep, e.g. with ``.price``, ``.volume`` or ``.revenue``."
-            )
-
-        data = {col: s for col, s in self.df(flatten=True).items()}
-        # Ensure volume can be overwritten, by removing conflicting volume information.
-        if col == "q" and "w" in data:
-            del data["w"]
-        elif col == "w" and "q" in data:
-            del data["q"]
-        data[col] = val
-        return flat.FlatPfLine(data)
-
-    def set_w(self, w: Union[pd.Series, float, int, tools.unit.Q_]) -> FlatPfLine:
-        """Set or update power timeseries [MW]; returns modified (and flattened) instance."""
-        return self._set_col_val("w", w)
-
-    def set_q(self, q: Union[pd.Series, float, int, tools.unit.Q_]) -> FlatPfLine:
-        """Set or update energy timeseries [MWh]; returns modified (and flattened) instance."""
-        return self._set_col_val("q", q)
-
-    def set_p(self, p: Union[pd.Series, float, int, tools.unit.Q_]) -> FlatPfLine:
-        """Set or update price timeseries [Eur/MWh]; returns modified (and flattened) instance."""
-        return self._set_col_val("p", p)
-
-    def set_r(self, r: Union[pd.Series, float, int, tools.unit.Q_]) -> FlatPfLine:
-        """Set or update revenue timeseries [MW]; returns modified (and flattened) instance."""
-        return self._set_col_val("r", r)
-
-    def set_volume(self, other: PfLine) -> FlatPfLine:
-        """Set or update volume information; returns modified (and flattened) instance."""
-        if not isinstance(other, PfLine) or other.kind is not Kind.VOLUME:
-            raise ValueError(
-                "Can only set volume equal to a volume-only PfLine. Use .volume to obtain such a PfLine."
-            )
-        return self.set_q(other.q)
-
-    def set_price(self, other: PfLine) -> FlatPfLine:
-        """Set or update price information; returns modified (and flattened) instance."""
-        if not isinstance(other, PfLine) or other.kind is not Kind.PRICE:
-            raise ValueError(
-                "Can only set price equal to a price-only PfLine. Use .price to obtain such a PfLine."
-            )
-        return self.set_p(other.p)
-
-    def set_revenue(self, other: PfLine) -> FlatPfLine:
-        """Set or update revenue information; returns modified (and flattened) instance."""
-        if not isinstance(other, PfLine) or other.kind is not Kind.REVENUE:
-            raise ValueError(
-                "Can only set revenue equal to a revenue-only PfLine. Use .revenue to obtain such a PfLine."
-            )
-        return self.set_r(other.r)
-
+    @abc.abstractmethod
     def po(self: PfLine, freq: str = "MS") -> pd.DataFrame:
         """Decompose the portfolio line into peak and offpeak values. Takes simple averages
         of volume [MW] and price [Eur/MWh] - does not hedge!
 
         Parameters
         ----------
         freq : {'MS' (months, default), 'QS' (quarters), 'AS' (years)}
             Frequency of resulting dataframe.
 
         Returns
         -------
         pd.DataFrame
             The dataframe shows a composition into peak and offpeak values.
-        """
-        if self.index.freq not in ["15T", "H"]:
-            raise ValueError(
-                "Only PfLines with (quarter)hourly values can be turned into peak and offpeak values."
-            )
-        if freq not in ["MS", "QS", "AS"]:
-            raise ValueError(
-                f"Value of paramater ``freq`` must be one of {'MS', 'QS', 'AS'} (got: {freq})."
-            )
-
-        prods = ("peak", "offpeak")
 
-        # Get values.
-        dfs = []
-        if "w" in self.kind.available:
-            vals = convert.tseries2bpoframe(self.w, freq)
-            vals.columns = pd.MultiIndex.from_product([vals.columns, ["w"]])
-            dfs.append(vals)
-        if "p" in self.kind.available:
-            vals = convert.tseries2bpoframe(self.p, freq)
-            vals.columns = pd.MultiIndex.from_product([vals.columns, ["p"]])
-            dfs.append(vals)
-        df = pd.concat(dfs, axis=1)
-
-        # Add duration.
-        durs = duration_bpo(df.index)
-        durs.columns = pd.MultiIndex.from_product([durs.columns, ["duration"]])
-        df = pd.concat([df, durs], axis=1)
-
-        # Add additional values and sort.
-        if "q" in self.kind.available:
-            for prod in prods:
-                df[(prod, "q")] = df[(prod, "w")] * df[(prod, "duration")]
-        if "r" in self.kind.available:
-            for prod in prods:
-                df[(prod, "r")] = (
-                    df[(prod, "q")] * df[(prod, "p")]
-                ).pint.to_base_units()
-        i = pd.MultiIndex.from_product([prods, ("duration", *self.kind.available)])
-        return df[i]
+        Notes
+        -----
+        Only relevant for hourly (and shorter) data.
+        """
+        ...
 
+    @abc.abstractmethod
     def hedge_with(
-        self: PfLine, p: PfLine, how: str = "val", freq: str = "MS", po: bool = None
+        self: PfLine,
+        p: PricePfLine,
+        how: str = "val",
+        freq: str = "MS",
+        po: bool = None,
     ) -> PfLine:
         """Hedge the volume in the portfolio line with a price curve.
 
         Parameters
         ----------
-        p : PfLine
+        p : PricePfLine
             Portfolio line with prices to be used in the hedge.
         how : str, optional (Default: 'val')
             Hedge-constraint. 'vol' for volumetric hedge, 'val' for value hedge.
         freq : {'D' (days), 'MS' (months, default), 'QS' (quarters), 'AS' (years)}
             Frequency of hedging products. E.g. 'QS' to hedge with quarter products.
         po : bool, optional
             Type of hedging products. Set to True to split hedge into peak and offpeak.
@@ -367,36 +208,298 @@
             Hedged volume and prices. Index with same frequency as original, but every
             timestamp within a given hedging frequency has the same volume [MW] and price.
             (or, one volume-price pair for peak, and another volume-price pair for offpeak.)
 
         Notes
         -----
         - If the PfLine contains prices, these are ignored.
-        - If ``p`` contains volumes, these are ignored.
         """
-        if self.kind is Kind.PRICE:
+        ...
+
+    @abc.abstractmethod
+    def __bool__(self) -> bool:
+        """Return True if object (i.e., its children) contains any non-zero data."""
+        ...
+
+    @abc.abstractmethod
+    def __eq__(self, other) -> bool:
+        """Return True if objects (i.e., their children) contain identical data."""
+        ...
+
+
+class VolumePfLine:
+    kind = Kind.VOLUME
+    w: pd.Series = property(lambda self: self.df["w"])
+    q: pd.Series = property(lambda self: self.df["q"])
+    p: pd.Series = series_property_raising_typeerror("price")
+    r: pd.Series = series_property_raising_typeerror("revenue")
+    volume: VolumePfLine = property(lambda self: self)
+    price: PricePfLine = series_property_raising_typeerror("price")
+    revenue: RevenuePfLine = series_property_raising_typeerror("revenue")
+
+
+class PricePfLine:
+    kind = Kind.PRICE
+    w: pd.Series = series_property_raising_typeerror("volume")
+    q: pd.Series = series_property_raising_typeerror("volume")
+    p: pd.Series = property(lambda self: self.df["p"])
+    r: pd.Series = series_property_raising_typeerror("revenue")
+    volume: VolumePfLine = series_property_raising_typeerror("volume")
+    price: PricePfLine = property(lambda self: self)
+    revenue: RevenuePfLine = series_property_raising_typeerror("revenue")
+
+
+class RevenuePfLine:
+    kind = Kind.REVENUE
+    w: pd.Series = series_property_raising_typeerror("volume")
+    q: pd.Series = series_property_raising_typeerror("volume")
+    p: pd.Series = series_property_raising_typeerror("price")
+    r: pd.Series = property(lambda self: self.df["r"])
+    volume: VolumePfLine = series_property_raising_typeerror("volume")
+    price: PricePfLine = series_property_raising_typeerror("price")
+    revenue: RevenuePfLine = property(lambda self: self)
+
+
+class CompletePfLine:
+    kind = Kind.COMPLETE
+    w: pd.Series = property(lambda self: self.df["w"])
+    q: pd.Series = property(lambda self: self.df["q"])
+    p: pd.Series = property(lambda self: self.df["p"])
+    r: pd.Series = property(lambda self: self.df["r"])
+
+
+class FlatPfLine(PfLine):
+    """Flat portfolio line, i.e., without children. Only has a single dataframe.
+
+    Notes
+    -----
+    * If the timeseries or values in ``data`` do not have a ``pint`` data type, the
+    standard units are assumed (MW, MWh, Eur, Eur/MWh).
+    * If the timeseries or values in ``data`` do have a ``pint`` data type, they are
+    converted into the standard units.
+    """
+
+    structure = Structure.FLAT
+
+    dataframe = dataframeexport.Flat.dataframe
+    flatten = flat_methods.flatten
+    po = prices.Flat.po
+    hedge_with = prices.Flat.hedge_with
+    # map_to_year => on child classes
+    loc = flat_methods.loc
+    __getitem__ = flat_methods.__getitem__
+    # __bool__ => on child classes
+    __eq__ = flat_methods.__eq__
+
+
+class NestedPfLine(PfLine, children.ChildFunctionality):
+    structure = Structure.NESTED
+
+    dataframe = dataframeexport.Nested.dataframe
+    flatten = nested_methods.flatten
+    po = prices.Nested.po
+    hedge_with = prices.Nested.hedge_with
+    map_to_year = nested_methods.map_to_year
+    loc = nested_methods.loc
+    __bool__ = nested_methods.__bool__
+    __eq__ = nested_methods.__eq__
+
+
+@dont_init_twice
+@dataclasses.dataclass(frozen=True, repr=False, eq=False)
+class FlatVolumePfLine(FlatPfLine, VolumePfLine, PfLine):
+    # Class is only called internally, so expect df to be in correct format. Here: with columns 'w', 'q'.
+    df: pd.DataFrame
+
+    def asfreq(self, freq: str = "MS") -> FlatVolumePfLine:
+        newdf = tools.changefreq.summable(self.df[["q"]], freq)
+        if not len(newdf):
             raise ValueError(
-                "Cannot hedge a PfLine that does not contain volume information."
+                f"There are no full periods available when changing to the frequency {freq}."
             )
-        if self.index.freq not in ["15T", "H", "D"]:
+        newdf["w"] = newdf["q"] / tools.duration.index(newdf.index)  # TODO: check unit
+        return FlatVolumePfLine(newdf)
+
+    @decorators.map_to_year_warning
+    def map_to_year(self, year: int, holiday_country: str = None) -> FlatVolumePfLine:
+        df = self.df[["w"]]  # Averageble data to allow mapping unequal-length periods
+        newdf = tools.changeyear.map_frame_to_year(df, year, holiday_country)
+        newdf["q"] = newdf["w"] * tools.duration.index(newdf.index)
+        return FlatVolumePfLine(newdf)
+
+    def __bool__(self) -> bool:
+        return not np.allclose(self.df["w"].pint.magnitude, 0.0)
+
+
+@dont_init_twice
+@dataclasses.dataclass(frozen=True, repr=False, eq=False)
+class NestedVolumePfLine(NestedPfLine, VolumePfLine, PfLine):
+    # Class is only called internally, so expect children to be in correct format. Here: all are volume-pflines.
+    children: Dict[str, VolumePfLine]
+    df: pd.DataFrame = dataclasses.field(init=False)
+
+    def __post_init__(self):
+        df = sum(child.df for child in self.children.values())
+        object.__setattr__(self, "df", df)
+
+    def asfreq(self, freq: str = "MS") -> NestedVolumePfLine:
+        newchildren = {name: child.asfreq(freq) for name, child in self.items()}
+        return NestedVolumePfLine(newchildren)
+
+
+@dont_init_twice
+@dataclasses.dataclass(frozen=True, repr=False, eq=False)
+class FlatPricePfLine(FlatPfLine, PricePfLine, PfLine):
+    # Class is only called internally, so expect df to be in correct format. Here: with column 'p'.
+    df: pd.DataFrame
+
+    def asfreq(self, freq: str = "MS") -> FlatPricePfLine:
+        newdf = tools.changefreq.averagable(self.df[["p"]], freq)
+        if not len(newdf):
             raise ValueError(
-                "Can only hedge a PfLine with daily or (quarter)hourly information."
+                f"There are no full periods available when changing to the frequency {freq}."
             )
-        if not isinstance(p, PfLine):
-            raise TypeError(
-                f"Parameter ``p`` must be a PfLine instance; got {type(p)}."
+        return FlatPricePfLine(newdf)
+
+    @decorators.map_to_year_warning
+    def map_to_year(self, year: int, holiday_country: str = None) -> FlatVolumePfLine:
+        df = self.df[["p"]]  # Averageble data to allow mapping unequal-length periods
+        newdf = tools.changeyear.map_frame_to_year(df, year, holiday_country)
+        return FlatPricePfLine(newdf)
+
+    def __bool__(self) -> bool:
+        return not np.allclose(self.df["p"].pint.magnitude, 0.0)
+
+
+@dont_init_twice
+@dataclasses.dataclass(frozen=True, repr=False, eq=False)
+class NestedPricePfLine(NestedPfLine, PricePfLine, PfLine):
+    # Class is only called internally, so expect children to be in correct format. Here: all are price-pflines.
+    children: Dict[str, PricePfLine]
+    df: pd.DataFrame = dataclasses.field(init=False)
+
+    def __post_init__(self):
+        df = sum(child.df for child in self.children.values())
+        object.__setattr__(self, "df", df)
+
+    def asfreq(self, freq: str = "MS") -> NestedPricePfLine:
+        newchildren = {name: child.asfreq(freq) for name, child in self.items()}
+        return NestedPricePfLine(newchildren)
+
+
+@dont_init_twice
+@dataclasses.dataclass(frozen=True, repr=False, eq=False)
+class FlatRevenuePfLine(FlatPfLine, RevenuePfLine, PfLine):
+    # Class is only called internally, so expect df to be in correct format. Here: with column 'r'.
+    df: pd.DataFrame
+
+    def asfreq(self, freq: str = "MS") -> FlatRevenuePfLine:
+        newdf = tools.changefreq.summable(self.df[["r"]], freq)
+        if not len(newdf):
+            raise ValueError(
+                f"There are no full periods available when changing to the frequency {freq}."
             )
-        if po is None:
-            po = self.index.freq in ["15T", "H"]  # default: peak/offpeak if possible
-        if po and self.index.freq not in ["15T", "H"]:
+        return FlatRevenuePfLine(newdf)
+
+    @decorators.map_to_year_warning
+    def map_to_year(self, year: int, holiday_country: str = None) -> FlatVolumePfLine:
+        # Assume that revenue is scales proportionately with duration of period.
+        # E.g. 290 Eur in leapyear Feb --> 280 Eur in non-leapyear Feb.
+        df = self.df[["r"]] * tools.duration.index(self.df.index)  # Make averageble
+        newdf = tools.changeyear.map_frame_to_year(df, year, holiday_country)
+        newdf = newdf / tools.duration.index(newdf.index)  # Make summable again
+        return FlatRevenuePfLine(newdf)
+
+    def __bool__(self) -> bool:
+        return not np.allclose(self.df["r"].pint.magnitude, 0.0)
+
+
+@dont_init_twice
+@dataclasses.dataclass(frozen=True, repr=False, eq=False)
+class NestedRevenuePfLine(NestedPfLine, RevenuePfLine, PfLine):
+    # Class is only called internally, so expect children to be in correct format. Here: all are revenue-pflines.
+    children: Dict[str, RevenuePfLine]
+    df: pd.DataFrame = dataclasses.field(init=False)
+
+    def __post_init__(self):
+        df = sum(child.df for child in self.children.values())
+        object.__setattr__(self, "df", df)
+
+    def asfreq(self, freq: str = "MS") -> NestedRevenuePfLine:
+        newchildren = {name: child.asfreq(freq) for name, child in self.items()}
+        return NestedRevenuePfLine(newchildren)
+
+
+@dont_init_twice
+@dataclasses.dataclass(frozen=True, repr=False, eq=False)
+class FlatCompletePfLine(FlatPfLine, CompletePfLine, PfLine):
+    # Class is only called internally, so expect df to be in correct format. Here: with columns 'w', 'q', 'p', 'r'.
+    df: pd.DataFrame
+
+    @property
+    def volume(self) -> FlatVolumePfLine:
+        return FlatVolumePfLine(self.df[["w", "q"]])
+
+    @property
+    def price(self) -> FlatPricePfLine:
+        return FlatPricePfLine(self.df[["p"]])
+
+    @property
+    def revenue(self) -> FlatRevenuePfLine:
+        return FlatRevenuePfLine(self.df[["r"]])
+
+    def asfreq(self, freq: str = "MS") -> FlatCompletePfLine:
+        newdf = tools.changefreq.summable(self.df[["q", "r"]], freq)
+        if not len(newdf):
             raise ValueError(
-                "Can only hedge with peak and offpeak products if PfLine has (quarter)hourly information."
+                f"There are no full periods available when changing to the frequency {freq}."
             )
+        newdf["w"] = newdf["q"] / tools.duration.index(newdf.index)
+        newdf["p"] = newdf["r"] / newdf["q"]
+        return FlatCompletePfLine(newdf)
+
+    @decorators.map_to_year_warning
+    def map_to_year(self, year: int, holiday_country: str = None) -> FlatVolumePfLine:
+        df = self.df[["w", "p"]]  # Averagable
+        newdf = tools.changeyear.map_frame_to_year(df, year, holiday_country)
+        newdf["q"] = newdf["w"] * tools.duration.index(newdf.index)
+        newdf["r"] = newdf["q"] * newdf["p"]
+        return FlatCompletePfLine(newdf)
+
+    def __bool__(self) -> bool:
+        return not (
+            np.allclose(self.df["w"].pint.magnitude, 0.0)
+            and np.allclose(self.df["r"].pint.magnitude, 0.0)
+        )
+
 
-        wout, pout = hedge.hedge(self.w, p.p, how, freq, po)
-        return flat.FlatPfLine({"w": wout, "p": pout})
+@dont_init_twice
+@dataclasses.dataclass(frozen=True, repr=False, eq=False)
+class NestedCompletePfLine(NestedPfLine, CompletePfLine, PfLine):
+    # Class is only called internally, so expect children to be in correct format. Here: all are complete-pflines.
+    children: Dict[str, CompletePfLine]
+    df: pd.DataFrame = dataclasses.field(init=False)
+
+    def __post_init__(self):
+        df = sum(child.df[["w", "q", "r"]] for child in self.children.values())
+        df["p"] = df["r"] / df["q"]
+        object.__setattr__(self, "df", df)
 
+    @property
+    def volume(self) -> NestedVolumePfLine:
+        newchildren = {name: child.volume for name, child in self.items()}
+        return NestedVolumePfLine(newchildren)
 
-# Must be at end, because they depend on PfLine existing.
-from . import enable_arithmatic, flat, interop, nested  # noqa
+    @property
+    def price(self) -> FlatPricePfLine:
+        # price of NestedCompletePfLine is not sum of prices of its children, so flatten first.
+        newdf = self.df[["p"]]
+        return FlatPricePfLine(newdf)
 
-enable_arithmatic.apply()
+    @property
+    def revenue(self) -> NestedRevenuePfLine:
+        newchildren = {name: child.revenue for name, child in self.items()}
+        return NestedRevenuePfLine(newchildren)
+
+    def asfreq(self, freq: str = "MS") -> NestedCompletePfLine:
+        newchildren = {name: child.asfreq(freq) for name, child in self.items()}
+        return NestedCompletePfLine(newchildren)
```

### Comparing `portfolyo-0.5.1/portfolyo/core/pfline/flat_helper.py` & `portfolyo-0.5.2/portfolyo/core/pfline/flat_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """Verify input data and turn into object needed in FlatPfLine instantiation."""
 
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, Tuple
 
 import pandas as pd
 
-# from . import flat, nested  #<-- moved to end of file
-from . import flat, interop, nested
-from .base import Kind
+from . import interop
+from .enums import Kind
 
 
-def dataframe(data: Any, __internal: bool = False) -> pd.DataFrame:
+def dataframe_and_kind(data: Any) -> Tuple[pd.DataFrame, Kind]:
     """From data, create a DataFrame with columns `w` and `q`, or column `p`, or column
     `r`, or all (`w`, `q`, `p`, `r`); with relevant units set to them. Also, do some data
-    verification."""
-    # Shortcut if PfLine is passed.
-    if isinstance(data, flat.FlatPfLine):
-        return data._df
-    if isinstance(data, nested.NestedPfLine):
-        # return data.flatten()._df  <-- don't use, causes infinite recursion due to __init__ calls.
-        return pd.DataFrame({col: getattr(data, col) for col in data.kind.available})
-    # Shortcut if called internally.
-    if __internal and isinstance(data, pd.DataFrame):
-        return data
+    verification, and find the kind of the data from the columns in the dataframe."""
+    df = _dataframe(data)
+    kind = _kind(df)
+    return df, kind
+
 
+def _dataframe(data: Any) -> pd.DataFrame:
+    """From data, create a DataFrame with columns `w` and `q`, or column `p`, or column
+    `r`, or all (`w`, `q`, `p`, `r`); with relevant units set to them. Also, do some data
+    verification."""
     # Turn into interoperability object.
     if isinstance(data, interop.InOp):
         inop = data
     else:
         inop = interop.InOp.from_data(data)
 
     # Check data types.
@@ -43,19 +41,15 @@
             " keys), or explicitly pass values with a ``pint`` unit, to indicate dimensionality."
         )
 
     # Make actual dataframe.
     return inop.to_timeseries().make_consistent().to_df()
 
 
-def kind(df: pd.DataFrame) -> Kind:
-    """Kind of data, based on columns in (consistent) dataframe."""
-    has_w, has_q, has_p, has_r = (col in df for col in "wqpr")
-    if has_w and has_q and not has_p and not has_r:
-        return Kind.VOLUME
-    if not has_w and not has_q and has_p and not has_r:
-        return Kind.PRICE
-    if not has_w and not has_q and not has_p and has_r:
-        return Kind.REVENUE
-    if has_w and has_q and has_p and has_r:
-        return Kind.COMPLETE
+def _kind(df: pd.DataFrame) -> Kind:
+    """Kind of data, based on columns in dataframe."""
+    found = set(df.columns)
+    for kind in Kind:
+        if set(kind.available) == found:
+            return kind
+
     raise ValueError(f"Unexpected columns for ``df``: {df.columns}.")
```

### Comparing `portfolyo-0.5.1/portfolyo/core/pfline/interop.py` & `portfolyo-0.5.2/portfolyo/core/pfline/interop.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Dict, Iterable, Mapping, Union
 
 import numpy as np
 import pandas as pd
 
 from ... import testing, tools
-from . import base, flat
+from . import classes, create
 
 if TYPE_CHECKING:  # needed to avoid circular imports
-    from .flat import FlatPfLine
+    from .classes import FlatPfLine
 
 _ATTRIBUTES = ("w", "q", "p", "r", "nodim", "agn")
 
 
 @dataclass(frozen=True)
 class InOp:
     """Class to check increase interoperability. Tries to extract power (w), energy (q),
@@ -402,20 +402,20 @@
 
 def pfline_or_nodimseries(
     data: Any, ref_index: pd.DatetimeIndex, agn_default: str = None
 ) -> Union[None, pd.Series, FlatPfLine]:
     """Turn ``data`` into PfLine if dimension-aware. If not, turn into Series."""
 
     # Already a PfLine.
-    if isinstance(data, base.PfLine):
+    if isinstance(data, classes.PfLine):
         return data
 
     # Can be turned into a PfLine.
     try:
-        return base.PfLine(data)
+        return create.pfline(data)
     except ValueError:
         pass
 
     # Turn into InOp object with timeseries.
     inop = InOp.from_data(data).assign_agn(agn_default).to_timeseries(ref_index)
 
     if inop.p is inop.q is inop.w is inop.r is inop.nodim is None and (
@@ -430,15 +430,15 @@
             "Cannot do this operation. If you meant to specify data of a certain dimension"
             " or unit, make it more explicit, either by specifying 'w', 'p', etc. as e.g."
             " a dictionary key, or by setting a unit e.g. in a pint Quantity."
         )
 
     elif inop.nodim is None:
         # Only dimension-aware data was supplied; must be able to turn into PfLine.
-        return flat.FlatPfLine(inop)
+        return create.flatpfline(inop)
 
     elif inop.p is inop.q is inop.w is inop.r is None:
         # Only dimensionless data was supplied; is Series of factors.
         return inop.nodim
 
     else:
         raise NotImplementedError(
```

### Comparing `portfolyo-0.5.1/portfolyo/core/pfline/nested_helper.py` & `portfolyo-0.5.2/portfolyo/core/pfline/nested_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,78 @@
 """Verify input data and turn into object needed in NestedPfLine instantiation."""
 
 from __future__ import annotations
 
-from typing import Any, Dict, Mapping, Tuple
 from collections import defaultdict
+from typing import Any, Dict, Mapping, Tuple
+
 import pandas as pd
 
 from ... import tools
-from .base import Kind, PfLine
+from . import classes, create
+from .enums import Kind
+
+
+def children_and_kind(data: Any) -> Tuple[Dict[str, classes.PfLine], Kind]:
+    mapping = _mapping(data)
+    children = _children(mapping)
+    kind = _kind(children)
+    return children, kind
 
 
-def make_mapping(data: Any) -> Mapping[Any, Any]:
+def _mapping(data: Any) -> Mapping[Any, Any]:
     """From data, create a mapping."""
-    # Shortcut if PfLine is passed.
 
     if isinstance(data, Mapping):
         return data
 
     elif isinstance(data, pd.DataFrame):
         children = {}
         # Get all sub-dataframes (or series) and turn into dictionary.
         for col in data.columns.get_level_values(0).unique():
             children[col] = data[col]
         return children
 
     raise TypeError(
-        f"Parameter ``data`` must be dict (or other Mapping) or pandas.DataFrame; got {type(data)}."
+        f"Parameter ``data`` must be dict (or other Mapping) or pandas.DataFrame; got {type(data).__name__}."
     )
 
 
-def children_and_kind(children: Dict[str, PfLine]) -> Tuple[Dict[str, PfLine], Kind]:
-    """Check number, kind, and indices of children; return corrected children and kind."""
-    # Number of children.
+def _children(mapping: Mapping) -> Dict[str, classes.PfLine]:
+    """From mapping, create dictionary of PfLines."""
+
+    # Create dictionary of PfLines.
+    children = {name: create.pfline(child) for name, child in mapping.items()}
+
+    # Assert valid keys.
+    for name in children:
+        if not isinstance(name, str):
+            raise TypeError(f"Name must be string; got {name} ({type(name)}).")
+        elif name in ["w", "q", "p", "r"]:
+            raise ValueError("Name cannot be one of 'w', 'q', 'p', 'r'.")
+
+    # Assert number of children.
     if len(children) == 0:
         raise ValueError("Must provide at least 1 child.")
+
     # Keep only overlapping part of indices.
     idx = tools.intersect.indices(*[child.index for child in children.values()])
     if len(idx) == 0:
         raise ValueError("PfLine indices have no overlap.")
-    children = {name: child.loc[idx] for name, child in children.items()}
+    return {name: child.loc[idx] for name, child in children.items()}
+
+
+def _kind(children: Dict[str, classes.PfLine]) -> Kind:
+    """Kind of data, based on children."""
 
     # Kind of children.
     kindset = set([child.kind for child in children.values()])
     if len(kindset) != 1:
         kinds1 = defaultdict(list)
         for name, child in children.items():
             kinds1[child.kind].append(name)
         kinds2 = {kind: ", ".join(names) for kind, names in kinds1.items()}
         kinds3 = " and ".join([f"{kind} ({names})" for kind, names in kinds2.items()])
         raise ValueError(f"All children must be of the same kind; found {kinds3}.")
     kind = next(iter(kindset))
 
-    return children, kind
-
-
-def dataframe(children: Dict[str, PfLine], kind: Kind) -> pd.DataFrame:
-    """Create dataframe with aggregated values."""
-    # All children have same kind, so same columns. Also, same indices, so same index.
-    df = sum(child._df for child in children.values())
-    if kind is Kind.COMPLETE:
-        df["p"] = df["r"] / df["q"]
-    return df
+    return kind
```

### Comparing `portfolyo-0.5.1/portfolyo/core/pfstate/enable_arithmatic.py` & `portfolyo-0.5.2/portfolyo/core/pfstate/arithmatic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,168 +1,198 @@
 """Add arithmatic to PfState classes."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Any, Union
 
 import pandas as pd
 
 from ... import tools
-from .. import pfline
+from ..pfline import PfLine, create
 from . import pfstate
 
 if TYPE_CHECKING:  # needed to avoid circular imports
-    from ..pfline import PfLine
-    from ..pfstate import PfState
+    from . import PfState
 
+from ... import testing
 
-def _prep_data(value, refindex: pd.DatetimeIndex) -> Union[pd.Series, PfLine, PfState]:
-    """Turn ``value`` into PfLine or PfState if possible. If not, turn into (normal or unit-aware) Series."""
 
-    # Already a PfState.
-    if isinstance(value, pfstate.PfState):
-        return value
+class Prep:
+    def assert_objects_indexcompatibility(fn):
+        """Indices must have same frequency and same start-of-day; if not, raise Error."""
 
-    # Already a PfLine.
-    if isinstance(value, pfline.PfLine):
-        return value
+        def wrapper(o1, o2, *args, **kwargs):
+            try:
+                testing.assert_indices_compatible(o1.index, o2.index)
+            except AssertionError as e:
+                raise NotImplementedError from e
+            return fn(o1, o2, *args, **kwargs)
 
-    # Series.
-    if isinstance(value, pd.Series):
-        if not hasattr(value, "pint"):  # has no unit
+        return wrapper
+
+    def standardize_other(fn):
+        """Turn other into None, PfState, PfLine, or Series."""
+
+        def wrapper(pfs: PfState, other: Any):
+            other = Prep._prep_data(other, pfs.index)
+            return fn(pfs, other)
+
+        return wrapper
+
+    def _prep_data(
+        value, refindex: pd.DatetimeIndex
+    ) -> Union[pd.Series, PfLine, PfState]:
+        """Turn ``value`` into PfLine or PfState if possible. If not, turn into (normal or unit-aware) Series."""
+
+        # None.
+        if value is None:
+            return None
+
+        # Already a PfState.
+        if isinstance(value, pfstate.PfState):
             return value
 
-        try:
-            name = tools.unit.to_name(value.pint.units)
-        except ValueError:
-            return value  # has unit, but unknown
-
-        if name not in ["p", "q", "w"]:
-            return value  # has know unit, but none from which PfLine can be made
-
-        return pfline.FlatPfLine({name: value})
-
-    # Just a single value.
-    if isinstance(value, int) or isinstance(value, float):
-        s = pd.Series(value, refindex)
-        return _prep_data(s, refindex)
-    elif isinstance(value, tools.unit.Q_):
-        s = pd.Series(value.magnitude, refindex, dtype=f"pint[{value.units:P}]")
-        return _prep_data(s, refindex)
-
-    raise TypeError(f"Cannot handle inputs of this type; got {type(value)}.")
-
-
-def _add_pfstates(pfs1: pfstate.PfState, pfs2: pfstate.PfState) -> pfstate.PfState:
-    """Add two pfstates."""
-    offtakevolume = pfs1.offtakevolume.volume + pfs2.offtakevolume.volume
-    sourced = pfs1.sourced + pfs2.sourced
-
-    # Unsourced price.
-    # . The following line works... but not if volume == 0.
-    # unsourcedprice = (pfs1.unsourced + pfs2.unsourced).price
-    # . Therefore, use weighted average.
-    values = pd.DataFrame({"s": pfs1.unsourcedprice.p, "o": pfs2.unsourcedprice.p})
-    weights = pd.DataFrame({"s": pfs1.unsourced.q, "o": pfs2.unsourced.q})
-    unsourcedprice = pfline.PfLine({"p": tools.wavg.dataframe(values, weights, axis=1)})
-
-    return pfstate.PfState(offtakevolume, unsourcedprice, sourced)
-
-
-def _nestedply_pfstate_and_series(
-    pfs: pfstate.PfState, s: pd.Series
-) -> pfstate.PfState:
-    """Multiply pfstate and Series."""
-    # Scale up volumes (and revenues), leave prices unchanged.
-    return pfstate.PfState(pfs.offtakevolume * s, pfs.unsourcedprice, pfs.sourced * s)
-
-
-def _divide_pfstates(pfs1: pfstate.PfState, pfs2: pfstate.PfState) -> pd.DataFrame:
-    """Divide two pfstates."""
-    series = {}
-    for top, bottom in [
-        ("offtake", "volume"),
-        ("sourced", "volume"),
-        ("sourced", "price"),
-        ("unsourced", "volume"),
-        ("unsourcedprice", "price"),
-        ("pnl_cost", "price"),
-    ]:
-        pfl1 = getattr(getattr(pfs1, top).flatten(), bottom)
-        pfl2 = getattr(getattr(pfs2, top).flatten(), bottom)
-        top = top.replace("unsourcedprice", "unsourced")
-        series[(top, bottom)] = pfl1 / pfl2
-    return pd.DataFrame(series)
-
-
-def _assert_index_compatibility(o1, o2):
-    if o1.index.freq != o2.index.freq:
-        raise NotImplementedError(
-            "Cannot do arithmatic with timeseries of unequal frequency."
-        )
-    if o1.index.tz != o2.index.tz:
-        raise NotImplementedError(
-            "Cannot do arithmatic with timeseries in unequal timezones."
-        )
+        # Already a PfLine.
+        if isinstance(value, PfLine):
+            return value
 
+        # Series.
+        if isinstance(value, pd.Series):
+            if not hasattr(value, "pint"):  # has no unit
+                return value
+
+            try:
+                name = tools.unit.to_name(value.pint.units)
+            except ValueError:
+                return value  # has unit, but unknown
+
+            if name not in ["p", "q", "w"]:
+                return value  # has know unit, but none from which PfLine can be made
+
+            return create.flatpfline({name: value})
+
+        # Just a single value.
+        if isinstance(value, int) or isinstance(value, float):
+            s = pd.Series(value, refindex)
+            return Prep._prep_data(s, refindex)
+        elif isinstance(value, tools.unit.Q_):
+            s = pd.Series(value.magnitude, refindex, dtype=f"pint[{value.units:P}]")
+            return Prep._prep_data(s, refindex)
+
+        raise TypeError(f"Cannot handle inputs of this type; got {type(value)}.")
+
+        # TODO: refactor and use inop
+
+    def returnself_if_otherNone(fn):
+        def wrapper(pfs: PfState, other: Any):
+            if other is None:
+                return pfs
+            return fn(pfs, other)
+
+        return wrapper
+
+    def raiseerror_if_otherNone(fn):
+        def wrapper(pfs: PfState, other: Any):
+            if other is None:
+                raise NotImplementedError("Cannot do this operation with this operand.")
+            return fn(pfs, other)
 
-class PfStateArithmatic:
+        return wrapper
 
+
+class PfStateArithmatic:
     METHODS = ["neg", "add", "radd", "sub", "rsub", "mul", "rmul", "truediv"]
 
-    def __neg__(self: PfState):
+    def __neg__(self: PfState) -> PfState:
         # invert volumes and revenues, leave prices unchanged.
         return self.__class__(-self.offtakevolume, self.unsourcedprice, -self.sourced)
 
-    def __add__(self: PfState, other):
-        if not other:
-            return self
-
-        other = _prep_data(other, self.index)  # other is now PfState, PfLine, or Series
-        _assert_index_compatibility(self, other)
-
+    @Prep.standardize_other  # other is None, PfState, Pfline, or Series
+    @Prep.returnself_if_otherNone  # other is PfState, PfLine, or Series...
+    @Prep.assert_objects_indexcompatibility  # ... with compatible index
+    def __add__(self: PfState, other: Any) -> PfState:
         # Other is a PfState.
         if isinstance(other, pfstate.PfState):
-            return _add_pfstates(self, other)
+            return Add.two_pfstates(self, other)
 
         raise NotImplementedError("This addition is not defined.")
 
-    __radd__ = __add__
-
-    def __sub__(self: PfState, other):
-        return self + -other if other else self  # defer to mul and neg
-
-    def __rsub__(self: PfState, other):
-        return other + -self  # defer to mul and neg
-
-    def __mul__(self: PfState, other):
-
-        other = _prep_data(other, self.index)  # other is now PfState, PfLine, or Series
-        _assert_index_compatibility(self, other)
+    def __radd__(self: PfState, other: Any) -> PfState:
+        return self + other  # defer to __add__
 
+    @Prep.returnself_if_otherNone  # catch pfstate - None
+    def __sub__(self: PfState, other: Any) -> PfState:
+        return self + -other  # defer to __add__ and __neg__
+
+    def __rsub__(self: PfState, other: Any) -> PfState:
+        return -self + other  # defer to __add__ and __neg__
+
+    @Prep.standardize_other  # other is None, PfState, Pfline, or Series
+    @Prep.raiseerror_if_otherNone  # other is PfState, Pfline, or Series
+    @Prep.assert_objects_indexcompatibility  # ... with a compatible index
+    def __mul__(self: PfState, other: Any) -> PfState:
         # Other is a Series (but not containing [power], [energy] or [price]).
         if isinstance(other, pd.Series):
-            return _nestedply_pfstate_and_series(self, other)
+            return Multiply.pfstate_and_series(self, other)
 
-        raise NotImplementedError("This nestedplication is not defined.")
+        raise NotImplementedError("This Multiplication is not defined.")
 
-    __rmul__ = __mul__
+    def __rmul__(self: PfState, other: Any) -> PfState:
+        return self * other  # defer to __mul__
 
+    @Prep.standardize_other  # other is None, PfState, Pfline, or Series
+    @Prep.raiseerror_if_otherNone  # other is PfState, Pfline, or Series
+    @Prep.assert_objects_indexcompatibility  # ... with a compatible index
     def __truediv__(self: PfState, other):
-        other = _prep_data(other, self.index)  # other is now PfState, PfLine, or Series
-        _assert_index_compatibility(self, other)
-
         # Other is a PfState.
         if isinstance(other, pfstate.PfState):
-            return _divide_pfstates(self, other)
+            return Divide.two_pfstates(self, other)
 
         # Other is a Series (but not containing [power], [energy] or [price]).
         if isinstance(other, pd.Series):
-            return self * (1 / other)  # defer to mul
+            return Multiply.pfstate_and_series(self, 1 / other)
 
         raise NotImplementedError("This division is not defined.")
 
 
-def apply():
-    for attr in PfStateArithmatic.METHODS:
-        attrname = f"__{attr}__"
-        setattr(pfstate.PfState, attrname, getattr(PfStateArithmatic, attrname))
+class Add:
+    def two_pfstates(pfs1: PfState, pfs2: PfState) -> PfState:
+        offtakevolume = pfs1.offtakevolume + pfs2.offtakevolume
+        sourced = pfs1.sourced + pfs2.sourced
+
+        # Unsourced price.
+        # . The following line works... but not if volume == 0.
+        # unsourcedprice = (pfs1.unsourced + pfs2.unsourced).price
+        # . Therefore, use weighted average.
+        values = pd.DataFrame({"s": pfs1.unsourcedprice.p, "o": pfs2.unsourcedprice.p})
+        weights = pd.DataFrame({"s": pfs1.unsourced.q, "o": pfs2.unsourced.q})
+        unsourcedprice = create.flatpfline(
+            {"p": tools.wavg.dataframe(values, weights, axis=1)}
+        )
+
+        return pfstate.PfState(offtakevolume, unsourcedprice, sourced)
+
+
+class Multiply:
+    def pfstate_and_series(pfs: PfState, s: pd.Series) -> PfState:
+        # Scale up volumes (and revenues), leave prices unchanged.
+        return pfstate.PfState(
+            pfs.offtakevolume * s, pfs.unsourcedprice, pfs.sourced * s
+        )
+
+
+class Divide:
+    def two_pfstates(pfs1: PfState, pfs2: PfState) -> pd.DataFrame:
+        series = {}
+        for top, bottom in [
+            ("offtake", "volume"),
+            ("sourced", "volume"),
+            ("sourced", "price"),
+            ("unsourced", "volume"),
+            ("unsourcedprice", "price"),
+            ("pnl_cost", "price"),
+        ]:
+            pfl1 = getattr(getattr(pfs1, top).flatten(), bottom)
+            pfl2 = getattr(getattr(pfs2, top).flatten(), bottom)
+            top = top.replace("unsourcedprice", "unsourced")
+            series[(top, bottom)] = pfl1 / pfl2
+        return pd.DataFrame(series)
```

### Comparing `portfolyo-0.5.1/portfolyo/core/pfstate/pfstate.py` & `portfolyo-0.5.2/portfolyo/core/pfstate/pfstate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """
 Dataframe-like class to hold energy-related timeseries, specific to portfolios, at a
 certain moment in time (e.g., at the current moment, without any historic data).
 """
 
 from __future__ import annotations
 
+import dataclasses
 import warnings
-from typing import Iterable, Optional, Union
+from typing import Iterable, Optional
 
 import pandas as pd
 
 from ... import tools
-from ..mixins import OtherOutput, PfStatePlot, PfStateText
+from ..mixins import ExcelClipboardOutput, PfStatePlot, PfStateText
 from ..ndframelike import NDFrameLike
-from ..pfline import NestedPfLine, PfLine
-from .pfstate_helper import make_pflines
+from ..pfline import PfLine, create
+from . import pfstate_helper
+from .arithmatic import PfStateArithmatic
 
 
-class PfState(NDFrameLike, PfStateText, PfStatePlot, OtherOutput):
+@dataclasses.dataclass(frozen=True, repr=False)
+class PfState(
+    NDFrameLike, PfStateText, PfStatePlot, ExcelClipboardOutput, PfStateArithmatic
+):
     """Class to hold timeseries information of an energy portfolio, at a specific moment.
 
     Parameters
     ----------
     offtakevolume: PfLine (volume-only)
     unsourcedprice: PfLine (price-only)
     sourced : PfLine (price-and-volume), optional
@@ -57,14 +62,18 @@
         portfolio is short and >0 if long. Identical to `.unsourced`, but with sign
         change for volumes and revenues (but not prices).
     pnl_cost : price-and-volume PfLine
         The expected costs needed to source the offtake volume; the sum of the sourced
         and unsourced positions.
     """
 
+    offtakevolume: PfLine
+    unsourcedprice: PfLine
+    sourced: Optional[PfLine] = None
+
     @classmethod
     def from_series(
         cls,
         *,
         pu: pd.Series,
         qo: Optional[pd.Series] = None,
         qs: Optional[pd.Series] = None,
@@ -88,128 +97,108 @@
             `ps` [Eur/MWh]
             If no volume has been sourced, all 4 sourced timeseries may be None.
 
         Returns
         -------
         PfState
         """
+        offtakevolume = create.flatpfline({"q": qo, "w": wo})
+        unsourcedprice = create.flatpfline({"p": pu})
         if not (ws is qs is rs is ps is None):
-            sourced = PfLine({"w": ws, "q": qs, "r": rs, "p": ps})
+            sourced = create.flatpfline({"w": ws, "q": qs, "r": rs, "p": ps})
         else:
             sourced = None
-        return cls(PfLine({"q": qo, "w": wo}), PfLine({"p": pu}), sourced)
+        return cls(offtakevolume, unsourcedprice, sourced)
 
-    def __init__(
-        self,
-        offtakevolume: Union[PfLine, pd.Series],
-        unsourcedprice: Union[PfLine, pd.Series],
-        sourced: Optional[PfLine] = None,
-    ):
-        # The only internal data of this class is stored as PfLines.
-        self._offtakevolume, self._unsourcedprice, self._sourced = make_pflines(
-            offtakevolume, unsourcedprice, sourced
+    def __post_init__(self):
+        offtakevolume, unsourcedprice, sourced = pfstate_helper.make_pflines(
+            self.offtakevolume, self.unsourcedprice, self.sourced
         )
+        object.__setattr__(self, "offtakevolume", offtakevolume)
+        object.__setattr__(self, "unsourcedprice", unsourcedprice)
+        object.__setattr__(self, "sourced", sourced)
 
     @property
     def index(self) -> pd.DatetimeIndex:  # from ABC
-        return self._offtakevolume.index
-
-    @property
-    def offtakevolume(self) -> PfLine:
-        return self._offtakevolume
-
-    @property
-    def unsourcedprice(self) -> PfLine:
-        return self._unsourcedprice
-
-    @property
-    def sourced(self) -> PfLine:
-        if self._sourced is None:
-            return PfLine(pd.DataFrame({"q": 0, "r": 0}, self.index))
-        else:
-            return self._sourced
+        return self.offtakevolume.index
 
     @property
     def offtake(self) -> PfLine:
         # Future development: return not volume-only but price-and-volume. (by including offtake prices)
-        return self._offtakevolume
+        return self.offtakevolume
 
     @property
     def unsourced(self) -> PfLine:
         return -(self.offtake.volume + self.sourced.volume) | self.unsourcedprice
 
     @property
     def netposition(self) -> PfLine:
         return -self.unsourced
 
     @property
     def pnl_cost(self):
-        return NestedPfLine({"sourced": self.sourced, "unsourced": self.unsourced})
+        return create.nestedpfline(
+            {"sourced": self.sourced, "unsourced": self.unsourced}
+        )
 
     @property
     def sourcedfraction(self) -> pd.Series:
         return self.sourced.volume / -self.offtake.volume
 
     @property
     def unsourcedfraction(self) -> pd.Series:
         return 1 - self.sourcedfraction
 
-    def df(
+    def dataframe(
         self,
         cols: Iterable[str] = None,
-        flatten: bool = False,
         *args,
         has_units: bool = True,
         **kwargs,
     ) -> pd.DataFrame:
         """DataFrame for portfolio state in default units.
 
         Parameters
         ----------
         cols : str, optional (default: all that are available)
             The columns (w, q, p, r) to include in the dataframe.
-        flatten : bool, optional (default: True)
-            - If True, include only aggregated timeseries (4 or less; 1 per dimension).
-            - If False, include all children and their (intermediate and final)
-              aggregations.
         has_units : bool, optional (default: True)
             - If True, return dataframe with ``pint`` units. (The unit can be extracted
               as a column level with ``.pint.dequantify()``).
             - If False, return dataframe with float values.
 
         Returns
         -------
         pd.DataFrame
         """
-
         dfs = []
         for part in ("offtakevolume", "pnl_cost", "sourced", "unsourced"):
-            fl = True if part == "pnl_cost" else flatten  # always flatten pnl_cost
-            dfin = self[part].df(cols, fl, has_units=has_units)
+            childlevels = 0 if part == "pnl_cost" else -1  # always flatten pnl_cost
+            dfin = self[part].dataframe(cols, childlevels, has_units=has_units)
             dfs.append(tools.frame.add_header(dfin, part))
         return tools.frame.concat(dfs, axis=1)
 
     # Methods that return new class instance.
 
     def set_offtakevolume(self, offtakevolume: PfLine) -> PfState:
         warnings.warn(
-            "This operation changes the unsourced volume. This causes inaccuracies in its price"
+            "This operation changes the unsourced volume. This causes inaccuracies in its price,"
             " if the portfolio state has a frequency that is longer than the spot market."
         )
-        return PfState(offtakevolume, self.unsourcedprice, self._sourced)
+        return PfState(offtakevolume, self.unsourcedprice, self.sourced)
 
     def set_unsourcedprice(self, unsourcedprice: PfLine) -> PfState:
-        return PfState(self.offtake.volume, unsourcedprice, self._sourced)
+        return PfState(self.offtake.volume, unsourcedprice, self.sourced)
 
     def set_sourced(self, sourced: PfLine) -> PfState:
         warnings.warn(
             "This operation changes the unsourced volume. This causes inaccuracies in its price"
             " if the portfolio state has a frequency that is longer than the spot market."
         )
-        return PfState(self._offtakevolume, self._unsourcedprice, sourced)
+        return PfState(self.offtakevolume, self.unsourcedprice, sourced)
 
     def add_sourced(self, add_sourced: PfLine) -> PfState:
         return self.set_sourced(self.sourced + add_sourced)  # warns
 
     def asfreq(self, freq: str = "MS") -> PfState:  # from ABC
         """Resample the Portfolio to a new frequency.
 
@@ -258,15 +247,15 @@
         Returns
         -------
         PfState
             which is fully hedged at time scales of `freq` or longer.
         """
         tosource = self.hedge_of_unsourced(how, freq, po)
         return self.__class__(
-            self._offtakevolume, self._unsourcedprice, self.sourced + tosource
+            self.offtakevolume, self.unsourcedprice, self.sourced + tosource
         )
 
     def mtm_of_sourced(self) -> PfLine:
         """Mark-to-Market value of sourced volume."""
         return self.sourced.volume * (self.unsourcedprice - self.sourced.price)
 
     # Dunder methods.
@@ -297,12 +286,7 @@
         self.pfs = pfs
 
     def __getitem__(self, arg) -> PfState:
         offtakevolume = self.pfs.offtake.volume.loc[arg]
         unsourcedprice = self.pfs.unsourcedprice.loc[arg]
         sourced = self.pfs.sourced.loc[arg]
         return PfState(offtakevolume, unsourcedprice, sourced)
-
-
-from . import enable_arithmatic  # noqa
-
-enable_arithmatic.apply()
```

### Comparing `portfolyo-0.5.1/portfolyo/core/pfstate/pfstate_helper.py` & `portfolyo-0.5.2/portfolyo/core/pfstate/pfstate_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,86 @@
 """Prepare/verify input data for PfState initialisation."""
 
 
 import warnings
 from typing import Any, Iterable
 
-from ... import tools
-from ..pfline import FlatPfLine, Kind, NestedPfLine, PfLine  # noqa
+import pandas as pd
+
+from ... import testing, tools
+from ..pfline import Kind, PfLine, create
 
 
 def make_pflines(
     offtakevolume: Any, unsourcedprice: Any, sourced: Any = None
 ) -> Iterable[PfLine]:
     """Take offtake, unsourced, sourced information. Do some data massaging and return
     3 PfLines: for offtake volume, unsourced price, and sourced price and volume.
     """
     # Ensure unsourced and offtake are specified.
     if offtakevolume is None or unsourcedprice is None:
         raise ValueError("Must specify offtake volume and unsourced prices.")
 
-    # Get everything as PfLine.
-    # . Offtake volume.
-    offtakevolume = PfLine(offtakevolume)  # force to be PfLine.
-    if offtakevolume.kind is Kind.PRICE:
+    # Offtake volume.
+    offtakevolume = prepare_offtakevolume(offtakevolume)
+    idx = offtakevolume.index
+
+    # Unsourced prices.
+    unsourcedprice = prepare_unsourcedprice(unsourcedprice, idx)
+
+    # Sourced volume/prices.
+    sourced = prepare_sourced(sourced, idx)
+
+    return offtakevolume, unsourcedprice, sourced
+
+
+def prepare_offtakevolume(offtakevolume: Any) -> PfLine:
+    offtakevolume = create.pfline(offtakevolume)  # force to be PfLine.
+    if "q" not in offtakevolume.kind.available:
         raise ValueError("Parameter ``offtakevolume`` does not contain volume.")
     elif offtakevolume.kind is Kind.COMPLETE:
         warnings.warn(
             "Parameter ``offtakevolume``: also contains price infomation; this is discarded."
         )
         offtakevolume = offtakevolume.volume
-    # . Unsourced prices.
-    unsourcedprice = PfLine(unsourcedprice)  # force to be PfLine.
-    if unsourcedprice.kind is Kind.VOLUME:
+    return offtakevolume
+
+
+def prepare_unsourcedprice(unsourcedprice: Any, ref_idx: pd.DatetimeIndex) -> PfLine:
+    unsourcedprice = create.pfline(unsourcedprice)  # force to be PfLine.
+    if "p" not in unsourcedprice.kind.available:
         raise ValueError("Parameter ``unsourcedprice`` does not contain prices.")
     elif unsourcedprice.kind is Kind.COMPLETE:
         warnings.warn(
             "Parameter ``unsourcedprice``: also contains volume infomation; this is discarded."
         )
         unsourcedprice = unsourcedprice.price
-    # . Sourced volume and prices.
-    if sourced is not None:
-        sourced = PfLine(sourced)
-        if sourced.kind is not Kind.COMPLETE:
-            raise ValueError("Parameter ``sourced`` does not contain price and volume.")
-
-    # Check/fix indices.
-    # . Frequencies.
-    freqs = [
-        o.index.freq for o in (offtakevolume, unsourcedprice, sourced) if o is not None
-    ]
-    if len(set(freqs)) != 1:
-        raise ValueError("PfLines have unequal frequency; resample first.")
-    # . Keep only overlapping part of indices.
-    idx = offtakevolume.index
-    if len(tools.intersect.indices(idx, unsourcedprice.index)) < len(idx):
+    try:
+        testing.assert_indices_compatible(ref_idx, unsourcedprice.index)
+    except AssertionError as e:
+        raise ValueError from e
+    if len(tools.intersect.indices(ref_idx, unsourcedprice.index)) < len(ref_idx):
         raise ValueError(
-            "Parameter ``unsourcedprice``: does not cover entire delivery period of ``offtakevolume``."
+            "Parameter ``unsourcedprice`` does not cover entire delivery period of"
+            " ``offtakevolume``."
         )
-    unsourcedprice = unsourcedprice.loc[idx]
-    if sourced is not None:
-        # Workaround for error in pandas intersection (#46702):
-        if len(tools.intersect.indices(idx, sourced.index)) < len(idx):
-            raise ValueError(
-                "Parameter ``sourced``: does not cover entire delivery period of ``offtakevolume``."
-            )
-        sourced = sourced.loc[idx]
+    return unsourcedprice.loc[ref_idx]
 
-    return offtakevolume, unsourcedprice, sourced
+
+def prepare_sourced(sourced: Any, ref_idx: pd.DatetimeIndex) -> PfLine:
+    if sourced is None:
+        return create.flatpfline(pd.DataFrame({"q": 0, "r": 0}, ref_idx))
+
+    sourced = create.pfline(sourced)
+    if sourced.kind is not Kind.COMPLETE:
+        raise ValueError("Parameter ``sourced`` does not contain price and volume.")
+    try:
+        testing.assert_indices_compatible(ref_idx, sourced.index)
+    except AssertionError as e:
+        raise ValueError from e
+    # Workaround for error in pandas intersection (#46702):
+    if len(tools.intersect.indices(ref_idx, sourced.index)) < len(ref_idx):
+        raise ValueError(
+            "Parameter ``sourced``: does not cover entire delivery period of"
+            " ``offtakevolume``."
+        )
+    return sourced.loc[ref_idx]
```

### Comparing `portfolyo-0.5.1/portfolyo/dev/develop.py` & `portfolyo-0.5.2/portfolyo/dev/develop.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import datetime as dt
 from typing import Dict, Union
 
 import numpy as np
 import pandas as pd
 
 from .. import tools
-from ..core.pfline import FlatPfLine, Kind, NestedPfLine, PfLine
+from ..core.pfline import FlatPfLine, Kind, Structure, NestedPfLine, PfLine, create
 from ..core.pfstate import PfState
 from . import mockup
 
 OK_COL_COMBOS = ["w", "q", "p", "pr", "qr", "qp", "wp", "wr"]
 
 
 def get_index(
@@ -124,36 +124,48 @@
     series = {col: get_series(i, col, has_unit, _seed=_seed) for col in columns}
     return pd.DataFrame(series)
 
 
 # Portfolio line.
 
 
+def get_pfline(
+    i: pd.DatetimeIndex = None,
+    kind: Kind = Kind.COMPLETE,
+    structure: Structure = Structure.FLAT,
+    *,
+    _seed: int = None,
+) -> FlatPfLine:
+    """Get a portfolio line."""
+    if structure is Structure.FLAT:
+        return get_flatpfline(i, kind, _seed=_seed)
+    else:
+        return get_nestedpfline(i, kind, _seed=_seed)
+
+
 def get_flatpfline(
     i: pd.DatetimeIndex = None, kind: Kind = Kind.COMPLETE, *, _seed: int = None
 ) -> FlatPfLine:
     """Get flat portfolio line, i.e. without children."""
-    if not isinstance(kind, Kind):
-        kind = Kind(kind)
     columns = {
         Kind.VOLUME: "q",
         Kind.PRICE: "p",
         Kind.REVENUE: "r",
         Kind.COMPLETE: "qr",
     }[kind]
-    return FlatPfLine(get_dataframe(i, columns, _seed=_seed))
+    return create.flatpfline(get_dataframe(i, columns, _seed=_seed))
 
 
 def get_nestedpfline(
     i: pd.DatetimeIndex = None, kind: Kind = Kind.COMPLETE, *, _seed: int = None
 ) -> NestedPfLine:
     """Get nested portfolio line. With 2 (flat) children of the same ``kind``."""
     if i is None:
         i = get_index(_seed=_seed)
-    return NestedPfLine(
+    return create.nestedpfline(
         {
             "A": get_flatpfline(i, kind, _seed=_seed),
             "B": get_flatpfline(i, kind, _seed=_seed),
         }
     )
 
 
@@ -180,15 +192,15 @@
     # Create nested PfLine.
     children = {}
     for c in range(childcount):
         name = f"part {prefix}{c}."
         children[name] = get_randompfline(
             i, kind, max_nlevels - 1, prefix=f"{prefix}{c}.", _seed=_seed
         )
-    return NestedPfLine(children)
+    return create.nestedpfline(children)
 
 
 # Portfolio state.
 
 
 def get_pfstate(i: pd.DatetimeIndex = None, avg=None, *, _seed: int = None) -> PfState:
     """Get portfolio state."""
```

### Comparing `portfolyo-0.5.1/portfolyo/dev/mockup.py` & `portfolyo-0.5.2/portfolyo/dev/mockup.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,23 +154,27 @@
         w_unit = w_offtake.pint.units
         sin = -1 * w_offtake.pint.magnitude
     else:
         w_unit = None
         sin = -1 * w_offtake
 
     # Do resampling.
-    def fn(sub_s):
+    def calc_wp(sub_s):
         wval = sub_s.mean() * (w_avg + rand_amp * np.random.uniform(-1, 1))
         pval = p_avg * (1 + rand_amp * np.random.uniform(-1, 1))
         return pd.DataFrame({"p": pval, "w": wval}, sub_s.index)
 
+    def group_and_calc(s):
+        return s.resample(freq, group_keys=False).apply(calc_wp)
+
     if sin.index.freq in ["15T", "H"]:
-        df = sin.groupby(is_peak_hour).apply(lambda s: s.resample(freq).apply(fn))
+        is_peak = is_peak_hour(sin.index)  # avoid running on each ts individually
+        df = sin.groupby(is_peak, group_keys=False).apply(group_and_calc)
     else:
-        df = sin.resample(freq).apply(fn)
+        df = group_and_calc(sin)
     w, p = df.w, df.p
 
     # Add unit if wanted.
     if has_unit:
         wunit = f"pint[{w_unit:P}]" if w_unit is not None else "pint[MW]"
         w = w.astype(wunit)
         p = p.astype("pint[Eur/MWh]")
```

### Comparing `portfolyo-0.5.1/portfolyo/prices/convert.py` & `portfolyo-0.5.2/portfolyo/prices/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,17 @@
     # Remove partial data
     s = tools.trim.frame(s, freq)
 
     # Handle possible units.
     sin, units = (s.pint.magnitude, s.pint.units) if hasattr(s, "pint") else (s, None)
 
     # Do calculations. Use normal mean, because all rows have same duration.
-    sout = sin.resample(freq).apply(lambda s: tseries2singlebpo(s, prefix))
+    sout = sin.resample(freq, group_keys=True).apply(
+        lambda s: tseries2singlebpo(s, prefix)
+    )
 
     # Handle possible units.
     if units is not None:
         sout = sout.astype(f"pint[{units}]")
     return sout.unstack()
```

### Comparing `portfolyo-0.5.1/portfolyo/prices/hedge.py` & `portfolyo-0.5.2/portfolyo/prices/hedge.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/prices/utils.py` & `portfolyo-0.5.2/portfolyo/prices/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,30 +76,30 @@
             f"Parameter ``freq`` must be one of {', '.join(tools.freq.FREQUENCIES)}; got {freq}."
         )
 
     if isinstance(ts_left, pd.DatetimeIndex):
         if freq in ["15T", "H"]:
             return tools.duration.index(ts_left, freq) * is_peak_hour(ts_left)
         elif freq == "D":
-            hours = ts_left.map(lambda ts: ts.isoweekday() < 6) * 12  # no unit
+            hours = ts_left.map(lambda ts: ts.isoweekday() < 6) * 12.0  # no unit
             return pd.Series(hours, ts_left, dtype="pint[h]")  # works even during dst
         else:
             # dur = ts_left.map(duration_peak)  # crashes due to behaviour of .map method
             hours = (duration_peak(ts, freq) for ts in ts_left)  # has unit
             return pd.Series(hours, ts_left, dtype="pint[h]")
 
     # Assume it's a single timestamp.
     if freq in ["15T", "H"]:
         return tools.duration.stamp(ts_left, freq) * is_peak_hour(ts_left)
     elif freq == "D":
-        return Q_(0 if ts_left.isoweekday() >= 6 else 12, "h")
+        return Q_(0.0 if ts_left.isoweekday() >= 6 else 12.0, "h")
     else:
         ts_right = tools.right.stamp(ts_left, freq)
         days = pd.date_range(ts_left, ts_right, freq="D", inclusive="left")
-        return Q_(sum(days.map(lambda day: day.isoweekday() < 6) * 12), "h")
+        return Q_(sum(days.map(lambda day: day.isoweekday() < 6) * 12.0), "h")
 
 
 def duration_offpeak(
     ts_left: Union[pd.Timestamp, pd.DatetimeIndex], freq: str = None
 ) -> Union[Q_, pd.Series]:
     """
     Total duration of offpeak periods in a timestamp.
```

### Comparing `portfolyo-0.5.1/portfolyo/testing/testing.py` & `portfolyo-0.5.2/portfolyo/testing/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 import pandas as pd
 
 from .. import tools
 from ..tools.unit import Q_
 
 
 @functools.wraps(pd.testing.assert_frame_equal)
-def assert_frame_equal(left, right, *args, **kwargs):
+def assert_frame_equal(left: pd.DataFrame, right: pd.DataFrame, *args, **kwargs):
     # Dataframes equal even if *order* of columns is not the same.
     left = tools.unit.drop_units(left).sort_index(axis=1)
     right = tools.unit.drop_units(right).sort_index(axis=1)
     left = left.replace([np.inf, -np.inf], np.nan)
     right = right.replace([np.inf, -np.inf], np.nan)
     pd.testing.assert_frame_equal(left, right, *args, **kwargs)
 
 
 @functools.wraps(pd.testing.assert_series_equal)
-def assert_series_equal(left, right, *args, **kwargs):
-
+def assert_series_equal(left: pd.Series, right: pd.Series, *args, **kwargs):
     if hasattr(left, "pint") and hasattr(right, "pint"):  # pint-series
         left, right = left.pint.to_base_units(), right.pint.to_base_units()
         assert left.pint.u == right.pint.u
         assert_series_equal(left.pint.m, right.pint.m, *args, **kwargs)
 
     elif left.dtype == right.dtype == object:  # maybe: series of Quantities
         try:
@@ -44,14 +43,21 @@
         right = right.replace([np.inf, -np.inf], np.nan)
         pd.testing.assert_series_equal(left, right, *args, **kwargs)
 
 
 assert_index_equal = pd.testing.assert_index_equal
 
 
+def assert_indices_compatible(left: pd.DatetimeIndex, right: pd.DatetimeIndex):
+    if (lf := left.freq) != (r := right.freq):
+        raise AssertionError(f"Indices have unequal frequency: {lf} and {r}.")
+    if (lf := left[0].time()) != (r := right[0].time()):
+        raise AssertionError(f"Indices that have unequal start-of-day; {lf} and {r}.")
+
+
 def assert_w_q_compatible(freq: str, w: pd.Series, q: pd.Series):
     """Assert if timeseries with power- and energy-values are consistent."""
     if freq == "15T":
         assert_series_equal(q, w * Q_(0.25, "h"), check_names=False)
     elif freq == "H":
         assert_series_equal(q, w * Q_(1.0, "h"), check_names=False)
     elif freq == "D":
```

### Comparing `portfolyo-0.5.1/portfolyo/tools/ceil.py` & `portfolyo-0.5.2/portfolyo/tools/ceil.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/changefreq.py` & `portfolyo-0.5.2/portfolyo/tools/changefreq.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/changeyear.py` & `portfolyo-0.5.2/portfolyo/tools/changeyear.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,14 @@
 
 
 def _map_index_to_index_daily(
     idx_source: pd.DatetimeIndex,
     idx_target: pd.DatetimeIndex,
     holiday_country: str = None,
 ) -> pd.Series:
-
     # Split into months.
     idx_source_by_m = {m: s.index for m, s in pd.Series(0, idx_source).resample("MS")}
     idx_target_by_m = {m: s.index for m, s in pd.Series(0, idx_target).resample("MS")}
 
     # Mapping on month-level.
     mapp_m = _map_index_to_index_monthlyandlonger(
         pd.DatetimeIndex(idx_source_by_m.keys(), freq="MS"),
@@ -207,15 +206,14 @@
     mapping.index.freq = "D"
     return mapping
 
 
 def _map_index_to_index_daily_samemonth(
     idx_source: pd.DatetimeIndex, idx_target: pd.DatetimeIndex, holiday_country: str
 ) -> pd.Series:
-
     months = set([*[ts.month for ts in idx_source], *[ts.month for ts in idx_target]])
     if len(months) > 1:
         raise ValueError(
             f"Indices must contain timestamps of only one calender month; found {months}."
         )
 
     source = characterize_index(idx_source, holiday_country)
```

### Comparing `portfolyo-0.5.1/portfolyo/tools/duration.py` & `portfolyo-0.5.2/portfolyo/tools/duration.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     24.0 h
     >>> duration.stamp(pd.Timestamp('2020-03-29'), 'D')
     24.0 h
     >>> duration.stamp(pd.Timestamp('2020-03-29', tz='Europe/Berlin'), 'D')
     23.0 h
     """
     if freq in ["15T", "H"]:
-        h = 1 if freq == "H" else 0.25
+        h = 1.0 if freq == "H" else 0.25
     else:
         h = (tools_right.stamp(ts, freq) - ts).total_seconds() / 3600
     return tools_unit.Q_(h, "h")
 
 
 def index(i: pd.DatetimeIndex) -> pd.Series:
     """Duration of a timestamp.
```

### Comparing `portfolyo-0.5.1/portfolyo/tools/floor.py` & `portfolyo-0.5.2/portfolyo/tools/floor.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/frame.py` & `portfolyo-0.5.2/portfolyo/tools/frame.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/freq.py` & `portfolyo-0.5.2/portfolyo/tools/freq.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,22 +26,23 @@
     ----------
     freq_source, freq_target : frequencies to compare.
     common_ts : timestamp, optional
         Timestamp to use as anchor from which to compare the two.
 
     Returns
     -------
-    1 (-1, 0) if source frequency must be upsampled (downsampled, no change) to obtain
-        target frequency.
+    * 1 if source frequency must be upsampled to obtain (i.e, is longer than) target frequency.
+    * 0 if source frequency is same as target frequency.
+    * -1 if source frequency must be downsampled to obtain (i.e, is shorter than) target frequency.
 
     Notes
     -----
     Arbitrarily using a time point as anchor to calculate the length of the time period
     from. May have influence on the ratio (duration of a month, quarter, year etc are
-    influenced by this), but, for most common frequencies, not on which is larger.
+    influenced by this), but, for most common frequencies, not on which is longer.
 
     Examples
     --------
     >>> freq.up_or_down('D', 'MS')
     -1
     >>> freq.up_or_down('MS', 'D')
     1
@@ -60,14 +61,48 @@
         return -1
     if common_ts == standard_common_ts:
         # If they are the same, try with another timestamp.
         return up_or_down(freq_source, freq_target, backup_common_ts)
     return 0  # only if both give the same answer.
 
 
+def longer_or_shorter(freq: str, freq_ref: str, common_ts: pd.Timedelta = None) -> int:
+    """
+    Compare frequency with reference frequency to see if it is longer or shorter.
+
+    Parameters
+    ----------
+    freq, freq_ref : frequencies to compare.
+    common_ts : timestamp, optional
+        Timestamp to use as anchor from which to compare the two.
+
+    Returns
+    -------
+    * 1 if frequency ``freq`` is longer than the reference frequency ``freq_ref``.
+    * 0 if frequencies are the same.
+    * -1 if frequency ``freq`` is shorter than the reference frequency ``freq_ref``.
+
+    Notes
+    -----
+    Arbitrarily using a time point as anchor to calculate the length of the time period
+    from. May have influence on the ratio (duration of a month, quarter, year etc are
+    influenced by this), but, for most common frequencies, not on which is longer.
+
+    Examples
+    --------
+    >>> freq.longer_or_shorter('D', 'MS')
+    -1
+    >>> freq.longer_or_shorter('MS', 'D')
+    1
+    >>> freq.longer_or_shorter('MS', 'MS')
+    0
+    """
+    return up_or_down(freq, freq_ref, common_ts)
+
+
 def _longestshortest(shortest: bool, *freqs: str):
     """Determine which frequency denotes the shortest or longest time period."""
     common_ts = pd.Timestamp("2020-01-01")
     ts = [common_ts + pd.tseries.frequencies.to_offset(fr) for fr in freqs]
     i = (np.argmin if shortest else np.argmax)(ts)
     return freqs[i]
```

### Comparing `portfolyo-0.5.1/portfolyo/tools/intersect.py` & `portfolyo-0.5.2/portfolyo/tools/intersect.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/isboundary.py` & `portfolyo-0.5.2/portfolyo/tools/isboundary.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/leftandright.py` & `portfolyo-0.5.2/portfolyo/tools/leftandright.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/peakperiod.py` & `portfolyo-0.5.2/portfolyo/tools/peakperiod.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/right.py` & `portfolyo-0.5.2/portfolyo/tools/right.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/righttoleft.py` & `portfolyo-0.5.2/portfolyo/tools/righttoleft.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/round.py` & `portfolyo-0.5.2/portfolyo/tools/round.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/standardize.py` & `portfolyo-0.5.2/portfolyo/tools/standardize.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/trim.py` & `portfolyo-0.5.2/portfolyo/tools/trim.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/tzone.py` & `portfolyo-0.5.2/portfolyo/tools/tzone.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/unit.py` & `portfolyo-0.5.2/portfolyo/tools/unit.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/unitdefinitions.txt` & `portfolyo-0.5.2/portfolyo/tools/unitdefinitions.txt`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/tools/wavg.py` & `portfolyo-0.5.2/portfolyo/tools/wavg.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,23 +71,29 @@
     if weights is None:
         return s.mean()
 
     # Prep: ensure weights is also a Series.
     if not isinstance(weights, pd.Series):
         weights = pd.Series(weights, s.index)
 
+    # Special case: if total weight is 0, but all original values are identical, return this value.
+    if np.isclose(weights.sum(), 0) and s.nunique() == 1:
+        return s.iloc[0]
+
+    # Prep: if a weight is 0, corresponding value is irrelevant. Even if it is NaN.
+    drop = weights == 0  # Replace with np.isclose? Must work with float and pint
+    if drop.any() and not drop.all():
+        keep = weights[~drop].index
+        s = s.loc[keep]
+        weights = weights.loc[keep]
     # Get multiplication factors as floats.
     factors = (weights / weights.sum()).astype(float)
     # Calculate the average.
     result = s.mul(factors).sum(skipna=False)  # float or quantity
 
-    # Special case: if total weight is 0, but all original values are identical, return this value.
-    if np.isclose(weights.sum(), 0) and s.nunique() == 1:
-        return s.iloc[0]
-
     return result
 
 
 def dataframe(
     df: pd.DataFrame,
     weights: Union[Iterable, pd.Series, pd.DataFrame] = None,
     axis: int = 0,
```

### Comparing `portfolyo-0.5.1/portfolyo/visualize/categories.py` & `portfolyo-0.5.2/portfolyo/visualize/categories.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         raise ValueError("Daily (or shorter) data should not be plotted as categories.")
 
     return [category(i, ts, y) for i, (ts, y) in enumerate(s.items())]
 
 
 def priolist(n):
     """Create list with n priority numbers, which indicate how important a given element
-    is on a categorical scale. The higher the number, the more easily it can be dropped."""
+    is on a categorical scale. The higher the number, the more easily it can be dropped.
+    """
     prio = 0
     prios = [prio]
     while len(prios) < n:
         prio += 1
         prios = [prios[i // 2] if i % 2 == 0 else prio for i in range(len(prios) * 2)]
     return prios[:n]
```

### Comparing `portfolyo-0.5.1/portfolyo/visualize/colors.py` & `portfolyo-0.5.2/portfolyo/visualize/colors.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/portfolyo/visualize/plot.py` & `portfolyo-0.5.2/portfolyo/visualize/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,16 @@
 
 
 @append_to_doc(docstringliteral_plotparameters)
 def plot_timeseries_as_jagged(
     ax: plt.Axes, s: pd.Series, labelfmt: str = "", cat: bool = None, **kwargs
 ) -> None:
     """Plot timeseries ``s`` to axis ``ax``, as jagged line and/or as markers. Use kwargs
-    ``linestyle`` and ``marker`` to specify line style and/or marker style. (Default: line only)."""
+    ``linestyle`` and ``marker`` to specify line style and/or marker style. (Default: line only).
+    """
     s = prepare_ax_and_s(ax, s)  # ensure unit compatibility (if possible)
 
     if use_categories(ax, s, cat):
         categories = Categories(s)
         ax.plot(categories.x(), categories.y(), **kwargs)
         ax.set_xticks(categories.x(MAX_XLABELS), categories.labels(MAX_XLABELS))
         set_data_labels(ax, categories.x(), categories.y(), labelfmt, False)
```

### Comparing `portfolyo-0.5.1/portfolyo.egg-info/PKG-INFO` & `portfolyo-0.5.2/portfolyo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolyo
-Version: 0.5.1
+Version: 0.5.2
 Summary: Analysing and manipulating timeseries related to power and gas offtake portfolios.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENCE
 
 portfolyo
```

### Comparing `portfolyo-0.5.1/portfolyo.egg-info/SOURCES.txt` & `portfolyo-0.5.2/portfolyo.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -14,27 +14,34 @@
 portfolyo.egg-info/requires.txt
 portfolyo.egg-info/top_level.txt
 portfolyo/core/__init__.py
 portfolyo/core/extendpandas.py
 portfolyo/core/ndframelike.py
 portfolyo/core/suppresswarnings.py
 portfolyo/core/mixins/__init__.py
-portfolyo/core/mixins/other.py
+portfolyo/core/mixins/excelclipboard.py
 portfolyo/core/mixins/plot.py
 portfolyo/core/mixins/text.py
 portfolyo/core/pfline/__init__.py
-portfolyo/core/pfline/base.py
-portfolyo/core/pfline/enable_arithmatic.py
-portfolyo/core/pfline/flat.py
+portfolyo/core/pfline/arithmatic.py
+portfolyo/core/pfline/children.py
+portfolyo/core/pfline/classes.py
+portfolyo/core/pfline/create.py
+portfolyo/core/pfline/dataframeexport.py
+portfolyo/core/pfline/decorators.py
+portfolyo/core/pfline/developernotes.py
+portfolyo/core/pfline/enums.py
 portfolyo/core/pfline/flat_helper.py
+portfolyo/core/pfline/flat_methods.py
 portfolyo/core/pfline/interop.py
-portfolyo/core/pfline/nested.py
 portfolyo/core/pfline/nested_helper.py
+portfolyo/core/pfline/nested_methods.py
+portfolyo/core/pfline/prices.py
 portfolyo/core/pfstate/__init__.py
-portfolyo/core/pfstate/enable_arithmatic.py
+portfolyo/core/pfstate/arithmatic.py
 portfolyo/core/pfstate/pfstate.py
 portfolyo/core/pfstate/pfstate_helper.py
 portfolyo/dev/__init__.py
 portfolyo/dev/develop.py
 portfolyo/dev/mockup.py
 portfolyo/prices/__init__.py
 portfolyo/prices/convert.py
```

### Comparing `portfolyo-0.5.1/setup.py` & `portfolyo-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.1/versioneer.py` & `portfolyo-0.5.2/versioneer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -277,21 +277,21 @@
 # pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
 # pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
 # pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
 # pylint:disable=attribute-defined-outside-init,too-many-arguments
 
 import configparser
 import errno
+import functools
 import json
 import os
 import re
 import subprocess
 import sys
 from typing import Callable, Dict
-import functools
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
 
 def get_root():
```

