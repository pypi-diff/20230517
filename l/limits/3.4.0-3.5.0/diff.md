# Comparing `tmp/limits-3.4.0.tar.gz` & `tmp/limits-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limits-3.4.0.tar", last modified: Mon Apr 17 13:05:59 2023, max compression
+DOS/MBR boot sector
```

## Comparing `limits-3.4.0.tar` & `limits-3.5.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.036538 limits-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-17 13:05:49.000000 limits-3.4.0/CLASSIFIERS
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-17 13:05:49.000000 limits-3.4.0/CONTRIBUTIONS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-17 13:05:49.000000 limits-3.4.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-17 13:05:49.000000 limits-3.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-17 13:05:49.000000 limits-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-17 13:05:59.036538 limits-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-17 13:05:49.000000 limits-3.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.024538 limits-3.4.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-04-17 13:05:49.000000 limits-3.4.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.028538 limits-3.4.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.028538 limits-3.4.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/async.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/custom-storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/strategies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/theme_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.040538 limits-3.4.0/limits/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-17 13:05:49.000000 limits-3.4.0/limits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-17 13:05:59.040538 limits-3.4.0/limits/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.028538 limits-3.4.0/limits/aio/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.032538 limits-3.4.0/limits/aio/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/memcached.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-17 13:05:49.000000 limits-3.4.0/limits/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-17 13:05:49.000000 limits-3.4.0/limits/limits.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:49.000000 limits-3.4.0/limits/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.024538 limits-3.4.0/limits/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.024538 limits-3.4.0/limits/resources/redis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.032538 limits-3.4.0/limits/resources/redis/lua_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-17 13:05:49.000000 limits-3.4.0/limits/resources/redis/lua_scripts/acquire_moving_window.lua
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-17 13:05:49.000000 limits-3.4.0/limits/resources/redis/lua_scripts/clear_keys.lua
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-17 13:05:49.000000 limits-3.4.0/limits/resources/redis/lua_scripts/incr_expire.lua
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-17 13:05:49.000000 limits-3.4.0/limits/resources/redis/lua_scripts/moving_window.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.032538 limits-3.4.0/limits/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/memcached.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/redis_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/redis_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-17 13:05:49.000000 limits-3.4.0/limits/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-17 13:05:49.000000 limits-3.4.0/limits/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-17 13:05:49.000000 limits-3.4.0/limits/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 13:05:49.000000 limits-3.4.0/limits/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.028538 limits-3.4.0/limits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-17 13:05:59.000000 limits-3.4.0/limits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-17 13:05:59.000000 limits-3.4.0/limits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:05:59.000000 limits-3.4.0/limits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:05:58.000000 limits-3.4.0/limits.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-17 13:05:59.000000 limits-3.4.0/limits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 13:05:59.000000 limits-3.4.0/limits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 13:05:49.000000 limits-3.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.036538 limits-3.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/main.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.036538 limits-3.4.0/requirements/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/async-etcd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/async-memcached.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/async-mongodb.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/async-redis.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/etcd.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/memcached.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/mongodb.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/redis.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/rediscluster.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-17 13:05:59.040538 limits-3.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1925 2023-04-17 13:05:49.000000 limits-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.036538 limits-3.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-17 13:05:49.000000 limits-3.4.0/tests/test_limit_granularities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-17 13:05:49.000000 limits-3.4.0/tests/test_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-17 13:05:49.000000 limits-3.4.0/tests/test_ratelimit_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-04-17 13:05:49.000000 limits-3.4.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-17 13:05:49.000000 limits-3.4.0/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-17 13:05:49.000000 limits-3.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-17 13:05:49.000000 limits-3.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.627705 limits-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-16 22:12:42.000000 limits-3.5.0/CLASSIFIERS
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-16 22:12:42.000000 limits-3.5.0/CONTRIBUTIONS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-16 22:12:42.000000 limits-3.5.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-16 22:12:42.000000 limits-3.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-16 22:12:42.000000 limits-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-16 22:12:50.627705 limits-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-16 22:12:42.000000 limits-3.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.619705 limits-3.5.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-05-16 22:12:42.000000 limits-3.5.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.619705 limits-3.5.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.619705 limits-3.5.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-16 22:12:42.000000 limits-3.5.0/doc/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-16 22:12:42.000000 limits-3.5.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-16 22:12:42.000000 limits-3.5.0/doc/source/async.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 22:12:42.000000 limits-3.5.0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-16 22:12:42.000000 limits-3.5.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-16 22:12:42.000000 limits-3.5.0/doc/source/custom-storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-16 22:12:42.000000 limits-3.5.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-16 22:12:42.000000 limits-3.5.0/doc/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-16 22:12:42.000000 limits-3.5.0/doc/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-16 22:12:42.000000 limits-3.5.0/doc/source/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 22:12:42.000000 limits-3.5.0/doc/source/strategies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-16 22:12:42.000000 limits-3.5.0/doc/source/theme_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.627705 limits-3.5.0/limits/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-16 22:12:42.000000 limits-3.5.0/limits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 22:12:50.627705 limits-3.5.0/limits/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.623705 limits-3.5.0/limits/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-16 22:12:42.000000 limits-3.5.0/limits/aio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.623705 limits-3.5.0/limits/aio/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-16 22:12:42.000000 limits-3.5.0/limits/aio/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-16 22:12:42.000000 limits-3.5.0/limits/aio/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-05-16 22:12:42.000000 limits-3.5.0/limits/aio/storage/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-16 22:12:42.000000 limits-3.5.0/limits/aio/storage/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-16 22:12:42.000000 limits-3.5.0/limits/aio/storage/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-05-16 22:12:42.000000 limits-3.5.0/limits/aio/storage/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14630 2023-05-16 22:12:42.000000 limits-3.5.0/limits/aio/storage/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-05-16 22:12:42.000000 limits-3.5.0/limits/aio/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-16 22:12:42.000000 limits-3.5.0/limits/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-16 22:12:42.000000 limits-3.5.0/limits/limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:42.000000 limits-3.5.0/limits/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.615705 limits-3.5.0/limits/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.615705 limits-3.5.0/limits/resources/redis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.623705 limits-3.5.0/limits/resources/redis/lua_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-16 22:12:42.000000 limits-3.5.0/limits/resources/redis/lua_scripts/acquire_moving_window.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-16 22:12:42.000000 limits-3.5.0/limits/resources/redis/lua_scripts/clear_keys.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-16 22:12:42.000000 limits-3.5.0/limits/resources/redis/lua_scripts/incr_expire.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 22:12:42.000000 limits-3.5.0/limits/resources/redis/lua_scripts/moving_window.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.623705 limits-3.5.0/limits/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-16 22:12:42.000000 limits-3.5.0/limits/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-16 22:12:42.000000 limits-3.5.0/limits/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-16 22:12:42.000000 limits-3.5.0/limits/storage/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-16 22:12:42.000000 limits-3.5.0/limits/storage/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-05-16 22:12:42.000000 limits-3.5.0/limits/storage/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-05-16 22:12:42.000000 limits-3.5.0/limits/storage/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-16 22:12:42.000000 limits-3.5.0/limits/storage/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-16 22:12:42.000000 limits-3.5.0/limits/storage/redis_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-16 22:12:42.000000 limits-3.5.0/limits/storage/redis_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-16 22:12:42.000000 limits-3.5.0/limits/storage/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-16 22:12:42.000000 limits-3.5.0/limits/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-16 22:12:42.000000 limits-3.5.0/limits/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-05-16 22:12:42.000000 limits-3.5.0/limits/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 22:12:42.000000 limits-3.5.0/limits/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.623705 limits-3.5.0/limits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-16 22:12:50.000000 limits-3.5.0/limits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-16 22:12:50.000000 limits-3.5.0/limits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:12:50.000000 limits-3.5.0/limits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:12:50.000000 limits-3.5.0/limits.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-16 22:12:50.000000 limits-3.5.0/limits.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 22:12:50.000000 limits-3.5.0/limits.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 22:12:42.000000 limits-3.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.623705 limits-3.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/main.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.627705 limits-3.5.0/requirements/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/storage/async-etcd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/storage/async-memcached.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/storage/async-mongodb.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/storage/async-redis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/storage/etcd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/storage/memcached.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/storage/mongodb.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/storage/redis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/storage/rediscluster.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-16 22:12:42.000000 limits-3.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-16 22:12:50.627705 limits-3.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1925 2023-05-16 22:12:42.000000 limits-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:12:50.627705 limits-3.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-16 22:12:42.000000 limits-3.5.0/tests/test_limit_granularities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-16 22:12:42.000000 limits-3.5.0/tests/test_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-16 22:12:42.000000 limits-3.5.0/tests/test_ratelimit_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-05-16 22:12:42.000000 limits-3.5.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-16 22:12:42.000000 limits-3.5.0/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-16 22:12:42.000000 limits-3.5.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-16 22:12:42.000000 limits-3.5.0/versioneer.py
```

### Comparing `limits-3.4.0/CLASSIFIERS` & `limits-3.5.0/CLASSIFIERS`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/HISTORY.rst` & `limits-3.5.0/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 .. :changelog:
 
 Changelog
 =========
 
+v3.5.0
+------
+Release Date: 2023-05-16
+
+* Bug Fix
+
+  * Handle ``cost`` > 8000 when using redis
+  * Remove arbitrary default timeout for redis+sentinel
+
 v3.4.0
 ------
 Release Date: 2023-04-17
 
 * Bug Fix
 
   * Remove use of weakreferences to storages in strategy
@@ -545,14 +554,15 @@
 
 
 
 
 
 
 
+
```

### Comparing `limits-3.4.0/LICENSE.txt` & `limits-3.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/PKG-INFO` & `limits-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limits
-Version: 3.4.0
+Version: 3.5.0
 Summary: Rate limiting utilities
 Home-page: https://limits.readthedocs.org
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 License: MIT
 Project-URL: Source, https://github.com/alisaifee/limits
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `limits-3.4.0/README.rst` & `limits-3.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/doc/Makefile` & `limits-3.5.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/doc/source/api.rst` & `limits-3.5.0/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/doc/source/async.rst` & `limits-3.5.0/doc/source/async.rst`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/doc/source/conf.py` & `limits-3.5.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/doc/source/custom-storage.rst` & `limits-3.5.0/doc/source/custom-storage.rst`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/doc/source/index.rst` & `limits-3.5.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/doc/source/installation.rst` & `limits-3.5.0/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/doc/source/quickstart.rst` & `limits-3.5.0/doc/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/doc/source/storage.rst` & `limits-3.5.0/doc/source/storage.rst`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/doc/source/strategies.rst` & `limits-3.5.0/doc/source/strategies.rst`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/doc/source/theme_config.py` & `limits-3.5.0/doc/source/theme_config.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/__init__.py` & `limits-3.5.0/limits/__init__.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/aio/storage/__init__.py` & `limits-3.5.0/limits/aio/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/aio/storage/base.py` & `limits-3.5.0/limits/aio/storage/base.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/aio/storage/etcd.py` & `limits-3.5.0/limits/aio/storage/etcd.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/aio/storage/memcached.py` & `limits-3.5.0/limits/aio/storage/memcached.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/aio/storage/memory.py` & `limits-3.5.0/limits/aio/storage/memory.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/aio/storage/mongodb.py` & `limits-3.5.0/limits/aio/storage/mongodb.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/aio/storage/redis.py` & `limits-3.5.0/limits/aio/storage/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,19 +345,14 @@
 
     Depends on :pypi:`coredis`
     """
 
     STORAGE_SCHEME = ["async+redis+sentinel"]
     """The storage scheme for redis accessed via a redis sentinel installation"""
 
-    DEFAULT_OPTIONS: Dict[str, Union[float, str, bool]] = {
-        "stream_timeout": 0.2,
-    }
-    "Default options passed to :class:`~coredis.sentinel.Sentinel`"
-
     DEPENDENCIES = {"coredis.sentinel": Version("3.4.0")}
 
     def __init__(
         self,
         uri: str,
         service_name: Optional[str] = None,
         use_replicas: bool = True,
@@ -398,16 +393,14 @@
         self.service_name = (
             parsed.path.replace("/", "") if parsed.path else service_name
         )
 
         if self.service_name is None:
             raise ConfigurationError("'service_name' not provided")
 
-        connection_options.setdefault("stream_timeout", 0.2)
-
         super(RedisStorage, self).__init__()
 
         self.dependency = self.dependencies["coredis.sentinel"].module
 
         self.sentinel = self.dependency.Sentinel(
             sentinel_configuration,
             sentinel_kwargs={**parsed_auth, **sentinel_options},
```

### Comparing `limits-3.4.0/limits/aio/strategies.py` & `limits-3.5.0/limits/aio/strategies.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/limits.py` & `limits-3.5.0/limits/limits.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/storage/__init__.py` & `limits-3.5.0/limits/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/storage/base.py` & `limits-3.5.0/limits/storage/base.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/storage/etcd.py` & `limits-3.5.0/limits/storage/etcd.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/storage/memcached.py` & `limits-3.5.0/limits/storage/memcached.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/storage/memory.py` & `limits-3.5.0/limits/storage/memory.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/storage/mongodb.py` & `limits-3.5.0/limits/storage/mongodb.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/storage/redis.py` & `limits-3.5.0/limits/storage/redis.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/storage/redis_cluster.py` & `limits-3.5.0/limits/storage/redis_cluster.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/storage/redis_sentinel.py` & `limits-3.5.0/limits/storage/redis_sentinel.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,14 @@
 
     Depends on :pypi:`redis` package
     """
 
     STORAGE_SCHEME = ["redis+sentinel"]
     """The storage scheme for redis accessed via a redis sentinel installation"""
 
-    DEFAULT_OPTIONS: Dict[str, Union[float, str, bool]] = {
-        "socket_timeout": 0.2,
-    }
-    "Default options passed to :class:`~redis.sentinel.Sentinel`"
-
     DEPENDENCIES = {"redis.sentinel": Version("3.0")}
 
     def __init__(
         self,
         uri: str,
         service_name: Optional[str] = None,
         use_replicas: bool = True,
@@ -75,15 +70,15 @@
         if self.service_name is None:
             raise ConfigurationError("'service_name' not provided")
 
         sentinel_dep = self.dependencies["redis.sentinel"].module
         self.sentinel: "redis.sentinel.Sentinel" = sentinel_dep.Sentinel(
             sentinel_configuration,
             sentinel_kwargs={**parsed_auth, **sentinel_options},
-            **{**self.DEFAULT_OPTIONS, **parsed_auth, **options}
+            **{**parsed_auth, **options}
         )
         self.storage = self.sentinel.master_for(self.service_name)
         self.storage_slave = self.sentinel.slave_for(self.service_name)
         self.use_replicas = use_replicas
         self.initialize_storage(uri)
 
     def get(self, key: str) -> int:
```

### Comparing `limits-3.4.0/limits/storage/registry.py` & `limits-3.5.0/limits/storage/registry.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/strategies.py` & `limits-3.5.0/limits/strategies.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/typing.py` & `limits-3.5.0/limits/typing.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits/util.py` & `limits-3.5.0/limits/util.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits.egg-info/PKG-INFO` & `limits-3.5.0/limits.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limits
-Version: 3.4.0
+Version: 3.5.0
 Summary: Rate limiting utilities
 Home-page: https://limits.readthedocs.org
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 License: MIT
 Project-URL: Source, https://github.com/alisaifee/limits
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `limits-3.4.0/limits.egg-info/SOURCES.txt` & `limits-3.5.0/limits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/limits.egg-info/requires.txt` & `limits-3.5.0/limits.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/setup.cfg` & `limits-3.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/setup.py` & `limits-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/tests/test_limit_granularities.py` & `limits-3.5.0/tests/test_limit_granularities.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/tests/test_limits.py` & `limits-3.5.0/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/tests/test_ratelimit_parser.py` & `limits-3.5.0/tests/test_ratelimit_parser.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/tests/test_storage.py` & `limits-3.5.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/tests/test_strategy.py` & `limits-3.5.0/tests/test_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,24 @@
         limiter = MovingWindowRateLimiter(storage)
         five_per_min = RateLimitItemPerMinute(5)
         limiter.hit(five_per_min, cost=5)
         assert not limiter.hit(five_per_min, cost=2)
         limiter.clear(five_per_min)
         assert limiter.hit(five_per_min)
 
+    @moving_window_storage
+    def test_moving_window_huge_cost_sync(self, uri, args, fixture):
+        storage = storage_from_string(uri, **args)
+        limiter = MovingWindowRateLimiter(storage)
+        many_per_min = RateLimitItemPerMinute(1_000_000)
+        limiter.hit(many_per_min, cost=1_000_000)
+        assert not limiter.hit(many_per_min, cost=2)
+        limiter.clear(many_per_min)
+        assert limiter.hit(many_per_min)
+
     @pytest.mark.memcached
     def test_moving_window_memcached(self, memcached):
         storage = MemcachedStorage("memcached://localhost:22122")
         with pytest.raises(NotImplementedError):
             MovingWindowRateLimiter(storage)
 
     @all_storage
```

### Comparing `limits-3.4.0/tests/test_utils.py` & `limits-3.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `limits-3.4.0/versioneer.py` & `limits-3.5.0/versioneer.py`

 * *Files identical despite different names*

