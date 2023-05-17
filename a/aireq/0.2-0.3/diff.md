# Comparing `tmp/aireq-0.2.tar.gz` & `tmp/aireq-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aireq-0.2.tar", last modified: Sun May 14 07:22:03 2023, max compression
+gzip compressed data, was "aireq-0.3.tar", last modified: Wed May 17 06:39:23 2023, max compression
```

## Comparing `aireq-0.2.tar` & `aireq-0.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 07:22:03.170451 aireq-0.2/
--rw-rw-rw-   0        0        0      106 2023-05-14 07:22:03.165430 aireq-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-14 07:22:03.037301 aireq-0.2/ai/
--rw-rw-rw-   0        0        0    15240 2023-05-14 06:59:07.000000 aireq-0.2/ai/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 07:22:03.156682 aireq-0.2/aireq.egg-info/
--rw-rw-rw-   0        0        0      106 2023-05-14 07:22:02.000000 aireq-0.2/aireq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-05-14 07:22:02.000000 aireq-0.2/aireq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 07:22:02.000000 aireq-0.2/aireq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-14 07:22:02.000000 aireq-0.2/aireq.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 07:22:03.159508 aireq-0.2/ippr/
--rw-rw-rw-   0        0        0     8186 2023-05-14 07:08:54.000000 aireq-0.2/ippr/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-14 07:22:03.171462 aireq-0.2/setup.cfg
--rw-rw-rw-   0        0        0      206 2023-05-14 07:19:37.000000 aireq-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:39:23.137003 aireq-0.3/
+-rw-rw-rw-   0        0        0      106 2023-05-17 06:39:23.137003 aireq-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 06:39:22.725950 aireq-0.3/ai/
+-rw-rw-rw-   0        0        0    15240 2023-05-14 06:59:07.000000 aireq-0.3/ai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:39:23.102714 aireq-0.3/aireq.egg-info/
+-rw-rw-rw-   0        0        0      106 2023-05-17 06:39:22.000000 aireq-0.3/aireq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-05-17 06:39:22.000000 aireq-0.3/aireq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 06:39:22.000000 aireq-0.3/aireq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-17 06:39:22.000000 aireq-0.3/aireq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 06:39:23.104493 aireq-0.3/ippr/
+-rw-rw-rw-   0        0        0     8186 2023-05-14 07:08:54.000000 aireq-0.3/ippr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:39:23.112768 aireq-0.3/mwa/
+-rw-rw-rw-   0        0        0     3230 2023-05-17 06:37:34.000000 aireq-0.3/mwa/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 06:39:23.137003 aireq-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      212 2023-05-17 06:32:50.000000 aireq-0.3/setup.py
```

### Comparing `aireq-0.2/ai/__init__.py` & `aireq-0.3/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `aireq-0.2/ippr/__init__.py` & `aireq-0.3/ippr/__init__.py`

 * *Files identical despite different names*

