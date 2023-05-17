# Comparing `tmp/taskbase-0.1.5.tar.gz` & `tmp/taskbase-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbase-0.1.5.tar", last modified: Tue May 16 13:51:12 2023, max compression
+gzip compressed data, was "taskbase-0.1.6.tar", last modified: Wed May 17 05:33:50 2023, max compression
```

## Comparing `taskbase-0.1.5.tar` & `taskbase-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 13:51:12.927576 taskbase-0.1.5/
--rw-rw-rw-   0        0        0        4 2023-05-16 10:18:40.000000 taskbase-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      427 2023-05-16 13:51:12.926579 taskbase-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-05-16 10:31:38.000000 taskbase-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 13:51:12.928582 taskbase-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      441 2023-05-16 13:50:57.000000 taskbase-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:51:12.914611 taskbase-0.1.5/taskbase/
--rw-rw-rw-   0        0        0       44 2023-05-16 13:41:59.000000 taskbase-0.1.5/taskbase/__init__.py
--rw-rw-rw-   0        0        0     2353 2023-05-16 13:39:12.000000 taskbase-0.1.5/taskbase/taskbase.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:51:12.923587 taskbase-0.1.5/taskbase.egg-info/
--rw-rw-rw-   0        0        0      427 2023-05-16 13:51:12.000000 taskbase-0.1.5/taskbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-05-16 13:51:12.000000 taskbase-0.1.5/taskbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 13:51:12.000000 taskbase-0.1.5/taskbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 13:51:12.000000 taskbase-0.1.5/taskbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 05:33:50.227681 taskbase-0.1.6/
+-rw-rw-rw-   0        0        0        4 2023-05-17 04:51:47.000000 taskbase-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      449 2023-05-17 05:33:50.226684 taskbase-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-05-16 10:31:38.000000 taskbase-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 05:33:50.228680 taskbase-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-05-17 05:32:18.000000 taskbase-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 05:33:50.212216 taskbase-0.1.6/taskbase/
+-rw-rw-rw-   0        0        0       30 2023-05-17 05:26:02.000000 taskbase-0.1.6/taskbase/__init__.py
+-rw-rw-rw-   0        0        0     2084 2023-05-17 05:25:45.000000 taskbase-0.1.6/taskbase/taskbase.py
+-rw-rw-rw-   0        0        0      428 2023-05-17 04:53:52.000000 taskbase-0.1.6/taskbase/test.py
+drwxrwxrwx   0        0        0        0 2023-05-17 05:33:50.222691 taskbase-0.1.6/taskbase.egg-info/
+-rw-rw-rw-   0        0        0      449 2023-05-17 05:33:50.000000 taskbase-0.1.6/taskbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-17 05:33:50.000000 taskbase-0.1.6/taskbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 05:33:50.000000 taskbase-0.1.6/taskbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-17 05:33:50.000000 taskbase-0.1.6/taskbase.egg-info/top_level.txt
```

