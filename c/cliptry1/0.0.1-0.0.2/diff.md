# Comparing `tmp/cliptry1-0.0.1.tar.gz` & `tmp/cliptry1-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliptry1-0.0.1.tar", last modified: Wed May 17 12:50:52 2023, max compression
+gzip compressed data, was "cliptry1-0.0.2.tar", last modified: Wed May 17 12:53:31 2023, max compression
```

## Comparing `cliptry1-0.0.1.tar` & `cliptry1-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 12:50:52.709722 cliptry1-0.0.1/
--rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      236 2023-05-17 12:50:52.706723 cliptry1-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 12:50:52.690723 cliptry1-0.0.1/cliptry1.egg-info/
--rw-rw-rw-   0        0        0      236 2023-05-17 12:50:52.000000 cliptry1-0.0.1/cliptry1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-17 12:50:52.000000 cliptry1-0.0.1/cliptry1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       50 2023-05-17 12:50:52.000000 cliptry1-0.0.1/cliptry1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-17 12:50:52.000000 cliptry1-0.0.1/cliptry1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-17 12:50:52.000000 cliptry1-0.0.1/cliptry1.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 12:50:52.698723 cliptry1-0.0.1/jaical/
--rw-rw-rw-   0        0        0      364 2023-05-16 09:28:54.000000 cliptry1-0.0.1/jaical/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-17 12:50:52.711723 cliptry1-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      434 2023-05-17 12:50:30.000000 cliptry1-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 12:53:31.975221 cliptry1-0.0.2/
+-rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      236 2023-05-17 12:53:31.973221 cliptry1-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 12:53:31.957713 cliptry1-0.0.2/cliptry1.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-05-17 12:53:31.000000 cliptry1-0.0.2/cliptry1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-17 12:53:31.000000 cliptry1-0.0.2/cliptry1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       39 2023-05-17 12:53:31.000000 cliptry1-0.0.2/cliptry1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-17 12:53:31.000000 cliptry1-0.0.2/cliptry1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 12:53:31.000000 cliptry1-0.0.2/cliptry1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 12:53:31.965222 cliptry1-0.0.2/jaical/
+-rw-rw-rw-   0        0        0      364 2023-05-16 09:28:54.000000 cliptry1-0.0.2/jaical/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 12:53:31.977222 cliptry1-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      412 2023-05-17 12:53:17.000000 cliptry1-0.0.2/setup.py
```

