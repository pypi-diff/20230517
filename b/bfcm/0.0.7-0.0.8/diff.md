# Comparing `tmp/bfcm-0.0.7.tar.gz` & `tmp/bfcm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfcm-0.0.7.tar", last modified: Thu Mar 23 17:07:31 2023, max compression
+gzip compressed data, was "bfcm-0.0.8.tar", last modified: Wed May 17 13:57:43 2023, max compression
```

## Comparing `bfcm-0.0.7.tar` & `bfcm-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 17:07:31.391000 bfcm-0.0.7/
--rw-rw-rw-   0        0        0     1144 2023-01-17 13:44:37.000000 bfcm-0.0.7/License.txt
--rw-rw-rw-   0        0        0      490 2023-03-23 17:07:31.365000 bfcm-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      944 2023-03-23 13:55:55.000000 bfcm-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 17:07:31.156000 bfcm-0.0.7/bfcm/
--rw-rw-rw-   0        0        0       27 2023-03-23 17:06:22.000000 bfcm-0.0.7/bfcm/__init__.py
--rw-rw-rw-   0        0        0     1730 2023-01-20 12:30:35.000000 bfcm-0.0.7/bfcm/bfcm.py
--rw-rw-rw-   0        0        0     7217 2023-03-23 17:03:09.000000 bfcm-0.0.7/bfcm/correlation_matrix.py
-drwxrwxrwx   0        0        0        0 2023-03-23 17:07:31.344000 bfcm-0.0.7/bfcm.egg-info/
--rw-rw-rw-   0        0        0      490 2023-03-23 17:07:30.000000 bfcm-0.0.7/bfcm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-03-23 17:07:30.000000 bfcm-0.0.7/bfcm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 17:07:30.000000 bfcm-0.0.7/bfcm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-03-23 17:07:30.000000 bfcm-0.0.7/bfcm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-23 17:07:31.381000 bfcm-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      566 2023-03-23 17:03:33.000000 bfcm-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:57:43.942000 bfcm-0.0.8/
+-rw-rw-rw-   0        0        0     1144 2023-05-17 12:44:41.000000 bfcm-0.0.8/License.txt
+-rw-rw-rw-   0        0        0      826 2023-05-17 13:57:43.931000 bfcm-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      789 2023-05-17 13:24:14.000000 bfcm-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 13:57:43.861000 bfcm-0.0.8/bfcm/
+-rw-rw-rw-   0        0        0       27 2023-05-17 12:44:41.000000 bfcm-0.0.8/bfcm/__init__.py
+-rw-rw-rw-   0        0        0     1730 2023-05-17 12:44:41.000000 bfcm-0.0.8/bfcm/bfcm.py
+-rw-rw-rw-   0        0        0     7217 2023-05-17 12:44:41.000000 bfcm-0.0.8/bfcm/correlation_matrix.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:57:43.920000 bfcm-0.0.8/bfcm.egg-info/
+-rw-rw-rw-   0        0        0      826 2023-05-17 13:57:43.000000 bfcm-0.0.8/bfcm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-05-17 13:57:43.000000 bfcm-0.0.8/bfcm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 13:57:43.000000 bfcm-0.0.8/bfcm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-17 13:57:43.000000 bfcm-0.0.8/bfcm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 13:57:43.940000 bfcm-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-05-17 13:22:16.000000 bfcm-0.0.8/setup.py
```

### Comparing `bfcm-0.0.7/License.txt` & `bfcm-0.0.8/License.txt`

 * *Files identical despite different names*

### Comparing `bfcm-0.0.7/bfcm/bfcm.py` & `bfcm-0.0.8/bfcm/bfcm.py`

 * *Files identical despite different names*

### Comparing `bfcm-0.0.7/bfcm/correlation_matrix.py` & `bfcm-0.0.8/bfcm/correlation_matrix.py`

 * *Files identical despite different names*

