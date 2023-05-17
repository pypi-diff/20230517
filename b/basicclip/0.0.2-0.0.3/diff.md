# Comparing `tmp/basicclip-0.0.2.tar.gz` & `tmp/basicclip-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicclip-0.0.2.tar", last modified: Wed May 17 11:08:49 2023, max compression
+gzip compressed data, was "basicclip-0.0.3.tar", last modified: Wed May 17 12:21:21 2023, max compression
```

## Comparing `basicclip-0.0.2.tar` & `basicclip-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 11:08:49.450070 basicclip-0.0.2/
--rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 basicclip-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      237 2023-05-17 11:08:49.448071 basicclip-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 basicclip-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 11:08:49.428560 basicclip-0.0.2/basicclip.egg-info/
--rw-rw-rw-   0        0        0      237 2023-05-17 11:08:49.000000 basicclip-0.0.2/basicclip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-17 11:08:49.000000 basicclip-0.0.2/basicclip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 11:08:49.000000 basicclip-0.0.2/basicclip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-17 11:08:49.000000 basicclip-0.0.2/basicclip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-17 11:08:49.000000 basicclip-0.0.2/basicclip.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 11:08:49.436557 basicclip-0.0.2/jaical/
--rw-rw-rw-   0        0        0      364 2023-05-16 09:28:54.000000 basicclip-0.0.2/jaical/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-17 11:08:49.453070 basicclip-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-05-17 11:08:33.000000 basicclip-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 12:21:21.334108 basicclip-0.0.3/
+-rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 basicclip-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      237 2023-05-17 12:21:21.331103 basicclip-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 basicclip-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 12:21:21.317106 basicclip-0.0.3/basicclip.egg-info/
+-rw-rw-rw-   0        0        0      237 2023-05-17 12:21:20.000000 basicclip-0.0.3/basicclip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-17 12:21:20.000000 basicclip-0.0.3/basicclip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       48 2023-05-17 12:21:20.000000 basicclip-0.0.3/basicclip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-17 12:21:20.000000 basicclip-0.0.3/basicclip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 12:21:20.000000 basicclip-0.0.3/basicclip.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 12:21:21.324105 basicclip-0.0.3/jaical/
+-rw-rw-rw-   0        0        0      364 2023-05-16 09:28:54.000000 basicclip-0.0.3/jaical/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 12:21:21.339106 basicclip-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      431 2023-05-17 12:21:00.000000 basicclip-0.0.3/setup.py
```

