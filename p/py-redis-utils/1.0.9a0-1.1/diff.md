# Comparing `tmp/py-redis-utils-1.0.9a0.tar.gz` & `tmp/py-redis-utils-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-redis-utils-1.0.9a0.tar", last modified: Wed May 17 10:24:25 2023, max compression
+gzip compressed data, was "py-redis-utils-1.1.tar", last modified: Wed May 17 10:33:45 2023, max compression
```

## Comparing `py-redis-utils-1.0.9a0.tar` & `py-redis-utils-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 10:24:25.620864 py-redis-utils-1.0.9a0/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      418 2023-05-17 10:24:25.620864 py-redis-utils-1.0.9a0/PKG-INFO
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     1361 2023-04-11 16:05:30.000000 py-redis-utils-1.0.9a0/README.md
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 10:24:25.620864 py-redis-utils-1.0.9a0/py_redis_utils.egg-info/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      418 2023-05-17 10:24:25.000000 py-redis-utils-1.0.9a0/py_redis_utils.egg-info/PKG-INFO
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      286 2023-05-17 10:24:25.000000 py-redis-utils-1.0.9a0/py_redis_utils.egg-info/SOURCES.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-05-17 10:24:25.000000 py-redis-utils-1.0.9a0/py_redis_utils.egg-info/dependency_links.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       63 2023-05-17 10:24:25.000000 py-redis-utils-1.0.9a0/py_redis_utils.egg-info/requires.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       13 2023-05-17 10:24:25.000000 py-redis-utils-1.0.9a0/py_redis_utils.egg-info/top_level.txt
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 10:24:25.620864 py-redis-utils-1.0.9a0/pyredisutils/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       65 2023-05-17 09:03:25.000000 py-redis-utils-1.0.9a0/pyredisutils/__init__.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     8140 2023-05-17 10:24:03.000000 py-redis-utils-1.0.9a0/pyredisutils/_decorators.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)    14305 2023-05-17 09:03:25.000000 py-redis-utils-1.0.9a0/pyredisutils/_settings.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-05-17 10:24:25.620864 py-redis-utils-1.0.9a0/setup.cfg
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      787 2023-05-17 10:24:14.000000 py-redis-utils-1.0.9a0/setup.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 10:33:45.370864 py-redis-utils-1.1/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      414 2023-05-17 10:33:45.370864 py-redis-utils-1.1/PKG-INFO
+-rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     1361 2023-04-11 16:05:30.000000 py-redis-utils-1.1/README.md
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 10:33:45.370864 py-redis-utils-1.1/py_redis_utils.egg-info/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      414 2023-05-17 10:33:45.000000 py-redis-utils-1.1/py_redis_utils.egg-info/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      286 2023-05-17 10:33:45.000000 py-redis-utils-1.1/py_redis_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-05-17 10:33:45.000000 py-redis-utils-1.1/py_redis_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       63 2023-05-17 10:33:45.000000 py-redis-utils-1.1/py_redis_utils.egg-info/requires.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       13 2023-05-17 10:33:45.000000 py-redis-utils-1.1/py_redis_utils.egg-info/top_level.txt
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-05-17 10:33:45.370864 py-redis-utils-1.1/pyredisutils/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       65 2023-05-17 09:03:25.000000 py-redis-utils-1.1/pyredisutils/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     8167 2023-05-17 10:33:37.000000 py-redis-utils-1.1/pyredisutils/_decorators.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)    14305 2023-05-17 09:03:25.000000 py-redis-utils-1.1/pyredisutils/_settings.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-05-17 10:33:45.370864 py-redis-utils-1.1/setup.cfg
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      784 2023-05-17 10:33:37.000000 py-redis-utils-1.1/setup.py
```

### Comparing `py-redis-utils-1.0.9a0/README.md` & `py-redis-utils-1.1/README.md`

 * *Files identical despite different names*

### Comparing `py-redis-utils-1.0.9a0/pyredisutils/_decorators.py` & `py-redis-utils-1.1/pyredisutils/_decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 redis_instance,
                 channel_name,
                 publish_template,
                 response_template,
                 publish_changes,
                 response_changes,
             )
-
+            print(settings)
             # Applies all necessary settings
             settings.get_token()
             settings.generate_id()
             settings.update_publish_replaces()
             settings.update_response_replaces()
             settings.transform_publish_template()
             settings.transform_response_template()
```

### Comparing `py-redis-utils-1.0.9a0/pyredisutils/_settings.py` & `py-redis-utils-1.1/pyredisutils/_settings.py`

 * *Files identical despite different names*

### Comparing `py-redis-utils-1.0.9a0/setup.py` & `py-redis-utils-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.0.9a"
+VERSION = "1.1"
 DESCRIPTION = "Utilities with Redis"
 
 # Setting up
 setup(
     name="py-redis-utils",
     version=VERSION,
     author="KE",
```

