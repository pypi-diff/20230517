# Comparing `tmp/neo4j-driver-5.8.0.tar.gz` & `tmp/neo4j-driver-5.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4j-driver-5.8.0.tar", last modified: Fri Apr 28 08:06:18 2023, max compression
+gzip compressed data, was "neo4j-driver-5.8.1.tar", last modified: Wed May 17 11:00:20 2023, max compression
```

## Comparing `neo4j-driver-5.8.0.tar` & `neo4j-driver-5.8.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.121752 neo4j-driver-5.8.0/
--rw-r--r--   0 root         (0) root         (0)    11360 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/LICENSE.APACHE2.txt
--rw-r--r--   0 root         (0) root         (0)     2762 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/LICENSE.PYTHON.txt
--rw-r--r--   0 root         (0) root         (0)      423 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      160 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/NOTICE.txt
--rw-r--r--   0 root         (0) root         (0)     6189 2023-04-28 08:06:18.121752 neo4j-driver-5.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5035 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     2912 2023-04-28 08:06:17.000000 neo4j-driver-5.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 08:06:18.121752 neo4j-driver-5.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2442 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.101752 neo4j-driver-5.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.105752 neo4j-driver-5.8.0/src/neo4j/
--rw-r--r--   0 root         (0) root         (0)     4635 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6648 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.109752 neo4j-driver-5.8.0/src/neo4j/_async/
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6561 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/auth_management.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/bookmark_manager.py
--rw-r--r--   0 root         (0) root         (0)    49948 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/driver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.109752 neo4j-driver-5.8.0/src/neo4j/_async/io/
--rw-r--r--   0 root         (0) root         (0)     1220 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35983 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/io/_bolt.py
--rw-r--r--   0 root         (0) root         (0)    16740 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/io/_bolt3.py
--rw-r--r--   0 root         (0) root         (0)    23378 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/io/_bolt4.py
--rw-r--r--   0 root         (0) root         (0)    24676 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/io/_bolt5.py
--rw-r--r--   0 root         (0) root         (0)    10670 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/io/_common.py
--rw-r--r--   0 root         (0) root         (0)    38631 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/io/_pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.109752 neo4j-driver-5.8.0/src/neo4j/_async/work/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/work/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27782 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/work/result.py
--rw-r--r--   0 root         (0) root         (0)    27600 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/work/session.py
--rw-r--r--   0 root         (0) root         (0)    11289 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/work/transaction.py
--rw-r--r--   0 root         (0) root         (0)     7448 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async/work/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.109752 neo4j-driver-5.8.0/src/neo4j/_async_compat/
--rw-r--r--   0 root         (0) root         (0)      755 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async_compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14870 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async_compat/concurrency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.113752 neo4j-driver-5.8.0/src/neo4j/_async_compat/network/
--rw-r--r--   0 root         (0) root         (0)      872 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async_compat/network/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25841 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async_compat/network/_bolt_socket.py
--rw-r--r--   0 root         (0) root         (0)     6223 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async_compat/network/_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.113752 neo4j-driver-5.8.0/src/neo4j/_async_compat/shims/
--rw-r--r--   0 root         (0) root         (0)     4939 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async_compat/shims/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2764 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_async_compat/util.py
--rw-r--r--   0 root         (0) root         (0)     4588 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_auth_management.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.113752 neo4j-driver-5.8.0/src/neo4j/_codec/
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.113752 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/
--rw-r--r--   0 root         (0) root         (0)      898 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4508 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.113752 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/_interface/
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/_interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.113752 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v1/
--rw-r--r--   0 root         (0) root         (0)      731 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7544 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v1/hydration_handler.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v1/spatial.py
--rw-r--r--   0 root         (0) root         (0)     8870 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v1/temporal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.113752 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v2/
--rw-r--r--   0 root         (0) root         (0)      730 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2753 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v2/hydration_handler.py
--rw-r--r--   0 root         (0) root         (0)     5002 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v2/temporal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.113752 neo4j-driver-5.8.0/src/neo4j/_codec/packstream/
--rw-r--r--   0 root         (0) root         (0)      707 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/packstream/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1308 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/packstream/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.113752 neo4j-driver-5.8.0/src/neo4j/_codec/packstream/v1/
--rw-r--r--   0 root         (0) root         (0)    16696 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_codec/packstream/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18295 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_conf.py
--rw-r--r--   0 root         (0) root         (0)    11673 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_data.py
--rw-r--r--   0 root         (0) root         (0)     2968 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_deadline.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5048 2023-04-28 08:06:16.000000 neo4j-driver-5.8.0/src/neo4j/_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.113752 neo4j-driver-5.8.0/src/neo4j/_optional_deps/
--rw-r--r--   0 root         (0) root         (0)      261 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_optional_deps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5907 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.113752 neo4j-driver-5.8.0/src/neo4j/_spatial/
--rw-r--r--   0 root         (0) root         (0)     3871 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_spatial/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.117752 neo4j-driver-5.8.0/src/neo4j/_sync/
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6377 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/auth_management.py
--rw-r--r--   0 root         (0) root         (0)     2779 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/bookmark_manager.py
--rw-r--r--   0 root         (0) root         (0)    49052 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/driver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.117752 neo4j-driver-5.8.0/src/neo4j/_sync/io/
--rw-r--r--   0 root         (0) root         (0)     1190 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35506 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/io/_bolt.py
--rw-r--r--   0 root         (0) root         (0)    16631 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/io/_bolt3.py
--rw-r--r--   0 root         (0) root         (0)    23173 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/io/_bolt4.py
--rw-r--r--   0 root         (0) root         (0)    24509 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/io/_bolt5.py
--rw-r--r--   0 root         (0) root         (0)    10393 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/io/_common.py
--rw-r--r--   0 root         (0) root         (0)    37987 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/io/_pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.117752 neo4j-driver-5.8.0/src/neo4j/_sync/work/
--rw-r--r--   0 root         (0) root         (0)      988 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/work/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27291 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/work/result.py
--rw-r--r--   0 root         (0) root         (0)    26864 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/work/session.py
--rw-r--r--   0 root         (0) root         (0)    10873 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/work/transaction.py
--rw-r--r--   0 root         (0) root         (0)     7268 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_sync/work/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.117752 neo4j-driver-5.8.0/src/neo4j/_work/
--rw-r--r--   0 root         (0) root         (0)     1030 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_work/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_work/eager_result.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_work/query.py
--rw-r--r--   0 root         (0) root         (0)    10365 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/_work/summary.py
--rw-r--r--   0 root         (0) root         (0)    10985 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/addressing.py
--rw-r--r--   0 root         (0) root         (0)    18240 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/api.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/auth_management.py
--rw-r--r--   0 root         (0) root         (0)     1330 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/conf.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/data.py
--rw-r--r--   0 root         (0) root         (0)     7802 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/debug.py
--rw-r--r--   0 root         (0) root         (0)    17262 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.117752 neo4j-driver-5.8.0/src/neo4j/graph/
--rw-r--r--   0 root         (0) root         (0)    11098 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/meta.py
--rw-r--r--   0 root         (0) root         (0)     1300 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/packstream.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/py.typed
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.117752 neo4j-driver-5.8.0/src/neo4j/spatial/
--rw-r--r--   0 root         (0) root         (0)     2081 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/spatial/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.121752 neo4j-driver-5.8.0/src/neo4j/time/
--rw-r--r--   0 root         (0) root         (0)    94998 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/time/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/time/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/time/_arithmetic.py
--rw-r--r--   0 root         (0) root         (0)     2871 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/time/_clock_implementations.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/time/_metaclasses.py
--rw-r--r--   0 root         (0) root         (0)     1118 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/time/arithmetic.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/time/clock_implementations.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/time/hydration.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/time/metaclasses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.121752 neo4j-driver-5.8.0/src/neo4j/work/
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/work/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1051 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/work/query.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-04-28 08:04:47.000000 neo4j-driver-5.8.0/src/neo4j/work/summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:06:18.121752 neo4j-driver-5.8.0/src/neo4j_driver.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6189 2023-04-28 08:06:18.000000 neo4j-driver-5.8.0/src/neo4j_driver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3210 2023-04-28 08:06:18.000000 neo4j-driver-5.8.0/src/neo4j_driver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 08:06:18.000000 neo4j-driver-5.8.0/src/neo4j_driver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-28 08:06:18.000000 neo4j-driver-5.8.0/src/neo4j_driver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-28 08:06:18.000000 neo4j-driver-5.8.0/src/neo4j_driver.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.678403 neo4j-driver-5.8.1/
+-rw-r--r--   0 root         (0) root         (0)    11360 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/LICENSE.APACHE2.txt
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/LICENSE.PYTHON.txt
+-rw-r--r--   0 root         (0) root         (0)      423 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/NOTICE.txt
+-rw-r--r--   0 root         (0) root         (0)     6189 2023-05-17 11:00:20.678403 neo4j-driver-5.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5035 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-05-17 11:00:20.000000 neo4j-driver-5.8.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 11:00:20.678403 neo4j-driver-5.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2442 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.662403 neo4j-driver-5.8.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.666403 neo4j-driver-5.8.1/src/neo4j/
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6648 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.666403 neo4j-driver-5.8.1/src/neo4j/_async/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6561 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/auth_management.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/bookmark_manager.py
+-rw-r--r--   0 root         (0) root         (0)    50031 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/driver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.666403 neo4j-driver-5.8.1/src/neo4j/_async/io/
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35983 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/io/_bolt.py
+-rw-r--r--   0 root         (0) root         (0)    16740 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/io/_bolt3.py
+-rw-r--r--   0 root         (0) root         (0)    23378 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/io/_bolt4.py
+-rw-r--r--   0 root         (0) root         (0)    24676 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/io/_bolt5.py
+-rw-r--r--   0 root         (0) root         (0)    10670 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/io/_common.py
+-rw-r--r--   0 root         (0) root         (0)    38631 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/io/_pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.670403 neo4j-driver-5.8.1/src/neo4j/_async/work/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/work/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27782 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/work/result.py
+-rw-r--r--   0 root         (0) root         (0)    27600 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/work/session.py
+-rw-r--r--   0 root         (0) root         (0)    11289 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/work/transaction.py
+-rw-r--r--   0 root         (0) root         (0)     7448 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async/work/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.670403 neo4j-driver-5.8.1/src/neo4j/_async_compat/
+-rw-r--r--   0 root         (0) root         (0)      755 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async_compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14870 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async_compat/concurrency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.670403 neo4j-driver-5.8.1/src/neo4j/_async_compat/network/
+-rw-r--r--   0 root         (0) root         (0)      872 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async_compat/network/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25841 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async_compat/network/_bolt_socket.py
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async_compat/network/_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.670403 neo4j-driver-5.8.1/src/neo4j/_async_compat/shims/
+-rw-r--r--   0 root         (0) root         (0)     4939 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async_compat/shims/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_async_compat/util.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_auth_management.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.670403 neo4j-driver-5.8.1/src/neo4j/_codec/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.670403 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/
+-rw-r--r--   0 root         (0) root         (0)      898 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4508 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.670403 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/_interface/
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/_interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.670403 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v1/
+-rw-r--r--   0 root         (0) root         (0)      731 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7544 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v1/hydration_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v1/spatial.py
+-rw-r--r--   0 root         (0) root         (0)     8870 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v1/temporal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.670403 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v2/
+-rw-r--r--   0 root         (0) root         (0)      730 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v2/hydration_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5002 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v2/temporal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.670403 neo4j-driver-5.8.1/src/neo4j/_codec/packstream/
+-rw-r--r--   0 root         (0) root         (0)      707 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/packstream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/packstream/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.670403 neo4j-driver-5.8.1/src/neo4j/_codec/packstream/v1/
+-rw-r--r--   0 root         (0) root         (0)    16696 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_codec/packstream/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18295 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_conf.py
+-rw-r--r--   0 root         (0) root         (0)    11673 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_data.py
+-rw-r--r--   0 root         (0) root         (0)     2968 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_deadline.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5545 2023-05-17 11:00:19.000000 neo4j-driver-5.8.1/src/neo4j/_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.670403 neo4j-driver-5.8.1/src/neo4j/_optional_deps/
+-rw-r--r--   0 root         (0) root         (0)      261 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_optional_deps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5907 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.674403 neo4j-driver-5.8.1/src/neo4j/_spatial/
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_spatial/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.674403 neo4j-driver-5.8.1/src/neo4j/_sync/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6377 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/auth_management.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/bookmark_manager.py
+-rw-r--r--   0 root         (0) root         (0)    49135 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/driver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.674403 neo4j-driver-5.8.1/src/neo4j/_sync/io/
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35506 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/io/_bolt.py
+-rw-r--r--   0 root         (0) root         (0)    16631 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/io/_bolt3.py
+-rw-r--r--   0 root         (0) root         (0)    23173 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/io/_bolt4.py
+-rw-r--r--   0 root         (0) root         (0)    24509 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/io/_bolt5.py
+-rw-r--r--   0 root         (0) root         (0)    10393 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/io/_common.py
+-rw-r--r--   0 root         (0) root         (0)    37987 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/io/_pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.674403 neo4j-driver-5.8.1/src/neo4j/_sync/work/
+-rw-r--r--   0 root         (0) root         (0)      988 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/work/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27291 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/work/result.py
+-rw-r--r--   0 root         (0) root         (0)    26864 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/work/session.py
+-rw-r--r--   0 root         (0) root         (0)    10873 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/work/transaction.py
+-rw-r--r--   0 root         (0) root         (0)     7268 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_sync/work/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.674403 neo4j-driver-5.8.1/src/neo4j/_work/
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_work/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_work/eager_result.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_work/query.py
+-rw-r--r--   0 root         (0) root         (0)    10365 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/_work/summary.py
+-rw-r--r--   0 root         (0) root         (0)    10985 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/addressing.py
+-rw-r--r--   0 root         (0) root         (0)    18240 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/api.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/auth_management.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/data.py
+-rw-r--r--   0 root         (0) root         (0)     7802 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/debug.py
+-rw-r--r--   0 root         (0) root         (0)    17262 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.674403 neo4j-driver-5.8.1/src/neo4j/graph/
+-rw-r--r--   0 root         (0) root         (0)    11098 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/meta.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/packstream.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.678403 neo4j-driver-5.8.1/src/neo4j/spatial/
+-rw-r--r--   0 root         (0) root         (0)     2081 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/spatial/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.678403 neo4j-driver-5.8.1/src/neo4j/time/
+-rw-r--r--   0 root         (0) root         (0)    95454 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/time/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/time/_arithmetic.py
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/time/_clock_implementations.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/time/_metaclasses.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/time/arithmetic.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/time/clock_implementations.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/time/hydration.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/time/metaclasses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.678403 neo4j-driver-5.8.1/src/neo4j/work/
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/work/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/work/query.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-17 10:59:04.000000 neo4j-driver-5.8.1/src/neo4j/work/summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:00:20.678403 neo4j-driver-5.8.1/src/neo4j_driver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6189 2023-05-17 11:00:20.000000 neo4j-driver-5.8.1/src/neo4j_driver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3210 2023-05-17 11:00:20.000000 neo4j-driver-5.8.1/src/neo4j_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 11:00:20.000000 neo4j-driver-5.8.1/src/neo4j_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-17 11:00:20.000000 neo4j-driver-5.8.1/src/neo4j_driver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-17 11:00:20.000000 neo4j-driver-5.8.1/src/neo4j_driver.egg-info/top_level.txt
```

### Comparing `neo4j-driver-5.8.0/LICENSE.APACHE2.txt` & `neo4j-driver-5.8.1/LICENSE.APACHE2.txt`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/LICENSE.PYTHON.txt` & `neo4j-driver-5.8.1/LICENSE.PYTHON.txt`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/PKG-INFO` & `neo4j-driver-5.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4j-driver
-Version: 5.8.0
+Version: 5.8.1
 Summary: Neo4j Bolt driver for Python
 Author-email: "Neo4j, Inc." <drivers@neo4j.com>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/neo4j/neo4j-python-driver
 Keywords: neo4j,graph,database
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `neo4j-driver-5.8.0/README.rst` & `neo4j-driver-5.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/pyproject.toml` & `neo4j-driver-5.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/setup.py` & `neo4j-driver-5.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_api.py` & `neo4j-driver-5.8.1/src/neo4j/_api.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/auth_management.py` & `neo4j-driver-5.8.1/src/neo4j/_async/auth_management.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/bookmark_manager.py` & `neo4j-driver-5.8.1/src/neo4j/_async/bookmark_manager.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/driver.py` & `neo4j-driver-5.8.1/src/neo4j/_async/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,17 +404,17 @@
         except (BoltHandshakeError, BoltSecurityError) as error:
             from ..exceptions import ServiceUnavailable
             raise ServiceUnavailable(str(error)) from error
 
 
 class _Direct:
 
+    # TODO: 6.0 - those attributes should be private
     default_host = "localhost"
     default_port = 7687
-
     default_target = ":"
 
     def __init__(self, address):
         self._address = address
 
     @property
     def address(self):
@@ -429,17 +429,17 @@
         address = Address.parse(target, default_host=cls.default_host,
                                 default_port=cls.default_port)
         return address
 
 
 class _Routing:
 
+    # TODO: 6.0 - those attributes should be private
     default_host = "localhost"
     default_port = 7687
-
     default_targets = ": :17601 :17687"
 
     def __init__(self, initial_addresses):
         self._initial_addresses = initial_addresses
 
     @property
     def initial_addresses(self):
@@ -801,20 +801,19 @@
             typing.Callable[[neo4j.AsyncResult], typing.Awaitable[T]]
         :param bookmark_manager_:
             Specify a bookmark manager to use.
 
             If present, the bookmark manager is used to keep the query causally
             consistent with all work executed using the same bookmark manager.
 
-            Defaults to the driver's :attr:`.query_bookmark_manager`.
+            Defaults to the driver's :attr:`.execute_query_bookmark_manager`.
 
             Pass :data:`None` to disable causal consistency.
         :type bookmark_manager_:
-            typing.Union[neo4j.AsyncBookmarkManager, neo4j.BookmarkManager,
-                         None]
+            typing.Union[AsyncBookmarkManager, BookmarkManager, None]
         :param kwargs: additional keyword parameters. None of these can end
             with a single underscore. This is to avoid collisions with the
             keyword configuration parameters of this method. If you need to
             pass such a parameter, use the ``parameters_`` parameter instead.
             Parameters passed as kwargs take precedence over those passed in
             ``parameters_``.
         :type kwargs: typing.Any
@@ -871,15 +870,15 @@
         This is the default :class:`AsyncBookmarkManager` used by
         :meth:`.execute_query`. This can be used to causally chain
         :meth:`.execute_query` calls and sessions. Example::
 
             async def example(driver: neo4j.AsyncDriver) -> None:
                 await driver.execute_query("<QUERY 1>")
                 async with driver.session(
-                    bookmark_manager=driver.query_bookmark_manager
+                    bookmark_manager=driver.execute_query_bookmark_manager
                 ) as session:
                     # every query inside this session will be causally chained
                     # (i.e., can read what was written by <QUERY 1>)
                     await session.run("<QUERY 2>")
                 # subsequent execute_query calls will be causally chained
                 # (i.e., can read what was written by <QUERY 2>)
                 await driver.execute_query("<QUERY 3>")
```

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/io/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_async/io/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/io/_bolt.py` & `neo4j-driver-5.8.1/src/neo4j/_async/io/_bolt.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/io/_bolt3.py` & `neo4j-driver-5.8.1/src/neo4j/_async/io/_bolt3.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/io/_bolt4.py` & `neo4j-driver-5.8.1/src/neo4j/_async/io/_bolt4.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/io/_bolt5.py` & `neo4j-driver-5.8.1/src/neo4j/_async/io/_bolt5.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/io/_common.py` & `neo4j-driver-5.8.1/src/neo4j/_async/io/_common.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/io/_pool.py` & `neo4j-driver-5.8.1/src/neo4j/_async/io/_pool.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/work/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_async/work/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/work/result.py` & `neo4j-driver-5.8.1/src/neo4j/_async/work/result.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/work/session.py` & `neo4j-driver-5.8.1/src/neo4j/_async/work/session.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/work/transaction.py` & `neo4j-driver-5.8.1/src/neo4j/_async/work/transaction.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async/work/workspace.py` & `neo4j-driver-5.8.1/src/neo4j/_async/work/workspace.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async_compat/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_async_compat/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async_compat/concurrency.py` & `neo4j-driver-5.8.1/src/neo4j/_async_compat/concurrency.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async_compat/network/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_async_compat/network/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async_compat/network/_bolt_socket.py` & `neo4j-driver-5.8.1/src/neo4j/_async_compat/network/_bolt_socket.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async_compat/network/_util.py` & `neo4j-driver-5.8.1/src/neo4j/_async_compat/network/_util.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async_compat/shims/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_async_compat/shims/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_async_compat/util.py` & `neo4j-driver-5.8.1/src/neo4j/_async_compat/util.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_auth_management.py` & `neo4j-driver-5.8.1/src/neo4j/_auth_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,28 +30,29 @@
 
 
 @preview("Auth managers are a preview feature.")
 @dataclass
 class ExpiringAuth:
     """Represents potentially expiring authentication information.
 
-    This class is used with :meth:`.AuthManagers.temporal` and
-    :meth:`.AsyncAuthManagers.temporal`.
+    This class is used with :meth:`.AuthManagers.expiration_based` and
+    :meth:`.AsyncAuthManagers.expiration_based`.
 
     :param auth: The authentication information.
     :param expires_in: The number of seconds until the authentication
         information expires. If :data:`None`, the authentication information
         is considered to not expire until the server explicitly indicates so.
 
     **This is a preview** (see :ref:`filter-warnings-ref`).
     It might be changed without following the deprecation policy.
     See also https://github.com/neo4j/neo4j-python-driver/wiki/preview-features
 
     .. seealso::
-        :meth:`.AuthManagers.temporal`, :meth:`.AsyncAuthManagers.temporal`
+        :meth:`.AuthManagers.expiration_based`,
+        :meth:`.AsyncAuthManagers.expiration_based`
 
     .. versionadded:: 5.8
     """
     auth: _TAuth
     expires_in: t.Optional[float] = None
```

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/hydration/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/hydration/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/hydration/_common.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/hydration/_common.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/hydration/_interface/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/hydration/_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v1/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v1/hydration_handler.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v1/hydration_handler.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v1/spatial.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v1/spatial.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v1/temporal.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v1/temporal.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v2/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v2/hydration_handler.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v2/hydration_handler.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/hydration/v2/temporal.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/hydration/v2/temporal.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/packstream/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/packstream/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/packstream/_common.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/packstream/_common.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_codec/packstream/v1/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_codec/packstream/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_conf.py` & `neo4j-driver-5.8.1/src/neo4j/_conf.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_data.py` & `neo4j-driver-5.8.1/src/neo4j/_data.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_deadline.py` & `neo4j-driver-5.8.1/src/neo4j/_deadline.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_exceptions.py` & `neo4j-driver-5.8.1/src/neo4j/_exceptions.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_meta.py` & `neo4j-driver-5.8.1/src/neo4j/_meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,27 +12,30 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+from __future__ import annotations
+
 import asyncio
 import tracemalloc
 import typing as t
 from functools import wraps
+from inspect import isclass
 from warnings import warn
 
 
 _FuncT = t.TypeVar("_FuncT", bound=t.Callable)
 
 
 # Can be automatically overridden in builds
 package = "neo4j-driver"
-version = "5.8.0"
+version = "5.8.1"
 deprecated_package = True
 
 
 def get_user_agent():
     """ Obtain the default user agent string sent to the server after
     a successful handshake.
     """
@@ -63,31 +66,15 @@
     ::
 
         @deprecated("'foo' has been deprecated in favour of 'bar'")
         def foo(x):
             pass
 
     """
-    def decorator(f):
-        if asyncio.iscoroutinefunction(f):
-            @wraps(f)
-            async def inner(*args, **kwargs):
-                deprecation_warn(message, stack_level=2)
-                return await f(*args, **kwargs)
-
-            return inner
-        else:
-            @wraps(f)
-            def inner(*args, **kwargs):
-                deprecation_warn(message, stack_level=2)
-                return f(*args, **kwargs)
-
-            return inner
-
-    return decorator
+    return _make_warning_decorator(message, deprecation_warn)
 
 
 def deprecated_property(message: str):
     def decorator(f):
         return property(deprecated(message)(f))
     return t.cast(property, decorator)
 
@@ -100,28 +87,14 @@
     """
 
 
 def experimental_warn(message, stack_level=1):
     warn(message, category=ExperimentalWarning, stacklevel=stack_level + 1)
 
 
-class PreviewWarning(Warning):
-    """ Base class for warnings about experimental features.
-    """
-
-
-def preview_warn(message, stack_level=1):
-    message += (
-        " It might be changed without following the deprecation policy. "
-        "See also "
-        "https://github.com/neo4j/neo4j-python-driver/wiki/preview-features."
-    )
-    warn(message, category=PreviewWarning, stacklevel=stack_level + 1)
-
-
 def experimental(message) -> t.Callable[[_FuncT], _FuncT]:
     """ Decorator for tagging experimental functions and methods.
 
     ::
 
         @experimental("'foo' is an experimental function and may be "
                       "removed in a future release")
@@ -143,37 +116,80 @@
             @wraps(f)
             def inner(*args, **kwargs):
                 experimental_warn(message, stack_level=2)
                 return f(*args, **kwargs)
 
             return inner
 
-    return decorator
+    return _make_warning_decorator(message, experimental_warn)
+
+
+class PreviewWarning(Warning):
+    """ Base class for warnings about experimental features.
+    """
+
+
+def preview_warn(message, stack_level=1):
+    message += (
+        " It might be changed without following the deprecation policy. "
+        "See also "
+        "https://github.com/neo4j/neo4j-python-driver/wiki/preview-features."
+    )
+    warn(message, category=PreviewWarning, stacklevel=stack_level + 1)
 
 
 def preview(message) -> t.Callable[[_FuncT], _FuncT]:
     """
     Decorator for tagging preview functions and methods.
 
         @preview("foo is a preview.")
         def foo(x):
             pass
     """
+
+    return _make_warning_decorator(message, preview_warn)
+
+
+if t.TYPE_CHECKING:
+    class _WarningFunc(t.Protocol):
+        def __call__(self, message: str, stack_level: int = 1) -> None:
+            ...
+else:
+    _WarningFunc = object
+
+
+def _make_warning_decorator(
+    message: str,
+    warning_func: _WarningFunc,
+) -> t.Callable[[_FuncT], _FuncT]:
     def decorator(f):
         if asyncio.iscoroutinefunction(f):
             @wraps(f)
             async def inner(*args, **kwargs):
-                preview_warn(message, stack_level=2)
+                warning_func(message, stack_level=2)
                 return await f(*args, **kwargs)
 
             return inner
+        if isclass(f):
+            if hasattr(f, "__init__"):
+                original_init = f.__init__
+                @wraps(original_init)
+                def inner(*args, **kwargs):
+                    warning_func(message, stack_level=2)
+                    return original_init(*args, **kwargs)
+
+                f.__init__ = inner
+                return f
+            raise TypeError(
+                "Cannot decorate class without __init__"
+            )
         else:
             @wraps(f)
             def inner(*args, **kwargs):
-                preview_warn(message, stack_level=2)
+                warning_func(message, stack_level=2)
                 return f(*args, **kwargs)
 
             return inner
 
     return decorator
```

### Comparing `neo4j-driver-5.8.0/src/neo4j/_routing.py` & `neo4j-driver-5.8.1/src/neo4j/_routing.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_spatial/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/auth_management.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/auth_management.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/bookmark_manager.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/bookmark_manager.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/driver.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,17 +403,17 @@
         except (BoltHandshakeError, BoltSecurityError) as error:
             from ..exceptions import ServiceUnavailable
             raise ServiceUnavailable(str(error)) from error
 
 
 class _Direct:
 
+    # TODO: 6.0 - those attributes should be private
     default_host = "localhost"
     default_port = 7687
-
     default_target = ":"
 
     def __init__(self, address):
         self._address = address
 
     @property
     def address(self):
@@ -428,17 +428,17 @@
         address = Address.parse(target, default_host=cls.default_host,
                                 default_port=cls.default_port)
         return address
 
 
 class _Routing:
 
+    # TODO: 6.0 - those attributes should be private
     default_host = "localhost"
     default_port = 7687
-
     default_targets = ": :17601 :17687"
 
     def __init__(self, initial_addresses):
         self._initial_addresses = initial_addresses
 
     @property
     def initial_addresses(self):
@@ -800,20 +800,19 @@
             typing.Callable[[neo4j.Result], typing.Union[T]]
         :param bookmark_manager_:
             Specify a bookmark manager to use.
 
             If present, the bookmark manager is used to keep the query causally
             consistent with all work executed using the same bookmark manager.
 
-            Defaults to the driver's :attr:`.query_bookmark_manager`.
+            Defaults to the driver's :attr:`.execute_query_bookmark_manager`.
 
             Pass :data:`None` to disable causal consistency.
         :type bookmark_manager_:
-            typing.Union[neo4j.BookmarkManager, neo4j.BookmarkManager,
-                         None]
+            typing.Union[BookmarkManager, BookmarkManager, None]
         :param kwargs: additional keyword parameters. None of these can end
             with a single underscore. This is to avoid collisions with the
             keyword configuration parameters of this method. If you need to
             pass such a parameter, use the ``parameters_`` parameter instead.
             Parameters passed as kwargs take precedence over those passed in
             ``parameters_``.
         :type kwargs: typing.Any
@@ -870,15 +869,15 @@
         This is the default :class:`BookmarkManager` used by
         :meth:`.execute_query`. This can be used to causally chain
         :meth:`.execute_query` calls and sessions. Example::
 
             def example(driver: neo4j.Driver) -> None:
                 driver.execute_query("<QUERY 1>")
                 with driver.session(
-                    bookmark_manager=driver.query_bookmark_manager
+                    bookmark_manager=driver.execute_query_bookmark_manager
                 ) as session:
                     # every query inside this session will be causally chained
                     # (i.e., can read what was written by <QUERY 1>)
                     session.run("<QUERY 2>")
                 # subsequent execute_query calls will be causally chained
                 # (i.e., can read what was written by <QUERY 2>)
                 driver.execute_query("<QUERY 3>")
```

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/io/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/io/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/io/_bolt.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/io/_bolt.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/io/_bolt3.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/io/_bolt3.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/io/_bolt4.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/io/_bolt4.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/io/_bolt5.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/io/_bolt5.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/io/_common.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/io/_common.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/io/_pool.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/io/_pool.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/work/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/work/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/work/result.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/work/result.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/work/session.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/work/session.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/work/transaction.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/work/transaction.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_sync/work/workspace.py` & `neo4j-driver-5.8.1/src/neo4j/_sync/work/workspace.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_work/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/_work/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_work/eager_result.py` & `neo4j-driver-5.8.1/src/neo4j/_work/eager_result.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_work/query.py` & `neo4j-driver-5.8.1/src/neo4j/_work/query.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/_work/summary.py` & `neo4j-driver-5.8.1/src/neo4j/_work/summary.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/addressing.py` & `neo4j-driver-5.8.1/src/neo4j/addressing.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/api.py` & `neo4j-driver-5.8.1/src/neo4j/api.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/auth_management.py` & `neo4j-driver-5.8.1/src/neo4j/auth_management.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/conf.py` & `neo4j-driver-5.8.1/src/neo4j/conf.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/data.py` & `neo4j-driver-5.8.1/src/neo4j/data.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/debug.py` & `neo4j-driver-5.8.1/src/neo4j/debug.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/exceptions.py` & `neo4j-driver-5.8.1/src/neo4j/exceptions.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/graph/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/meta.py` & `neo4j-driver-5.8.1/src/neo4j/meta.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/packstream.py` & `neo4j-driver-5.8.1/src/neo4j/packstream.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/routing.py` & `neo4j-driver-5.8.1/src/neo4j/routing.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/spatial/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/time/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/time/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 as a number of utility functions.
 """
 
 
 from __future__ import annotations
 
 import re
+import typing
 import typing as t
 from datetime import (
     date,
     datetime,
     time,
     timedelta,
     timezone,
@@ -1228,37 +1229,37 @@
 
     # INSTANCE METHODS #
 
     if t.TYPE_CHECKING:
 
         def replace(
             self,
-            year: int = ...,
-            month: int = ...,
-            day: int = ...,
+            year: te.SupportsIndex = ...,
+            month: te.SupportsIndex = ...,
+            day: te.SupportsIndex = ...,
             **kwargs: object
         ) -> Date:
             ...
 
     else:
 
         def replace(self, **kwargs) -> Date:
             """Return a :class:`.Date` with one or more components replaced.
 
             :Keyword Arguments:
-               * **year** (`int`): overwrite the year -
-                 default: `self.year`
-               * **month** (`int`): overwrite the month -
-                 default: `self.month`
-               * **day** (`int`): overwrite the day -
-                 default: `self.day`
+               * **year** (:class:`typing.SupportsIndex`):
+                 overwrite the year - default: `self.year`
+               * **month** (:class:`typing.SupportsIndex`):
+                 overwrite the month - default: `self.month`
+               * **day** (:class:`typing.SupportsIndex`):
+                 overwrite the day - default: `self.day`
             """
-            return Date(kwargs.get("year", self.__year),
-                        kwargs.get("month", self.__month),
-                        kwargs.get("day", self.__day))
+            return Date(int(kwargs.get("year", self.__year)),
+                        int(kwargs.get("month", self.__month)),
+                        int(kwargs.get("day", self.__day)))
 
     def time_tuple(self) -> struct_time:
         """Convert the date to :class:`time.struct_time`."""
         _, _, day_of_week = self.year_week_day
         _, day_of_year = self.year_day
         return struct_time((self.year, self.month, self.day, 0, 0, 0, day_of_week - 1, day_of_year, -1))
 
@@ -1762,44 +1763,45 @@
 
     # INSTANCE METHODS #
 
     if t.TYPE_CHECKING:
 
         def replace(  # type: ignore[override]
             self,
-            hour: int = ...,
-            minute: int = ...,
-            second: int = ...,
-            nanosecond: int = ...,
+            hour: te.SupportsIndex = ...,
+            minute: te.SupportsIndex = ...,
+            second: te.SupportsIndex = ...,
+            nanosecond: te.SupportsIndex = ...,
             tzinfo: t.Optional[_tzinfo] = ...,
             **kwargs: object
         ) -> Time:
             ...
 
     else:
 
         def replace(self, **kwargs) -> Time:
             """Return a :class:`.Time` with one or more components replaced.
 
             :Keyword Arguments:
-               * **hour** (`int`): overwrite the hour -
-                 default: `self.hour`
-               * **minute** (`int`): overwrite the minute -
-                 default: `self.minute`
-               * **second** (`int`): overwrite the second -
-                 default: `int(self.second)`
-               * **nanosecond** (`int`): overwrite the nanosecond -
-                 default: `self.nanosecond`
-               * **tzinfo** (`datetime.tzinfo` or `None`):
+               * **hour** (:class:`typing.SupportsIndex`):
+                 overwrite the hour - default: `self.hour`
+               * **minute** (:class:`typing.SupportsIndex`):
+                 overwrite the minute - default: `self.minute`
+               * **second** (:class:`typing.SupportsIndex`):
+                 overwrite the second - default: `int(self.second)`
+               * **nanosecond** (:class:`typing.SupportsIndex`):
+                 overwrite the nanosecond - default: `self.nanosecond`
+               * **tzinfo** (:class:`datetime.tzinfo` or `None`):
                  overwrite the timezone - default: `self.tzinfo`
             """
-            return Time(hour=kwargs.get("hour", self.__hour),
-                        minute=kwargs.get("minute", self.__minute),
-                        second=kwargs.get("second", self.__second),
-                        nanosecond=kwargs.get("nanosecond", self.__nanosecond),
+            return Time(hour=int(kwargs.get("hour", self.__hour)),
+                        minute=int(kwargs.get("minute", self.__minute)),
+                        second=int(kwargs.get("second", self.__second)),
+                        nanosecond=int(kwargs.get("nanosecond",
+                                                  self.__nanosecond)),
                         tzinfo=kwargs.get("tzinfo", self.__tzinfo))
 
     def _utc_offset(self, dt=None):
         if self.tzinfo is None:
             return None
         try:
             value = self.tzinfo.utcoffset(dt)
@@ -2512,21 +2514,21 @@
         """The time with timezone info."""
         return self.__time
 
     if t.TYPE_CHECKING:
 
         def replace(  # type: ignore[override]
             self,
-            year: int = ...,
-            month: int = ...,
-            day: int = ...,
-            hour: int = ...,
-            minute: int = ...,
-            second: int = ...,
-            nanosecond: int = ...,
+            year: te.SupportsIndex = ...,
+            month: te.SupportsIndex = ...,
+            day: te.SupportsIndex = ...,
+            hour: te.SupportsIndex = ...,
+            minute: te.SupportsIndex = ...,
+            second: te.SupportsIndex = ...,
+            nanosecond: te.SupportsIndex = ...,
             tzinfo: t.Optional[_tzinfo] = ...,
             **kwargs: object
         ) -> DateTime:
             ...
 
     else:
```

### Comparing `neo4j-driver-5.8.0/src/neo4j/time/__main__.py` & `neo4j-driver-5.8.1/src/neo4j/time/__main__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/time/_arithmetic.py` & `neo4j-driver-5.8.1/src/neo4j/time/_arithmetic.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/time/_clock_implementations.py` & `neo4j-driver-5.8.1/src/neo4j/time/_clock_implementations.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/time/_metaclasses.py` & `neo4j-driver-5.8.1/src/neo4j/time/_metaclasses.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/time/arithmetic.py` & `neo4j-driver-5.8.1/src/neo4j/time/arithmetic.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/time/clock_implementations.py` & `neo4j-driver-5.8.1/src/neo4j/time/clock_implementations.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/time/hydration.py` & `neo4j-driver-5.8.1/src/neo4j/time/hydration.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/time/metaclasses.py` & `neo4j-driver-5.8.1/src/neo4j/time/metaclasses.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/work/__init__.py` & `neo4j-driver-5.8.1/src/neo4j/work/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/work/query.py` & `neo4j-driver-5.8.1/src/neo4j/work/query.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j/work/summary.py` & `neo4j-driver-5.8.1/src/neo4j/work/summary.py`

 * *Files identical despite different names*

### Comparing `neo4j-driver-5.8.0/src/neo4j_driver.egg-info/PKG-INFO` & `neo4j-driver-5.8.1/src/neo4j_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4j-driver
-Version: 5.8.0
+Version: 5.8.1
 Summary: Neo4j Bolt driver for Python
 Author-email: "Neo4j, Inc." <drivers@neo4j.com>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/neo4j/neo4j-python-driver
 Keywords: neo4j,graph,database
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `neo4j-driver-5.8.0/src/neo4j_driver.egg-info/SOURCES.txt` & `neo4j-driver-5.8.1/src/neo4j_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

