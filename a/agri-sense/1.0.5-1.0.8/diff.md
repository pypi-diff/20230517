# Comparing `tmp/agri_sense-1.0.5.tar.gz` & `tmp/agri_sense-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agri_sense-1.0.5.tar", last modified: Wed May 17 05:52:49 2023, max compression
+gzip compressed data, was "agri_sense-1.0.8.tar", last modified: Wed May 17 07:37:35 2023, max compression
```

## Comparing `agri_sense-1.0.5.tar` & `agri_sense-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 05:52:49.864472 agri_sense-1.0.5/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       21 2023-05-16 04:33:47.000000 agri_sense-1.0.5/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      220 2023-05-17 05:52:49.864472 agri_sense-1.0.5/PKG-INFO
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 05:52:49.864472 agri_sense-1.0.5/agri_sense/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       36 2023-05-17 05:52:24.000000 agri_sense-1.0.5/agri_sense/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-16 04:48:26.000000 agri_sense-1.0.5/agri_sense/main.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 05:52:49.864472 agri_sense-1.0.5/agri_sense.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      220 2023-05-17 05:52:49.000000 agri_sense-1.0.5/agri_sense.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      247 2023-05-17 05:52:49.000000 agri_sense-1.0.5/agri_sense.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-17 05:52:49.000000 agri_sense-1.0.5/agri_sense.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-17 05:52:49.000000 agri_sense-1.0.5/agri_sense.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       11 2023-05-17 05:52:49.000000 agri_sense-1.0.5/agri_sense.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       96 2023-05-17 05:25:02.000000 agri_sense-1.0.5/requirements.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-17 05:52:49.864472 agri_sense-1.0.5/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      359 2023-05-17 05:52:48.000000 agri_sense-1.0.5/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 07:37:35.866579 agri_sense-1.0.8/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       21 2023-05-16 04:33:47.000000 agri_sense-1.0.8/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      220 2023-05-17 07:37:35.866579 agri_sense-1.0.8/PKG-INFO
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 07:37:35.866579 agri_sense-1.0.8/agri_sense/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       36 2023-05-17 07:37:13.000000 agri_sense-1.0.8/agri_sense/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-16 04:48:26.000000 agri_sense-1.0.8/agri_sense/main.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 07:37:35.866579 agri_sense-1.0.8/agri_sense.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      220 2023-05-17 07:37:35.000000 agri_sense-1.0.8/agri_sense.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      247 2023-05-17 07:37:35.000000 agri_sense-1.0.8/agri_sense.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-17 07:37:35.000000 agri_sense-1.0.8/agri_sense.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-17 07:37:35.000000 agri_sense-1.0.8/agri_sense.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       11 2023-05-17 07:37:35.000000 agri_sense-1.0.8/agri_sense.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       96 2023-05-17 05:25:02.000000 agri_sense-1.0.8/requirements.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-17 07:37:35.866579 agri_sense-1.0.8/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      359 2023-05-17 07:37:26.000000 agri_sense-1.0.8/setup.py
```

