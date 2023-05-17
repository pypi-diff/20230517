# Comparing `tmp/awstuff-0.0.tar.gz` & `tmp/awstuff-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/awstuff-0.0.tar", last modified: Thu May 11 16:50:18 2023, max compression
+gzip compressed data, was "awstuff-0.1.tar", last modified: Wed May 17 00:32:11 2023, max compression
```

## Comparing `awstuff-0.0.tar` & `awstuff-0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 danbrickell   (501) staff       (20)        0 2023-05-11 16:50:18.000000 awstuff-0.0/
--rw-r--r--   0 danbrickell   (501) staff       (20)      252 2023-05-11 16:50:18.000000 awstuff-0.0/PKG-INFO
-drwxr-xr-x   0 danbrickell   (501) staff       (20)        0 2023-05-11 16:50:18.000000 awstuff-0.0/awstuff.egg-info/
--rw-r--r--   0 danbrickell   (501) staff       (20)      252 2023-05-11 16:50:18.000000 awstuff-0.0/awstuff.egg-info/PKG-INFO
--rw-r--r--   0 danbrickell   (501) staff       (20)        1 2023-05-11 16:50:18.000000 awstuff-0.0/awstuff.egg-info/not-zip-safe
--rw-r--r--   0 danbrickell   (501) staff       (20)      212 2023-05-11 16:50:18.000000 awstuff-0.0/awstuff.egg-info/SOURCES.txt
--rw-r--r--   0 danbrickell   (501) staff       (20)        8 2023-05-11 16:50:18.000000 awstuff-0.0/awstuff.egg-info/top_level.txt
--rw-r--r--   0 danbrickell   (501) staff       (20)        1 2023-05-11 16:50:18.000000 awstuff-0.0/awstuff.egg-info/dependency_links.txt
--rwxr-xr-x   0 danbrickell   (501) staff       (20)      255 2023-05-10 16:06:51.000000 awstuff-0.0/setup.py
--rwxr-xr-x   0 danbrickell   (501) staff       (20)       59 2023-05-11 16:50:18.000000 awstuff-0.0/setup.cfg
-drwxr-xr-x   0 danbrickell   (501) staff       (20)        0 2023-05-11 16:50:18.000000 awstuff-0.0/awstuff/
--rw-r--r--   0 danbrickell   (501) staff       (20)     3511 2023-05-11 16:45:39.000000 awstuff-0.0/awstuff/load_fxs.py
--rwxr-xr-x   0 danbrickell   (501) staff       (20)       19 2023-05-11 16:46:31.000000 awstuff-0.0/awstuff/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:32:11.409747 awstuff-0.1/
+-rw-rw-rw-   0        0        0      236 2023-05-17 00:32:11.409747 awstuff-0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 00:32:11.393748 awstuff-0.1/awstuff/
+-rw-rw-rw-   0        0        0     3449 2023-05-17 00:27:47.000000 awstuff-0.1/awstuff/Functions.py
+-rw-rw-rw-   0        0        0       33 2023-05-17 00:29:39.000000 awstuff-0.1/awstuff/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:32:11.408747 awstuff-0.1/awstuff.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-05-17 00:32:11.000000 awstuff-0.1/awstuff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-05-17 00:32:11.000000 awstuff-0.1/awstuff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 00:32:11.000000 awstuff-0.1/awstuff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 00:31:25.000000 awstuff-0.1/awstuff.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-05-17 00:32:11.000000 awstuff-0.1/awstuff.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 00:32:11.414747 awstuff-0.1/setup.cfg
+-rw-rw-rw-   0        0        0      255 2023-05-17 00:32:08.000000 awstuff-0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `awstuff-0.0/awstuff/load_fxs.py` & `awstuff-0.1/awstuff/Functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-"""Copy JSON event data from source to new bucket\'s /raw/"""
-
 import boto3
 import botocore
 import os
 import sys
 import yaml
 
-class Load_fxs:
+class Functions:
     """ Helper functions for interacting with AWS"""
 
 
     def parse_yaml(file):
         """Exposes configuration YAML file
 
         Args:
```

