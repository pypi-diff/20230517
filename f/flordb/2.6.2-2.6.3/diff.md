# Comparing `tmp/flordb-2.6.2.tar.gz` & `tmp/flordb-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flordb-2.6.2.tar", last modified: Thu May 11 17:45:07 2023, max compression
+gzip compressed data, was "flordb-2.6.3.tar", last modified: Wed May 17 00:26:37 2023, max compression
```

## Comparing `flordb-2.6.2.tar` & `flordb-2.6.3.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.447242 flordb-2.6.2/
--rw-r--r--   0 rogarcia   (501) staff       (20)    11357 2023-03-12 17:55:35.000000 flordb-2.6.2/LICENSE
--rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-05-11 17:45:07.447132 flordb-2.6.2/PKG-INFO
--rw-r--r--   0 rogarcia   (501) staff       (20)     7667 2023-03-12 20:12:23.000000 flordb-2.6.2/README.md
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.436805 flordb-2.6.2/flor/
--rw-r--r--   0 rogarcia   (501) staff       (20)      244 2023-05-10 13:18:25.000000 flordb-2.6.2/flor/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      799 2023-05-10 13:21:04.000000 flordb-2.6.2/flor/__main__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      544 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/constants.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2330 2023-05-10 13:21:04.000000 flordb-2.6.2/flor/database.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     6142 2023-05-04 17:16:10.000000 flordb-2.6.2/flor/flags.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.437800 flordb-2.6.2/flor/hlast/
--rw-r--r--   0 rogarcia   (501) staff       (20)     4159 2023-03-23 13:19:05.000000 flordb-2.6.2/flor/hlast/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8884 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gtpropagate.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.439803 flordb-2.6.2/flor/hlast/gumtree/
--rw-r--r--   0 rogarcia   (501) staff       (20)     6322 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2916 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/adapter.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/idmap.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1085 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/priorityq.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2110 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/python.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8350 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/test.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      903 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/tree.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2273 2023-03-23 13:19:05.000000 flordb-2.6.2/flor/hlast/visitors.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2634 2023-03-22 14:08:08.000000 flordb-2.6.2/flor/iterator.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.439948 flordb-2.6.2/flor/journal/
--rw-r--r--   0 rogarcia   (501) staff       (20)     2946 2023-03-22 14:08:08.000000 flordb-2.6.2/flor/journal/__init__.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.440456 flordb-2.6.2/flor/journal/entry/
--rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      710 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      284 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/constants.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.441577 flordb-2.6.2/flor/journal/entry/data/
--rw-r--r--   0 rogarcia   (501) staff       (20)      427 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/data/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      588 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/data/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2073 2023-03-23 13:19:05.000000 flordb-2.6.2/flor/journal/entry/data/dataframe.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2093 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/data/reference.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1904 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/data/torch_chkpt.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      711 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/data/value.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.442530 flordb-2.6.2/flor/journal/entry/metadata/
--rw-r--r--   0 rogarcia   (501) staff       (20)      149 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/metadata/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      461 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/metadata/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      741 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/metadata/bracket.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1032 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/metadata/eof.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.443200 flordb-2.6.2/flor/journal/tree/
--rw-r--r--   0 rogarcia   (501) staff       (20)       23 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/tree/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1285 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/tree/block.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      929 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/tree/group.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3472 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/tree/tree.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     4231 2023-03-22 14:08:08.000000 flordb-2.6.2/flor/journal/tree/window.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1998 2023-04-14 18:08:18.000000 flordb-2.6.2/flor/kits.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.444208 flordb-2.6.2/flor/logger/
--rw-r--r--   0 rogarcia   (501) staff       (20)     2219 2023-05-10 13:18:25.000000 flordb-2.6.2/flor/logger/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2179 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/logger/checkpoint_logger.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1592 2023-05-04 17:16:10.000000 flordb-2.6.2/flor/logger/exp_json.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      536 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/logger/future.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2013 2023-03-16 16:35:51.000000 flordb-2.6.2/flor/logger/log_records.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.445063 flordb-2.6.2/flor/query/
--rw-r--r--   0 rogarcia   (501) staff       (20)     8262 2023-05-10 13:31:42.000000 flordb-2.6.2/flor/query/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3658 2023-03-15 23:49:42.000000 flordb-2.6.2/flor/query/database.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1862 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/query/engine.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2503 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/query/pivot.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8773 2023-03-22 14:08:08.000000 flordb-2.6.2/flor/query/unpack.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.445664 flordb-2.6.2/flor/shelf/
--rw-r--r--   0 rogarcia   (501) staff       (20)        0 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/shelf/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2492 2023-05-10 13:18:25.000000 flordb-2.6.2/flor/shelf/cwd_shelf.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3176 2023-05-10 13:18:25.000000 flordb-2.6.2/flor/shelf/home_shelf.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.446414 flordb-2.6.2/flor/skipblock/
--rw-r--r--   0 rogarcia   (501) staff       (20)       32 2023-03-12 17:55:36.000000 flordb-2.6.2/flor/skipblock/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      689 2023-03-12 17:55:36.000000 flordb-2.6.2/flor/skipblock/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2623 2023-03-22 14:08:08.000000 flordb-2.6.2/flor/skipblock/readblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      349 2023-03-12 17:55:36.000000 flordb-2.6.2/flor/skipblock/seemblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3819 2023-04-14 18:08:18.000000 flordb-2.6.2/flor/skipblock/writeblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      600 2023-03-22 14:08:08.000000 flordb-2.6.2/flor/state.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      564 2023-04-04 22:53:53.000000 flordb-2.6.2/flor/utils.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.446996 flordb-2.6.2/flordb.egg-info/
--rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-05-11 17:45:07.000000 flordb-2.6.2/flordb.egg-info/PKG-INFO
--rw-r--r--   0 rogarcia   (501) staff       (20)     1670 2023-05-11 17:45:07.000000 flordb-2.6.2/flordb.egg-info/SOURCES.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)        1 2023-05-11 17:45:07.000000 flordb-2.6.2/flordb.egg-info/dependency_links.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)       91 2023-05-11 17:45:07.000000 flordb-2.6.2/flordb.egg-info/requires.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)        5 2023-05-11 17:45:07.000000 flordb-2.6.2/flordb.egg-info/top_level.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)       38 2023-05-11 17:45:07.447294 flordb-2.6.2/setup.cfg
--rw-r--r--   0 rogarcia   (501) staff       (20)      904 2023-05-11 17:44:55.000000 flordb-2.6.2/setup.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.323162 flordb-2.6.3/
+-rw-r--r--   0 rogarcia   (501) staff       (20)    11357 2023-03-12 17:55:35.000000 flordb-2.6.3/LICENSE
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-05-17 00:26:37.323044 flordb-2.6.3/PKG-INFO
+-rw-r--r--   0 rogarcia   (501) staff       (20)     7667 2023-03-12 20:12:23.000000 flordb-2.6.3/README.md
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.314523 flordb-2.6.3/flor/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      269 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1779 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/__main__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      922 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/batch.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      544 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/constants.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4416 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/database.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     6283 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/flags.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.315228 flordb-2.6.3/flor/hlast/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4159 2023-03-23 13:19:05.000000 flordb-2.6.3/flor/hlast/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8884 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gtpropagate.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.316408 flordb-2.6.3/flor/hlast/gumtree/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     6322 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2916 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/adapter.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/idmap.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1085 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/priorityq.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2110 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/python.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8350 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/test.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      903 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/hlast/gumtree/tree.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2273 2023-03-23 13:19:05.000000 flordb-2.6.3/flor/hlast/visitors.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2634 2023-03-22 14:08:08.000000 flordb-2.6.3/flor/iterator.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.316544 flordb-2.6.3/flor/journal/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2946 2023-03-22 14:08:08.000000 flordb-2.6.3/flor/journal/__init__.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.317005 flordb-2.6.3/flor/journal/entry/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      710 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      284 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/constants.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.318059 flordb-2.6.3/flor/journal/entry/data/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      427 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/data/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      588 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/data/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2073 2023-03-23 13:19:05.000000 flordb-2.6.3/flor/journal/entry/data/dataframe.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2093 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/data/reference.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1904 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/data/torch_chkpt.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      711 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/data/value.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.318828 flordb-2.6.3/flor/journal/entry/metadata/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      149 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/metadata/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      461 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/metadata/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      741 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/metadata/bracket.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1032 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/entry/metadata/eof.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.319429 flordb-2.6.3/flor/journal/tree/
+-rw-r--r--   0 rogarcia   (501) staff       (20)       23 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/tree/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1285 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/tree/block.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      929 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/tree/group.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3472 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/journal/tree/tree.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4231 2023-03-22 14:08:08.000000 flordb-2.6.3/flor/journal/tree/window.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1998 2023-04-14 18:08:18.000000 flordb-2.6.3/flor/kits.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.320338 flordb-2.6.3/flor/logger/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2219 2023-05-10 13:18:25.000000 flordb-2.6.3/flor/logger/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2179 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/logger/checkpoint_logger.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1592 2023-05-04 17:16:10.000000 flordb-2.6.3/flor/logger/exp_json.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      536 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/logger/future.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2013 2023-03-16 16:35:51.000000 flordb-2.6.3/flor/logger/log_records.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.321045 flordb-2.6.3/flor/query/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     7946 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/query/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3716 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/query/database.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1862 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/query/engine.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2503 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/query/pivot.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     9180 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/query/unpack.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.321380 flordb-2.6.3/flor/shelf/
+-rw-r--r--   0 rogarcia   (501) staff       (20)        0 2023-03-12 17:55:35.000000 flordb-2.6.3/flor/shelf/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2558 2023-05-17 00:21:40.000000 flordb-2.6.3/flor/shelf/cwd_shelf.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3176 2023-05-10 13:18:25.000000 flordb-2.6.3/flor/shelf/home_shelf.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.322153 flordb-2.6.3/flor/skipblock/
+-rw-r--r--   0 rogarcia   (501) staff       (20)       32 2023-03-12 17:55:36.000000 flordb-2.6.3/flor/skipblock/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      689 2023-03-12 17:55:36.000000 flordb-2.6.3/flor/skipblock/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2623 2023-03-22 14:08:08.000000 flordb-2.6.3/flor/skipblock/readblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      349 2023-03-12 17:55:36.000000 flordb-2.6.3/flor/skipblock/seemblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3819 2023-04-14 18:08:18.000000 flordb-2.6.3/flor/skipblock/writeblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      600 2023-03-22 14:08:08.000000 flordb-2.6.3/flor/state.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      564 2023-04-04 22:53:53.000000 flordb-2.6.3/flor/utils.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-17 00:26:37.322899 flordb-2.6.3/flordb.egg-info/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-05-17 00:26:37.000000 flordb-2.6.3/flordb.egg-info/PKG-INFO
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1684 2023-05-17 00:26:37.000000 flordb-2.6.3/flordb.egg-info/SOURCES.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)        1 2023-05-17 00:26:37.000000 flordb-2.6.3/flordb.egg-info/dependency_links.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)       91 2023-05-17 00:26:37.000000 flordb-2.6.3/flordb.egg-info/requires.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)        5 2023-05-17 00:26:37.000000 flordb-2.6.3/flordb.egg-info/top_level.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)       38 2023-05-17 00:26:37.323193 flordb-2.6.3/setup.cfg
+-rw-r--r--   0 rogarcia   (501) staff       (20)      904 2023-05-17 00:26:19.000000 flordb-2.6.3/setup.py
```

### Comparing `flordb-2.6.2/LICENSE` & `flordb-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/PKG-INFO` & `flordb-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flordb
-Version: 2.6.2
+Version: 2.6.3
 Summary: Fast Low-Overhead Recovery
 Home-page: https://github.com/ucbrise/flor
 Author: Rolando Garcia
 Author-email: rogarcia@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `flordb-2.6.2/README.md` & `flordb-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/constants.py` & `flordb-2.6.3/flor/constants.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/flags.py` & `flordb-2.6.3/flor/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,21 +186,30 @@
         if not skip:
             self.nsp, sys.argv[:] = self.parse_known_args()
 
 
 parser = CLI_Args()
 
 
+def is_interactive():
+    try:
+        get_ipython()
+        return True
+    except:
+        return False
+
+
 def parse():
     State.import_time = time()
     if "--flor" in sys.argv:
         parser.parse_record()
     elif "--replay_flor" in sys.argv:
         parser.parse_replay()
-    parser.parse_remaining()
+    if not is_interactive():
+        parser.parse_remaining()
 
 
 __all__ = [
     "NAME",
     "REPLAY",
     "INDEX",
     "MODE",
```

### Comparing `flordb-2.6.2/flor/hlast/__init__.py` & `flordb-2.6.3/flor/hlast/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/hlast/gtpropagate.py` & `flordb-2.6.3/flor/hlast/gtpropagate.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/hlast/gumtree/__init__.py` & `flordb-2.6.3/flor/hlast/gumtree/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/hlast/gumtree/adapter.py` & `flordb-2.6.3/flor/hlast/gumtree/adapter.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/hlast/gumtree/idmap.py` & `flordb-2.6.3/flor/hlast/gumtree/idmap.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/hlast/gumtree/priorityq.py` & `flordb-2.6.3/flor/hlast/gumtree/priorityq.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/hlast/gumtree/python.py` & `flordb-2.6.3/flor/hlast/gumtree/python.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/hlast/gumtree/test.py` & `flordb-2.6.3/flor/hlast/gumtree/test.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/hlast/gumtree/tree.py` & `flordb-2.6.3/flor/hlast/gumtree/tree.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/hlast/visitors.py` & `flordb-2.6.3/flor/hlast/visitors.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/iterator.py` & `flordb-2.6.3/flor/iterator.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/__init__.py` & `flordb-2.6.3/flor/journal/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/entry/__init__.py` & `flordb-2.6.3/flor/journal/entry/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/entry/abstract.py` & `flordb-2.6.3/flor/journal/entry/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/entry/data/abstract.py` & `flordb-2.6.3/flor/journal/entry/data/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/entry/data/dataframe.py` & `flordb-2.6.3/flor/journal/entry/data/dataframe.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/entry/data/reference.py` & `flordb-2.6.3/flor/journal/entry/data/reference.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/entry/data/torch_chkpt.py` & `flordb-2.6.3/flor/journal/entry/data/torch_chkpt.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/entry/data/value.py` & `flordb-2.6.3/flor/journal/entry/data/value.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/entry/metadata/bracket.py` & `flordb-2.6.3/flor/journal/entry/metadata/bracket.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/entry/metadata/eof.py` & `flordb-2.6.3/flor/journal/entry/metadata/eof.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/tree/block.py` & `flordb-2.6.3/flor/journal/tree/block.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/tree/group.py` & `flordb-2.6.3/flor/journal/tree/group.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/tree/tree.py` & `flordb-2.6.3/flor/journal/tree/tree.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/journal/tree/window.py` & `flordb-2.6.3/flor/journal/tree/window.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/kits.py` & `flordb-2.6.3/flor/kits.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/logger/__init__.py` & `flordb-2.6.3/flor/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/logger/checkpoint_logger.py` & `flordb-2.6.3/flor/logger/checkpoint_logger.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/logger/exp_json.py` & `flordb-2.6.3/flor/logger/exp_json.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/logger/future.py` & `flordb-2.6.3/flor/logger/future.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/logger/log_records.py` & `flordb-2.6.3/flor/logger/log_records.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/query/__init__.py` & `flordb-2.6.3/flor/query/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 "value",
             ],
         )
         .astype(
             {
                 "projid": str,
                 "runid": str,
-                "tstamp": np.datetime64,
+                "tstamp": 'datetime64[ns]',
                 "vid": str,
                 "epoch": int,
                 "step": int,
                 "name": str,
                 "value": object,
             }
         )
@@ -145,15 +145,15 @@
         df.query(where_clause)[list(DATA_PREP)]
         .drop_duplicates()
         .merge(
             pd.DataFrame(database.get_schedule(DATA_PREP)).astype(
                 {
                     "projid": str,
                     "runid": str,
-                    "tstamp": np.datetime64,
+                    "tstamp": 'datetime64[ns]',
                     "vid": str,
                     "seconds": float,
                 }
             ),
             how="inner",
             on=DATA_PREP,
         )[
@@ -178,15 +178,15 @@
             df.query(where_clause)[list(OUTR_LOOP)]
             .drop_duplicates()
             .merge(
                 pd.DataFrame(database.get_schedule(OUTR_LOOP)).astype(
                     {
                         "projid": str,
                         "runid": str,
-                        "tstamp": np.datetime64,
+                        "tstamp": 'datetime64[ns]',
                         "vid": str,
                         "epoch": int,
                         "seconds": float,
                     }
                 ),
                 how="inner",
                 on=OUTR_LOOP,
@@ -211,15 +211,15 @@
             df.query(where_clause)[list(OUTR_LOOP)]
             .drop_duplicates()
             .merge(
                 pd.DataFrame(database.get_schedule(OUTR_LOOP)).astype(
                     {
                         "projid": str,
                         "runid": str,
-                        "tstamp": np.datetime64,
+                        "tstamp": 'datetime64[ns]',
                         "vid": str,
                         "epoch": int,
                         "seconds": float,
                     }
                 ),
                 how="inner",
                 on=OUTR_LOOP,
@@ -238,21 +238,8 @@
         res = input("Continue [Y/n]? ")
         if res.strip().lower() != "n":
             batch_replay(apply_vars, path, versions, INNR_LOOP)
     else:
         raise
 
 
-def batch(table: pd.DataFrame):
-    cli_args = []
-    records = table.to_dict(orient="records")
-    for record in records:
-        s = ""
-        for k, v in record.items():
-            if v is None or math.isnan(v):
-                continue
-            s += f"--{k} {v} "
-        cli_args.append(s)
-        print(s)
-
-
-__all__ = ["log_records", "full_pivot", "clear_stash", "replay", "batch"]
+__all__ = ["log_records", "full_pivot", "clear_stash", "replay"]
```

### Comparing `flordb-2.6.2/flor/query/database.py` & `flordb-2.6.3/flor/query/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 
 def exists():
     return dbp is not None and dbp.exists()
 
 
 def start_db(projid: str):
     global dbp
+    # print('projid', projid)
     dir_n = "_".join(projid.split("_")[0:-1])
+    # print('dir_n', dir_n)
     dbp = home_shelf.florin / Path(dir_n).with_suffix(SUFFIX)
     is_first_start = not dbp.exists()
     assert State.db_conn is None, "Did you try to start_db more than once?"
     State.db_conn = sqlite3.connect(dbp)
     if is_first_start:
         init_db()
```

### Comparing `flordb-2.6.2/flor/query/engine.py` & `flordb-2.6.3/flor/query/engine.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/query/pivot.py` & `flordb-2.6.3/flor/query/pivot.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/query/unpack.py` & `flordb-2.6.3/flor/query/unpack.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,20 +60,20 @@
     active_branch = State.active_branch
     try:
         commits = filtered_versions()
         for version in commits["RECORD"]:
             if wmrk is not None and version.hexsha in wmrk:
                 break
             try:
-                # print(f"STEPPING IN {version.hexsha}")
+                print(f"STEPPING IN {version.hexsha}")
                 r.git.checkout(version)
                 cp_seconds(version)
                 cp_log_records(version)
             except Exception as e:
-                print(e)
+                print("Line 72 Exception", e)
     finally:
         r.git.checkout(active_branch)
 
 
 def cp_seconds(version):
     assert State.db_conn is not None
     hexsha, message = version.hexsha, version.message
@@ -212,14 +212,28 @@
                 "vid": hexsha,
                 "epoch": -1,
                 "step": -1,
                 "name": user_var,
                 "value": d[user_var],
             }
         )
+    if "CLI" in d:
+        for user_var in d['CLI']:
+            data.append({
+                "projid": cwd_shelf.get_projid(),
+                "runid": d["NAME"],
+                "tstamp": tstamp.stem,
+                "vid": hexsha,
+                "epoch": -1,
+                "step": -1,
+                "name": user_var,
+                "value": d['CLI'][user_var],
+            })
+
+
     if "KVS" in d:
         # LEGACY
         _kvs = d["KVS"]
 
         for k in _kvs:
             if len(k.split(".")) >= 3:
                 z = k.split(".")
```

### Comparing `flordb-2.6.2/flor/shelf/cwd_shelf.py` & `flordb-2.6.3/flor/shelf/cwd_shelf.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 
 import atexit
 
 PATH = Path(".flor")
 
 
 def get_projid():
-    if flags.NAME is None:
-        return ""
     if State.common_dir is None:
         r = Repo()
         State.common_dir = Path(r.common_dir)
     return (
         os.path.basename(os.path.dirname(str(State.common_dir)))
         + "_"
         + str(State.active_branch)
@@ -66,29 +64,33 @@
             "--contains", str(State.repo.head.commit.hexsha)
         )
     return False
 
 
 @atexit.register
 def flush():
-    path = home_shelf.close()
-    cond = in_shadow_branch()
-    projid = get_projid()
-
     if flags.NAME and not flags.REPLAY:
+        path = home_shelf.close()
+        cond = in_shadow_branch()
+        projid = get_projid()
+
         assert cond
         log_records.flush(projid, str(State.timestamp))
         exp_json.put("PROJID", projid)
         exp_json.put("EPOCHS", State.epoch)
         exp_json.flush()
         repo = State.repo
         assert repo is not None
         repo.git.add("-A")
         repo.index.commit(f"RECORD::{flags.NAME}")
     elif flags.NAME and flags.REPLAY:
+        path = home_shelf.close()
+        cond = in_shadow_branch()
+        projid = get_projid()
+
         assert cond
         for k in [k for k in exp_json.record_d if not k.isupper()]:
             log_records.put_dp(k, exp_json.record_d[k])
 
         log_records.flush(projid, str(State.timestamp))
 
     if State.db_conn:
```

### Comparing `flordb-2.6.2/flor/shelf/home_shelf.py` & `flordb-2.6.3/flor/shelf/home_shelf.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/skipblock/abstract.py` & `flordb-2.6.3/flor/skipblock/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/skipblock/readblock.py` & `flordb-2.6.3/flor/skipblock/readblock.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/skipblock/writeblock.py` & `flordb-2.6.3/flor/skipblock/writeblock.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/state.py` & `flordb-2.6.3/flor/state.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flor/utils.py` & `flordb-2.6.3/flor/utils.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.2/flordb.egg-info/PKG-INFO` & `flordb-2.6.3/flordb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flordb
-Version: 2.6.2
+Version: 2.6.3
 Summary: Fast Low-Overhead Recovery
 Home-page: https://github.com/ucbrise/flor
 Author: Rolando Garcia
 Author-email: rogarcia@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `flordb-2.6.2/flordb.egg-info/SOURCES.txt` & `flordb-2.6.3/flordb.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 flor/__init__.py
 flor/__main__.py
+flor/batch.py
 flor/constants.py
 flor/database.py
 flor/flags.py
 flor/iterator.py
 flor/kits.py
 flor/state.py
 flor/utils.py
```

### Comparing `flordb-2.6.2/setup.py` & `flordb-2.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import io
 
 with io.open("README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="flordb",
-    version="2.6.2",
+    version="2.6.3",
     author="Rolando Garcia",
     author_email="rogarcia@berkeley.edu",
     description="Fast Low-Overhead Recovery",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ucbrise/flor",
     packages=setuptools.find_packages(),
```

