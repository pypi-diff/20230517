# Comparing `tmp/aiuv-0.7.tar.gz` & `tmp/aiuv-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiuv-0.7.tar", last modified: Sun May 14 05:57:09 2023, max compression
+gzip compressed data, was "aiuv-0.8.tar", last modified: Wed May 17 05:19:33 2023, max compression
```

## Comparing `aiuv-0.7.tar` & `aiuv-0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 05:57:09.763072 aiuv-0.7/
--rw-rw-rw-   0        0        0        0 2023-05-11 10:25:19.000000 aiuv-0.7/Licence.txt
--rw-rw-rw-   0        0        0      144 2023-05-14 05:57:09.755077 aiuv-0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-14 05:57:09.723228 aiuv-0.7/aiuv.egg-info/
--rw-rw-rw-   0        0        0      144 2023-05-14 05:57:09.000000 aiuv-0.7/aiuv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-05-14 05:57:09.000000 aiuv-0.7/aiuv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 05:57:09.000000 aiuv-0.7/aiuv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-14 05:57:09.000000 aiuv-0.7/aiuv.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 05:57:09.755077 aiuv-0.7/pkg/
--rw-rw-rw-   0        0        0    22163 2023-05-14 05:56:41.000000 aiuv-0.7/pkg/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-14 05:57:09.763072 aiuv-0.7/setup.cfg
--rw-rw-rw-   0        0        0      183 2023-05-14 05:56:48.000000 aiuv-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 05:19:33.857010 aiuv-0.8/
+-rw-rw-rw-   0        0        0        0 2023-05-11 10:25:19.000000 aiuv-0.8/Licence.txt
+-rw-rw-rw-   0        0        0      144 2023-05-17 05:19:33.856012 aiuv-0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 05:19:33.853011 aiuv-0.8/aiuv.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-05-17 05:19:33.000000 aiuv-0.8/aiuv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-05-17 05:19:33.000000 aiuv-0.8/aiuv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 05:19:33.000000 aiuv-0.8/aiuv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-17 05:19:33.000000 aiuv-0.8/aiuv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 05:19:33.855012 aiuv-0.8/pkg/
+-rw-rw-rw-   0        0        0    37268 2023-05-17 05:18:17.000000 aiuv-0.8/pkg/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 05:19:33.858010 aiuv-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      183 2023-05-17 05:17:25.000000 aiuv-0.8/setup.py
```

