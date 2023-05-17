# Comparing `tmp/dexchange-sms-1.0.0.tar.gz` & `tmp/dexchange-sms-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexchange-sms-1.0.0.tar", last modified: Wed May 17 02:29:02 2023, max compression
+gzip compressed data, was "dexchange-sms-1.0.1.tar", last modified: Wed May 17 02:45:36 2023, max compression
```

## Comparing `dexchange-sms-1.0.0.tar` & `dexchange-sms-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 disso      (501) staff       (20)        0 2023-05-17 02:29:02.825035 dexchange-sms-1.0.0/
--rw-r--r--   0 disso      (501) staff       (20)      150 2023-05-17 02:29:02.824605 dexchange-sms-1.0.0/PKG-INFO
-drwxr-xr-x   0 disso      (501) staff       (20)        0 2023-05-17 02:29:02.823864 dexchange-sms-1.0.0/dexchange_sms.egg-info/
--rw-r--r--   0 disso      (501) staff       (20)      150 2023-05-17 02:29:02.000000 dexchange-sms-1.0.0/dexchange_sms.egg-info/PKG-INFO
--rw-r--r--   0 disso      (501) staff       (20)      192 2023-05-17 02:29:02.000000 dexchange-sms-1.0.0/dexchange_sms.egg-info/SOURCES.txt
--rw-r--r--   0 disso      (501) staff       (20)        1 2023-05-17 02:29:02.000000 dexchange-sms-1.0.0/dexchange_sms.egg-info/dependency_links.txt
--rw-r--r--   0 disso      (501) staff       (20)        9 2023-05-17 02:29:02.000000 dexchange-sms-1.0.0/dexchange_sms.egg-info/requires.txt
--rw-r--r--   0 disso      (501) staff       (20)        1 2023-05-17 02:29:02.000000 dexchange-sms-1.0.0/dexchange_sms.egg-info/top_level.txt
--rw-r--r--   0 disso      (501) staff       (20)       38 2023-05-17 02:29:02.825179 dexchange-sms-1.0.0/setup.cfg
--rw-r--r--   0 disso      (501) staff       (20)      282 2023-05-17 02:28:45.000000 dexchange-sms-1.0.0/setup.py
+drwxr-xr-x   0 disso      (501) staff       (20)        0 2023-05-17 02:45:36.045034 dexchange-sms-1.0.1/
+-rw-r--r--   0 disso      (501) staff       (20)      150 2023-05-17 02:45:36.044505 dexchange-sms-1.0.1/PKG-INFO
+-rw-r--r--   0 disso      (501) staff       (20)     1201 2023-05-17 02:44:40.000000 dexchange-sms-1.0.1/README.md
+drwxr-xr-x   0 disso      (501) staff       (20)        0 2023-05-17 02:45:36.043937 dexchange-sms-1.0.1/dexchange_sms.egg-info/
+-rw-r--r--   0 disso      (501) staff       (20)      150 2023-05-17 02:45:35.000000 dexchange-sms-1.0.1/dexchange_sms.egg-info/PKG-INFO
+-rw-r--r--   0 disso      (501) staff       (20)      202 2023-05-17 02:45:35.000000 dexchange-sms-1.0.1/dexchange_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 disso      (501) staff       (20)        1 2023-05-17 02:45:35.000000 dexchange-sms-1.0.1/dexchange_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 disso      (501) staff       (20)        9 2023-05-17 02:45:35.000000 dexchange-sms-1.0.1/dexchange_sms.egg-info/requires.txt
+-rw-r--r--   0 disso      (501) staff       (20)        1 2023-05-17 02:45:35.000000 dexchange-sms-1.0.1/dexchange_sms.egg-info/top_level.txt
+-rw-r--r--   0 disso      (501) staff       (20)       38 2023-05-17 02:45:36.045208 dexchange-sms-1.0.1/setup.cfg
+-rw-r--r--   0 disso      (501) staff       (20)      282 2023-05-17 02:44:56.000000 dexchange-sms-1.0.1/setup.py
```

