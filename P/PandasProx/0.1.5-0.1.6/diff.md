# Comparing `tmp/PandasProx-0.1.5.tar.gz` & `tmp/PandasProx-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PandasProx-0.1.5.tar", last modified: Wed May 17 12:52:19 2023, max compression
+gzip compressed data, was "PandasProx-0.1.6.tar", last modified: Wed May 17 12:54:32 2023, max compression
```

## Comparing `PandasProx-0.1.5.tar` & `PandasProx-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:52:19.812220 PandasProx-0.1.5/
--rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:52:19.812220 PandasProx-0.1.5/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)       34 2023-05-17 11:47:24.000000 PandasProx-0.1.5/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       79 2023-05-17 12:52:19.812220 PandasProx-0.1.5/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      505 2023-05-17 12:52:02.000000 PandasProx-0.1.5/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:52:19.808220 PandasProx-0.1.5/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:52:19.812220 PandasProx-0.1.5/src/PandasProx.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:52:19.000000 PandasProx-0.1.5/src/PandasProx.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-17 12:52:19.000000 PandasProx-0.1.5/src/PandasProx.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:52:19.000000 PandasProx-0.1.5/src/PandasProx.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2023-05-17 12:52:19.000000 PandasProx-0.1.5/src/PandasProx.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:52:19.000000 PandasProx-0.1.5/src/PandasProx.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:54:32.728548 PandasProx-0.1.6/
+-rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:54:32.728548 PandasProx-0.1.6/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)       34 2023-05-17 11:47:24.000000 PandasProx-0.1.6/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       79 2023-05-17 12:54:32.728548 PandasProx-0.1.6/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      505 2023-05-17 12:54:21.000000 PandasProx-0.1.6/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:54:32.728548 PandasProx-0.1.6/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:54:32.728548 PandasProx-0.1.6/src/PandasProx.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      226 2023-05-17 12:54:32.000000 PandasProx-0.1.6/src/PandasProx.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-17 12:54:32.000000 PandasProx-0.1.6/src/PandasProx.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:54:32.000000 PandasProx-0.1.6/src/PandasProx.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2023-05-17 12:54:32.000000 PandasProx-0.1.6/src/PandasProx.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-17 12:54:32.000000 PandasProx-0.1.6/src/PandasProx.egg-info/top_level.txt
```

