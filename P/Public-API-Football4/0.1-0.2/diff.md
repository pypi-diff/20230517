# Comparing `tmp/Public_API_Football4-0.1.tar.gz` & `tmp/Public_API_Football4-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Public_API_Football4-0.1.tar", last modified: Tue May 16 20:59:09 2023, max compression
+gzip compressed data, was "Public_API_Football4-0.2.tar", last modified: Tue May 16 22:34:49 2023, max compression
```

## Comparing `Public_API_Football4-0.1.tar` & `Public_API_Football4-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 20:59:09.068124 Public_API_Football4-0.1/
--rw-rw-rw-   0        0        0     1068 2023-05-16 19:36:53.000000 Public_API_Football4-0.1/LICENCE.txt
--rw-rw-rw-   0        0        0      234 2023-05-16 20:59:09.067124 Public_API_Football4-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 20:59:09.066124 Public_API_Football4-0.1/Public_API_Football4.egg-info/
--rw-rw-rw-   0        0        0      234 2023-05-16 20:59:08.000000 Public_API_Football4-0.1/Public_API_Football4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-05-16 20:59:09.000000 Public_API_Football4-0.1/Public_API_Football4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 20:59:08.000000 Public_API_Football4-0.1/Public_API_Football4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 20:59:08.000000 Public_API_Football4-0.1/Public_API_Football4.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 20:59:08.000000 Public_API_Football4-0.1/Public_API_Football4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 20:59:09.068124 Public_API_Football4-0.1/setup.cfg
--rw-rw-rw-   0        0        0      355 2023-05-16 20:58:56.000000 Public_API_Football4-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:34:49.147637 Public_API_Football4-0.2/
+-rw-rw-rw-   0        0        0     1068 2023-05-16 19:36:53.000000 Public_API_Football4-0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0      234 2023-05-16 22:34:49.147637 Public_API_Football4-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 22:34:49.146640 Public_API_Football4-0.2/Public_API_Football4.egg-info/
+-rw-rw-rw-   0        0        0      234 2023-05-16 22:34:49.000000 Public_API_Football4-0.2/Public_API_Football4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-05-16 22:34:49.000000 Public_API_Football4-0.2/Public_API_Football4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 22:34:49.000000 Public_API_Football4-0.2/Public_API_Football4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 22:34:49.000000 Public_API_Football4-0.2/Public_API_Football4.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 22:34:49.000000 Public_API_Football4-0.2/Public_API_Football4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 22:34:49.147637 Public_API_Football4-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      355 2023-05-16 22:34:35.000000 Public_API_Football4-0.2/setup.py
```

### Comparing `Public_API_Football4-0.1/LICENCE.txt` & `Public_API_Football4-0.2/LICENCE.txt`

 * *Files identical despite different names*

