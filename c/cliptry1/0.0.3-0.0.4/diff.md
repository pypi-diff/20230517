# Comparing `tmp/cliptry1-0.0.3.tar.gz` & `tmp/cliptry1-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliptry1-0.0.3.tar", last modified: Wed May 17 12:59:19 2023, max compression
+gzip compressed data, was "cliptry1-0.0.4.tar", last modified: Wed May 17 13:05:19 2023, max compression
```

## Comparing `cliptry1-0.0.3.tar` & `cliptry1-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 12:59:19.969146 cliptry1-0.0.3/
--rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      236 2023-05-17 12:59:19.967145 cliptry1-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 12:59:19.953318 cliptry1-0.0.3/cliptry1.egg-info/
--rw-rw-rw-   0        0        0      236 2023-05-17 12:59:19.000000 cliptry1-0.0.3/cliptry1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-17 12:59:19.000000 cliptry1-0.0.3/cliptry1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       48 2023-05-17 12:59:19.000000 cliptry1-0.0.3/cliptry1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-17 12:59:19.000000 cliptry1-0.0.3/cliptry1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-17 12:59:19.000000 cliptry1-0.0.3/cliptry1.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 12:59:19.960149 cliptry1-0.0.3/jaical/
--rw-rw-rw-   0        0        0      435 2023-05-17 12:56:16.000000 cliptry1-0.0.3/jaical/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-17 12:59:19.971145 cliptry1-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      430 2023-05-17 12:58:56.000000 cliptry1-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:05:19.156081 cliptry1-0.0.4/
+-rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      236 2023-05-17 13:05:19.152081 cliptry1-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 13:05:19.134435 cliptry1-0.0.4/cliptry1.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-05-17 13:05:18.000000 cliptry1-0.0.4/cliptry1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-17 13:05:18.000000 cliptry1-0.0.4/cliptry1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      172 2023-05-17 13:05:18.000000 cliptry1-0.0.4/cliptry1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-17 13:05:18.000000 cliptry1-0.0.4/cliptry1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 13:05:18.000000 cliptry1-0.0.4/cliptry1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 13:05:19.146435 cliptry1-0.0.4/jaical/
+-rw-rw-rw-   0        0        0      466 2023-05-17 13:02:57.000000 cliptry1-0.0.4/jaical/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 13:05:19.157081 cliptry1-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      565 2023-05-17 13:05:06.000000 cliptry1-0.0.4/setup.py
```

