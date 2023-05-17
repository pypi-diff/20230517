# Comparing `tmp/taskbase-0.1.6.tar.gz` & `tmp/taskbase-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbase-0.1.6.tar", last modified: Wed May 17 05:33:50 2023, max compression
+gzip compressed data, was "taskbase-0.1.7.tar", last modified: Wed May 17 05:58:06 2023, max compression
```

## Comparing `taskbase-0.1.6.tar` & `taskbase-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 05:33:50.227681 taskbase-0.1.6/
--rw-rw-rw-   0        0        0        4 2023-05-17 04:51:47.000000 taskbase-0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0      449 2023-05-17 05:33:50.226684 taskbase-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-05-16 10:31:38.000000 taskbase-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-17 05:33:50.228680 taskbase-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-05-17 05:32:18.000000 taskbase-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 05:33:50.212216 taskbase-0.1.6/taskbase/
--rw-rw-rw-   0        0        0       30 2023-05-17 05:26:02.000000 taskbase-0.1.6/taskbase/__init__.py
--rw-rw-rw-   0        0        0     2084 2023-05-17 05:25:45.000000 taskbase-0.1.6/taskbase/taskbase.py
--rw-rw-rw-   0        0        0      428 2023-05-17 04:53:52.000000 taskbase-0.1.6/taskbase/test.py
-drwxrwxrwx   0        0        0        0 2023-05-17 05:33:50.222691 taskbase-0.1.6/taskbase.egg-info/
--rw-rw-rw-   0        0        0      449 2023-05-17 05:33:50.000000 taskbase-0.1.6/taskbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-17 05:33:50.000000 taskbase-0.1.6/taskbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 05:33:50.000000 taskbase-0.1.6/taskbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-17 05:33:50.000000 taskbase-0.1.6/taskbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 05:58:06.895145 taskbase-0.1.7/
+-rw-rw-rw-   0        0        0      104 2023-05-17 05:44:40.000000 taskbase-0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     1258 2023-05-17 05:58:06.893125 taskbase-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-05-17 05:57:43.000000 taskbase-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 05:58:06.895145 taskbase-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      457 2023-05-17 05:57:57.000000 taskbase-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 05:58:06.881434 taskbase-0.1.7/taskbase/
+-rw-rw-rw-   0        0        0       30 2023-05-17 05:26:02.000000 taskbase-0.1.7/taskbase/__init__.py
+-rw-rw-rw-   0        0        0     2084 2023-05-17 05:25:45.000000 taskbase-0.1.7/taskbase/taskbase.py
+-rw-rw-rw-   0        0        0      437 2023-05-17 05:47:05.000000 taskbase-0.1.7/taskbase/test.py
+drwxrwxrwx   0        0        0        0 2023-05-17 05:58:06.891159 taskbase-0.1.7/taskbase.egg-info/
+-rw-rw-rw-   0        0        0     1258 2023-05-17 05:58:06.000000 taskbase-0.1.7/taskbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-17 05:58:06.000000 taskbase-0.1.7/taskbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 05:58:06.000000 taskbase-0.1.7/taskbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-17 05:58:06.000000 taskbase-0.1.7/taskbase.egg-info/top_level.txt
```

### Comparing `taskbase-0.1.6/taskbase/taskbase.py` & `taskbase-0.1.7/taskbase/taskbase.py`

 * *Files identical despite different names*

