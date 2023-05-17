# Comparing `tmp/urturn-0.0.2.tar.gz` & `tmp/urturn-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urturn-0.0.2.tar", last modified: Mon Mar  6 08:07:23 2023, max compression
+gzip compressed data, was "urturn-0.1.0.tar", last modified: Wed May 17 19:52:43 2023, max compression
```

## Comparing `urturn-0.0.2.tar` & `urturn-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 08:07:23.330624 urturn-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-06 08:06:59.000000 urturn-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-06 08:07:23.330624 urturn-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-06 08:06:59.000000 urturn-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 08:07:23.330624 urturn-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-03-06 08:06:59.000000 urturn-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 08:07:23.330624 urturn-0.0.2/urturn/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-06 08:07:23.000000 urturn-0.0.2/urturn/REQUIREMENTS
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-06 08:07:23.000000 urturn-0.0.2/urturn/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 08:06:59.000000 urturn-0.0.2/urturn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-06 08:06:59.000000 urturn-0.0.2/urturn/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-06 08:06:59.000000 urturn-0.0.2/urturn/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-06 08:06:59.000000 urturn-0.0.2/urturn/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 08:07:23.330624 urturn-0.0.2/urturn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-06 08:07:23.000000 urturn-0.0.2/urturn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-06 08:07:23.000000 urturn-0.0.2/urturn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 08:07:23.000000 urturn-0.0.2/urturn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-06 08:07:23.000000 urturn-0.0.2/urturn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:52:43.983918 urturn-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 19:52:33.000000 urturn-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-17 19:52:43.983918 urturn-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 19:52:33.000000 urturn-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:52:43.983918 urturn-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-17 19:52:33.000000 urturn-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:52:43.983918 urturn-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-17 19:52:33.000000 urturn-0.1.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-17 19:52:33.000000 urturn-0.1.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-17 19:52:33.000000 urturn-0.1.0/tests/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-17 19:52:33.000000 urturn-0.1.0/tests/test_webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:52:43.983918 urturn-0.1.0/urturn/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn/REQUIREMENTS
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:52:33.000000 urturn-0.1.0/urturn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-17 19:52:33.000000 urturn-0.1.0/urturn/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-17 19:52:33.000000 urturn-0.1.0/urturn/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-17 19:52:33.000000 urturn-0.1.0/urturn/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-17 19:52:33.000000 urturn-0.1.0/urturn/webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:52:43.983918 urturn-0.1.0/urturn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn.egg-info/top_level.txt
```

### Comparing `urturn-0.0.2/LICENSE` & `urturn-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `urturn-0.0.2/setup.py` & `urturn-0.1.0/setup.py`

 * *Files identical despite different names*

