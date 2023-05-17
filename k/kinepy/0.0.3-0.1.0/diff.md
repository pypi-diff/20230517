# Comparing `tmp/kinepy-0.0.3.tar.gz` & `tmp/kinepy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kinepy-0.0.3.tar", last modified: Tue Nov 22 09:23:46 2022, max compression
+gzip compressed data, was "kinepy-0.1.0.tar", last modified: Wed May 17 07:04:49 2023, max compression
```

## Comparing `kinepy-0.0.3.tar` & `kinepy-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 09:23:46.279355 kinepy-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2022-11-22 09:23:33.000000 kinepy-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      327 2022-11-22 09:23:46.279355 kinepy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2168 2022-11-22 09:23:33.000000 kinepy-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 09:23:46.275355 kinepy-0.0.3/kinepy/
--rw-r--r--   0 runner    (1001) docker     (122)    14767 2022-11-22 09:23:33.000000 kinepy-0.0.3/kinepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8502 2022-11-22 09:23:33.000000 kinepy-0.0.3/kinepy/compilation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9138 2022-11-22 09:23:33.000000 kinepy-0.0.3/kinepy/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (122)     3155 2022-11-22 09:23:33.000000 kinepy-0.0.3/kinepy/geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2419 2022-11-22 09:23:33.000000 kinepy-0.0.3/kinepy/interactions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9645 2022-11-22 09:23:33.000000 kinepy-0.0.3/kinepy/kinematic.py
--rw-r--r--   0 runner    (1001) docker     (122)    17414 2022-11-22 09:23:33.000000 kinepy-0.0.3/kinepy/linkage.py
--rw-r--r--   0 runner    (1001) docker     (122)     6282 2022-11-22 09:23:33.000000 kinepy-0.0.3/kinepy/metajoints.py
--rw-r--r--   0 runner    (1001) docker     (122)     2667 2022-11-22 09:23:33.000000 kinepy-0.0.3/kinepy/solid.py
--rw-r--r--   0 runner    (1001) docker     (122)     3933 2022-11-22 09:23:33.000000 kinepy-0.0.3/kinepy/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 09:23:46.279355 kinepy-0.0.3/kinepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      327 2022-11-22 09:23:46.000000 kinepy-0.0.3/kinepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      348 2022-11-22 09:23:46.000000 kinepy-0.0.3/kinepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-22 09:23:46.000000 kinepy-0.0.3/kinepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2022-11-22 09:23:46.000000 kinepy-0.0.3/kinepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2022-11-22 09:23:46.279355 kinepy-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      406 2022-11-22 09:23:33.000000 kinepy-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:04:49.732165 kinepy-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-17 07:04:34.000000 kinepy-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-17 07:04:49.732165 kinepy-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-17 07:04:34.000000 kinepy-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:04:49.732165 kinepy-0.1.0/kinepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 07:04:34.000000 kinepy-0.1.0/kinepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-05-17 07:04:34.000000 kinepy-0.1.0/kinepy/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-17 07:04:34.000000 kinepy-0.1.0/kinepy/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:04:49.732165 kinepy-0.1.0/kinepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-17 07:04:49.000000 kinepy-0.1.0/kinepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 07:04:49.000000 kinepy-0.1.0/kinepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:04:49.000000 kinepy-0.1.0/kinepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 07:04:49.000000 kinepy-0.1.0/kinepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-17 07:04:49.732165 kinepy-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-17 07:04:34.000000 kinepy-0.1.0/setup.py
```

### Comparing `kinepy-0.0.3/LICENSE` & `kinepy-0.1.0/LICENSE`

 * *Files identical despite different names*

