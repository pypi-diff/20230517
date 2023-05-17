# Comparing `tmp/connectome-0.6.0.tar.gz` & `tmp/connectome-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome-0.6.0.tar", last modified: Sun Apr  9 19:36:32 2023, max compression
+gzip compressed data, was "connectome-0.6.1.tar", last modified: Wed May 17 15:01:47 2023, max compression
```

## Comparing `connectome-0.6.0.tar` & `connectome-0.6.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.310780 connectome-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-04-09 19:36:30.000000 connectome-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-09 19:36:30.000000 connectome-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-09 19:36:32.310780 connectome-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-09 19:36:30.000000 connectome-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.302780 connectome-0.6.0/connectome/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.306780 connectome-0.6.0/connectome/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/cache/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/cache/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.306780 connectome-0.6.0/connectome/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/containers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/containers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/containers/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/containers/reversible.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.306780 connectome-0.6.0/connectome/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/node_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/vm.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.306780 connectome-0.6.0/connectome/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/complex_edges.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/factory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/metaclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.310780 connectome-0.6.0/connectome/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.306780 connectome-0.6.0/connectome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-09 19:36:32.000000 connectome-0.6.0/connectome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-09 19:36:32.000000 connectome-0.6.0/connectome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:36:32.000000 connectome-0.6.0/connectome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 19:36:32.000000 connectome-0.6.0/connectome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 19:36:32.000000 connectome-0.6.0/connectome.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-09 19:36:30.000000 connectome-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 19:36:30.000000 connectome-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:36:32.310780 connectome-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-09 19:36:30.000000 connectome-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.416990 connectome-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-05-17 15:01:42.000000 connectome-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 15:01:42.000000 connectome-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-17 15:01:47.416990 connectome-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-17 15:01:42.000000 connectome-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.412990 connectome-0.6.1/connectome/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.412990 connectome-0.6.1/connectome/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/cache/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/cache/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.412990 connectome-0.6.1/connectome/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/containers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/containers/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/containers/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/containers/reversible.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.412990 connectome-0.6.1/connectome/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/node_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.416990 connectome-0.6.1/connectome/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/complex_edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/factory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/metaclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.416990 connectome-0.6.1/connectome/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.412990 connectome-0.6.1/connectome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-17 15:01:47.000000 connectome-0.6.1/connectome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-17 15:01:47.000000 connectome-0.6.1/connectome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:01:47.000000 connectome-0.6.1/connectome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 15:01:47.000000 connectome-0.6.1/connectome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 15:01:47.000000 connectome-0.6.1/connectome.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-17 15:01:42.000000 connectome-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 15:01:42.000000 connectome-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:01:47.416990 connectome-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-17 15:01:42.000000 connectome-0.6.1/setup.py
```

### Comparing `connectome-0.6.0/LICENSE` & `connectome-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/PKG-INFO` & `connectome-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: connectome
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library for datasets containing heterogeneous data
 Home-page: https://github.com/neuro-ml/connectome
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/connectome/archive/v0.6.0.tar.gz
+Download-URL: https://github.com/neuro-ml/connectome/archive/v0.6.1.tar.gz
 Keywords: dag,dataset,cache,consistency
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `connectome-0.6.0/README.md` & `connectome-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/cache/base.py` & `connectome-0.6.1/connectome/cache/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/cache/disk.py` & `connectome-0.6.1/connectome/cache/disk.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import logging
 
 from tarn import PickleKeyStorage
+from tarn.interface import MaybeLabels
 
 from .base import Cache
 
 logger = logging.getLogger(__name__)
 
 
 class DiskCache(Cache):
-    def __init__(self, pool: PickleKeyStorage):
+    def __init__(self, pool: PickleKeyStorage, labels: MaybeLabels = None):
         super().__init__()
         self.cache = pool
+        self.labels = labels
 
     def prepare(self, param):
         raw = param.value
         context = self.cache.prepare(raw)
         return context.digest, context
 
     def get(self, key, context):
         return self.cache.read(context, error=False)
 
     def set(self, key, value, context):
-        self.cache.write(context, value, error=False)
+        self.cache.write(context, value, error=False, labels=self.labels)
```

### Comparing `connectome-0.6.0/connectome/cache/memory.py` & `connectome-0.6.1/connectome/cache/memory.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/containers/base.py` & `connectome-0.6.1/connectome/containers/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/containers/context.py` & `connectome-0.6.1/connectome/containers/context.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/containers/group.py` & `connectome-0.6.1/connectome/containers/group.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/containers/reversible.py` & `connectome-0.6.1/connectome/containers/reversible.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/engine/base.py` & `connectome-0.6.1/connectome/engine/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/engine/compiler.py` & `connectome-0.6.1/connectome/engine/compiler.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/engine/edges.py` & `connectome-0.6.1/connectome/engine/edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/engine/executor.py` & `connectome-0.6.1/connectome/engine/executor.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/engine/graph.py` & `connectome-0.6.1/connectome/engine/graph.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/engine/node_hash.py` & `connectome-0.6.1/connectome/engine/node_hash.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/engine/utils.py` & `connectome-0.6.1/connectome/engine/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/engine/vm.py` & `connectome-0.6.1/connectome/engine/vm.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/interface/blocks.py` & `connectome-0.6.1/connectome/interface/blocks.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/interface/complex_edges.py` & `connectome-0.6.1/connectome/interface/complex_edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/interface/edges.py` & `connectome-0.6.1/connectome/interface/edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/interface/factory.py` & `connectome-0.6.1/connectome/interface/factory.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/interface/metaclasses.py` & `connectome-0.6.1/connectome/interface/metaclasses.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/interface/nodes.py` & `connectome-0.6.1/connectome/interface/nodes.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/interface/utils.py` & `connectome-0.6.1/connectome/interface/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/layers/apply.py` & `connectome-0.6.1/connectome/layers/apply.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/layers/base.py` & `connectome-0.6.1/connectome/layers/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/layers/cache.py` & `connectome-0.6.1/connectome/layers/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Container as ContainerType, Sequence, Union
 
 import numpy as np
 from tarn import DiskDict, HashKeyStorage, PickleKeyStorage
 from tarn.config import StorageConfig, init_storage
+from tarn.interface import MaybeLabels
 
 from ..cache import Cache, DiskCache, MemoryCache
 from ..containers import EdgesBag, IdentityContext
 from ..engine import CacheEdge, Details, ImpureEdge, Node, TreeNode
 from ..serializers import ChainSerializer, JsonSerializer, NumpySerializer, PickleSerializer, Serializer
 from ..utils import AntiSet, PathLike, StringsLike, node_to_dict, to_seq
 from .base import Layer
@@ -110,24 +111,25 @@
     impure
         whether to allow caching of `impure` functions
     remote
         remote locations that are used to fetch the cache from (if available)
     """
 
     def __init__(self, index: PathLikes, storage: HashKeyStorage, serializer: SerializersLike, names: StringsLike, *,
-                 impure: bool = False):
+                 impure: bool = False, labels: MaybeLabels = None):
         super().__init__(names=names, impure=impure)
         names, serializer = _normalize_disk_arguments(names, serializer)
-        self.storage = DiskCache(PickleKeyStorage(index, storage, serializer))
+        self.storage = DiskCache(PickleKeyStorage(index, storage, serializer), labels=labels)
 
     def _get_storage(self) -> Cache:
         return self.storage
 
     @classmethod
-    def simple(cls, *names, root: PathLike, serializer: Union[Serializer, Sequence[Serializer]] = None):
+    def simple(cls, *names, root: PathLike, serializer: Union[Serializer, Sequence[Serializer]] = None, 
+               labels: MaybeLabels = None):
         """
         A simple version of caching to disk with adequate default settings.
 
         Parameters
         ----------
         names:
             the field names to cache
@@ -154,15 +156,15 @@
         if serializer is None:
             serializer = ChainSerializer(
                 JsonSerializer(),
                 NumpySerializer({np.bool_: 1, np.int_: 1}),
                 PickleSerializer(),
             )
 
-        return cls(index, HashKeyStorage(DiskDict(storage)), serializer, names)
+        return cls(index, HashKeyStorage(DiskDict(storage)), serializer, names, labels=labels)
 
 
 def _normalize_disk_arguments(names, serializer):
     return to_seq(names), _resolve_serializer(serializer)
 
 
 def _resolve_serializer(serializer):
```

### Comparing `connectome-0.6.0/connectome/layers/columns.py` & `connectome-0.6.1/connectome/layers/columns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from itertools import starmap
 from math import ceil
 from typing import Any, Generator, Union
 
 from tarn import HashKeyStorage, PickleKeyStorage
+from tarn.interface import MaybeLabels
 from tqdm.auto import tqdm
 
 from ..cache import DiskCache, MemoryCache
 from ..containers import EdgesBag, IdentityContext
 from ..engine import Command, Details, Edge, Graph, HashOutput, Node, NodeHash, NodeHashes, Request, Response, TreeNode
 from ..engine.node_hash import ApplyHash
 from ..exceptions import DependencyError
@@ -37,24 +38,24 @@
     shard_size
         the size of a disk storage shard. If int - an absolute size value is used,
         if float - a portion relative to the dataset is used,
         if None - all the entries are grouped in a single shard
     """
 
     def __init__(self, index: PathLikes, storage: HashKeyStorage, serializer: SerializersLike, names: StringsLike, *,
-                 verbose: bool = False, shard_size: Union[int, float, None] = None):
+                 verbose: bool = False, shard_size: Union[int, float, None] = None, labels: MaybeLabels = None):
         if shard_size == 1:
             raise ValueError(f'Shard size of 1 is ambiguous. Use None if you want to have a single shard')
         names, serializer = _normalize_disk_arguments(names, serializer)
 
         super().__init__()
         self.names = names
         self.shard_size = shard_size
         self.verbose = verbose
-        self.disk = DiskCache(PickleKeyStorage(index, storage, serializer))
+        self.disk = DiskCache(PickleKeyStorage(index, storage, serializer), labels=labels)
         self.ram = MemoryCache(None)
 
     def _prepare_container(self, previous: EdgesBag) -> EdgesBag:
         details = Details(type(self))
         copy = previous.freeze(details)
         mapping = TreeNode.from_edges(copy.edges)
         outputs_copy = node_to_dict(copy.outputs)
```

### Comparing `connectome-0.6.0/connectome/layers/filter.py` & `connectome-0.6.1/connectome/layers/filter.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/layers/join.py` & `connectome-0.6.1/connectome/layers/join.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/layers/merge.py` & `connectome-0.6.1/connectome/layers/merge.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome/utils.py` & `connectome-0.6.1/connectome/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/connectome.egg-info/PKG-INFO` & `connectome-0.6.1/connectome.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: connectome
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library for datasets containing heterogeneous data
 Home-page: https://github.com/neuro-ml/connectome
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/connectome/archive/v0.6.0.tar.gz
+Download-URL: https://github.com/neuro-ml/connectome/archive/v0.6.1.tar.gz
 Keywords: dag,dataset,cache,consistency
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `connectome-0.6.0/connectome.egg-info/SOURCES.txt` & `connectome-0.6.1/connectome.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/pyproject.toml` & `connectome-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `connectome-0.6.0/setup.py` & `connectome-0.6.1/setup.py`

 * *Files identical despite different names*

