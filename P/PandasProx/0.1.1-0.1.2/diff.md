# Comparing `tmp/PandasProx-0.1.1.tar.gz` & `tmp/PandasProx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PandasProx-0.1.1.tar", last modified: Wed May 17 12:01:31 2023, max compression
+gzip compressed data, was "PandasProx-0.1.2.tar", last modified: Wed May 17 12:34:11 2023, max compression
```

## Comparing `PandasProx-0.1.1.tar` & `PandasProx-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:01:31.526202 PandasProx-0.1.1/
--rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:01:31.526202 PandasProx-0.1.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)       34 2023-05-17 11:47:24.000000 PandasProx-0.1.1/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       79 2023-05-17 12:01:31.530202 PandasProx-0.1.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      386 2023-05-17 12:00:50.000000 PandasProx-0.1.1/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:01:31.526202 PandasProx-0.1.1/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:01:31.526202 PandasProx-0.1.1/src/PandasProx.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:01:31.000000 PandasProx-0.1.1/src/PandasProx.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-17 12:01:31.000000 PandasProx-0.1.1/src/PandasProx.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:01:31.000000 PandasProx-0.1.1/src/PandasProx.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2023-05-17 12:01:31.000000 PandasProx-0.1.1/src/PandasProx.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:01:31.000000 PandasProx-0.1.1/src/PandasProx.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:34:11.424359 PandasProx-0.1.2/
+-rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:34:11.424359 PandasProx-0.1.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)       34 2023-05-17 11:47:24.000000 PandasProx-0.1.2/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       79 2023-05-17 12:34:11.424359 PandasProx-0.1.2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      472 2023-05-17 12:33:47.000000 PandasProx-0.1.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:34:11.424359 PandasProx-0.1.2/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:34:11.424359 PandasProx-0.1.2/src/PandasProx.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:34:11.000000 PandasProx-0.1.2/src/PandasProx.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-17 12:34:11.000000 PandasProx-0.1.2/src/PandasProx.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:34:11.000000 PandasProx-0.1.2/src/PandasProx.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2023-05-17 12:34:11.000000 PandasProx-0.1.2/src/PandasProx.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:34:11.000000 PandasProx-0.1.2/src/PandasProx.egg-info/top_level.txt
```

