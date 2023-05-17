# Comparing `tmp/agri_sense-1.4.tar.gz` & `tmp/agri_sense-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agri_sense-1.4.tar", last modified: Wed May 17 08:11:33 2023, max compression
+gzip compressed data, was "agri_sense-1.5.tar", last modified: Wed May 17 08:18:24 2023, max compression
```

## Comparing `agri_sense-1.4.tar` & `agri_sense-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:11:33.469446 agri_sense-1.4/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       21 2023-05-16 04:33:47.000000 agri_sense-1.4/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      218 2023-05-17 08:11:33.469446 agri_sense-1.4/PKG-INFO
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:11:33.469446 agri_sense-1.4/agri_sense/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       34 2023-05-17 08:10:00.000000 agri_sense-1.4/agri_sense/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-16 04:48:26.000000 agri_sense-1.4/agri_sense/main.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:11:33.469446 agri_sense-1.4/agri_sense.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      218 2023-05-17 08:11:33.000000 agri_sense-1.4/agri_sense.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      247 2023-05-17 08:11:33.000000 agri_sense-1.4/agri_sense.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-17 08:11:33.000000 agri_sense-1.4/agri_sense.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-17 08:11:33.000000 agri_sense-1.4/agri_sense.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       11 2023-05-17 08:11:33.000000 agri_sense-1.4/agri_sense.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       96 2023-05-17 08:09:59.000000 agri_sense-1.4/requirements.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-17 08:11:33.469446 agri_sense-1.4/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      357 2023-05-17 08:11:30.000000 agri_sense-1.4/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:18:24.645505 agri_sense-1.5/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       21 2023-05-16 04:33:47.000000 agri_sense-1.5/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      218 2023-05-17 08:18:24.645505 agri_sense-1.5/PKG-INFO
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:18:24.641504 agri_sense-1.5/agri_sense/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       99 2023-05-17 08:15:57.000000 agri_sense-1.5/agri_sense/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-16 04:48:26.000000 agri_sense-1.5/agri_sense/main.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 08:18:24.645505 agri_sense-1.5/agri_sense.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      218 2023-05-17 08:18:24.000000 agri_sense-1.5/agri_sense.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      247 2023-05-17 08:18:24.000000 agri_sense-1.5/agri_sense.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-17 08:18:24.000000 agri_sense-1.5/agri_sense.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-17 08:18:24.000000 agri_sense-1.5/agri_sense.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       11 2023-05-17 08:18:24.000000 agri_sense-1.5/agri_sense.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       96 2023-05-17 08:09:59.000000 agri_sense-1.5/requirements.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-17 08:18:24.645505 agri_sense-1.5/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      357 2023-05-17 08:18:19.000000 agri_sense-1.5/setup.py
```

