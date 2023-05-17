# Comparing `tmp/remoulade-1.0.1.tar.gz` & `tmp/remoulade-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remoulade-1.0.1.tar", last modified: Mon May 15 08:12:41 2023, max compression
+gzip compressed data, was "remoulade-1.1.0.tar", last modified: Wed May 17 07:45:34 2023, max compression
```

## Comparing `remoulade-1.0.1.tar` & `remoulade-1.1.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.064906 remoulade-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-15 08:12:27.000000 remoulade-1.0.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-05-15 08:12:27.000000 remoulade-1.0.1/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-15 08:12:27.000000 remoulade-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-05-15 08:12:41.064906 remoulade-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-15 08:12:27.000000 remoulade-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.052905 remoulade-1.0.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      275 2023-05-15 08:12:27.000000 remoulade-1.0.1/bin/remoulade-gevent
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-15 08:12:27.000000 remoulade-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.056905 remoulade-1.0.1/remoulade/
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.056905 remoulade-1.0.1/remoulade/api/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/api/apispec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/api/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/api/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    17143 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.056905 remoulade-1.0.1/remoulade/brokers/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/brokers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/brokers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/brokers/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/brokers/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.056905 remoulade-1.0.1/remoulade/cancel/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/cancel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/cancel/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.056905 remoulade-1.0.1/remoulade/cancel/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/cancel/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/cancel/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/cancel/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/cancel/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/cancel/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.056905 remoulade-1.0.1/remoulade/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/cli/remoulade_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/cli/remoulade_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/cli/remoulade_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/collection_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.060906 remoulade-1.0.1/remoulade/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/helpers/actor_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/helpers/backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/helpers/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/helpers/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.060906 remoulade-1.0.1/remoulade/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/age_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/catch_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/current_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/logging_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/max_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/max_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/retries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/middleware/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.060906 remoulade-1.0.1/remoulade/rate_limits/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/rate_limits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/rate_limits/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.060906 remoulade-1.0.1/remoulade/rate_limits/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/rate_limits/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/rate_limits/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/rate_limits/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/rate_limits/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/rate_limits/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/rate_limits/rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/rate_limits/window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.060906 remoulade-1.0.1/remoulade/results/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/results/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.060906 remoulade-1.0.1/remoulade/results/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/results/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/results/backends/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/results/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/results/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/results/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/results/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.060906 remoulade-1.0.1/remoulade/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.060906 remoulade-1.0.1/remoulade/state/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/state/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.064906 remoulade-1.0.1/remoulade/state/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/state/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/state/backends/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/state/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/state/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/state/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/state/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-05-15 08:12:27.000000 remoulade-1.0.1/remoulade/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:12:41.056905 remoulade-1.0.1/remoulade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-05-15 08:12:40.000000 remoulade-1.0.1/remoulade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-15 08:12:41.000000 remoulade-1.0.1/remoulade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 08:12:40.000000 remoulade-1.0.1/remoulade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-15 08:12:40.000000 remoulade-1.0.1/remoulade.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-15 08:12:40.000000 remoulade-1.0.1/remoulade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 08:12:40.000000 remoulade-1.0.1/remoulade.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-15 08:12:41.064906 remoulade-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-15 08:12:27.000000 remoulade-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.079785 remoulade-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-17 07:45:24.000000 remoulade-1.1.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-05-17 07:45:24.000000 remoulade-1.1.0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-17 07:45:24.000000 remoulade-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-17 07:45:34.079785 remoulade-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-17 07:45:24.000000 remoulade-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.071785 remoulade-1.1.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      275 2023-05-17 07:45:24.000000 remoulade-1.1.0/bin/remoulade-gevent
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-17 07:45:24.000000 remoulade-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.071785 remoulade-1.1.0/remoulade/
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.071785 remoulade-1.1.0/remoulade/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/api/apispec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/api/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/api/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17143 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.071785 remoulade-1.1.0/remoulade/brokers/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/brokers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/brokers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/brokers/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/brokers/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.075785 remoulade-1.1.0/remoulade/cancel/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/cancel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/cancel/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.075785 remoulade-1.1.0/remoulade/cancel/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/cancel/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/cancel/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/cancel/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/cancel/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/cancel/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.075785 remoulade-1.1.0/remoulade/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/cli/remoulade_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/cli/remoulade_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/cli/remoulade_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/collection_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.075785 remoulade-1.1.0/remoulade/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/helpers/actor_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/helpers/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/helpers/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/helpers/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.075785 remoulade-1.1.0/remoulade/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/age_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/catch_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/current_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/logging_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/max_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/max_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/middleware/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.075785 remoulade-1.1.0/remoulade/rate_limits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/rate_limits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/rate_limits/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.075785 remoulade-1.1.0/remoulade/rate_limits/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/rate_limits/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/rate_limits/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/rate_limits/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/rate_limits/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/rate_limits/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/rate_limits/rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/rate_limits/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.075785 remoulade-1.1.0/remoulade/results/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/results/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.075785 remoulade-1.1.0/remoulade/results/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/results/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/results/backends/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/results/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/results/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/results/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/results/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.075785 remoulade-1.1.0/remoulade/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.079785 remoulade-1.1.0/remoulade/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/state/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.079785 remoulade-1.1.0/remoulade/state/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/state/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/state/backends/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/state/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/state/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/state/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/state/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-05-17 07:45:24.000000 remoulade-1.1.0/remoulade/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:45:34.071785 remoulade-1.1.0/remoulade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-17 07:45:33.000000 remoulade-1.1.0/remoulade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-17 07:45:34.000000 remoulade-1.1.0/remoulade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:45:33.000000 remoulade-1.1.0/remoulade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-17 07:45:33.000000 remoulade-1.1.0/remoulade.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-17 07:45:33.000000 remoulade-1.1.0/remoulade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 07:45:33.000000 remoulade-1.1.0/remoulade.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-17 07:45:34.079785 remoulade-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-17 07:45:24.000000 remoulade-1.1.0/setup.py
```

### Comparing `remoulade-1.0.1/COPYING` & `remoulade-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/COPYING.LESSER` & `remoulade-1.1.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/PKG-INFO` & `remoulade-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remoulade
-Version: 1.0.1
+Version: 1.1.0
 Summary: Background Processing for Python 3.
 Author: Wiremind
 Author-email: dev@wiremind.io
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: rabbitmq
 Provides-Extra: redis
 Provides-Extra: server
 Provides-Extra: postgres
+Provides-Extra: pydantic
 Provides-Extra: all
 Provides-Extra: dev
 License-File: COPYING
 License-File: COPYING.LESSER
 
 <img src="https://remoulade.readthedocs.io/en/latest/_static/logo.png" align="right" width="131" />
```

### Comparing `remoulade-1.0.1/README.md` & `remoulade-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/__init__.py` & `remoulade-1.1.0/remoulade/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,8 +86,8 @@
     # Workers
     "Worker",
     # Scheduler
     "get_scheduler",
     "set_scheduler",
 ]
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
```

### Comparing `remoulade-1.0.1/remoulade/__main__.py` & `remoulade-1.1.0/remoulade/__main__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/actor.py` & `remoulade-1.1.0/remoulade/actor.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/api/apispec.py` & `remoulade-1.1.0/remoulade/api/apispec.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/api/main.py` & `remoulade-1.1.0/remoulade/api/main.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/api/scheduler.py` & `remoulade-1.1.0/remoulade/api/scheduler.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/api/state.py` & `remoulade-1.1.0/remoulade/api/state.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/broker.py` & `remoulade-1.1.0/remoulade/broker.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/brokers/__init__.py` & `remoulade-1.1.0/remoulade/brokers/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/brokers/local.py` & `remoulade-1.1.0/remoulade/brokers/local.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/brokers/rabbitmq.py` & `remoulade-1.1.0/remoulade/brokers/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/brokers/stub.py` & `remoulade-1.1.0/remoulade/brokers/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/cancel/__init__.py` & `remoulade-1.1.0/remoulade/cancel/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/cancel/backend.py` & `remoulade-1.1.0/remoulade/cancel/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/cancel/backends/__init__.py` & `remoulade-1.1.0/remoulade/cancel/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/cancel/backends/redis.py` & `remoulade-1.1.0/remoulade/cancel/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/cancel/backends/stub.py` & `remoulade-1.1.0/remoulade/cancel/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/cancel/errors.py` & `remoulade-1.1.0/remoulade/cancel/errors.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/cancel/middleware.py` & `remoulade-1.1.0/remoulade/cancel/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/cli/remoulade_ls.py` & `remoulade-1.1.0/remoulade/cli/remoulade_ls.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/cli/remoulade_run.py` & `remoulade-1.1.0/remoulade/cli/remoulade_run.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/cli/remoulade_scheduler.py` & `remoulade-1.1.0/remoulade/cli/remoulade_scheduler.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/collection_results.py` & `remoulade-1.1.0/remoulade/collection_results.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/common.py` & `remoulade-1.1.0/remoulade/common.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/composition.py` & `remoulade-1.1.0/remoulade/composition.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/errors.py` & `remoulade-1.1.0/remoulade/errors.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/generic.py` & `remoulade-1.1.0/remoulade/generic.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/helpers/__init__.py` & `remoulade-1.1.0/remoulade/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/helpers/actor_arguments.py` & `remoulade-1.1.0/remoulade/helpers/actor_arguments.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/helpers/backoff.py` & `remoulade-1.1.0/remoulade/helpers/backoff.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/helpers/queues.py` & `remoulade-1.1.0/remoulade/helpers/queues.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/helpers/reduce.py` & `remoulade-1.1.0/remoulade/helpers/reduce.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/logging.py` & `remoulade-1.1.0/remoulade/logging.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/message.py` & `remoulade-1.1.0/remoulade/message.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/__init__.py` & `remoulade-1.1.0/remoulade/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/age_limit.py` & `remoulade-1.1.0/remoulade/middleware/age_limit.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/catch_error.py` & `remoulade-1.1.0/remoulade/middleware/catch_error.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/current_message.py` & `remoulade-1.1.0/remoulade/middleware/current_message.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/logging_metadata.py` & `remoulade-1.1.0/remoulade/middleware/logging_metadata.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/max_memory.py` & `remoulade-1.1.0/remoulade/middleware/max_memory.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/max_tasks.py` & `remoulade-1.1.0/remoulade/middleware/max_tasks.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/middleware.py` & `remoulade-1.1.0/remoulade/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/pipelines.py` & `remoulade-1.1.0/remoulade/middleware/pipelines.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/prometheus.py` & `remoulade-1.1.0/remoulade/middleware/prometheus.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/retries.py` & `remoulade-1.1.0/remoulade/middleware/retries.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/shutdown.py` & `remoulade-1.1.0/remoulade/middleware/shutdown.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/threading.py` & `remoulade-1.1.0/remoulade/middleware/threading.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/middleware/time_limit.py` & `remoulade-1.1.0/remoulade/middleware/time_limit.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/rate_limits/__init__.py` & `remoulade-1.1.0/remoulade/rate_limits/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/rate_limits/backend.py` & `remoulade-1.1.0/remoulade/rate_limits/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/rate_limits/backends/__init__.py` & `remoulade-1.1.0/remoulade/rate_limits/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/rate_limits/backends/redis.py` & `remoulade-1.1.0/remoulade/rate_limits/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/rate_limits/backends/stub.py` & `remoulade-1.1.0/remoulade/rate_limits/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/rate_limits/bucket.py` & `remoulade-1.1.0/remoulade/rate_limits/bucket.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/rate_limits/concurrent.py` & `remoulade-1.1.0/remoulade/rate_limits/concurrent.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/rate_limits/rate_limiter.py` & `remoulade-1.1.0/remoulade/rate_limits/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/rate_limits/window.py` & `remoulade-1.1.0/remoulade/rate_limits/window.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/result.py` & `remoulade-1.1.0/remoulade/result.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/results/__init__.py` & `remoulade-1.1.0/remoulade/results/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/results/backend.py` & `remoulade-1.1.0/remoulade/results/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 
 #: Canary value that is returned when a result hasn't been set yet.
 class Missing:
     pass
 
 
 #: A type alias representing backend results.
-class BackendResult(namedtuple("BackendResult", ("result", "error", "forgot"))):
-    def __new__(cls, *, result, error, forgot=False):
-        return super().__new__(cls, result, error, forgot)
+class BackendResult(namedtuple("BackendResult", ("result", "error", "forgot", "actor_name"))):
+    def __new__(cls, *, result, error, forgot=False, actor_name=None):
+        return super().__new__(cls, result, error, forgot, actor_name)
 
     def asdict(self):
         return self._asdict()
 
 
-ForgottenResult = BackendResult(result=None, error=None, forgot=True)
+ForgottenResult = BackendResult(result=None, error=None, forgot=True, actor_name=None)
 
 
 class ResultBackend:
     """ABC for result backends.
 
     Parameters:
       namespace(str): The logical namespace under which the data
```

### Comparing `remoulade-1.0.1/remoulade/results/backends/__init__.py` & `remoulade-1.1.0/remoulade/results/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/results/backends/local.py` & `remoulade-1.1.0/remoulade/results/backends/local.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/results/backends/redis.py` & `remoulade-1.1.0/remoulade/results/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/results/backends/stub.py` & `remoulade-1.1.0/remoulade/results/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/results/errors.py` & `remoulade-1.1.0/remoulade/results/errors.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/results/middleware.py` & `remoulade-1.1.0/remoulade/results/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,24 +78,30 @@
             )
         except:  # noqa
             pipe_on_error = False
 
         results = []
         if store_results:
             if exception is None:
-                results.append((message.message_id, BackendResult(result=result, error=None)))
+                results.append(
+                    (message.message_id, BackendResult(result=result, error=None, actor_name=message.actor_name))
+                )
             elif message_failed:
                 error_str = self._serialize_exception(exception)
-                results.append((message.message_id, BackendResult(result=None, error=error_str)))
+                results.append(
+                    (message.message_id, BackendResult(result=None, error=error_str, actor_name=message.actor_name))
+                )
 
         # even if the actor do not have store_results, we need to invalidate the messages in the pipeline that has it
         if message_failed and not pipe_on_error:
             error_str = self._serialize_exception(exception)
             exception = ParentFailed(f"{message} failed because of {error_str}")
-            children_result = BackendResult(result=None, error=self._serialize_exception(exception))
+            children_result = BackendResult(
+                result=None, error=self._serialize_exception(exception), actor_name=message.actor_name
+            )
 
             for message_id in self._get_children_message_ids(
                 broker, self.get_option("pipe_target", broker=broker, message=message)
             ):
                 results.append((message_id, children_result))
 
         if results:
```

### Comparing `remoulade-1.0.1/remoulade/scheduler/__init__.py` & `remoulade-1.1.0/remoulade/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/scheduler/scheduler.py` & `remoulade-1.1.0/remoulade/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/state/backend.py` & `remoulade-1.1.0/remoulade/state/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/state/backends/__init__.py` & `remoulade-1.1.0/remoulade/state/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/state/backends/postgres.py` & `remoulade-1.1.0/remoulade/state/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/state/backends/redis.py` & `remoulade-1.1.0/remoulade/state/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/state/backends/stub.py` & `remoulade-1.1.0/remoulade/state/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/state/middleware.py` & `remoulade-1.1.0/remoulade/state/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/utils.py` & `remoulade-1.1.0/remoulade/utils.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade/worker.py` & `remoulade-1.1.0/remoulade/worker.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/remoulade.egg-info/PKG-INFO` & `remoulade-1.1.0/remoulade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remoulade
-Version: 1.0.1
+Version: 1.1.0
 Summary: Background Processing for Python 3.
 Author: Wiremind
 Author-email: dev@wiremind.io
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: rabbitmq
 Provides-Extra: redis
 Provides-Extra: server
 Provides-Extra: postgres
+Provides-Extra: pydantic
 Provides-Extra: all
 Provides-Extra: dev
 License-File: COPYING
 License-File: COPYING.LESSER
 
 <img src="https://remoulade.readthedocs.io/en/latest/_static/logo.png" align="right" width="131" />
```

### Comparing `remoulade-1.0.1/remoulade.egg-info/SOURCES.txt` & `remoulade-1.1.0/remoulade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/setup.cfg` & `remoulade-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `remoulade-1.0.1/setup.py` & `remoulade-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 dependencies = ["prometheus-client>=0.2", "pytz", "python-dateutil>=2.8.0", "typing-extensions>=3.7"]
 
 extra_dependencies = {
     "rabbitmq": ["amqpstorm>=2.6,<3"],
     "redis": ["redis~=4.5"],
     "server": ["flask>=1.1,<2.2", "marshmallow>=3", "flask-apispec"],
     "postgres": ["sqlalchemy>=1.4.29,<2", "psycopg2==2.9.5"],
+    "pydantic": ["pydantic<2", "simplejson"]
 }
 
 extra_dependencies["all"] = list(set(sum(extra_dependencies.values(), [])))
 extra_dependencies["dev"] = extra_dependencies["all"] + [
     # Docs
     "alabaster",
     "sphinx==4.1.1",
```

