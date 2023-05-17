# Comparing `tmp/PandasProx-0.1.2.tar.gz` & `tmp/PandasProx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PandasProx-0.1.2.tar", last modified: Wed May 17 12:34:11 2023, max compression
+gzip compressed data, was "PandasProx-0.1.3.tar", last modified: Wed May 17 12:36:58 2023, max compression
```

## Comparing `PandasProx-0.1.2.tar` & `PandasProx-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:34:11.424359 PandasProx-0.1.2/
--rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:34:11.424359 PandasProx-0.1.2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)       34 2023-05-17 11:47:24.000000 PandasProx-0.1.2/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       79 2023-05-17 12:34:11.424359 PandasProx-0.1.2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      472 2023-05-17 12:33:47.000000 PandasProx-0.1.2/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:34:11.424359 PandasProx-0.1.2/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:34:11.424359 PandasProx-0.1.2/src/PandasProx.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:34:11.000000 PandasProx-0.1.2/src/PandasProx.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-17 12:34:11.000000 PandasProx-0.1.2/src/PandasProx.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:34:11.000000 PandasProx-0.1.2/src/PandasProx.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2023-05-17 12:34:11.000000 PandasProx-0.1.2/src/PandasProx.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:34:11.000000 PandasProx-0.1.2/src/PandasProx.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:36:58.197207 PandasProx-0.1.3/
+-rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:36:58.197207 PandasProx-0.1.3/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)       34 2023-05-17 11:47:24.000000 PandasProx-0.1.3/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       79 2023-05-17 12:36:58.197207 PandasProx-0.1.3/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      484 2023-05-17 12:36:38.000000 PandasProx-0.1.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:36:58.193207 PandasProx-0.1.3/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:36:58.193207 PandasProx-0.1.3/src/PandasProx.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:36:58.000000 PandasProx-0.1.3/src/PandasProx.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-17 12:36:58.000000 PandasProx-0.1.3/src/PandasProx.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:36:58.000000 PandasProx-0.1.3/src/PandasProx.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2023-05-17 12:36:58.000000 PandasProx-0.1.3/src/PandasProx.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:36:58.000000 PandasProx-0.1.3/src/PandasProx.egg-info/top_level.txt
```

