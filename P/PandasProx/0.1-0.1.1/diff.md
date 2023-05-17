# Comparing `tmp/PandasProx-0.1.tar.gz` & `tmp/PandasProx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PandasProx-0.1.tar", last modified: Wed May 17 11:53:08 2023, max compression
+gzip compressed data, was "PandasProx-0.1.1.tar", last modified: Wed May 17 12:01:31 2023, max compression
```

## Comparing `PandasProx-0.1.tar` & `PandasProx-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 11:53:08.691870 PandasProx-0.1/
--rw-rw-r--   0 user      (1000) user      (1000)      224 2023-05-17 11:53:08.691870 PandasProx-0.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)       34 2023-05-17 11:47:24.000000 PandasProx-0.1/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       79 2023-05-17 11:53:08.691870 PandasProx-0.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      363 2023-05-17 11:52:55.000000 PandasProx-0.1/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 11:53:08.691870 PandasProx-0.1/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 11:53:08.691870 PandasProx-0.1/src/PandasProx.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      224 2023-05-17 11:53:08.000000 PandasProx-0.1/src/PandasProx.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-17 11:53:08.000000 PandasProx-0.1/src/PandasProx.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 11:53:08.000000 PandasProx-0.1/src/PandasProx.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2023-05-17 11:53:08.000000 PandasProx-0.1/src/PandasProx.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 11:53:08.000000 PandasProx-0.1/src/PandasProx.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:01:31.526202 PandasProx-0.1.1/
+-rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:01:31.526202 PandasProx-0.1.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)       34 2023-05-17 11:47:24.000000 PandasProx-0.1.1/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       79 2023-05-17 12:01:31.530202 PandasProx-0.1.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      386 2023-05-17 12:00:50.000000 PandasProx-0.1.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:01:31.526202 PandasProx-0.1.1/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:01:31.526202 PandasProx-0.1.1/src/PandasProx.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:01:31.000000 PandasProx-0.1.1/src/PandasProx.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-17 12:01:31.000000 PandasProx-0.1.1/src/PandasProx.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:01:31.000000 PandasProx-0.1.1/src/PandasProx.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2023-05-17 12:01:31.000000 PandasProx-0.1.1/src/PandasProx.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:01:31.000000 PandasProx-0.1.1/src/PandasProx.egg-info/top_level.txt
```

