# Comparing `tmp/dexchange-sms-1.0.0.tar.gz` & `tmp/dexchange-sms-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexchange-sms-1.0.0.tar", last modified: Wed May 17 02:29:02 2023, max compression
+gzip compressed data, was "dexchange-sms-1.0.2.tar", last modified: Wed May 17 02:52:32 2023, max compression
```

## Comparing `dexchange-sms-1.0.0.tar` & `dexchange-sms-1.0.2.tar`

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
+drwxr-xr-x   0 disso      (501) staff       (20)        0 2023-05-17 02:52:32.369977 dexchange-sms-1.0.2/
+-rw-r--r--   0 disso      (501) staff       (20)     1612 2023-05-17 02:52:32.369505 dexchange-sms-1.0.2/PKG-INFO
+-rw-r--r--   0 disso      (501) staff       (20)     1201 2023-05-17 02:44:40.000000 dexchange-sms-1.0.2/README.md
+drwxr-xr-x   0 disso      (501) staff       (20)        0 2023-05-17 02:52:32.368723 dexchange-sms-1.0.2/dexchange_sms.egg-info/
+-rw-r--r--   0 disso      (501) staff       (20)     1612 2023-05-17 02:52:32.000000 dexchange-sms-1.0.2/dexchange_sms.egg-info/PKG-INFO
+-rw-r--r--   0 disso      (501) staff       (20)      202 2023-05-17 02:52:32.000000 dexchange-sms-1.0.2/dexchange_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 disso      (501) staff       (20)        1 2023-05-17 02:52:32.000000 dexchange-sms-1.0.2/dexchange_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 disso      (501) staff       (20)        9 2023-05-17 02:52:32.000000 dexchange-sms-1.0.2/dexchange_sms.egg-info/requires.txt
+-rw-r--r--   0 disso      (501) staff       (20)        1 2023-05-17 02:52:32.000000 dexchange-sms-1.0.2/dexchange_sms.egg-info/top_level.txt
+-rw-r--r--   0 disso      (501) staff       (20)       38 2023-05-17 02:52:32.370172 dexchange-sms-1.0.2/setup.cfg
+-rw-r--r--   0 disso      (501) staff       (20)      650 2023-05-17 02:52:22.000000 dexchange-sms-1.0.2/setup.py
```

