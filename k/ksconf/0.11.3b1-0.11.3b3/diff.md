# Comparing `tmp/ksconf-0.11.3b1.tar.gz` & `tmp/ksconf-0.11.3b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ksconf-0.11.3b1.tar", last modified: Mon May 15 13:09:35 2023, max compression
+gzip compressed data, was "ksconf-0.11.3b3.tar", last modified: Wed May 17 15:30:06 2023, max compression
```

## Comparing `ksconf-0.11.3b1.tar` & `ksconf-0.11.3b3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.291230 ksconf-0.11.3b1/ksconf/
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/app/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/app/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/app/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/app/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/builder/
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/builder/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/builder/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/builder/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/commands/
--rw-r--r--   0 runner    (1001) docker     (123)    22120 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    22959 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/promote.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/restexport.py
--rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/restpublish.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/unarchive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/commands/xmlformat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/conf/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/conf/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/conf/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/conf/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14340 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/setup_entrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/util/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/util/completers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/util/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/util/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/util/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.295230 ksconf-0.11.3b1/ksconf/vc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/vc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/vc/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/ksconf/xmlformat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:35.291230 ksconf-0.11.3b1/ksconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 13:09:35.000000 ksconf-0.11.3b1/ksconf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:09:20.000000 ksconf-0.11.3b1/ksconf.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-15 13:09:35.299230 ksconf-0.11.3b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-15 13:09:10.000000 ksconf-0.11.3b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.656025 ksconf-0.11.3b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-17 15:30:06.656025 ksconf-0.11.3b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.640025 ksconf-0.11.3b3/ksconf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.644025 ksconf-0.11.3b3/ksconf/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/app/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/app/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/app/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.648025 ksconf-0.11.3b3/ksconf/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/builder/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/builder/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/builder/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.652025 ksconf-0.11.3b3/ksconf/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22959 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/promote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/restexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/restpublish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/unarchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/xmlformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.652025 ksconf-0.11.3b3/ksconf/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/conf/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/conf/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/conf/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18679 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/conf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.652025 ksconf-0.11.3b3/ksconf/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14340 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/setup_entrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.652025 ksconf-0.11.3b3/ksconf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/util/completers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/util/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/util/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/util/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.656025 ksconf-0.11.3b3/ksconf/vc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/vc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/vc/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/xmlformat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.644025 ksconf-0.11.3b3/ksconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:29:51.000000 ksconf-0.11.3b3/ksconf.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-17 15:30:06.656025 ksconf-0.11.3b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/setup.py
```

### Comparing `ksconf-0.11.3b1/LICENSE` & `ksconf-0.11.3b3/LICENSE`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/PKG-INFO` & `ksconf-0.11.3b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksconf
-Version: 0.11.3b1
+Version: 0.11.3b3
 Summary: KSCONF: Ksconf Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
```

### Comparing `ksconf-0.11.3b1/README.md` & `ksconf-0.11.3b3/README.md`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/__init__.py` & `ksconf-0.11.3b3/ksconf/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/__main__.py` & `ksconf-0.11.3b3/ksconf/__main__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/app/__init__.py` & `ksconf-0.11.3b3/ksconf/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/app/deploy.py` & `ksconf-0.11.3b3/ksconf/app/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             t = eval(dc_field.type)
             if issubclass(t, PurePath):
                 value = fspath(value)
                 data[dc_field.name] = value
         return data
 
     @classmethod
-    def from_dict(self, data: dict) -> "DeployAction":
+    def from_dict(self, data: dict) -> DeployAction:
         data = data.copy()
         action = data.pop("action")
         action = DeployActionType(action)
         da_class = get_deploy_action_class(action)
         for dc_field in fields(da_class):
             if dc_field.name == "action":
                 continue
@@ -151,25 +151,25 @@
     def to_dict(self) -> dict:
         d = {
             "actions": [a.to_dict() for a in self.actions]
         }
         return d
 
     @classmethod
-    def from_dict(cls, data: dict) -> "DeploySequence":
+    def from_dict(cls, data: dict) -> DeploySequence:
         seq = cls()
         for action in data["actions"]:
             da = DeployAction.from_dict(action)
             seq.add(da)
         return seq
 
     @classmethod
     def from_manifest(
             cls,
-            manifest: AppManifest) -> "DeploySequence":
+            manifest: AppManifest) -> DeploySequence:
         """
         Fresh deploy of an app from scratch.
 
         (There should probably be a new
         op-code for this, eventually instead of listing every single file.)
         """
         dc = cls()
@@ -179,15 +179,15 @@
             dc.add(DeployActionType.EXTRACT_FILE, "create", f.path, mode=f.mode, hash=f.hash)
         return dc
 
     @classmethod
     def from_manifest_transformation(
             cls,
             base: AppManifest,
-            target: AppManifest) -> "DeploySequence":
+            target: AppManifest) -> DeploySequence:
         seq = cls()
         if base is None:
             return cls.from_manifest(target)
         if base.name != target.name:
             raise ValueError(f"Manifest must have the same app name.  {base.name} != {target.name}")
         seq.add(DeployAction_SourceReference(target.source, target.hash))
         seq.add(DeployAction_SetAppName(target.name))
```

### Comparing `ksconf-0.11.3b1/ksconf/app/facts.py` & `ksconf-0.11.3b3/ksconf/app/facts.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         return asdict(self)
 
     def to_tiny_dict(self, *keep_attrs) -> dict:
         """ Return dict representation, discarding the Nones """
         return {k: v for k, v in asdict(self).items() if v is not None or k in keep_attrs}
 
     @classmethod
-    def from_conf(cls, name, conf: ConfType) -> "AppFacts":
+    def from_conf(cls, name, conf: ConfType) -> AppFacts:
         """
         Create AppFacts from an app.conf configuration content.
         """
         new = cls(name)
 
         type_mapping = {f.name: f.type for f in fields(cls) if f.type in ("bool", "int")}
 
@@ -110,15 +110,15 @@
                 stanza = conf[stanza_name]
                 for attr in attributes:
                     if attr in stanza:
                         setattr(new, attr, convert_attr(attr, stanza[attr]))
         return new
 
     @classmethod
-    def from_app_dir(cls, app_path: Path) -> "AppFacts":
+    def from_app_dir(cls, app_path: Path) -> AppFacts:
         """
         Create an AppFacts from a local file system.  This expects a standard
         (non-layered) installed or extracted app folder.  Both ``default`` and
         ``local`` are considered.
         """
         app_path = Path(app_path)
         app_conf_paths = [
```

### Comparing `ksconf-0.11.3b1/ksconf/app/manifest.py` & `ksconf-0.11.3b3/ksconf/app/manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def to_dict(self):
         d = asdict(self)
         d["path"] = fspath(self.path)
         return d
 
     @classmethod
-    def from_dict(cls, data: dict) -> "AppManifestFile":
+    def from_dict(cls, data: dict) -> AppManifestFile:
         return cls(PurePosixPath(data["path"]), data["mode"], data["size"], data["hash"])
 
 
 @dataclass
 class AppManifest:
     name: str = None
     source: str = None
@@ -93,15 +93,15 @@
         parts.insert(0, self.name)
         payload = "\n".join(parts)
         h = hashlib.new(self.hash_algorithm)
         h.update(payload.encode("utf-8"))
         return h.hexdigest()
 
     @classmethod
-    def from_dict(cls, data: dict) -> "AppManifest":
+    def from_dict(cls, data: dict) -> AppManifest:
         files = [AppManifestFile.from_dict(f) for f in data["files"]]
         o = cls(data["name"], source=data["source"],
                 hash_algorithm=data["hash_algorithm"], files=files)
         o._hash = data["hash"]
         return o
 
     def to_dict(self):
@@ -112,15 +112,15 @@
             "hash": self.hash,
             "files": [f.to_dict() for f in self.files]
         }
         return d
 
     @classmethod
     def from_archive(cls, archive: Path,
-                     calculate_hash=True) -> "AppManifest":
+                     calculate_hash=True) -> AppManifest:
         """
         Create as new AppManifest from a tarball.  Set ``calculate_hash`` as
         False when only a file listing is needed.
         """
         manifest = cls(source=fspath(archive))
         app_names = set()
         archive = Path(archive)
@@ -148,15 +148,15 @@
         manifest.name = app_names.pop()
         return manifest
 
     @classmethod
     def from_filesystem(cls, path: Path,
                         name: str = None,
                         follow_symlinks=False,
-                        calculate_hash=True) -> "AppManifest":
+                        calculate_hash=True) -> AppManifest:
         """
         Create as new AppManifest from an existing directory structure.
         Set ``calculate_hash`` as False when only a file listing is needed.
         """
         path = Path(path)
         if name is None:
             name = path.name
@@ -216,15 +216,15 @@
                     self._manifest = AppManifest.from_dict(self._manifest_dict)
                 except KeyError as e:
                     raise AppManifestStorageError(f"Error loading manifest {e}")
 
         return self._manifest
 
     @classmethod
-    def from_dict(cls, data: dict) -> "StoredArchiveManifest":
+    def from_dict(cls, data: dict) -> StoredArchiveManifest:
         o = cls(Path(data["archive"]), data["size"], data["mtime"], data["hash"])
         o._manifest_dict = data["manifest"]
         return o
 
     def to_dict(self):
         return {
             "archive": fspath(self.archive),
@@ -236,38 +236,38 @@
 
     def write_json_manifest(self, manifest_file: Path):
         data = self.to_dict()
         with open(manifest_file, "w") as fp:
             json.dump(data, fp, indent=1)
 
     @classmethod
-    def read_json_manifest(cls, manifest_file: Path) -> "StoredArchiveManifest":
+    def read_json_manifest(cls, manifest_file: Path) -> StoredArchiveManifest:
         with open(manifest_file) as fp:
             data = json.load(fp)
         return cls.from_dict(data)
 
     @classmethod
     def from_file(cls,
                   archive: Path,
                   manifest: AppManifest
-                  ) -> "StoredArchiveManifest":
+                  ) -> StoredArchiveManifest:
         """
         Construct instance from a tarball.
         """
         stat = archive.stat()
 
         hash = file_hash(archive, MANIFEST_HASH)
         o = cls(archive, stat.st_size, stat.st_mtime, hash)
         o._manifest = manifest
         return o
 
     @classmethod
     def from_json_manifest(cls,
                            archive: Path,
-                           stored_file: Path) -> "StoredArchiveManifest":
+                           stored_file: Path) -> StoredArchiveManifest:
         """
         Attempt to load as stored manifest from archive & stored manifest paths.
         If the archive has changed since the manifest was stored, then an
         exception will be raised indicating the reason for invalidation.
         """
         # XXX: Optimization: tests if archive is newer than stored_file.  No need to open/parse JSON.
         if not stored_file:
@@ -338,15 +338,15 @@
         try:
             sam = StoredArchiveManifest.from_json_manifest(archive, manifest_file)
             manifest = sam.manifest
         except AppManifestStorageError as e:
             print(f"WARN:   loading stored manifest failed:  {e}")
 
     if manifest is None:
-        print(f"Calculating manifest for {archive}")
+        # print(f"Calculating manifest for {archive}")
         manifest = AppManifest.from_archive(archive)
 
         # We assume that a previously stored manifest has already undergone the
         # path check.  Checks should be redone from within the extraction process.
         manifest.check_paths()
 
         if write_manifest:
```

### Comparing `ksconf-0.11.3b1/ksconf/archive.py` & `ksconf-0.11.3b3/ksconf/archive.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/builder/__init__.py` & `ksconf-0.11.3b3/ksconf/builder/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import absolute_import, unicode_literals
+from __future__ import absolute_import, annotations, unicode_literals
 
 import argparse
 import inspect
 import os
 import re
 import sys
+from pathlib import Path
 from subprocess import Popen
-from typing import Callable, List
+from typing import Callable, List, TextIO
 
 from ksconf.compat import handle_py3_kw_only_args
 from ksconf.consts import EXIT_CODE_INTERNAL_ERROR, KSCONF_DEBUG
 
 QUIET = -1
 NORMAL = 0
 VERBOSE = 1
@@ -23,23 +24,27 @@
 class BuildCacheException(Exception):
     pass
 
 
 class BuildStep:
     __slots__ = ["build_path", "source_path", "dist_path", "config", "verbosity", "_output"]
 
-    def __init__(self, build, source=None, dist=None, output=sys.stdout):
+    def __init__(self,
+                 build: Path,
+                 source: Path = None,
+                 dist: Path = None,
+                 output: TextIO = sys.stdout):
         self.build_path = build
         self.source_path = source
         self.dist_path = dist
         self.config = {}
         self.verbosity = 0
         self._output = output
 
-    def alternate_path(self, path):
+    def alternate_path(self, path) -> BuildStep:
         """ Construct a new BuildStep instance with only 'build_path' altered. """
         cls = self.__class__
         instance = cls(path)
         for slot in cls.__slots__:
             if slot != "build_path":
                 setattr(instance, slot, getattr(self, slot))
         return instance
```

### Comparing `ksconf-0.11.3b1/ksconf/builder/cache.py` & `ksconf-0.11.3b3/ksconf/builder/cache.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/builder/core.py` & `ksconf-0.11.3b3/ksconf/builder/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
         * outputs       (do we need this, can we just detect this??)
                         Default to "." (everything)
         * timeout=0     Seconds before cache should be considered stale
         * name=None     If not given, default to the short name of the function.
                         (Cache "slot"), must be filesystem safe]
 """
 
+from __future__ import annotations
+
 from functools import wraps
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import List, Union
 
 from ksconf.builder import QUIET, VERBOSE, BuildCacheException, BuildStep
 from ksconf.builder.cache import CachedRun, FileSet
@@ -37,56 +39,59 @@
     h = hashlib.new("sha256")
     code = inspect.getsource(f).encode("utf-8")
     h.update(code)
     return h.hexdigest()
 
 
 class BuildManager:
-    """ Management of individual build steps
+    """ Supports an application building process by managing individual build steps
 
     .. versionadded:: v0.8.0
     """
 
     def __init__(self):
-        self.source_path = None
-        self.build_path = None
-        self.dist_path = None
+        self.source_path: Path = None
+        self.build_path: Path = None
+        self.dist_path: Path = None
         self.cache_path = None
         self._cache_enabled = True
         self._taint = False
         self._folder_set = False
 
     def taint_cache(self):
         self._taint = True
 
     def disable_cache(self):
         self._cache_enabled = False
 
-    def get_build_step(self, output=None):
+    def get_build_step(self, output=None) -> BuildStep:
         kw = {}
         if output:
             kw["output"] = output
         step = BuildStep(self.build_path, self.source_path, self.dist_path, **kw)
         return step
 
-    def set_folders(self, source_path, build_path, dist_path=None):
+    def set_folders(self,
+                    source_path: Path,
+                    build_path: Path,
+                    dist_path: Path = None):
         self._folder_set = True
         self.source_path = Path(source_path).absolute()
         self.build_path = Path(build_path).absolute()
         if dist_path:
             self.dist_path = Path(dist_path).absolute()
         else:
             # Assume 'dist' lives along side 'build'
             self.dist_path = self.build_path.with_name("dist")
         self.cache_path = self.build_path.with_suffix(".cache")
 
     def is_folders_set(self):
         return self._folder_set
 
-    def get_cache_info(self, name):
+    def get_cache_info(self, name: str) -> CachedRun:
         path = self.cache_path / name
         cache_info = CachedRun(path)
         if self._taint:
             cache_info.taint()
         if not self._cache_enabled:
             cache_info.disable()
         return cache_info
```

### Comparing `ksconf-0.11.3b1/ksconf/builder/steps.py` & `ksconf-0.11.3b3/ksconf/builder/steps.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/cli.py` & `ksconf-0.11.3b3/ksconf/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,18 +88,18 @@
     badparser.add_argument('args', nargs=argparse.REMAINDER)
 
 
 def build_cli_parser(do_formatter=False):
     parser_kwargs = dict(
         fromfile_prefix_chars="@",
         description=_cli_description,
-        prog="ksconf")
-    if sys.version_info > (3, 5):
         # Disable abbreviations as they could lead to accidental assignment as the CLI grows.
-        parser_kwargs["allow_abbrev"] = False
+        allow_abbrev=False,
+        prog="ksconf")
+
     if do_formatter:
         parser_kwargs["formatter_class"] = DescriptionHelpFormatterPreserveLayout
     parser = argparse.ArgumentParser(**parser_kwargs)
     subparsers = parser.add_subparsers()
 
     # XXX: Lazyload version information; this launches 'git' which is expensive.
     version_info = []
```

### Comparing `ksconf-0.11.3b1/ksconf/combine.py` & `ksconf-0.11.3b3/ksconf/combine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # -*- coding: utf-8 -*-
 """
-XXX: Split out conf, spec, binary file handlers into separate registerable (and therefore easily extendable) functions (using decorators, possibly)
 XXX: Move the overwrite-as-necessary logic into a subclass; for several use cases we just don't care because 'target' is a brand new directory
 """
 
-from __future__ import absolute_import, unicode_literals
+from __future__ import absolute_import, annotations, unicode_literals
 
 import os
 import re
 import sys
 from io import open
+from os import fspath
+from pathlib import Path
+from typing import Callable
 
 from ksconf.commands import ConfFileProxy
+from ksconf.compat import List, Tuple
 from ksconf.conf.delta import show_text_diff
 from ksconf.conf.merge import merge_conf_files
 from ksconf.conf.parser import PARSECONF_MID, PARSECONF_STRICT
 from ksconf.consts import SMART_CREATE, SMART_NOCHANGE, SMART_UPDATE
-from ksconf.layer import DirectLayerRoot, DotDLayerRoot, LayerConfig, LayerFilter, LayerRootBase
+from ksconf.layer import (DirectLayerRoot, DotDLayerRoot, LayerConfig,
+                          LayerFile, LayerFilter, LayerRootBase)
 from ksconf.util.compare import file_compare
 from ksconf.util.file import _is_binary_file, smart_copy
 
 
 class LayerCombinerException(Exception):
     pass
 
@@ -52,14 +56,16 @@
             -> post_combine()           Optional, cleanup leftover files
     """
 
     # Note this is case sensitive.  Don't be lazy, name your files correctly  :-)
     conf_file_re = re.compile(r"([a-z_-]+\.conf|(default|local)\.meta)$")
     spec_file_re = re.compile(r"\.conf\.spec$")
 
+    filetype_handlers: List[Tuple[Callable, Callable]] = []
+
     def __init__(self,
                  follow_symlink: bool = False,
                  banner: str = "",
                  dry_run: bool = False,
                  quiet: bool = False):
         self.layer_root: LayerRootBase = None
         self.config = LayerConfig()
@@ -74,20 +80,38 @@
         self.layer_names_all = set()
         self.layer_names_used = set()
 
         # Not a great long-term design, but good enough for initial conversion from command-based design
         self.stdout = sys.stdout
         self.stderr = sys.stderr
 
-    def set_source_dirs(self, sources: list):
+    @classmethod
+    def register_regex(cls, regex_match):
+        """ Decorator that matches a filename regex and if it matches, it
+        executes the decorator handler.
+        """
+        cre = re.compile(regex_match)
+
+        def match_f(file: Path):
+            if cre.search(file.name):
+                return True
+            return False
+
+        def wrapper(handle_f):
+            cls.filetype_handlers.append((match_f, handle_f))
+            return handle_f
+
+        return wrapper
+
+    def set_source_dirs(self, sources: List[Path]):
         self.layer_root = DirectLayerRoot(config=self.config)
         for src in sources:
-            self.layer_root.add_layer(src)
+            self.layer_root.add_layer(Path(src))
 
-    def set_layer_root(self, root):
+    def set_layer_root(self, root: LayerRootBase.Layer):
         layer_root = DotDLayerRoot(config=self.config)
         layer_root.set_root(root)
         self.layer_root = layer_root
 
     def add_layer_filter(self, action, pattern):
         self.layer_filter.add_rule(action, pattern)
 
@@ -101,83 +125,77 @@
         self.prepare(target)
         # Build a common tree of all src files.
         src_file_listing = layer_root.list_files()
         src_file_listing = self.pre_combine_inventory(target, src_file_listing)
         self.combine_files(target, src_file_listing)
         self.post_combine(target)
 
-    def prepare(self, target):
+    def prepare(self, target: Path):
         """ Start the combine process.  This includes directory checking,
         applying layer filtering, and marker file handling. """
         layer_root, layer_filter = self.layer_root, self.layer_filter
+        target = Path(target)
 
         self.prepare_target_dir(target)
 
         self.layer_names_all.update(layer_root.list_layer_names())
         if layer_root.apply_filter(layer_filter):
             self.layer_names_used.update(layer_root.list_layer_names())
         else:
             self.layer_names_used.update(self.layer_names_all)
 
-    def prepare_target_dir(self, target):
+    def prepare_target_dir(self, target: Path):
         """ Hook to ensure destination directory is ready for use.  This can be overridden
         to adder marker file handling for use cases that need it (e.g., the 'combine' command)
         """
-        if not os.path.isdir(target):
-            os.mkdir(target)
+        if not target.is_dir():
+            target.mkdir()
 
-    def pre_combine_inventory(self, target, src_files):
+    def pre_combine_inventory(self, target: Path, src_files: List[LayerFile]) -> List[LayerFile]:
         """ Hook point for pre-processing before any files are copied/merged """
         del target
         return src_files
 
     def post_combine(self, target):
         """ Hook point for post-processing after all copy/merge operations have been completed. """
         del target
 
     def combine_files(self, target, src_files):
         layer_root = self.layer_root
-
-        def physical_paths(l: LayerRootBase.File):
-            return [s.physical_path for s in l]
-
         for src_file in sorted(src_files):
-            # Source file must be in sort order (10-x is lower prio and therefore replaced by 90-z)
+            do_copy = True
             sources = list(layer_root.get_file(src_file))
             try:
                 dest_fn = sources[0].logical_path
             except IndexError:
                 raise LayerCombinerException("File disappeared during execution?  {src_file}\n")
 
-            dest_path = os.path.join(target, dest_fn)
+            dest_path: Path = target / dest_fn
 
             # Make missing destination folder, if missing
-            dest_dir = os.path.dirname(dest_path)
-            if not os.path.isdir(dest_dir) and not self.dry_run:
-                os.makedirs(dest_dir)
+            dest_dir: Path = dest_path.parent
+            if not dest_dir.is_dir() and not self.dry_run:
+                dest_dir.mkdir(parents=True)
 
             # Determine handling method based on source count and filename pattern
-            if len(sources) == 1:
-                # Copy only file (most common case)
-                method = "copy"
-            elif self.spec_file_re.search(dest_fn):
-                method = "concatenate"
-            elif self.conf_file_re.search(dest_fn):
-                method = "merge"
-            else:
-                # Copy highest precedence
-                method = "copy"
+            if len(sources) > 1:
+                for matcher, handler in self.filetype_handlers:
+                    if matcher(dest_fn):
+                        msg = handler(self, dest_path, sources, self.dry_run)
+                        if msg and not self.quiet:
+                            self.stderr.write(f"{msg}\n")
+                        do_copy = False
 
-            if method == "copy":
-                # self.stderr.write(f"Considering {dest_fn:50}  NON-CONF Copy from source:  "
+            if do_copy:
+                # self.stderr.write(f"Considering {fspath(dest_fn):50}  NON-CONF Copy from source:  "
                 #                   f"{sources[-1].physical_path!r}\n")
                 # Always use the last file in the list (since last directory always wins)
                 src_file = sources[-1].physical_path
                 if self.dry_run:
-                    if os.path.isfile(dest_path):
+                    if dest_path.is_file():
                         if file_compare(src_file, dest_path):
                             smart_rc = SMART_NOCHANGE
                         else:
                             if (_is_binary_file(src_file) or _is_binary_file(dest_path)):
                                 # Binary files.  Can't compare...
                                 smart_rc = "DRY-RUN (NO-DIFF=BIN)"
                             else:
@@ -185,64 +203,64 @@
                                 smart_rc = "DRY-RUN (DIFF)"
                     else:
                         smart_rc = "DRY-RUN (NEW)"
                 else:
                     smart_rc = smart_copy(src_file, dest_path)
                 if smart_rc != SMART_NOCHANGE:
                     if not self.quiet:
-                        self.stderr.write(f"Copy <{smart_rc}>   {dest_path:50}  from {src_file}\n")
+                        self.stderr.write(f"Copy <{smart_rc}>   {fspath(dest_path):50}  from {src_file}\n")
                 del src_file
 
-            elif method == "merge":
-                try:
-                    # Handle merging conf files
-                    dest = ConfFileProxy(dest_path, "r+",
-                                         parse_profile=PARSECONF_MID)
-                    srcs = [ConfFileProxy(s.physical_path, "r",
-                                          parse_profile=PARSECONF_STRICT) for s in sources]
-                    # self.stderr.write(f"Considering {dest_fn:50}  CONF MERGE from source:  "
-                    #                   f"{1!sources[0].physical_path}\n")
-                    smart_rc = merge_conf_files(dest, srcs, dry_run=self.dry_run,
-                                                banner_comment=self.banner)
-                    if smart_rc != SMART_NOCHANGE:
-                        if not self.quiet:
-                            self.stderr.write(f"Merge <{smart_rc}>   {dest_path:50}  "
-                                              f"from {physical_paths(sources)!r}\n")
-                finally:
-                    # Protect against any dangling open files:  (ResourceWarning: unclosed file)
-                    dest.close()
-                    for src in srcs:
-                        src.close()
-                    del srcs, dest
-
-            elif method == "concatenate":
-                combined_content = ""
-                last_mtime = max(src.mtime for src in sources)
-                for src in sources:
-                    with open(src, "r") as stream:
-                        content = stream.read()
-                        if not content.endswith("\n"):
-                            content += "\n"
-                        combined_content += content
-                        del content
-                smart_rc = SMART_CREATE
-                if os.path.isfile(dest_path):
-                    with open(dest_path) as stream:
-                        dest_content = stream.read()
-                    if dest_content == combined_content:
-                        smart_rc = SMART_NOCHANGE
-                    else:
-                        smart_rc = SMART_UPDATE
-                    del dest_content
 
-                if not self.dry_run:
-                    with open(dest_path, "w") as stream:
-                        stream.write(combined_content)
+@LayerCombiner.register_regex(r"([a-z_-]+\.conf|(default|local)\.meta)$")
+def handle_merge_conf_files(context: LayerCombiner,
+                            dest_path: Path,
+                            sources: List[LayerFile],
+                            dry_run):
+    sources_physical = [fspath(p.physical_path) for p in sources]
+    message = None
+    # Note that latest mtime logic is handled by merge_conf_files()
+    try:
+        # Handle merging conf files
+        dest = ConfFileProxy(dest_path, "r+", parse_profile=PARSECONF_MID)
+        srcs = [ConfFileProxy(s, "r", parse_profile=PARSECONF_STRICT) for s in sources_physical]
+        # self.stderr.write(f"Considering {dest_fn:50}  CONF MERGE from source:  "
+        #                   f"{1!sources[0].physical_path}\n")
+        smart_rc = merge_conf_files(dest, srcs, dry_run=dry_run,
+                                    banner_comment=context.banner)
+        if smart_rc != SMART_NOCHANGE:
+            message = f"Merge <{smart_rc}>   {fspath(dest_path):50}  from {sources_physical!r}"
+    finally:
+        # Protect against any dangling open files:  (ResourceWarning: unclosed file)
+        dest.close()
+        for src in srcs:
+            src.close()
+    return message
+
+
+@LayerCombiner.register_regex(r"\.conf\.spec$")
+def handle_spec_concatenate(context: LayerCombiner,
+                            dest_path: Path,
+                            sources: List[LayerFile],
+                            dry_run):
+    sources_physical = [fspath(p.physical_path) for p in sources]
+    combined_content = ""
+    last_mtime = max(src.mtime for src in sources)
+    for src in sources:
+        content = src.physical_path.read_text()
+        if not content.endswith("\n"):
+            content += "\n"
+        combined_content += content
+    smart_rc = SMART_CREATE
+    if dest_path.is_file():
+        dest_content = dest_path.read_text()
+        if dest_content == combined_content:
+            smart_rc = SMART_NOCHANGE
+        else:
+            smart_rc = SMART_UPDATE
+
+    if not dry_run:
+        dest_path.write_text(combined_content)
 
-                if smart_rc != SMART_NOCHANGE:
-                    if not self.quiet:
-                        self.stderr.write(f"Concatenate <{smart_rc}>   {dest_path:50}  "
-                                          f"from {physical_paths(sources)!r}\n")
-                os.utime(dest_path, (last_mtime, last_mtime))
-                del combined_content
-            else:
-                raise AssertionError(f"Internal implementation error.  Unknown method={method}")
+    os.utime(dest_path, (last_mtime, last_mtime))
+    if smart_rc != SMART_NOCHANGE:
+        return f"Concatenate <{smart_rc}>   {fspath(dest_path):50}  from {sources_physical!r}"
```

### Comparing `ksconf-0.11.3b1/ksconf/commands/__init__.py` & `ksconf-0.11.3b3/ksconf/commands/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     def get_file(self, relpath):
         path = os.path.join(self.name, relpath)
         return ConfFileProxy(path, self._mode, parse_profile=self._parse_profile, is_file=True)
 
 
 class ConfFileProxy:
     def __init__(self, name, mode, stream=None, parse_profile=None, is_file=None):
-        self.name = name
+        self.name = os.fspath(name)
         self._mode = mode
         if is_file is not None:
             self._is_file = is_file
         elif stream:
             self._is_file = False
         elif self.writable() or os.path.isfile(name):
             self._is_file = True
```

### Comparing `ksconf-0.11.3b1/ksconf/commands/check.py` & `ksconf-0.11.3b3/ksconf/commands/check.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/commands/combine.py` & `ksconf-0.11.3b3/ksconf/commands/combine.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,23 @@
     ksconf combine default.d/* --target=default
 
 """
 from __future__ import absolute_import, unicode_literals
 
 import os
 from io import open
+from pathlib import Path
 
 from ksconf.combine import LayerCombiner, LayerCombinerException
 from ksconf.commands import KsconfCmd, dedent
+from ksconf.compat import List
 from ksconf.consts import (EXIT_CODE_BAD_ARGS, EXIT_CODE_COMBINE_MARKER_MISSING,
                            EXIT_CODE_MISSING_ARG, EXIT_CODE_NO_SUCH_FILE)
 from ksconf.filter import create_filtered_list
+from ksconf.layer import LayerFile
 from ksconf.util.completers import DirectoriesCompleter
 from ksconf.util.file import expand_glob_list, relwalk, splglob_simple
 
 CONTROLLED_DIR_MARKER = ".ksconf_controlled"
 
 
 class LayerCombinerExceptionCode(LayerCombinerException):
@@ -44,63 +47,63 @@
                  keep_existing: bool = False, **kwargs):
         super().__init__(*args, **kwargs)
         self.target_extra_files: set = None
         self.disable_marker = disable_marker
         self.disable_cleanup = disable_cleanup
         self.keep_existing = keep_existing
 
-    def prepare_target_dir(self, target):
+    def prepare_target_dir(self, target: Path):
         """
         Handle marker file and ensure that target directory gets created safely.
         """
-        marker_file = os.path.join(target, CONTROLLED_DIR_MARKER)
-        if os.path.isdir(target):
-            if not self.disable_marker and not os.path.isfile(marker_file):
+        marker_file: Path = target / CONTROLLED_DIR_MARKER
+        if target.is_dir():
+            if not self.disable_marker and not marker_file.is_file():
                 self.stderr.write("Target directory already exists, but it appears to have been "
                                   "created by some other means.  Marker file missing.\n")
                 raise LayerCombinerExceptionCode("Target directory exists without marker file",
                                                  EXIT_CODE_COMBINE_MARKER_MISSING)
 
         elif self.dry_run:
             self.stderr.write("Skipping creating destination directory {target} (dry-run)\n")
         else:
             try:
-                os.mkdir(target)
+                target.mkdir()
             except OSError as e:
                 self.stderr.write(f"Unable to create destination directory {target}.  {e}\n")
                 raise LayerCombinerExceptionCode(f"Unable to create destination directory {target}",
                                                  EXIT_CODE_NO_SUCH_FILE)
             self.stderr.write(f"Created destination directory {target}\n")
             if not self.disable_marker:
-                with open(marker_file, "w") as f:
-                    f.write("This directory is managed by KSCONF.  Don't touch\n")
+                marker_file.write_text("This directory is managed by KSCONF.  Don't touch\n")
 
-    def pre_combine_inventory(self, target, src_files):
+    def pre_combine_inventory(self, target: Path, src_files: List[LayerFile]) -> List[LayerFile]:
         """
         Find a set of files that exist in the target folder, but in NO source folder (for cleanup)
         """
         config = self.config
 
         self.stderr.write(f"Layers detected:  {self.layer_names_all}\n")
         if self.layer_names_all != self.layer_names_used:
             self.stderr.write(f"Layers after filter: {self.layer_names_used}\n")
 
         # Convert src_files to a set to speed up
         src_files = set(src_files)
         self.target_extra_files = set()
-        for (root, dirs, files) in relwalk(target, followlinks=config.follow_symlink):
+        for (root, _, files) in relwalk(target, followlinks=config.follow_symlink):
+            root = Path(root)
             for fn in files:
-                tgt_file = os.path.join(root, fn)
+                tgt_file = root / fn
                 if tgt_file not in src_files:
                     if fn == CONTROLLED_DIR_MARKER or config.block_files.search(fn):
                         continue  # pragma: no cover (peephole optimization)
                     self.target_extra_files.add(tgt_file)
         return src_files
 
-    def post_combine(self, target):
+    def post_combine(self, target: Path):
         """
         Handle cleanup of extra files
         """
         target_extra_files = self.target_extra_files
         if target_extra_files:
             if self.disable_cleanup:
                 self.stderr.write("Cleanup operations disabled by user.\n")
@@ -114,15 +117,16 @@
             for dest_fn in target_extra_files:
                 if keep_existing.match_path(dest_fn):
                     self.stderr.write(f"Keep existing file {dest_fn}\n")
                 elif self.disable_cleanup:
                     self.stderr.write(f"Skip cleanup of unwanted file {dest_fn}\n")
                 else:
                     self.stderr.write(f"Remove unwanted file {dest_fn}\n")
-                    os.unlink(os.path.join(target, dest_fn))
+                    f: Path = target / dest_fn
+                    f.unlink()
 
 
 class CombineCmd(KsconfCmd):
     help = dedent("""\
     Combine configuration files across multiple source directories into a single
     destination directory.  This allows for an arbitrary number of Splunk
     configuration layers to coexist within a single app.  Useful in both ongoing
```

### Comparing `ksconf-0.11.3b1/ksconf/commands/diff.py` & `ksconf-0.11.3b3/ksconf/commands/diff.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/commands/filter.py` & `ksconf-0.11.3b3/ksconf/commands/filter.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/commands/merge.py` & `ksconf-0.11.3b3/ksconf/commands/merge.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/commands/minimize.py` & `ksconf-0.11.3b3/ksconf/commands/minimize.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/commands/package.py` & `ksconf-0.11.3b3/ksconf/commands/package.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/commands/promote.py` & `ksconf-0.11.3b3/ksconf/commands/promote.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/commands/restexport.py` & `ksconf-0.11.3b3/ksconf/commands/restexport.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/commands/restpublish.py` & `ksconf-0.11.3b3/ksconf/commands/restpublish.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/commands/snapshot.py` & `ksconf-0.11.3b3/ksconf/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/commands/sort.py` & `ksconf-0.11.3b3/ksconf/commands/sort.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/commands/unarchive.py` & `ksconf-0.11.3b3/ksconf/commands/unarchive.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/commands/xmlformat.py` & `ksconf-0.11.3b3/ksconf/commands/xmlformat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/compat.py` & `ksconf-0.11.3b3/ksconf/compat.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,36 @@
 Silly simple Python version compatibility items
 """
 
 import sys
 
 # Since 'list' in Python 3.7 doesn't support __class_getitem__ (See PEP 560)
 # We could just always import from typing, but that appears to cause some issues
-# with type hinting, and this appears to work correctly.
-if sys.version_info < (3, 8):
-    from typing import List, Tuple
+# with type hinting, and this appears to work correctly.  Most of this appears
+# to have changed in Python 3.8 and 3.9 (differs by type. hence the test-and-see approach)
+
+''' # Alternate, needs more testing; not sure about the assignment part
+# Another option would be to just assign directly into the typing module, what could go wrong?
+
+from typing import Dict, List, Set, Tuple
+for t in ("dict", "list", "set", "tuple"):
+    try:
+        T = t.capitalize()
+        eval(f"{t}[str]")
+        globals()[T] = globals[t]
+    except TypeError:
+        pass
+'''
+
+if sys.version_info < (3, 9):
+    from typing import Dict, List, Set, Tuple
 else:
+    Dict = dict
     List = list
+    Set = set
     Tuple = tuple
 
 
 try:
     # Python 3.9 and later
     from functools import cache
 except ImportError:
@@ -62,12 +79,14 @@
                         .format(caller, list(kw)[0]))
     return out
 
 
 del sys
 
 __all__ = [
+    "Dict",
     "List",
+    "Set",
     "Tuple",
     "cache",
     "handle_py3_kw_only_args",
 ]
```

### Comparing `ksconf-0.11.3b1/ksconf/conf/delta.py` & `ksconf-0.11.3b3/ksconf/conf/delta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import difflib
 import os
 from collections import Counter, defaultdict
 from dataclasses import dataclass
 from enum import Enum
 from io import open
-from os import PathLike
+from os import PathLike, fspath
 from typing import List, NamedTuple, Sequence, TextIO, Union
 
 from ksconf.conf.parser import GLOBAL_STANZA, ConfType, StanzaType, _format_stanza, default_encoding
 from ksconf.consts import EXIT_CODE_DIFF_CHANGE, EXIT_CODE_DIFF_EQUAL, EXIT_CODE_DIFF_NO_COMMON
 from ksconf.util.compare import cmp_sets
 from ksconf.util.terminal import ANSI_BOLD, ANSI_GREEN, ANSI_RED, ANSI_RESET, ANSI_YELLOW, TermColor
 
@@ -85,15 +85,15 @@
             self.mtime = 0
 
     def __str__(self):
         if isinstance(self.mtime, (int, float)):
             ts = datetime.datetime.fromtimestamp(self.mtime)
         else:
             ts = self.mtime
-        return "{0:50} {1}".format(self.name, ts)
+        return f"{fspath(self.name):50} {ts}"
 
 
 def compare_stanzas(a: StanzaType, b: StanzaType,
                     stanza_name: str,
                     replace_level: DiffLevel = DiffLevel.GLOBAL
                     ) -> List[DiffOp]:
     """
```

### Comparing `ksconf-0.11.3b1/ksconf/conf/merge.py` & `ksconf-0.11.3b3/ksconf/conf/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import absolute_import, unicode_literals
 
 import os
 import shutil
 import sys
 from copy import deepcopy
+from os import fspath
 from typing import List
 
 from ksconf.commands import ConfFileProxy
 from ksconf.conf.delta import compare_cfgs, show_diff
 from ksconf.conf.parser import (GLOBAL_STANZA, ConfType, _extract_comments,
                                 inject_section_comments, parse_conf, write_conf)
 from ksconf.consts import SMART_UPDATE, SmartEnum
```

### Comparing `ksconf-0.11.3b1/ksconf/conf/meta.py` & `ksconf-0.11.3b3/ksconf/conf/meta.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/conf/parser.py` & `ksconf-0.11.3b3/ksconf/conf/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,28 @@
 
 import codecs
 import os
 import re
 from enum import Enum
 from io import StringIO, open
 from os import PathLike
+from pathlib import Path
 from typing import Dict, Generator, Iterable, List, TextIO, Tuple, Union
 
 from ..consts import SmartEnum
 from ..util.compare import fileobj_compare
 
 default_encoding = "utf-8"
 
 
 # Type definitions
 
 StanzaType = Dict[str, str]
 ConfType = Dict[str, StanzaType]
-PathType = Union[PathLike, str]
+PathType = Union[Path, str]
 _StreamInput = Union[TextIO, Iterable[str]]
 _StreamOutput = Union[PathType, TextIO]
 _StreamNameFile = Union[PathType, _StreamInput]
 ParserConfig = Dict
 
 
 class Token:
@@ -384,37 +385,37 @@
 
 def smart_write_conf(filename: PathType,
                      conf: ConfType,
                      stanza_delim: str = "\n",
                      sort: bool = True,
                      temp_suffix: str = ".tmp",
                      mtime: float = None) -> SmartEnum:
-    if os.path.isfile(filename):
+    filename = Path(filename)
+    if filename.is_file():
         temp = StringIO()
         write_conf_stream(temp, conf, stanza_delim, sort)
         with open(filename, encoding=default_encoding) as dest:
             file_diff = fileobj_compare(temp, dest)
         if file_diff:
             return SmartEnum.NOCHANGE
         else:
-            tempfile = filename + temp_suffix
-            with open(tempfile, "w", encoding=default_encoding) as dest:
-                dest.write(temp.getvalue())
+            tempfile: Path = filename.with_name(filename.name + temp_suffix)
+            tempfile.write_text(temp.getvalue(), encoding=default_encoding)
             if mtime:
                 os.utime(tempfile, (mtime, mtime))
             os.unlink(filename)
             os.rename(tempfile, filename)
             return SmartEnum.UPDATE
     else:
-        tempfile = filename + temp_suffix
+        tempfile = filename.with_name(filename.name + temp_suffix)
         with open(tempfile, "w", encoding=default_encoding) as dest:
             write_conf_stream(dest, conf, stanza_delim, sort)
-        if mtime:
-            os.utime(tempfile, (mtime, mtime))
         os.rename(tempfile, filename)
+        if mtime:
+            os.utime(filename, (mtime, mtime))
         return SmartEnum.CREATE
 
 
 def _format_stanza(stanza: Union[str, Token]) -> str:
     """ Return a more human readable stanza name."""
     if stanza is GLOBAL_STANZA:
         return "GLOBAL"
```

### Comparing `ksconf-0.11.3b1/ksconf/consts.py` & `ksconf-0.11.3b3/ksconf/consts.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/filter.py` & `ksconf-0.11.3b3/ksconf/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import absolute_import, unicode_literals
 
 import fnmatch
 import os
 import re
 import sys
 from collections import Counter
+from pathlib import Path
 
 from ksconf.conf.parser import GLOBAL_STANZA
 from ksconf.util.file import splglob_to_regex
 
 # It seems like each item on the list should be capability of having it's own type and flags (which could be inherited, at may not be known at the time the rules are first initialized)
 # The should still be some phase that each "Rule" goes though (1) creation to set core attributes, (2) prep where things can be compiled, syntax checked, and any default flags should be available by this time, and (3) evalute against a specific value for true/false.
 # This would allow things like a special prefix to lazy-switch modes (for example:  ~regex~, or only do fnmatching if there's a wildcard otherwise stick with simple string matching, ...)
@@ -37,14 +38,17 @@
                 if line and line[0] != "#":
                     items.append(line)
         if self.flags & self.VERBOSE:
             sys.stderr.write(f"Loaded {len(items)} patterns from {path}\n")
         return items
 
     def feed(self, item, filter=None):
+        if isinstance(item, Path):
+            item = os.fspath(item)
+
         if item.startswith("file://"):
             # File ingestion mode
             filename = item[7:]
             for item in self._feed_from_file(filename):
                 self.feed(item, filter)
         else:
             if filter:
@@ -82,14 +86,16 @@
             return self.default
         if self.flags & self.INVERT:
             return not result
         else:
             return result
 
     def match_path(self, path):
+        if isinstance(path, Path):
+            path = os.fspath(path)
         if os.path.sep != "/":
             path = path.replace(os.path.sep, "/")
         return self.match(path)
 
     def match_stanza(self, stanza):
         """ Same as match(), but handle GLOBAL_STANZA gracefully. """
         if stanza is GLOBAL_STANZA:
```

### Comparing `ksconf-0.11.3b1/ksconf/layer.py` & `ksconf-0.11.3b3/ksconf/layer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
-import os
 import re
 from collections import defaultdict
 from fnmatch import fnmatch
-from os import PathLike
-from typing import Type
+from os import PathLike, stat_result
+from pathlib import Path, PurePath
+from tempfile import NamedTemporaryFile
+from typing import Any, Callable, Iterator
 
+from ksconf.compat import Dict, List, Set, Tuple
 from ksconf.util.file import relwalk
 
 """
 
 LayerRootBase has one or more 'Layer', each layer has one or more 'File's.
 
 
@@ -42,50 +44,152 @@
 This must work with an explicitly given list of layers
 
 """
 
 
 def _path_join(*parts):
     """ A slightly smarter / more flexible path appender.
-    Drop any None or "." elements
+    Drop any None
     """
-    parts = [p for p in parts if p is not None]
-    return os.path.join(*parts)
+    return Path(*filter(None, parts))
 
 
-def path_in_layer(layer, path, sep=os.path.sep):
+def path_in_layer(layer: Path, path: Path) -> Path:
     """ Check to see if path exist within layer.
     Returns either None, or the path without the shared prefix with layer.
     """
     # Using 'sep' over os.path.join / os.path.split should be okay here as we should only ever be
     # given relative paths (no Windows UNC/drive letters)
     if layer is None:
         # Return as-is, since layer is root
         return path
-    layer_parts = layer.split(sep)
+    # layer_parts = layer.split(sep)
+    layer_parts = layer.parts
     layer_count = len(layer_parts)
-    path_parts = path.split(sep)
+    path_parts = path.parts
     if len(path_parts) < layer_count:
-        return False
+        return None
+    # Q: Are we recreating path.relative_to()?
     path_suffix = path_parts[:layer_count]
     if layer_parts != path_suffix:
-        return False
-    return sep.join(path_parts[layer_count:])
+        return None
+    return Path(*path_parts[layer_count:])
 
 
 # Exceptions
 
 class LayerException(Exception):
     pass
 
 
 class LayerUsageException(LayerException):
     pass
 
 
+class LayerFile(PathLike):
+    __slots__ = ["layer", "relative_path", "_stat"]
+
+    def __init__(self,
+                 layer: LayerRootBase.Layer,
+                 relative_path: PurePath,
+                 stat: stat_result = None):
+        self.layer = layer
+        self.relative_path = relative_path
+        self._stat = stat
+
+    def __fspath__(self) -> str:
+        return self.resource_path
+
+    @staticmethod
+    def match(path: PurePath):
+        return True
+
+    @property
+    def physical_path(self) -> Path:
+        return _path_join(self.layer.root, self.layer.physical_path, self.relative_path)
+
+    @property
+    def logical_path(self) -> Path:
+        return _path_join(self.layer.logical_path, self.relative_path)
+
+    resource_path = physical_path
+
+    @property
+    def stat(self) -> stat_result:
+        if self._stat is None:
+            self._stat = self.physical_path.stat()
+        return self._stat
+
+    @property
+    def size(self):
+        return self.stat.st_size
+
+    @property
+    def mtime(self):
+        return self.stat.st_mtime
+
+
+class TemplatedLayerFile(LayerFile):
+
+    __slots__ = ["_temp_resource"]
+    template_context: dict = {}
+
+    def __init__(self, *args, **kwargs):
+        super(TemplatedLayerFile, self).__init__(*args, **kwargs)
+        self._temp_resource = None
+
+    def __del__(self):
+        if getattr(self, "_temp_resource", None) and self._temp_resource.is_file():
+            self._temp_resource.unlink()
+
+    @staticmethod
+    def match(path: PurePath):
+        return path.suffix == ".j2"
+
+    @staticmethod
+    def transform_name(path: PurePath):
+        return path.with_name(path.name[:-3])
+
+    def render(self, template_path: Path) -> str:
+        from jinja2 import Environment, StrictUndefined
+        environment = Environment(undefined=StrictUndefined)
+        # TODO:  Use file system loader; allowing other file imports
+        template = environment.from_string(template_path.read_text())
+        return template.render(**self.template_context)
+
+    @property
+    def logical_path(self) -> Path:
+        return _path_join(self.layer.logical_path,
+                          self.transform_name(self.relative_path))
+
+    @property
+    def physical_path(self) -> Path:
+        return _path_join(self.layer.root, self.layer.physical_path, self.relative_path)
+
+    @property
+    def resource_path(self) -> Path:
+        if not self._temp_resource:
+            # Temporary file will be removed in instance destructor
+            tf = NamedTemporaryFile(delete=False)
+            self._temp_resource = Path(tf.name)
+            self._temp_resource.write_text(self.render(self.physical_path))
+        return self._temp_resource
+
+
+def layer_file_factory(layer, path: PurePath, *args, **kwargs) -> LayerFile:
+    # XXX: Add a dynamic registration process; decorators, subclass init hook?
+    classes = [
+        TemplatedLayerFile,
+        LayerFile,
+    ]
+    for cls in classes:
+        if cls.match(path):
+            return cls(layer, path, *args, **kwargs)
+
+
 class LayerFilter:
     _valid_actions = ("include", "exclude")
 
     def __init__(self):
         self._rules = []
 
     def add_rule(self, action, pattern):
@@ -97,15 +201,15 @@
             if action == "include":
                 first_filter = ("exclude", "*")
             elif "exclude":
                 first_filter = ("include", "*")
             self._rules.append(first_filter)
         self._rules.append((action, pattern))
 
-    def evaluate(self, layer: "LayerRootBase.Layer") -> bool:
+    def evaluate(self, layer: LayerRootBase.Layer) -> bool:
         response = True
         layer_name = layer.name
         for rule_action, rule_pattern in self._rules:
             if fnmatch(layer_name, rule_pattern):
                 response = rule_action == "include"
         return response
 
@@ -117,158 +221,161 @@
     def __init__(self):
         # Set defaults
         self.follow_symlink = False
         self.block_files = re.compile(r"\.(bak|swp)$")
         self.block_dirs = {".git"}
 
 
-class LayerRootBase:
-    """ All 'path's here are relative to the ROOT. """
+R_walk = Iterator[Tuple[Path, List[str], List[str]]]
 
-    class File(PathLike):
-        __slots__ = ["layer", "relative_path", "_stat"]
 
-        def __init__(self, layer, relative_path, stat=None):
-            self.layer = layer
-            self.relative_path = relative_path
-            self._stat = stat
-
-        def __fspath__(self) -> str:
-            return self.physical_path
-
-        @property
-        def physical_path(self):
-            return _path_join(self.layer.root, self.layer.physical_path, self.relative_path)
-
-        @property
-        def logical_path(self):
-            return _path_join(self.layer.logical_path, self.relative_path)
-
-        @property
-        def stat(self):
-            if self._stat is None:
-                self._stat = os.stat(self.physical_path)
-            return self._stat
-
-        @property
-        def size(self):
-            return self.stat.st_size
-
-        @property
-        def mtime(self):
-            return self.stat.st_mtime
+class LayerRootBase:
+    """ All 'path's here are relative to the ROOT. """
 
     class Layer:
         """ Basic layer Container:   Connects logical and physical paths. """
-        __slots__ = ["name", "root", "logical_path", "physical_path", "config", "_file_cls"]
+        __slots__ = ["name", "root", "logical_path", "physical_path", "config",
+                     "_file_factory", "_cache_files"]
 
-        def __init__(self, name: str, root: str, physical: str, logical: str,
-                     config: LayerConfig, file_cls: Type):
+        def __init__(self, name: str,
+                     root: Path,
+                     physical: PurePath,
+                     logical: PurePath,
+                     config: LayerConfig,
+                     file_factory: Callable):
             self.name = name
             self.root = root
             self.physical_path = physical
             self.logical_path = logical
             self.config = config
-            self._file_cls = file_cls
+            self._file_factory = file_factory
+            self._cache_files: List[LayerFile] = []
 
-        def walk(self):
+        def walk(self) -> R_walk:
             # In the simple case, this is good enough.   Some subclasses will need to override
             for (root, dirs, files) in relwalk(_path_join(self.root, self.physical_path),
                                                followlinks=self.config.follow_symlink):
+                root = Path(root)
                 files = [f for f in files if not self.config.block_files.search(f)]
                 for d in list(dirs):
                     if d in self.config.block_dirs:
                         dirs.remove(d)
                 yield (root, dirs, files)
 
-        def list_files(self):
-            File = self._file_cls
-            for (top, dirs, files) in self.walk():
+        def iter_files(self) -> Iterator[LayerFile]:
+            for (top, _, files) in self.walk():
                 for file in files:
-                    yield File(self, _path_join(top, file))
+                    yield self._file_factory(self, top / file)
+
+        def list_files(self) -> List[LayerFile]:
+            if not self._cache_files:
+                self._cache_files = list(self.iter_files())
+            return self._cache_files
 
-        def get_file(self, path):
+        def get_file(self, path: Path) -> LayerFile:
             """ Return file object (by logical path), if it exists in this layer. """
+            # TODO:  Optimize by making a dict with a logical_path as the key
+            for file in self.list_files():
+                if file.logical_path == path:
+                    if file.physical_path.is_file():
+                        return file
+                    else:
+                        return None
+
+            '''
             # XXX: There's probably ways to optimize this.  fine for now (correctness over speed)
-            File = self._file_cls
             rel_path = path_in_layer(self.logical_path, path)
             if not rel_path:
                 return None
-            file_ = File(self, rel_path)
-            if os.path.isfile(file_.physical_path):
+            file_ = self._file_factory(self, rel_path)
+            if file_.physical_path.is_file():
                 return file_
             '''
-            path_p = _path_join(self.root, self.physical_path, rel_path)
-            if os.path.isfile(path_p):
-                return File(self, rel_path)
-            '''
 
-    def __init__(self, config=None):
-        self._layers = []
-        self.layer_filter = None
+    # LayerRootBase
+    def __init__(self, config: LayerConfig = None):
+        self._layers: List[LayerRootBase.Layer] = []
         self.config = config or LayerConfig()
 
-    def apply_filter(self, layer_filter):
+    def apply_filter(self, layer_filter: LayerFilter) -> bool:
         """
         Apply a destructive filter to all layers.  layer_filter(layer) will be called one for each
         layer, if the filter returns True than the layer is kept.  Root layers are always kept.
+
+        Returns True if layers were removed
         """
         layers = [l for l in self._layers if layer_filter(l)]
         result = self._layers != layers
         self._layers = layers
         return result
 
     def order_layers(self):
         raise NotImplementedError
 
-    def add_layer(self, layer, do_sort=True):
+    def add_layer(self, layer: Layer, do_sort=True):
         self._layers.append(layer)
         if do_sort:
             self.order_layers()
 
-    def list_layers(self):
+    def list_layers(self) -> List[Layer]:
         return self._layers
 
-    def list_layer_names(self):
+    def get_layers_by_name(self, name: str) -> Iterator[LayerRootBase.Layer]:
+        for layer in self.list_layers():
+            if layer.name == name:
+                yield layer
+
+    def list_layer_names(self) -> List[str]:
         return [l.name for l in self.list_layers()]
 
-    def list_files(self):
+    def iter_all_files(self) -> Iterator[LayerFile]:
+        """ Iterator over all physical files. """
+        for layer in self._layers:
+            yield from layer.iter_files()
+
+    def list_physical_files(self) -> List[LayerFile]:
+        files = set()
+        for file_ in self.iter_all_files():
+            files.add(file_.physical_path)
+        return list(files)
+
+    def list_logical_files(self) -> List[LayerFile]:
         """ Return a list of logical paths. """
         files = set()
-        for layer in self._layers:
-            for file_ in layer.list_files():
-                files.add(file_.logical_path)
+        for file_ in self.iter_all_files():
+            files.add(file_.logical_path)
         return list(files)
 
-    def get_file(self, path):
+    def get_file(self, path) -> Iterator[LayerFile]:
         """ return all layers associated with the given relative path. """
         for layer in self._layers:
             file_ = layer.get_file(path)
             if file_:
                 yield file_
 
-    def get_path_layers(self, path):
-        pass
+    # Legacy names
+    list_files = list_logical_files
 
 
 class DirectLayerRoot(LayerRootBase):
     """
     A very simple direct LayerRoot implementation that relies on all layer paths to be explicitly
     given without any automatic detection mechanisms.  You can think of this as the legacy
     implementation.
     """
 
-    def add_layer(self, path):
-        Layer, File = self.Layer, self.File
+    def add_layer(self, path: Path):
+        Layer = self.Layer
         # Layer name should be considered arbitrary and unimportant here
-        layer_name = os.path.basename(path)
-        if not os.path.isdir(path):
+        layer_name = path.name
+        if not path.is_dir():
             raise LayerUsageException("Layers must be directories.  "
                                       f"Given path '{path}' is not a directory.")
-        layer = Layer(layer_name, path, None, None, config=self.config, file_cls=File)
+        layer = Layer(layer_name, path, None, None, config=self.config,
+                      file_factory=layer_file_factory)
         super(DirectLayerRoot, self).add_layer(layer)
 
     def order_layers(self):
         # No op.  Irrelevant as layers are given (CLI) in the order they should be applied.
         pass
 
 
@@ -315,20 +422,26 @@
 # Q:  How do we mark "mount-points" in the directory structure to keep multiple layers
 #     from claiming the same files?????
 class DotDLayerRoot(LayerRootBase):
 
     class Layer(LayerRootBase.Layer):
         __slots__ = ["prune_points"]
 
-        def __init__(self, name, root, physical, logical, config, file_cls, prune_points=None):
+        def __init__(self, name: str,
+                     root: Path,
+                     physical: PurePath,
+                     logical: PurePath,
+                     config: LayerConfig,
+                     file_factory: Callable,
+                     prune_points: Set[Path] = None):
             super(DotDLayerRoot.Layer, self).__init__(name, root, physical, logical, config=config,
-                                                      file_cls=file_cls)
-            self.prune_points = set(prune_points) if prune_points else set()
+                                                      file_factory=file_factory)
+            self.prune_points: Set[Path] = set(prune_points) if prune_points else set()
 
-        def walk(self):
+        def walk(self) -> R_walk:
             for (root, dirs, files) in super(DotDLayerRoot.Layer, self).walk():
                 if root in self.prune_points:
                     # Cleanup files/dirs to keep walk() from descending deeper
                     del dirs[:]
                 else:
                     yield (root, dirs, files)
 
@@ -348,76 +461,77 @@
 
     mount_regex = re.compile(r"(?P<realname>[\w_.-]+)\.d$")
     layer_regex = re.compile(r"(?P<layer>\d\d-[\w_.-]+)")
 
     def __init__(self, config=None):
         super(DotDLayerRoot, self).__init__(config)
         # self.root = None
-        self._root_layer = None
-        self._mount_points = defaultdict(list)
+        self._root_layer: LayerRootBase.Layer = None
+        self._mount_points: Dict[Path, List[str]] = defaultdict(list)
 
-    def apply_filter(self, layer_filter):
+    def apply_filter(self, layer_filter: LayerFilter):
         # Apply filter function, but also be sure to keep the root layer
         def fltr(l):
             return l is self._root_layer or layer_filter(l)
         return super(DotDLayerRoot, self).apply_filter(fltr)
 
-    def set_root(self, root, follow_symlinks=None):
+    def set_root(self, root: Path, follow_symlinks=None):
         """ Set a root path, and auto discover all '.d' directories.
 
         Note:  We currently only support '.d/<layer>' directories, a file like
         `default.d/10-props.conf` won't be handled here.
         """
-        Layer, File = self.Layer, self.File
+        Layer = self.Layer
+        root = Path(root)
         if follow_symlinks is None:
             follow_symlinks = self.config.follow_symlink
 
         for (top, dirs, files) in relwalk(root, topdown=False, followlinks=follow_symlinks):
             del files
-
-            top_dirname, top_basename = os.path.split(top)
-            mount_mo = self.mount_regex.match(top_basename)
-
+            top = Path(top)
+            mount_mo = self.mount_regex.match(top.name)
             if mount_mo:
                 for dir_ in dirs:
                     dir_mo = self.layer_regex.match(dir_)
                     if dir_mo:
                         # XXX: Nested layers breakage, must substitute multiple ".d" folders in `top`
                         layer = Layer(dir_mo.group("layer"),
                                       root,
-                                      physical=os.path.join(top, dir_),
-                                      logical=os.path.join(top_dirname, mount_mo.group("realname")),
+                                      physical=top / dir_,
+                                      logical=top.parent / mount_mo.group("realname"),
                                       config=self.config,
-                                      file_cls=File)
+                                      file_factory=layer_file_factory)
                         self.add_layer(layer)
                         self._mount_points[top].append(dir_)
                     else:
                         # XXX: Give the user the option of logging the near-matches (could indicate a
                         # problem in the config, or could be some other legit directory structure)
                         '''
                         print(f"LAYER NEAR MISS:  {top} looks like a mount point, but {dir_} doesn't "
                               "follow the expected convention")
                         '''
                         pass
-            elif top.endswith(".d"):
+            elif top.name.endswith(".d"):
                 '''
                 print(f"MOUNT NEAR MISS:  {top}")
                 '''
                 pass
 
         # XXX: Adding <root> should be skipped if (and only if) root itself if a '.d' folder
         # Very last operation, add the top directory as the final layer (lowest rank)
-        prune_points = [os.path.join(mount, layer) for mount, layers in self._mount_points.items()
+        prune_points = [mount / layer
+                        for mount, layers in self._mount_points.items()
                         for layer in layers]
-        layer = Layer("<root>", root, None, None, config=self.config, file_cls=File,
+        layer = Layer("<root>", root, None, None, config=self.config,
+                      file_factory=layer_file_factory,
                       prune_points=prune_points)
         self.add_layer(layer, do_sort=False)
         self._root_layer = layer
 
-    def list_layers(self):
+    def list_layers(self) -> List[Layer]:
         # Return all but the root layer.
         # Avoiding self._layers[:-1] because there could be cases where root isn't included.
         return [l for l in self._layers if l is not self._root_layer]
 
     def order_layers(self):
         # Sort based on layer name (or other sorting priority:  00-<name> to 99-<name>
         self._layers.sort(key=lambda l: l.name)
```

### Comparing `ksconf-0.11.3b1/ksconf/package.py` & `ksconf-0.11.3b3/ksconf/package.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/setup_entrypoints.py` & `ksconf-0.11.3b3/ksconf/setup_entrypoints.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/util/__init__.py` & `ksconf-0.11.3b3/ksconf/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/util/compare.py` & `ksconf-0.11.3b3/ksconf/util/compare.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/util/completers.py` & `ksconf-0.11.3b3/ksconf/util/completers.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/util/file.py` & `ksconf-0.11.3b3/ksconf/util/file.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/util/rest.py` & `ksconf-0.11.3b3/ksconf/util/rest.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/util/terminal.py` & `ksconf-0.11.3b3/ksconf/util/terminal.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/vc/git.py` & `ksconf-0.11.3b3/ksconf/vc/git.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf/xmlformat.py` & `ksconf-0.11.3b3/ksconf/xmlformat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf.egg-info/PKG-INFO` & `ksconf-0.11.3b3/ksconf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksconf
-Version: 0.11.3b1
+Version: 0.11.3b3
 Summary: KSCONF: Ksconf Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
```

### Comparing `ksconf-0.11.3b1/ksconf.egg-info/SOURCES.txt` & `ksconf-0.11.3b3/ksconf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/ksconf.egg-info/entry_points.txt` & `ksconf-0.11.3b3/ksconf.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b1/setup.py` & `ksconf-0.11.3b3/setup.py`

 * *Files identical despite different names*

