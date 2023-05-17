# Comparing `tmp/agri_sense-1.2.tar.gz` & `tmp/agri_sense-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agri_sense-1.2.tar", last modified: Wed May 17 07:56:40 2023, max compression
+gzip compressed data, was "agri_sense-1.3.tar", last modified: Wed May 17 08:01:57 2023, max compression
```

## Comparing `agri_sense-1.2.tar` & `agri_sense-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 07:56:40.907855 agri_sense-1.2/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       21 2023-05-16 04:33:47.000000 agri_sense-1.2/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      218 2023-05-17 07:56:40.907855 agri_sense-1.2/PKG-INFO
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 07:56:40.903855 agri_sense-1.2/agri_sense/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 07:53:24.000000 agri_sense-1.2/agri_sense/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-16 04:48:26.000000 agri_sense-1.2/agri_sense/main.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 07:56:40.907855 agri_sense-1.2/agri_sense.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      218 2023-05-17 07:56:40.000000 agri_sense-1.2/agri_sense.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      247 2023-05-17 07:56:40.000000 agri_sense-1.2/agri_sense.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-17 07:56:40.000000 agri_sense-1.2/agri_sense.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-17 07:56:40.000000 agri_sense-1.2/agri_sense.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       11 2023-05-17 07:56:40.000000 agri_sense-1.2/agri_sense.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       96 2023-05-17 05:25:02.000000 agri_sense-1.2/requirements.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-17 07:56:40.907855 agri_sense-1.2/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      357 2023-05-17 07:56:32.000000 agri_sense-1.2/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:01:57.652551 agri_sense-1.3/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       21 2023-05-16 04:33:47.000000 agri_sense-1.3/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      218 2023-05-17 08:01:57.652551 agri_sense-1.3/PKG-INFO
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:01:57.652551 agri_sense-1.3/agri_sense/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 08:01:32.000000 agri_sense-1.3/agri_sense/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-16 04:48:26.000000 agri_sense-1.3/agri_sense/main.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:01:57.652551 agri_sense-1.3/agri_sense.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      218 2023-05-17 08:01:57.000000 agri_sense-1.3/agri_sense.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      247 2023-05-17 08:01:57.000000 agri_sense-1.3/agri_sense.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-17 08:01:57.000000 agri_sense-1.3/agri_sense.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-17 08:01:57.000000 agri_sense-1.3/agri_sense.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       11 2023-05-17 08:01:57.000000 agri_sense-1.3/agri_sense.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       96 2023-05-17 05:25:02.000000 agri_sense-1.3/requirements.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-17 08:01:57.652551 agri_sense-1.3/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      357 2023-05-17 08:01:55.000000 agri_sense-1.3/setup.py
```

