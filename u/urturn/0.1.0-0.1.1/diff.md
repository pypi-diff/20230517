# Comparing `tmp/urturn-0.1.0.tar.gz` & `tmp/urturn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urturn-0.1.0.tar", last modified: Wed May 17 19:52:43 2023, max compression
+gzip compressed data, was "urturn-0.1.1.tar", last modified: Wed May 17 20:02:16 2023, max compression
```

## Comparing `urturn-0.1.0.tar` & `urturn-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:52:43.983918 urturn-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 19:52:33.000000 urturn-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-17 19:52:43.983918 urturn-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 19:52:33.000000 urturn-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:52:43.983918 urturn-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-17 19:52:33.000000 urturn-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:52:43.983918 urturn-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-17 19:52:33.000000 urturn-0.1.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-17 19:52:33.000000 urturn-0.1.0/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-17 19:52:33.000000 urturn-0.1.0/tests/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-17 19:52:33.000000 urturn-0.1.0/tests/test_webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:52:43.983918 urturn-0.1.0/urturn/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn/REQUIREMENTS
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:52:33.000000 urturn-0.1.0/urturn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-17 19:52:33.000000 urturn-0.1.0/urturn/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-17 19:52:33.000000 urturn-0.1.0/urturn/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-17 19:52:33.000000 urturn-0.1.0/urturn/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-17 19:52:33.000000 urturn-0.1.0/urturn/webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:52:43.983918 urturn-0.1.0/urturn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 19:52:43.000000 urturn-0.1.0/urturn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:02:16.603979 urturn-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 20:01:59.000000 urturn-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-17 20:02:16.599979 urturn-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 20:01:59.000000 urturn-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:02:16.603979 urturn-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-17 20:01:59.000000 urturn-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:02:16.595979 urturn-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-17 20:01:59.000000 urturn-0.1.1/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-17 20:01:59.000000 urturn-0.1.1/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-17 20:01:59.000000 urturn-0.1.1/tests/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-17 20:01:59.000000 urturn-0.1.1/tests/test_webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:02:16.599979 urturn-0.1.1/urturn/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 20:02:16.000000 urturn-0.1.1/urturn/REQUIREMENTS
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 20:02:16.000000 urturn-0.1.1/urturn/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:01:59.000000 urturn-0.1.1/urturn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-17 20:01:59.000000 urturn-0.1.1/urturn/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-17 20:01:59.000000 urturn-0.1.1/urturn/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:02:16.599979 urturn-0.1.1/urturn/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-17 20:01:59.000000 urturn-0.1.1/urturn/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-17 20:01:59.000000 urturn-0.1.1/urturn/templates/job_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-17 20:01:59.000000 urturn-0.1.1/urturn/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-17 20:01:59.000000 urturn-0.1.1/urturn/webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:02:16.599979 urturn-0.1.1/urturn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-17 20:02:16.000000 urturn-0.1.1/urturn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-17 20:02:16.000000 urturn-0.1.1/urturn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:02:16.000000 urturn-0.1.1/urturn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 20:02:16.000000 urturn-0.1.1/urturn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 20:02:16.000000 urturn-0.1.1/urturn.egg-info/top_level.txt
```

### Comparing `urturn-0.1.0/LICENSE` & `urturn-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `urturn-0.1.0/setup.py` & `urturn-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,12 +51,12 @@
     description="Analyse git repositories",
     long_description="Analyse git repositories",
     url="https://github.com/MatthiasRieck/urturn",
     packages=setuptools.find_packages(exclude=["tests*"]),
     package_data={"urturn": [
         "VERSION",
         "REQUIREMENTS",
-        "analysis/merge_debt/report_templates/*",
+        "templates/*",
     ]},
     include_package_data=True,
     install_requires=requires,  # determined by requirements.txt
 )
```

### Comparing `urturn-0.1.0/tests/test_job.py` & `urturn-0.1.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.0/tests/test_scheduler.py` & `urturn-0.1.1/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.0/tests/test_trigger.py` & `urturn-0.1.1/tests/test_trigger.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.0/tests/test_webapp.py` & `urturn-0.1.1/tests/test_webapp.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.0/urturn/job.py` & `urturn-0.1.1/urturn/job.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.0/urturn/scheduler.py` & `urturn-0.1.1/urturn/scheduler.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.0/urturn/trigger.py` & `urturn-0.1.1/urturn/trigger.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.0/urturn/webapp.py` & `urturn-0.1.1/urturn/webapp.py`

 * *Files identical despite different names*

