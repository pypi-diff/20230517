# Comparing `tmp/sentry-redis-tools-0.1.5.tar.gz` & `tmp/sentry-redis-tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-redis-tools-0.1.5.tar", last modified: Wed Apr 26 19:05:01 2023, max compression
+gzip compressed data, was "sentry-redis-tools-0.1.6.tar", last modified: Wed May 17 17:01:26 2023, max compression
```

## Comparing `sentry-redis-tools-0.1.5.tar` & `sentry-redis-tools-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:05:01.142792 sentry-redis-tools-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-26 19:05:01.142792 sentry-redis-tools-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:05:01.142792 sentry-redis-tools-0.1.5/sentry_redis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/sentry_redis_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/sentry_redis_tools/cardinality_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/sentry_redis_tools/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/sentry_redis_tools/failover_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/sentry_redis_tools/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/sentry_redis_tools/sliding_windows_rate_limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:05:01.142792 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-26 19:05:00.000000 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-26 19:05:01.000000 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:05:00.000000 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:05:00.000000 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 19:05:00.000000 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 19:05:00.000000 sentry-redis-tools-0.1.5/sentry_redis_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:05:01.142792 sentry-redis-tools-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-26 19:04:55.000000 sentry-redis-tools-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:01:26.646076 sentry-redis-tools-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-17 17:01:26.642076 sentry-redis-tools-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:01:26.642076 sentry-redis-tools-0.1.6/sentry_redis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/cardinality_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/failover_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/retrying_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/sentry_redis_tools/sliding_windows_rate_limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:01:26.642076 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-17 17:01:26.000000 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-17 17:01:26.000000 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:01:26.000000 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:01:26.000000 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 17:01:26.000000 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 17:01:26.000000 sentry-redis-tools-0.1.6/sentry_redis_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:01:26.646076 sentry-redis-tools-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-17 17:01:23.000000 sentry-redis-tools-0.1.6/setup.py
```

### Comparing `sentry-redis-tools-0.1.5/sentry_redis_tools/cardinality_limiter.py` & `sentry-redis-tools-0.1.6/sentry_redis_tools/cardinality_limiter.py`

 * *Files identical despite different names*

### Comparing `sentry-redis-tools-0.1.5/sentry_redis_tools/failover_redis.py` & `sentry-redis-tools-0.1.6/sentry_redis_tools/failover_redis.py`

 * *Files identical despite different names*

### Comparing `sentry-redis-tools-0.1.5/sentry_redis_tools/metrics.py` & `sentry-redis-tools-0.1.6/sentry_redis_tools/metrics.py`

 * *Files identical despite different names*

### Comparing `sentry-redis-tools-0.1.5/sentry_redis_tools/sliding_windows_rate_limiter.py` & `sentry-redis-tools-0.1.6/sentry_redis_tools/sliding_windows_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `sentry-redis-tools-0.1.5/setup.py` & `sentry-redis-tools-0.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import find_packages, setup
 
 from typing import Sequence
 
 
 setup(
     name="sentry-redis-tools",
-    version="0.1.5",
+    version="0.1.6",
     author="Sentry",
     author_email="oss@sentry.io",
+    license="Apache-2.0",
     url="https://github.com/getsentry/sentry-redis-tools",
     description="Common utilities related to how Sentry uses Redis",
     zip_safe=False,
     install_requires=['redis>=3.0'],
     packages=find_packages(exclude=("tests", "tests.*")),
     package_data={"sentry_redis_tools": ["py.typed"]},
     include_package_data=True,
```

