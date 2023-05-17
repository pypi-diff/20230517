# Comparing `tmp/a1rnctf-0.1.1.tar.gz` & `tmp/a1rnctf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\a1rnctf-0.1.1.tar", last modified: Wed May 17 06:18:54 2023, max compression
+gzip compressed data, was "dist\a1rnctf-0.1.2.tar", last modified: Wed May 17 15:37:21 2023, max compression
```

## Comparing `a1rnctf-0.1.1.tar` & `a1rnctf-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 06:18:54.000000 a1rnctf-0.1.1/
--rw-rw-rw-   0        0        0      371 2023-05-17 06:18:54.000000 a1rnctf-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-05-17 06:18:54.000000 a1rnctf-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      477 2023-05-17 06:18:26.000000 a1rnctf-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 06:18:54.000000 a1rnctf-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-17 06:18:54.000000 a1rnctf-0.1.1/src/a1rnctf.egg-info/
--rw-rw-rw-   0        0        0      371 2023-05-17 06:18:54.000000 a1rnctf-0.1.1/src/a1rnctf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-05-17 06:18:54.000000 a1rnctf-0.1.1/src/a1rnctf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 06:18:54.000000 a1rnctf-0.1.1/src/a1rnctf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 06:18:54.000000 a1rnctf-0.1.1/src/a1rnctf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 15:37:21.000000 a1rnctf-0.1.2/
+-rw-rw-rw-   0        0        0      371 2023-05-17 15:37:21.000000 a1rnctf-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-05-17 15:37:21.000000 a1rnctf-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-05-17 15:36:57.000000 a1rnctf-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:37:21.000000 a1rnctf-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 15:37:21.000000 a1rnctf-0.1.2/src/a1rnctf.egg-info/
+-rw-rw-rw-   0        0        0      371 2023-05-17 15:37:21.000000 a1rnctf-0.1.2/src/a1rnctf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-05-17 15:37:21.000000 a1rnctf-0.1.2/src/a1rnctf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 15:37:21.000000 a1rnctf-0.1.2/src/a1rnctf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 15:37:21.000000 a1rnctf-0.1.2/src/a1rnctf.egg-info/top_level.txt
```

