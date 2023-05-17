# Comparing `tmp/agri_sense-1.0.0.tar.gz` & `tmp/agri_sense-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agri_sense-1.0.0.tar", last modified: Wed May 17 05:14:48 2023, max compression
+gzip compressed data, was "agri_sense-1.0.1.tar", last modified: Wed May 17 05:31:16 2023, max compression
```

## Comparing `agri_sense-1.0.0.tar` & `agri_sense-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 05:14:48.814623 agri_sense-1.0.0/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       21 2023-05-16 04:33:47.000000 agri_sense-1.0.0/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      220 2023-05-17 05:14:48.814623 agri_sense-1.0.0/PKG-INFO
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 05:14:48.814623 agri_sense-1.0.0/agri_sense/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 05:05:10.000000 agri_sense-1.0.0/agri_sense/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-16 04:48:26.000000 agri_sense-1.0.0/agri_sense/main.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 05:14:48.814623 agri_sense-1.0.0/agri_sense.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      220 2023-05-17 05:14:48.000000 agri_sense-1.0.0/agri_sense.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      247 2023-05-17 05:14:48.000000 agri_sense-1.0.0/agri_sense.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-17 05:14:48.000000 agri_sense-1.0.0/agri_sense.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-17 05:14:48.000000 agri_sense-1.0.0/agri_sense.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       11 2023-05-17 05:14:48.000000 agri_sense-1.0.0/agri_sense.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-16 04:48:26.000000 agri_sense-1.0.0/requirements.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-17 05:14:48.814623 agri_sense-1.0.0/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      410 2023-05-17 05:09:18.000000 agri_sense-1.0.0/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 05:31:16.131602 agri_sense-1.0.1/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       21 2023-05-16 04:33:47.000000 agri_sense-1.0.1/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      220 2023-05-17 05:31:16.131602 agri_sense-1.0.1/PKG-INFO
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 05:31:16.131602 agri_sense-1.0.1/agri_sense/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 05:05:10.000000 agri_sense-1.0.1/agri_sense/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-16 04:48:26.000000 agri_sense-1.0.1/agri_sense/main.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 05:31:16.131602 agri_sense-1.0.1/agri_sense.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      220 2023-05-17 05:31:16.000000 agri_sense-1.0.1/agri_sense.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      247 2023-05-17 05:31:16.000000 agri_sense-1.0.1/agri_sense.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-17 05:31:16.000000 agri_sense-1.0.1/agri_sense.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-17 05:31:16.000000 agri_sense-1.0.1/agri_sense.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       11 2023-05-17 05:31:16.000000 agri_sense-1.0.1/agri_sense.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       96 2023-05-17 05:25:02.000000 agri_sense-1.0.1/requirements.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-17 05:31:16.131602 agri_sense-1.0.1/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      359 2023-05-17 05:30:45.000000 agri_sense-1.0.1/setup.py
```

