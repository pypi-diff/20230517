# Comparing `tmp/file-managers-0.4.0.tar.gz` & `tmp/file-managers-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file-managers-0.4.0.tar", last modified: Tue May 16 17:56:43 2023, max compression
+gzip compressed data, was "file-managers-0.7.0.tar", last modified: Wed May 17 07:49:05 2023, max compression
```

## Comparing `file-managers-0.4.0.tar` & `file-managers-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 musfiqdehan  (1000) musfiqdehan  (1000)        0 2023-05-16 17:56:43.279620 file-managers-0.4.0/
--rw-rw-r--   0 musfiqdehan  (1000) musfiqdehan  (1000)      318 2023-05-16 17:56:43.279620 file-managers-0.4.0/PKG-INFO
--rw-rw-r--   0 musfiqdehan  (1000) musfiqdehan  (1000)       92 2023-05-16 08:11:05.000000 file-managers-0.4.0/README.md
-drwxrwxr-x   0 musfiqdehan  (1000) musfiqdehan  (1000)        0 2023-05-16 17:56:43.279620 file-managers-0.4.0/file_managers/
--rw-rw-r--   0 musfiqdehan  (1000) musfiqdehan  (1000)       46 2023-05-16 07:10:38.000000 file-managers-0.4.0/file_managers/__init__.py
-drwxrwxr-x   0 musfiqdehan  (1000) musfiqdehan  (1000)        0 2023-05-16 17:56:43.279620 file-managers-0.4.0/file_managers.egg-info/
--rw-rw-r--   0 musfiqdehan  (1000) musfiqdehan  (1000)      318 2023-05-16 17:56:43.000000 file-managers-0.4.0/file_managers.egg-info/PKG-INFO
--rw-rw-r--   0 musfiqdehan  (1000) musfiqdehan  (1000)      228 2023-05-16 17:56:43.000000 file-managers-0.4.0/file_managers.egg-info/SOURCES.txt
--rw-rw-r--   0 musfiqdehan  (1000) musfiqdehan  (1000)        1 2023-05-16 17:56:43.000000 file-managers-0.4.0/file_managers.egg-info/dependency_links.txt
--rw-rw-r--   0 musfiqdehan  (1000) musfiqdehan  (1000)       12 2023-05-16 17:56:43.000000 file-managers-0.4.0/file_managers.egg-info/requires.txt
--rw-rw-r--   0 musfiqdehan  (1000) musfiqdehan  (1000)       14 2023-05-16 17:56:43.000000 file-managers-0.4.0/file_managers.egg-info/top_level.txt
--rw-rw-r--   0 musfiqdehan  (1000) musfiqdehan  (1000)       38 2023-05-16 17:56:43.279620 file-managers-0.4.0/setup.cfg
--rw-rw-r--   0 musfiqdehan  (1000) musfiqdehan  (1000)      397 2023-05-16 17:55:11.000000 file-managers-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:49:05.228365 file-managers-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-17 07:49:05.228365 file-managers-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-17 07:48:57.000000 file-managers-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:49:05.224365 file-managers-0.7.0/file_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 07:48:57.000000 file-managers-0.7.0/file_managers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:49:05.228365 file-managers-0.7.0/file_managers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-17 07:49:05.000000 file-managers-0.7.0/file_managers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-17 07:49:05.000000 file-managers-0.7.0/file_managers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:49:05.000000 file-managers-0.7.0/file_managers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 07:49:05.000000 file-managers-0.7.0/file_managers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 07:49:05.000000 file-managers-0.7.0/file_managers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:49:05.228365 file-managers-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-17 07:48:57.000000 file-managers-0.7.0/setup.py
```

