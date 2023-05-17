# Comparing `tmp/ksconf-0.11.3b3.tar.gz` & `tmp/ksconf-0.11.3b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ksconf-0.11.3b3.tar", last modified: Wed May 17 15:30:06 2023, max compression
+gzip compressed data, was "ksconf-0.11.3b4.tar", last modified: Wed May 17 17:58:05 2023, max compression
```

## Comparing `ksconf-0.11.3b3.tar` & `ksconf-0.11.3b4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.656025 ksconf-0.11.3b3/
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-17 15:30:06.656025 ksconf-0.11.3b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.640025 ksconf-0.11.3b3/ksconf/
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.644025 ksconf-0.11.3b3/ksconf/app/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/app/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/app/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/app/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.648025 ksconf-0.11.3b3/ksconf/builder/
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/builder/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/builder/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/builder/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.652025 ksconf-0.11.3b3/ksconf/commands/
--rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    22959 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/promote.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/restexport.py
--rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/restpublish.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/unarchive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/commands/xmlformat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.652025 ksconf-0.11.3b3/ksconf/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/conf/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/conf/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/conf/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    18679 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/conf/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.652025 ksconf-0.11.3b3/ksconf/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14340 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/setup_entrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.652025 ksconf-0.11.3b3/ksconf/util/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/util/completers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/util/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/util/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/util/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.656025 ksconf-0.11.3b3/ksconf/vc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/vc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/vc/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/ksconf/xmlformat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:06.644025 ksconf-0.11.3b3/ksconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 15:30:06.000000 ksconf-0.11.3b3/ksconf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:29:51.000000 ksconf-0.11.3b3/ksconf.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-17 15:30:06.656025 ksconf-0.11.3b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-17 15:29:39.000000 ksconf-0.11.3b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.438895 ksconf-0.11.3b4/ksconf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.438895 ksconf-0.11.3b4/ksconf/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/app/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/app/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/app/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.438895 ksconf-0.11.3b4/ksconf/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/builder/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/builder/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/builder/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/ksconf/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22959 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/promote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/restexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/restpublish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/unarchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/commands/xmlformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/ksconf/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/conf/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/conf/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/conf/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18679 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/conf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/ksconf/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15135 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/setup_entrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/ksconf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/util/completers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/util/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/util/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/util/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/ksconf/vc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/vc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/vc/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/ksconf/xmlformat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:58:05.438895 ksconf-0.11.3b4/ksconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 17:58:05.000000 ksconf-0.11.3b4/ksconf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:57:51.000000 ksconf-0.11.3b4/ksconf.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-17 17:58:05.442895 ksconf-0.11.3b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-17 17:57:41.000000 ksconf-0.11.3b4/setup.py
```

### Comparing `ksconf-0.11.3b3/LICENSE` & `ksconf-0.11.3b4/LICENSE`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/PKG-INFO` & `ksconf-0.11.3b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksconf
-Version: 0.11.3b3
+Version: 0.11.3b4
 Summary: KSCONF: Ksconf Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
```

### Comparing `ksconf-0.11.3b3/README.md` & `ksconf-0.11.3b4/README.md`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/__init__.py` & `ksconf-0.11.3b4/ksconf/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/__main__.py` & `ksconf-0.11.3b4/ksconf/__main__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/app/__init__.py` & `ksconf-0.11.3b4/ksconf/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/app/deploy.py` & `ksconf-0.11.3b4/ksconf/app/deploy.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/app/facts.py` & `ksconf-0.11.3b4/ksconf/app/facts.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/app/manifest.py` & `ksconf-0.11.3b4/ksconf/app/manifest.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/archive.py` & `ksconf-0.11.3b4/ksconf/archive.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/builder/__init__.py` & `ksconf-0.11.3b4/ksconf/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/builder/cache.py` & `ksconf-0.11.3b4/ksconf/builder/cache.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/builder/core.py` & `ksconf-0.11.3b4/ksconf/builder/core.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/builder/steps.py` & `ksconf-0.11.3b4/ksconf/builder/steps.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/cli.py` & `ksconf-0.11.3b4/ksconf/cli.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/combine.py` & `ksconf-0.11.3b4/ksconf/combine.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/__init__.py` & `ksconf-0.11.3b4/ksconf/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/check.py` & `ksconf-0.11.3b4/ksconf/commands/check.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/combine.py` & `ksconf-0.11.3b4/ksconf/commands/combine.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/diff.py` & `ksconf-0.11.3b4/ksconf/commands/diff.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/filter.py` & `ksconf-0.11.3b4/ksconf/commands/filter.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/merge.py` & `ksconf-0.11.3b4/ksconf/commands/merge.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/minimize.py` & `ksconf-0.11.3b4/ksconf/commands/minimize.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/package.py` & `ksconf-0.11.3b4/ksconf/commands/package.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/promote.py` & `ksconf-0.11.3b4/ksconf/commands/promote.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/restexport.py` & `ksconf-0.11.3b4/ksconf/commands/restexport.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/restpublish.py` & `ksconf-0.11.3b4/ksconf/commands/restpublish.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/snapshot.py` & `ksconf-0.11.3b4/ksconf/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/sort.py` & `ksconf-0.11.3b4/ksconf/commands/sort.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/unarchive.py` & `ksconf-0.11.3b4/ksconf/commands/unarchive.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/commands/xmlformat.py` & `ksconf-0.11.3b4/ksconf/commands/xmlformat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/compat.py` & `ksconf-0.11.3b4/ksconf/compat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/conf/delta.py` & `ksconf-0.11.3b4/ksconf/conf/delta.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/conf/merge.py` & `ksconf-0.11.3b4/ksconf/conf/merge.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/conf/meta.py` & `ksconf-0.11.3b4/ksconf/conf/meta.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/conf/parser.py` & `ksconf-0.11.3b4/ksconf/conf/parser.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/consts.py` & `ksconf-0.11.3b4/ksconf/consts.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/filter.py` & `ksconf-0.11.3b4/ksconf/filter.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/layer.py` & `ksconf-0.11.3b4/ksconf/layer.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/package.py` & `ksconf-0.11.3b4/ksconf/package.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from __future__ import absolute_import, unicode_literals
+from __future__ import absolute_import, annotations, unicode_literals
 
 import hashlib
 import os
 import re
 import shutil
 import tarfile
 import tempfile
+from functools import wraps
+from os import fspath
 from typing import TextIO
 
 from ksconf.app.manifest import AppManifest
 from ksconf.combine import LayerCombiner
 from ksconf.conf.merge import merge_app_local, merge_conf_dicts
 from ksconf.conf.parser import conf_attr_boolean, parse_conf, update_conf
 from ksconf.consts import KSCONF_DEBUG
@@ -51,25 +53,36 @@
 class PackagingException(Exception):
     pass
 
 
 class AppPackager:
 
     def __init__(self, src_path, app_name: str, output: TextIO):
-        self.src_path = src_path
+        self.src_path = fspath(src_path)
         self.app_name = app_name
         self.build_dir = None
         self.app_dir = None
         self.output = output
         self._var_magic = None
 
+    def require_active_context(funct):
+        """ Decorator to mark member functions that cannot be used until the
+        context manager has been activated.
+        """
+        @wraps(funct)
+        def wrapper(self: AppPackager, *args, **kwargs):
+            assert self.build_dir, "Context manager not yet active"
+            return funct(self, *args, **kwargs)
+        return wrapper
+
     def cleanup(self):
         # Do we need  https://stackoverflow.com/a/21263493/315892  (Windows): -- See tests/cli_helper
         shutil.rmtree(self.build_dir)
         self.build_dir = None
+        self.app_dir = None
 
     def expand_var(self, value):
         """ Expand a variable, if present
 
         :param str value:  String that main contain ``{{variable}}`` substitution.
         :return: Expanded value
         :rtype: str
@@ -82,28 +95,30 @@
         :param str value:  String that may contain ``{{variable}}`` substitution.
         :return:  Expanded value if variables were expanded, else False
         :rtype: str
         """
         new_value = self._var_magic.expand(value)
         return new_value if new_value != value else False
 
+    @require_active_context
     def combine(self, src, filters, layer_method="dir.d", allow_symlink=False):
         combiner = LayerCombiner(follow_symlink=allow_symlink, quiet=True)
         if layer_method == "dir.d":
             combiner.set_layer_root(src)
         elif layer_method == "disable":
             combiner.set_source_dirs([src])
         else:
             raise NotImplementedError(f"layer_method of '{layer_method}' is not supported.  "
                                       "Please use 'dir.d' or 'disable'.")
         for action, path in filters:
             combiner.add_layer_filter(action, path)
         combiner.combine(self.app_dir)
         self._var_magic.meta["layers"] = combiner.layer_names_used
 
+    @require_active_context
     def blocklist(self, patterns):
         # XXX: Rewrite explicitly blocklist '.git' dir, because '.git*' wasn't working here. :=(
 
         # For now we just delete files out the build directory.  Not sophisticated, but it works
         # Do we need relwalker here?  relwalk
         from fnmatch import fnmatch
         for (root, dirs, files) in os.walk(self.build_dir, topdown=True):
@@ -119,36 +134,39 @@
                 for pattern in patterns:
                     if ("*" in pattern and fnmatch(path, pattern)) or d == pattern:
                         self.output.write(f"Blocked dir:  {path}  (pattern: {pattern})\n")
                         dirs.remove(d)
                         shutil.rmtree(path)
                         break
 
+    @require_active_context
     def merge_local(self):
         # XXX:  Rename this "promote_local()" ?
         """
         Find everything in local, if it has a corresponding file in default, merge.
         """
         # XXX: No logging/reporting done here :-(
         merge_app_local(self.app_dir)
         # Cleanup anything remaining in local
         self.block_local(report=False)
 
+    @require_active_context
     def block_local(self, report=True):
         local_dir = os.path.join(self.app_dir, "local")
         if os.path.isdir(local_dir):
             if report:
                 self.output.write("Removing local directory.\n")
             shutil.rmtree(local_dir)
         local_meta = os.path.join(self.app_dir, "metadata", "local.meta")
         if os.path.isfile(local_meta):
             if report:
                 self.output.write("Removing local.meta\n")
             os.unlink(local_meta)
 
+    @require_active_context
     def update_app_conf(self, version: str = None, build: str = None):
         """ Update version and/or build in ``apps.conf`` """
         app_settings = [
             ("launcher", "version", version),
             ("install", "build", build),
         ]
         appconf_file = find_conf_in_layers(self.app_dir, "app.conf") or \
@@ -167,14 +185,15 @@
                                           f"(From {value})\n")
                         value = new_value
                     else:
                         self.output.write(f"\tUpdate app.conf:  [{stanza}] "
                                           f"{attr} = {value}\n")
                     conf[stanza][attr] = value
 
+    @require_active_context
     def check(self):
         """ Run safety checks prior to building archive:
 
         1.  Set app name based on app.conf [package] id, if set.  Otherwise confirm that the package
             id and top-level folder names align.
         2.  Check for files or directories starting with ``.``, makes AppInspect very grumpy!
         """
@@ -202,14 +221,15 @@
 
         for root, dirs, files in os.walk(self.app_dir):
             for items, t in [(dirs, "directory"), (files, "file")]:
                 for name in items:
                     if name[0] == ".":
                         self.output.write(f"Found hidden {t}:  {root}/{name}\n")
 
+    @require_active_context
     def make_archive(self, filename):
         """ Create a compressed tarball of the build directory.
         """
         # type: (str) -> str
         # if os.path.isfile(filename):
         #    raise ValueError(f"Destination file already exists:  {filename}")
         app_name = self.expand_var(self.app_name)
@@ -226,14 +246,15 @@
             self.output.write(f"Creating archive:  {filename}\n")
 
         normalize_directory_mtime(self.app_dir)
         with tarfile.open(filename, mode="w:gz") as spl:
             spl.add(self.app_dir, arcname=self.app_name)
         return filename
 
+    @require_active_context
     def make_manifest(self, calculate_hash=True) -> AppManifest:
         """
         Create a manifest of the app's contents.
         """
         app_name = self.expand_var(self.app_name)
         manifest = AppManifest.from_filesystem(self.app_dir, name=app_name,
                                                calculate_hash=calculate_hash)
@@ -247,15 +268,18 @@
             self.app_dir = os.path.join(self.build_dir, "app")
         else:
             self.app_dir = os.path.join(self.build_dir, self.app_name)
         self._var_magic = AppVarMagic(self.src_path, self.app_dir)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.cleanup()
+        try:
+            self.cleanup()
+        finally:
+            self.app_dir = None
 
 
 class AppVarMagicException(KeyError):
     pass
 
 
 class AppVarMagic:
@@ -263,21 +287,21 @@
 
     def __init__(self, src_dir, build_dir, meta=None):
         self._cache = {}
         self.src_dir = src_dir
         self.build_dir = build_dir
         self.meta = meta or {}
 
-    def expand(self, value):
+    def expand(self, value: str) -> str:
         """ A simple Jinja2 like {{VAR}} substitution mechanism. """
-        # type (str) -> str
         def replace(match_obj):
             var = match_obj.group(1)
             return self[var]
         if value:
+            value = str(value)
             return re.sub(r"\{\{\s*([\w_]+)\s*\}\}", replace, value)
         return value
 
     def git_single_line(self, *args):
         out = git_cmd(args, cwd=self.src_dir)
         if out.returncode != 0:
             return f"git-errorcode-{out.returncode}"
```

### Comparing `ksconf-0.11.3b3/ksconf/setup_entrypoints.py` & `ksconf-0.11.3b4/ksconf/setup_entrypoints.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/util/__init__.py` & `ksconf-0.11.3b4/ksconf/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/util/compare.py` & `ksconf-0.11.3b4/ksconf/util/compare.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/util/completers.py` & `ksconf-0.11.3b4/ksconf/util/completers.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/util/file.py` & `ksconf-0.11.3b4/ksconf/util/file.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/util/rest.py` & `ksconf-0.11.3b4/ksconf/util/rest.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/util/terminal.py` & `ksconf-0.11.3b4/ksconf/util/terminal.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/vc/git.py` & `ksconf-0.11.3b4/ksconf/vc/git.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf/xmlformat.py` & `ksconf-0.11.3b4/ksconf/xmlformat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf.egg-info/PKG-INFO` & `ksconf-0.11.3b4/ksconf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksconf
-Version: 0.11.3b3
+Version: 0.11.3b4
 Summary: KSCONF: Ksconf Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
```

### Comparing `ksconf-0.11.3b3/ksconf.egg-info/SOURCES.txt` & `ksconf-0.11.3b4/ksconf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/ksconf.egg-info/entry_points.txt` & `ksconf-0.11.3b4/ksconf.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ksconf-0.11.3b3/setup.py` & `ksconf-0.11.3b4/setup.py`

 * *Files identical despite different names*

