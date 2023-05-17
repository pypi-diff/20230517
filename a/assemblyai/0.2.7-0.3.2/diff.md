# Comparing `tmp/assemblyai-0.2.7.tar.gz` & `tmp/assemblyai-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/assemblyai-0.2.7.tar", last modified: Thu Jul 19 20:25:24 2018, max compression
+gzip compressed data, was "assemblyai-0.3.2.tar", last modified: Wed May 17 20:22:12 2023, max compression
```

## Comparing `assemblyai-0.2.7.tar` & `assemblyai-0.3.2.tar`

### file list

```diff
@@ -1,44 +1,29 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-19 20:25:24.000000 assemblyai-0.2.7/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-19 20:25:24.000000 assemblyai-0.2.7/assemblyai/
--rw-r--r--   0 travis    (2000) travis    (2000)      141 2018-07-19 20:23:41.000000 assemblyai-0.2.7/assemblyai/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      228 2018-07-19 20:23:41.000000 assemblyai-0.2.7/assemblyai/cli.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1830 2018-07-19 20:23:41.000000 assemblyai-0.2.7/assemblyai/client.py
--rw-r--r--   0 travis    (2000) travis    (2000)      162 2018-07-19 20:23:41.000000 assemblyai-0.2.7/assemblyai/config.py
--rw-r--r--   0 travis    (2000) travis    (2000)      921 2018-07-19 20:23:41.000000 assemblyai-0.2.7/assemblyai/exceptions.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2001 2018-07-19 20:23:41.000000 assemblyai-0.2.7/assemblyai/model.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4975 2018-07-19 20:23:41.000000 assemblyai-0.2.7/assemblyai/transcript.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-19 20:25:24.000000 assemblyai-0.2.7/assemblyai.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     7481 2018-07-19 20:25:24.000000 assemblyai-0.2.7/assemblyai.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      735 2018-07-19 20:25:24.000000 assemblyai-0.2.7/assemblyai.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-07-19 20:25:24.000000 assemblyai-0.2.7/assemblyai.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       52 2018-07-19 20:25:24.000000 assemblyai-0.2.7/assemblyai.egg-info/entry_points.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-07-19 20:25:24.000000 assemblyai-0.2.7/assemblyai.egg-info/not-zip-safe
--rw-r--r--   0 travis    (2000) travis    (2000)       28 2018-07-19 20:25:24.000000 assemblyai-0.2.7/assemblyai.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       11 2018-07-19 20:25:24.000000 assemblyai-0.2.7/assemblyai.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-19 20:25:24.000000 assemblyai-0.2.7/docs/
--rw-r--r--   0 travis    (2000) travis    (2000)      611 2018-07-19 20:23:41.000000 assemblyai-0.2.7/docs/Makefile
--rw-r--r--   0 travis    (2000) travis    (2000)       28 2018-07-19 20:23:41.000000 assemblyai-0.2.7/docs/authors.rst
--rwxr-xr-x   0 travis    (2000) travis    (2000)     4904 2018-07-19 20:23:41.000000 assemblyai-0.2.7/docs/conf.py
--rw-r--r--   0 travis    (2000) travis    (2000)       33 2018-07-19 20:23:41.000000 assemblyai-0.2.7/docs/contributing.rst
--rw-r--r--   0 travis    (2000) travis    (2000)      268 2018-07-19 20:23:41.000000 assemblyai-0.2.7/docs/credits.rst
--rw-r--r--   0 travis    (2000) travis    (2000)       28 2018-07-19 20:23:41.000000 assemblyai-0.2.7/docs/history.rst
--rw-r--r--   0 travis    (2000) travis    (2000)      318 2018-07-19 20:23:41.000000 assemblyai-0.2.7/docs/index.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     1223 2018-07-19 20:23:41.000000 assemblyai-0.2.7/docs/installation.rst
--rw-r--r--   0 travis    (2000) travis    (2000)      772 2018-07-19 20:23:41.000000 assemblyai-0.2.7/docs/make.bat
--rw-r--r--   0 travis    (2000) travis    (2000)       27 2018-07-19 20:23:41.000000 assemblyai-0.2.7/docs/readme.rst
--rw-r--r--   0 travis    (2000) travis    (2000)       75 2018-07-19 20:23:41.000000 assemblyai-0.2.7/docs/usage.rst
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-19 20:25:24.000000 assemblyai-0.2.7/tests/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-19 20:25:24.000000 assemblyai-0.2.7/tests/data/
--rw-r--r--   0 travis    (2000) travis    (2000)    61700 2018-07-19 20:23:41.000000 assemblyai-0.2.7/tests/data/office.mp3
--rw-r--r--   0 travis    (2000) travis    (2000)      869 2018-07-19 20:23:41.000000 assemblyai-0.2.7/tests/test_cli.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4439 2018-07-19 20:23:41.000000 assemblyai-0.2.7/tests/test_client.py
--rw-r--r--   0 travis    (2000) travis    (2000)      156 2018-07-19 20:23:41.000000 assemblyai-0.2.7/AUTHORS.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     3730 2018-07-19 20:23:41.000000 assemblyai-0.2.7/CONTRIBUTING.rst
--rw-r--r--   0 travis    (2000) travis    (2000)      278 2018-07-19 20:23:41.000000 assemblyai-0.2.7/HISTORY.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     1068 2018-07-19 20:23:41.000000 assemblyai-0.2.7/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)      280 2018-07-19 20:23:41.000000 assemblyai-0.2.7/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     5078 2018-07-19 20:23:41.000000 assemblyai-0.2.7/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)     3329 2018-07-19 20:23:41.000000 assemblyai-0.2.7/README.rst
--rw-r--r--   0 travis    (2000) travis    (2000)      452 2018-07-19 20:25:24.000000 assemblyai-0.2.7/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)     1617 2018-07-19 20:23:41.000000 assemblyai-0.2.7/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7481 2018-07-19 20:25:24.000000 assemblyai-0.2.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:12.961701 assemblyai-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-17 20:22:03.000000 assemblyai-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-05-17 20:22:12.957700 assemblyai-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-17 20:22:03.000000 assemblyai-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:12.957700 assemblyai-0.3.2/assemblyai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-17 20:22:03.000000 assemblyai-0.3.2/assemblyai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-17 20:22:03.000000 assemblyai-0.3.2/assemblyai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-17 20:22:03.000000 assemblyai-0.3.2/assemblyai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-17 20:22:03.000000 assemblyai-0.3.2/assemblyai/lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-05-17 20:22:03.000000 assemblyai-0.3.2/assemblyai/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44507 2023-05-17 20:22:03.000000 assemblyai-0.3.2/assemblyai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:12.957700 assemblyai-0.3.2/assemblyai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-05-17 20:22:12.000000 assemblyai-0.3.2/assemblyai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-17 20:22:12.000000 assemblyai-0.3.2/assemblyai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:22:12.000000 assemblyai-0.3.2/assemblyai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 20:22:12.000000 assemblyai-0.3.2/assemblyai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 20:22:12.000000 assemblyai-0.3.2/assemblyai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:22:12.961701 assemblyai-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-17 20:22:03.000000 assemblyai-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:12.957700 assemblyai-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:12.957700 assemblyai-0.3.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/test_lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/test_transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/test_transcript.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `assemblyai-0.2.7/assemblyai.egg-info/SOURCES.txt` & `assemblyai-0.3.2/assemblyai.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,22 @@
-AUTHORS.rst
-CONTRIBUTING.rst
-HISTORY.rst
 LICENSE
-MANIFEST.in
 README.md
-README.rst
-setup.cfg
 setup.py
 assemblyai/__init__.py
-assemblyai/cli.py
+assemblyai/api.py
 assemblyai/client.py
-assemblyai/config.py
-assemblyai/exceptions.py
-assemblyai/model.py
-assemblyai/transcript.py
+assemblyai/lemur.py
+assemblyai/transcriber.py
+assemblyai/types.py
 assemblyai.egg-info/PKG-INFO
 assemblyai.egg-info/SOURCES.txt
 assemblyai.egg-info/dependency_links.txt
-assemblyai.egg-info/entry_points.txt
-assemblyai.egg-info/not-zip-safe
 assemblyai.egg-info/requires.txt
 assemblyai.egg-info/top_level.txt
-docs/Makefile
-docs/authors.rst
-docs/conf.py
-docs/contributing.rst
-docs/credits.rst
-docs/history.rst
-docs/index.rst
-docs/installation.rst
-docs/make.bat
-docs/readme.rst
-docs/usage.rst
-tests/test_cli.py
-tests/test_client.py
-tests/data/office.mp3
+tests/__init__.py
+tests/unit/__init__.py
+tests/unit/conftest.py
+tests/unit/factories.py
+tests/unit/test_domains.py
+tests/unit/test_lemur.py
+tests/unit/test_transcriber.py
+tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.2.7/LICENSE` & `assemblyai-0.3.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018, AssemblyAI
+Copyright (c) 2023 AssemblyAI
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

