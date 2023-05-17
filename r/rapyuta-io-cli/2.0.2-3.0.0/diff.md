# Comparing `tmp/rapyuta-io-cli-2.0.2.tar.gz` & `tmp/rapyuta-io-cli-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapyuta-io-cli-2.0.2.tar", last modified: Thu Apr 20 12:39:59 2023, max compression
+gzip compressed data, was "rapyuta-io-cli-3.0.0.tar", last modified: Wed May 17 13:12:46 2023, max compression
```

## Comparing `rapyuta-io-cli-2.0.2.tar` & `rapyuta-io-cli-3.0.0.tar`

### file list

```diff
@@ -1,200 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.608095 rapyuta-io-cli-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-04-20 12:39:59.608095 rapyuta-io-cli-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.572095 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-04-20 12:39:59.000000 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4398 2023-04-20 12:39:59.000000 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 12:39:59.000000 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-20 12:39:59.000000 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-04-20 12:39:59.000000 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-20 12:39:59.000000 rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.572095 rapyuta-io-cli-2.0.2/riocli/
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.576094 rapyuta-io-cli-2.0.2/riocli/apply/
--rw-r--r--   0 runner    (1001) docker     (122)     3798 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1446 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/apply/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)    15225 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/apply/parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/apply/resolver.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/apply/template.py
--rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/apply/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.576094 rapyuta-io-cli-2.0.2/riocli/auth/
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/logout.py
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/staging.py
--rw-r--r--   0 runner    (1001) docker     (122)      911 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/token.py
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/auth/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.580095 rapyuta-io-cli-2.0.2/riocli/build/
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/import_build.py
--rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/trigger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/build/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.580095 rapyuta-io-cli-2.0.2/riocli/chart/
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     3182 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/search.py
--rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/chart/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.580095 rapyuta-io-cli-2.0.2/riocli/completion/
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/completion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.580095 rapyuta-io-cli-2.0.2/riocli/config/
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.584095 rapyuta-io-cli-2.0.2/riocli/deployment/
--rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2820 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)    14705 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/model.py
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/deployment/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.588095 rapyuta-io-cli-2.0.2/riocli/device/
--rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     6340 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     4083 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/label.py
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3301 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/metric.py
--rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/onboard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.588095 rapyuta-io-cli-2.0.2/riocli/device/tools/
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/device_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/forward.py
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/rapyuta_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/scp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/service.py
--rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/topic.py
--rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/device/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.588095 rapyuta-io-cli-2.0.2/riocli/disk/
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/disk/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/disk/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/disk/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3105 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/disk/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/disk/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.588095 rapyuta-io-cli-2.0.2/riocli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.588095 rapyuta-io-cli-2.0.2/riocli/jsonschema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/jsonschema/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.592095 rapyuta-io-cli-2.0.2/riocli/managedservice/
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/managedservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/managedservice/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/managedservice/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/managedservice/list_providers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2042 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/managedservice/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3977 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/managedservice/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.592095 rapyuta-io-cli-2.0.2/riocli/marketplace/
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/marketplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/marketplace/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     4032 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/marketplace/install.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/marketplace/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3365 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/marketplace/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.592095 rapyuta-io-cli-2.0.2/riocli/model/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5730 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.596095 rapyuta-io-cli-2.0.2/riocli/network/
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4238 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/native_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/routed_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     6168 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/network/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.596095 rapyuta-io-cli-2.0.2/riocli/package/
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     9446 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/package/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.596095 rapyuta-io-cli-2.0.2/riocli/parameter/
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2969 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/download.py
--rw-r--r--   0 runner    (1001) docker     (122)     1187 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/upload.py
--rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/parameter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.600095 rapyuta-io-cli-2.0.2/riocli/project/
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     3816 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/project/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.600095 rapyuta-io-cli-2.0.2/riocli/rosbag/
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/rosbag/blob.py
--rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/rosbag/job.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/rosbag/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.604095 rapyuta-io-cli-2.0.2/riocli/secret/
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/docker_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     3442 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/import_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/source_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/secret/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.604095 rapyuta-io-cli-2.0.2/riocli/shell/
--rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/shell/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.604095 rapyuta-io-cli-2.0.2/riocli/static_route/
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/open.py
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/static_route/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.604095 rapyuta-io-cli-2.0.2/riocli/usergroup/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/usergroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/usergroup/list.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:39:59.608095 rapyuta-io-cli-2.0.2/riocli/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3381 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/selector.py
--rw-r--r--   0 runner    (1001) docker     (122)     1602 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/spinner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/riocli/utils/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 12:39:59.608095 rapyuta-io-cli-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-04-20 12:39:48.000000 rapyuta-io-cli-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.538149 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-05-17 13:12:46.000000 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4616 2023-05-17 13:12:46.000000 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:12:46.000000 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-17 13:12:46.000000 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-05-17 13:12:46.000000 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-17 13:12:46.000000 rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.538149 rapyuta-io-cli-3.0.0/riocli/
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.538149 rapyuta-io-cli-3.0.0/riocli/apply/
+-rw-r--r--   0 runner    (1001) docker     (122)     3908 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/apply/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15241 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/apply/parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8273 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/apply/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/apply/template.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/apply/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.538149 rapyuta-io-cli-3.0.0/riocli/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4016 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/logout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2663 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/staging.py
+-rw-r--r--   0 runner    (1001) docker     (122)      911 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3799 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/auth/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.538149 rapyuta-io-cli-3.0.0/riocli/build/
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/import_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/build/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.542149 rapyuta-io-cli-3.0.0/riocli/chart/
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3182 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/chart/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.542149 rapyuta-io-cli-3.0.0/riocli/completion/
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/completion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.542149 rapyuta-io-cli-3.0.0/riocli/config/
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.542149 rapyuta-io-cli-3.0.0/riocli/deployment/
+-rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2861 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16564 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/deployment/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.542149 rapyuta-io-cli-3.0.0/riocli/device/
+-rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6340 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4083 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/label.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3301 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/metric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/onboard.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/device/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/device_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/forward.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/rapyuta_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/scp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/topic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/device/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/disk/
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/disk/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/disk/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/disk/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/disk/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/disk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/jsonschema/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/managedservice/
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/managedservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/managedservice/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/managedservice/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1325 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/managedservice/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1273 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/managedservice/list_providers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/managedservice/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/model/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5730 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/network/
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/native_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/routed_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6168 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/network/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/organization/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/organization/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/organization/select.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.546149 rapyuta-io-cli-3.0.0/riocli/package/
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9344 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/package/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.550149 rapyuta-io-cli-3.0.0/riocli/parameter/
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2982 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1187 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/upload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/parameter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.550149 rapyuta-io-cli-3.0.0/riocli/project/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.550149 rapyuta-io-cli-3.0.0/riocli/project/features/
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/features/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/project/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.550149 rapyuta-io-cli-3.0.0/riocli/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/rosbag/blob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/rosbag/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/rosbag/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.550149 rapyuta-io-cli-3.0.0/riocli/secret/
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/docker_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3442 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/import_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/source_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/secret/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.550149 rapyuta-io-cli-3.0.0/riocli/shell/
+-rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/shell/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/riocli/static_route/
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1849 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/open.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/static_route/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/riocli/usergroup/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/usergroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/usergroup/list.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/riocli/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2386 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/selector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1602 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/utils/ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/riocli/v2client/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/v2client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11183 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/v2client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/riocli/vpn/
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/vpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4909 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/vpn/connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/vpn/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/vpn/ping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/vpn/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/riocli/vpn/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 13:12:46.554149 rapyuta-io-cli-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1692 2023-05-17 13:12:34.000000 rapyuta-io-cli-3.0.0/setup.py
```

### Comparing `rapyuta-io-cli-2.0.2/PKG-INFO` & `rapyuta-io-cli-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 2.0.2
+Version: 3.0.0
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-2.0.2/README.md` & `rapyuta-io-cli-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/PKG-INFO` & `rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 2.0.2
+Version: 3.0.0
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-2.0.2/rapyuta_io_cli.egg-info/SOURCES.txt` & `rapyuta-io-cli-3.0.0/rapyuta_io_cli.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 riocli/device/label.py
 riocli/device/list.py
 riocli/device/metric.py
 riocli/device/model.py
 riocli/device/onboard.py
 riocli/device/topic.py
 riocli/device/util.py
+riocli/device/vpn.py
 riocli/device/tools/__init__.py
 riocli/device/tools/device_init.py
 riocli/device/tools/forward.py
 riocli/device/tools/rapyuta_logs.py
 riocli/device/tools/scp.py
 riocli/device/tools/service.py
 riocli/device/tools/ssh.py
@@ -85,36 +86,34 @@
 riocli/disk/list.py
 riocli/disk/model.py
 riocli/disk/util.py
 riocli/exceptions/__init__.py
 riocli/jsonschema/__init__.py
 riocli/jsonschema/validate.py
 riocli/managedservice/__init__.py
+riocli/managedservice/delete.py
 riocli/managedservice/inspect.py
 riocli/managedservice/list.py
 riocli/managedservice/list_providers.py
 riocli/managedservice/model.py
-riocli/managedservice/util.py
-riocli/marketplace/__init__.py
-riocli/marketplace/inspect.py
-riocli/marketplace/install.py
-riocli/marketplace/list.py
-riocli/marketplace/util.py
 riocli/model/__init__.py
 riocli/model/base.py
 riocli/network/__init__.py
 riocli/network/create.py
 riocli/network/delete.py
 riocli/network/inspect.py
 riocli/network/list.py
 riocli/network/logs.py
 riocli/network/model.py
 riocli/network/native_network.py
 riocli/network/routed_network.py
 riocli/network/util.py
+riocli/organization/__init__.py
+riocli/organization/list.py
+riocli/organization/select.py
 riocli/package/__init__.py
 riocli/package/create.py
 riocli/package/delete.py
 riocli/package/deployment.py
 riocli/package/inspect.py
 riocli/package/list.py
 riocli/package/model.py
@@ -131,14 +130,16 @@
 riocli/project/create.py
 riocli/project/delete.py
 riocli/project/inspect.py
 riocli/project/list.py
 riocli/project/model.py
 riocli/project/select.py
 riocli/project/util.py
+riocli/project/features/__init__.py
+riocli/project/features/vpn.py
 riocli/rosbag/__init__.py
 riocli/rosbag/blob.py
 riocli/rosbag/job.py
 riocli/rosbag/util.py
 riocli/secret/__init__.py
 riocli/secret/create.py
 riocli/secret/delete.py
@@ -163,8 +164,16 @@
 riocli/usergroup/list.py
 riocli/utils/__init__.py
 riocli/utils/context.py
 riocli/utils/execute.py
 riocli/utils/mermaid.py
 riocli/utils/selector.py
 riocli/utils/spinner.py
-riocli/utils/ssh_tunnel.py
+riocli/utils/ssh_tunnel.py
+riocli/v2client/__init__.py
+riocli/v2client/client.py
+riocli/vpn/__init__.py
+riocli/vpn/connect.py
+riocli/vpn/disconnect.py
+riocli/vpn/ping.py
+riocli/vpn/status.py
+riocli/vpn/util.py
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/__main__.py` & `rapyuta-io-cli-3.0.0/riocli/__main__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/apply/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/apply/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 @click.option('--dryrun', '-d', is_flag=True, default=False, help='dry run the yaml files without applying any change')
 @click.option('--values', '-v',
               help="path to values yaml file. key/values specified in the values file can be used as variables in template yamls")
 @click.option('--secrets', '-s',
               help="secret files are sops encoded value files. rio-cli expects sops to be authorized for decoding files on this computer")
 @click.option('--workers', '-w', help="number of parallel workers while running apply command. defaults to 6.",
               type=int)
-@click.option('--silent', type=click.BOOL, default=False, help="Skip confirmation")
+@click.option('-f', '--force', '--silent', 'silent', is_flag=True, type=click.BOOL, default=False,
+              help="Skip confirmation")
 @click.argument('files', nargs=-1)
 def apply(values: str, secrets: str, files: Iterable[str], dryrun: bool = False, workers: int = 6,
           silent: bool = False) -> None:
     """
     Apply resource manifests
     """
     glob_files, abs_values, abs_secrets = process_files_values_secrets(
@@ -70,15 +71,16 @@
     help_options_color='green',
 )
 @click.option('--dryrun', '-d', is_flag=True, default=False, help='dry run the yaml files without applying any change')
 @click.option('--values', '-v',
               help="path to values yaml file. key/values specified in the values file can be used as variables in template yamls")
 @click.option('--secrets', '-s',
               help="secret files are sops encoded value files. rio-cli expects sops to be authorized for decoding files on this computer")
-@click.option('--silent', type=click.BOOL, default=False, help="Skip confirmation")
+@click.option('-f', '--force', '--silent', 'silent', is_flag=True, type=click.BOOL, default=False,
+              help="Skip confirmation")
 @click.argument('files', nargs=-1)
 def delete(values: str, secrets: str, files: Iterable[str], dryrun: bool = False, silent: bool = False) -> None:
     """
     Removes resources defined in the manifest
     """
     glob_files, abs_values, abs_secrets = process_files_values_secrets(
         files, values, secrets)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/apply/explain.py` & `rapyuta-io-cli-3.0.0/riocli/apply/explain.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,14 @@
 def explain(resource: str, templates: str = None) -> None:
     if templates:
         path = Path(templates)
     else:
         path = Path(__file__).parent.joinpath('manifests')
 
     for each in path.glob('**/*'):
-        if resource in each.name:
+        if resource + '.yaml' == each.name:
             with open(each) as f:
-                click.secho(f.readlines())
+                click.echo_via_pager(f.readlines())
                 raise SystemExit(0)
 
     click.secho("[Err] Resource \"{}\" not found".format(resource), fg='red')
     raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/apply/parse.py` & `rapyuta-io-cli-3.0.0/riocli/apply/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 
     def _register_object(self, data):
         try:
             key = self._get_object_key(data)
             self.objects[key] = data
             self.resolved_objects[key] = {'src': 'local', 'manifest': data}
         except KeyError:
-            print("key error {}".format(data))
+            click.secho("Key error {}".format(data), fg='red')
             return
 
     def _load_file_content(self, file_name, is_value=False, is_secret=False):
         if not is_secret:
             with open(file_name) as opened:
                 data = opened.read()
         else:
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/apply/resolver.py` & `rapyuta-io-cli-3.0.0/riocli/apply/resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import typing
 
 from munch import munchify
 from rapyuta_io import DeploymentPhaseConstants
 from rapyuta_io.utils.rest_client import HttpMethod, RestClient
 
 from riocli.build.model import Build
+from riocli.config import new_v2_client
 from riocli.config.config import Configuration
 from riocli.deployment.model import Deployment
 from riocli.device.model import Device
 from riocli.disk.model import Disk
 from riocli.managedservice.model import ManagedService
 from riocli.network.model import Network
 from riocli.package.model import Package
@@ -73,14 +74,15 @@
     }
 
     GUID_KEYS = ['guid', 'GUID', 'uuid', 'ID', 'Id', 'id']
     NAME_KEYS = ['name', 'urlPrefix', 'buildName']
 
     def __init__(self, client):
         self.client = client
+        self.v2client = new_v2_client()
 
     @functools.lru_cache()
     def list_objects(self, kind):
         return self._list_functors(kind)()
 
     @functools.lru_cache()
     def find_guid(self, name, kind, *args):
@@ -107,15 +109,15 @@
             else:
                 return None, None
         return None, None
 
     def _guid_functor(self, kind):
         mapping = {
             'secret': lambda x: munchify(x).guid,
-            "project": lambda x: munchify(x).guid,
+            "project": lambda x: munchify(x).metadata.guid,
             "package": lambda x: munchify(x)['id'],
             "staticroute": lambda x: munchify(x)['guid'],
             "build": lambda x: munchify(x)['guid'],
             "deployment": lambda x: munchify(x)['deploymentId'],
             "network": lambda x: munchify(x)['guid'],
             # This is only temporarily like this
             "disk": lambda x: munchify(x)['internalDeploymentGUID'],
@@ -123,15 +125,15 @@
             "managedservice": lambda x: munchify(x)['metadata']['name'],
         }
         return mapping[kind]
 
     def _list_functors(self, kind):
         mapping = {
             'secret': self.client.list_secrets,
-            "project": self.client.list_projects,
+            "project": self.v2client.list_projects,
             "package": self.client.get_all_packages,
             "staticroute": self.client.get_all_static_routes,
             "build": self.client.list_builds,
             "deployment": functools.partial(self.client.get_all_deployments,
                                             phases=[DeploymentPhaseConstants.SUCCEEDED,
                                                     DeploymentPhaseConstants.PROVISIONING]),
             "network": self._list_networks,
@@ -141,15 +143,15 @@
         }
 
         return mapping[kind]
 
     def _find_functors(self, kind):
         mapping = {
             'secret': self._generate_find_guid_functor(),
-            "project": self._generate_find_guid_functor(),
+            "project": lambda name, projects: filter(lambda i: i.metadata.name == name, projects),
             "package": lambda name, obj_list, version: filter(
                 lambda x: name == x.name and version == x['packageVersion'], obj_list),
             "staticroute": lambda name, obj_list: filter(lambda x: name == '-'.join(x.urlPrefix.split('-')[:-1]),
                                                          obj_list),
             "build": self._generate_find_guid_functor(name_field='buildName'),
             "deployment": self._generate_find_guid_functor(),
             "network": self._generate_find_guid_functor(),
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/apply/template.py` & `rapyuta-io-cli-3.0.0/riocli/apply/template.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/apply/util.py` & `rapyuta-io-cli-3.0.0/riocli/apply/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/auth/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/auth/login.py` & `rapyuta-io-cli-3.0.0/riocli/parameter/download.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,58 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import typing
+from tempfile import mkdtemp
+from xmlrpc.client import Boolean
+
 import click
-from click_help_colors import HelpColorsCommand
+from click_spinner import spinner
 
-from riocli.auth.util import select_project, get_token
-from riocli.utils.context import get_root_context
+from riocli.config import new_client
+from riocli.parameter.utils import display_trees
 
 
-@click.command(
-    cls=HelpColorsCommand,
-    help_headers_color='yellow',
-    help_options_color='green',
-)
-@click.option('--email', type=str,
-              help='Email of the Rapyuta.io account')
-@click.option('--password', type=str,
-              help='Password for the Rapyuta.io account')
-@click.option('--project', type=str, default=None,
-              help='Context will be set to the Project after authentication')
-@click.option('--interactive/--no-interactive', is_flag=True, type=bool, default=True,
-              help='Make login interactive')
-@click.pass_context
-def login(ctx: click.Context, email: str, password: str, project: str, interactive: bool):
-    """
-    Log into the Rapyuta.io account using the CLI. This is required to use most of the
-    functionalities of the CLI.
-    """
+# -----------------------------------------------------------------------------
+#
+# Configurations
+# Args
+#    path,  tree_names,  delete_existing=True|False
+# -----------------------------------------------------------------------------
 
-    if interactive:
-        email = email or click.prompt('Email')
-        password = password or click.prompt('Password', hide_input=True)
 
-    if not email:
-        click.secho('email not specified')
-        raise SystemExit(1)
-    if not password:
-        click.secho('password not specified')
+@click.command('download')
+@click.option('--tree-names', type=click.STRING, multiple=True, default=None, help='Tree names to fetch')
+@click.option('--overwrite', '--delete-existing', 'delete_existing', is_flag=True,
+              help='Overwrite existing parameter tree')
+@click.argument('path', type=click.Path(exists=True), required=False)
+def download_configurations(path: str, tree_names: typing.Tuple[str] = None, delete_existing: Boolean = False) -> None:
+    """
+    Download the Configuration Parameter trees.
+    """
+    if path is None:
+        # Not using the Context Manager because we need to persist the Temporary directory.
+        path = mkdtemp()
+
+    click.secho('Downloading at {}'.format(path))
+
+    try:
+        client = new_client()
+
+        with spinner():
+            client.download_configurations(path, tree_names=list(tree_names),
+                                           delete_existing_trees=delete_existing)
+
+        click.secho('✅ Configuration Parameters downloaded successfully', fg='green')
+    except Exception as e:
+        click.secho(e, fg='red')
         raise SystemExit(1)
-
-    ctx = get_root_context(ctx)
-    ctx.obj.data['email_id'] = email
-    ctx.obj.data['password'] = password
-    ctx.obj.data['auth_token'] = get_token(email, password)
-
-    # Save if the file does not already exist
-    if not ctx.obj.exists or not interactive:
-        ctx.obj.save()
-    else:
-        click.echo("[Warning] rio already has a config file present")
-        click.confirm('Do you want to override the config', abort=True)
-
-    if not interactive and not project:
-        click.echo('Logged in successfully!')
-        return
-
-    select_project(ctx.obj, project=project)
-    ctx.obj.save()
-    click.echo('Logged in successfully!')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/auth/logout.py` & `rapyuta-io-cli-3.0.0/riocli/auth/logout.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/auth/refresh_token.py` & `rapyuta-io-cli-3.0.0/riocli/auth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/auth/staging.py` & `rapyuta-io-cli-3.0.0/riocli/auth/staging.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 
-from riocli.auth.login import select_project
+from riocli.auth.login import select_project, select_organization
 from riocli.auth.util import get_token
 from riocli.config import Configuration
 from riocli.utils.context import get_root_context
 
 _STAGING_ENVIRONMENT_SUBDOMAIN = "apps.okd4v2.okd4beta.rapyuta.io"
 _NAMED_ENVIRONMENTS = ["v11", "v12", "v13", "v14", "v15", "qa", "dev"]
 
@@ -44,15 +44,16 @@
     ctx.obj.data.pop('project_id', None)
     email = ctx.obj.data.get('email_id', None)
     password = ctx.obj.data.get('password', None)
     ctx.obj.save()
 
     ctx.obj.data['auth_token'] = get_token(email, password)
 
-    select_project(ctx.obj)
+    organization = select_organization(ctx.obj)
+    select_project(ctx.obj, organization=organization)
     ctx.obj.save()
 
 
 def _validate_environment(name: str) -> bool:
     valid = name in _NAMED_ENVIRONMENTS or name.startswith('pr')
     if not valid:
         click.secho('Invalid staging environment!', fg='red')
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/auth/status.py` & `rapyuta-io-cli-3.0.0/riocli/auth/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/auth/token.py` & `rapyuta-io-cli-3.0.0/riocli/auth/token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/auth/util.py` & `rapyuta-io-cli-3.0.0/riocli/project/delete.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,63 +7,36 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import os
-
 import click
 from click_spinner import spinner
-from rapyuta_io import Client
-from rapyuta_io.utils import UnauthorizedError
 
-from riocli.config import Configuration
-from riocli.project.util import find_project_guid
-from riocli.utils.selector import show_selection
+from riocli.config import new_v2_client
+from riocli.project.util import name_to_guid
 
 
-def select_project(config: Configuration, project: str = None) -> None:
+@click.command('delete')
+@click.option('--force', '-f', '--silent', 'force', is_flag=True,
+              help='Skip confirmation')
+@click.argument('project-name', type=str)
+@name_to_guid
+def delete_project(force: bool, project_name: str, project_guid: str) -> None:
     """
-    Launches the project selection prompt by listing all the projects.
-    Sets the choice in the given configuration.
+    Deletes the project from the Platform
     """
-    client = config.new_client(with_project=False)
-
-    project_guid = None
-    if project:
-        project_guid = project if project.startswith('project-') else find_project_guid(client, project)
-
-    projects = client.list_projects()
-    # Sort projects based on their names for an easier selection
-    projects = sorted(projects, key=lambda p: p.name.lower())
-    project_map = dict()
-
-    for project in projects:
-        project_map[project.guid] = project.name
-
-    if not project_guid:
-        project_guid = show_selection(project_map, header='Select the project to activate')
-
-    config.data['project_id'] = project_guid
-    config.data['project_name'] = project_map[project_guid]
-
-
-def get_token(email: str, password: str) -> str:
-    """
-    Generates a new token using email and password.
-    """
-    config = Configuration()
-    if 'environment' in config.data:
-        os.environ['RIO_CONFIG'] = config.filepath
+    if not force:
+        click.confirm(
+            'Deleting project {} ({})'.format(project_name, project_guid),
+            abort=True)
 
     try:
+        client = new_v2_client()
         with spinner():
-            token = Client.get_auth_token(email, password)
-        return token
-    except UnauthorizedError:
-        click.secho("incorrect email/password", fg='red')
-        raise SystemExit(1)
+            client.delete_project(project_guid)
+        click.secho('Project deleted successfully!', fg='green')
     except Exception as e:
-        click.secho(e, fg='red')
+        click.secho('failed to delete project: {}'.format(e), fg='red')
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/bootstrap.py` & `rapyuta-io-cli-3.0.0/riocli/bootstrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "2.0.2"
+__version__ = "3.0.0"
 
 import click
 import rapyuta_io.version
 from click import Context
 from click_help_colors import HelpColorsGroup
 from click_plugins import with_plugins
 from pkg_resources import iter_entry_points
@@ -28,23 +28,24 @@
 from riocli.chart import chart
 from riocli.completion import completion
 from riocli.config import Configuration
 from riocli.deployment import deployment
 from riocli.device import device
 from riocli.disk import disk
 from riocli.managedservice import managedservice
-from riocli.marketplace import marketplace
 from riocli.network import network
+from riocli.organization import organization
 from riocli.package import package
 from riocli.parameter import parameter
 from riocli.project import project
 from riocli.rosbag import rosbag
 from riocli.secret import secret
 from riocli.shell import shell, deprecated_repl
 from riocli.static_route import static_route
+from riocli.vpn import vpn
 
 
 @with_plugins(iter_entry_points('riocli.plugins'))
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
     help_headers_color="yellow",
@@ -84,14 +85,15 @@
 cli.add_command(secret)
 cli.add_command(package)
 cli.add_command(deployment)
 cli.add_command(static_route)
 cli.add_command(rosbag)
 cli.add_command(network)
 cli.add_command(completion)
-cli.add_command(marketplace)
 cli.add_command(parameter)
 cli.add_command(disk)
 cli.add_command(shell)
 cli.add_command(deprecated_repl)
 cli.add_command(managedservice)
 cli.add_command(template)
+cli.add_command(organization)
+cli.add_command(vpn)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/build/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/build/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/build/create.py` & `rapyuta-io-cli-3.0.0/riocli/build/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/build/delete.py` & `rapyuta-io-cli-3.0.0/riocli/build/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/build/import_build.py` & `rapyuta-io-cli-3.0.0/riocli/build/import_build.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/build/inspect.py` & `rapyuta-io-cli-3.0.0/riocli/build/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/build/list.py` & `rapyuta-io-cli-3.0.0/riocli/build/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/build/logs.py` & `rapyuta-io-cli-3.0.0/riocli/build/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/build/model.py` & `rapyuta-io-cli-3.0.0/riocli/build/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 from rapyuta_io import Build as v1Build, Client, BuildOptions, CatkinOption
 
+from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
-from riocli.jsonschema.validate import validate_manifest, load_schema
 
 
 class Build(Model):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
@@ -71,8 +71,8 @@
 
     @staticmethod
     def validate(data):
         """
         Validates if build data is matching with its corresponding schema
         """
         schema = load_schema('build')
-        validate_manifest(instance=data, schema=schema)
+        schema.validate(data)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/build/trigger.py` & `rapyuta-io-cli-3.0.0/riocli/build/trigger.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/build/util.py` & `rapyuta-io-cli-3.0.0/riocli/build/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/chart/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/chart/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/chart/apply.py` & `rapyuta-io-cli-3.0.0/riocli/chart/apply.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/chart/chart.py` & `rapyuta-io-cli-3.0.0/riocli/chart/chart.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/chart/delete.py` & `rapyuta-io-cli-3.0.0/riocli/chart/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/chart/info.py` & `rapyuta-io-cli-3.0.0/riocli/chart/info.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/chart/list.py` & `rapyuta-io-cli-3.0.0/riocli/chart/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/chart/search.py` & `rapyuta-io-cli-3.0.0/riocli/chart/search.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/chart/util.py` & `rapyuta-io-cli-3.0.0/riocli/chart/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/completion/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/config/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/parameter/list.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,37 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from riocli.config.config import Configuration
+import click
+from rapyuta_io.utils.rest_client import HttpMethod
 
+from riocli.parameter.utils import _api_call
+from riocli.utils import tabulate_data
 
-def new_client(config_inst: Configuration = None, with_project: bool = True):
+
+@click.command('list')
+def list_configuration_trees() -> None:
     """
-    new_client is a simple wrapper around the Configuration's new_client method. It can be called
-    directly without initializing the Configuration first. It initializes the Configuration if not
-    given already and then calls its new_client method.
+    List the Configuration Parameter Trees.
     """
-    if not config_inst:
-        config_inst = Configuration()
+    try:
+        data = _api_call(HttpMethod.GET)
+        if 'data' not in data:
+            raise Exception('Something went wrong!')
+
+        trees = [[tree] for tree in data['data']]
+
+        tabulate_data(trees, headers=['Tree Name'])
 
-    return config_inst.new_client(with_project=with_project)
+    except Exception as e:
+        click.secho(str(e), fg='red')
+        raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/config/config.py` & `rapyuta-io-cli-3.0.0/riocli/config/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import errno
 import json
 import os
+import uuid
 
 from click import get_app_dir
 from rapyuta_io import Client
 
 from riocli.exceptions import LoggedOut, NoProjectSelected
+from riocli.v2client import Client as v2Client
 
 
 class Configuration(object):
     """
     Configuration defines a class to define operations on the CLI's configuration file centrally.
     The class can be initialized irrespective of if the actual file exists or not. The object will
     automatically read the file if one exists and exposes the data through the `data` field.
@@ -75,14 +77,31 @@
             raise NoProjectSelected
 
         if not with_project:
             project = None
 
         return Client(auth_token=token, project=project)
 
+    def new_v2_client(self, with_project: bool = True) -> v2Client:
+        if 'auth_token' not in self.data:
+            raise LoggedOut
+
+        if 'environment' in self.data:
+            os.environ['RIO_CONFIG'] = self.filepath
+
+        token = self.data.get('auth_token', None)
+        project = self.data.get('project_id', None)
+        if with_project and project is None:
+            raise NoProjectSelected
+
+        if not with_project:
+            project = None
+
+        return v2Client(self, auth_token=token, project=project)
+
     def get_auth_header(self) -> dict:
         if not ('auth_token' in self.data and 'project_id' in self.data):
             raise LoggedOut
 
         token, project = self.data['auth_token'], self.data['project_id']
         if not token.startswith('Bearer'):
             token = 'Bearer {}'.format(token)
@@ -99,7 +118,15 @@
     @filepath.setter
     def filepath(self, value: str):
         self._filepath = value
 
     @property
     def piping_server(self):
         return self.data.get('piping_server', self.PIPING_SERVER)
+
+    @property
+    def machine_id(self):
+        if 'machine_id' not in self.data:
+            self.data['machine_id'] = str(uuid.uuid4())
+            self.save()
+
+        return self.data.get('machine_id')
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/deployment/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/deployment/delete.py` & `rapyuta-io-cli-3.0.0/riocli/deployment/delete.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from click_spinner import spinner
 
 from riocli.config import new_client
 from riocli.deployment.util import name_to_guid
 
 
 @click.command('delete')
-@click.option('--force', '-f', is_flag=True, default=False, help='Skip confirmation')
+@click.option('--force', '-f', '--silent', is_flag=True, default=False,
+              help='Skip confirmation')
 @click.argument('deployment-name', type=str)
 @name_to_guid
 def delete_deployment(force: bool, deployment_name: str, deployment_guid: str) -> None:
     """
     Delete the deployment from the Platform
     """
     if not force:
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/deployment/inspect.py` & `rapyuta-io-cli-3.0.0/riocli/deployment/inspect.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,12 +59,13 @@
         'dependent_deployments': deployment.dependentDeployments,
         'labels': deployment.labels,
         'in_use': deployment.inUse,
         'used_by': deployment.usedBy,
         'phase': deployment.phase,
         'status': deployment.status,
         'component_info': deployment.componentInfo,
-        'dependent_deployment_status': deployment.dependentDeploymentStatus,
-        'errors': deployment.errors,
-        'package_dependency_status': deployment.packageDependencyStatus,
-        'core_networks': deployment.coreNetworks,
+        'dependent_deployment_status': deployment.get(
+            'dependentDeploymentStatus'),
+        'errors': deployment.get('errors'),
+        'package_dependency_status': deployment.get('packageDependencyStatus'),
+        'core_networks': deployment.get('coreNetworks'),
     }
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/deployment/list.py` & `rapyuta-io-cli-3.0.0/riocli/deployment/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/deployment/logs.py` & `rapyuta-io-cli-3.0.0/riocli/deployment/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/deployment/model.py` & `rapyuta-io-cli-3.0.0/riocli/deployment/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,75 +17,76 @@
 import click
 from rapyuta_io import Client
 from rapyuta_io.clients.catalog_client import Package
 from rapyuta_io.clients.deployment import DeploymentNotRunningException
 from rapyuta_io.clients.native_network import NativeNetwork
 from rapyuta_io.clients.package import ProvisionConfiguration, RestartPolicy, \
     ExecutableMount
-from rapyuta_io.clients.rosbag import ROSBagJob, ROSBagOptions, \
-    ROSBagCompression, UploadOptions, \
-    ROSBagOnDemandUploadOptions, ROSBagTimeRange, ROSBagUploadTypes, \
-    OverrideOptions, TopicOverrideInfo
+from rapyuta_io.clients.rosbag import (
+    ROSBagJob, ROSBagOptions, ROSBagCompression,
+    UploadOptions, ROSBagOnDemandUploadOptions, ROSBagTimeRange,
+    ROSBagUploadTypes, OverrideOptions, TopicOverrideInfo)
 from rapyuta_io.clients.routed_network import RoutedNetwork
 
 from riocli.deployment.errors import ERRORS
 from riocli.deployment.util import add_mount_volume_provision_config
+from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
 from riocli.package.util import find_package_guid
 from riocli.static_route.util import find_static_route_guid
-from riocli.jsonschema.validate import validate_manifest, load_schema
 
 
 class Deployment(Model):
     RESTART_POLICY = {
         'always': RestartPolicy.Always,
         'never': RestartPolicy.Never,
         'onfailure': RestartPolicy.OnFailure
     }
 
     def find_object(self, client: Client) -> typing.Any:
-        guid, obj = self.rc.find_depends({'kind': 'deployment', 'nameOrGUID': self.metadata.name})
-        if not guid:
-            return False
-
-        return obj
+        guid, obj = self.rc.find_depends(
+            {"kind": "deployment", "nameOrGUID": self.metadata.name})
+        return obj if guid else False
 
     def create_object(self, client: Client) -> typing.Any:
-        pkg_guid, pkg = self.rc.find_depends(self.metadata.depends, self.metadata.depends.version)
+        pkg_guid, pkg = self.rc.find_depends(self.metadata.depends,
+                                             self.metadata.depends.version)
 
         if pkg_guid:
             pkg = client.get_package(pkg_guid)
         pkg.update()
 
         default_plan = pkg['plans'][0]
+        plan_id = default_plan['planId']
         internal_component = default_plan['internalComponents'][0]
-
-        __planId = default_plan['planId']
-        __componentName = internal_component.componentName
+        component_name = internal_component.componentName
+        component = default_plan['components']['components'][0]
+        executables = component['executables']
         runtime = internal_component['runtime']
 
         if 'runtime' in self.spec and runtime != self.spec.runtime:
-            click.secho('>> runtime mismatch => ' +
-                        'deployment:{}.runtime !== package:{}.runtime '.format(
-                            self.metadata.name, pkg['packageName']
-                        ), fg='red'
-                        )
+            click.secho(
+                '>> runtime mismatch => ' +
+                'deployment:{}.runtime !== package:{}.runtime '.format(
+                    self.metadata.name, pkg['packageName']
+                ), fg='red')
             return
 
-        provision_config = pkg.get_provision_configuration(__planId)
+        provision_config = pkg.get_provision_configuration(plan_id)
 
         # add label
         if 'labels' in self.metadata:
             for key, value in self.metadata.labels.items():
                 provision_config.add_label(key, value)
 
         # Add envArgs
         if 'envArgs' in self.spec:
             for items in self.spec.envArgs:
-                provision_config.add_parameter(__componentName, items.name, items.value)
+                provision_config.add_parameter(component_name, items.name,
+                                               items.value)
 
         # Add Dependent Deployment
         if 'depends' in self.spec:
             for item in self.spec.depends:
                 dep_guid, dep = self.rc.find_depends(item)
                 if dep is None and dep_guid:
                     dep = client.get_deployment(dep_guid)
@@ -101,94 +102,136 @@
                         network_obj, network_interface=network_depends.get('interface', None))
                 if type(network_obj) == NativeNetwork:
                     provision_config.add_native_network(
                         network_obj, network_interface=network_depends.get('interface', None))
 
         if 'rosBagJobs' in self.spec:
             for req_job in self.spec.rosBagJobs:
-                provision_config.add_rosbag_job(__componentName, self._form_rosbag_job(req_job))
+                provision_config.add_rosbag_job(component_name,
+                                                self._form_rosbag_job(req_job))
 
         if self.spec.runtime == 'cloud':
             if 'staticRoutes' in self.spec:
                 for stroute in self.spec.staticRoutes:
                     route_guid, route = self.rc.find_depends(stroute.depends)
                     if route is None and route_guid:
                         route = client.get_static_route(route_guid)
-                    provision_config.add_static_route(__componentName, stroute.name, route)
+                    provision_config.add_static_route(component_name,
+                                                      stroute.name, route)
 
             # Add Disk
             if 'volumes' in self.spec:
                 disk_mounts = {}
                 for vol in self.spec.volumes:
                     disk_guid, disk = self.rc.find_depends(vol.depends)
                     if disk_guid not in disk_mounts:
                         disk_mounts[disk_guid] = []
 
                     disk_mounts[disk_guid].append(
                         ExecutableMount(vol.execName, vol.mountPath, vol.subPath))
 
                 for disk_guid in disk_mounts.keys():
                     disk = client.get_volume_instance(disk_guid)
-                    provision_config.mount_volume(__componentName, volume=disk,
-                                                  executable_mounts=disk_mounts[disk_guid])
+                    provision_config.mount_volume(component_name, volume=disk,
+                                                  executable_mounts=
+                                                  disk_mounts[disk_guid])
 
             # TODO: Managed Services is currently limited to `cloud` deployments
             # since we don't expose `elasticsearch` outside Openshift. This may
             # change in the future.
             if 'managedServices' in self.spec:
                 managed_services = []
                 for managed_service in self.spec.managedServices:
                     managed_services.append({
                         'instance': managed_service.depends.nameOrGUID,
                     })
                 provision_config.context['managedServices'] = managed_services
 
+            # inject the vpn managedservice instance if the flag is set to
+            # true. 'rio-internal-headscale' is the default vpn instance
+            if 'features' in self.spec:
+                if 'vpn' in self.spec.features and self.spec.features.vpn.enabled:
+                    provision_config.context['managedServices'] = [{
+                        "instance": "rio-internal-headscale"
+                    }]
+
+                if 'params' in self.spec.features and self.spec.features.params.enabled:
+                    component_id = internal_component.componentId
+                    tree_names = self.spec.features.params.get('trees', [])
+                    disable_sync = self.spec.features.params.get('disableSync',
+                                                                 False)
+
+                    args = []
+                    for e in executables:
+                        args.append({
+                            'executableId': e['id'],
+                            'paramTreeNames': tree_names,
+                            'enableParamSync': not disable_sync
+                        })
+
+                    context = provision_config.context
+                    if 'component_context' not in context:
+                        context['component_context'] = {}
+
+                    component_context = context['component_context']
+                    if component_id not in component_context:
+                        component_context[component_id] = {}
+
+                    component_context[component_id][
+                        'param_sync_exec_args'] = args
+
         if self.spec.runtime == 'device':
-            device_guid, device = self.rc.find_depends(self.spec.device.depends)
+            device_guid, device = self.rc.find_depends(
+                self.spec.device.depends)
             if device is None and device_guid:
                 device = client.get_device(device_guid)
-            provision_config.add_device(__componentName, device=device, set_component_alias=False)
+
+            provision_config.add_device(
+                component_name,
+                device=device,
+                set_component_alias=False
+            )
 
             if 'restart' in self.spec:
                 provision_config.add_restart_policy(
-                    __componentName, self.RESTART_POLICY[self.spec.restart.lower()])
-
-            # Add Network
-            # if self.spec.rosNetworks:
-            # for network in self.spec.rosNetworks:
-            # network_type =
+                    component_name,
+                    self.RESTART_POLICY[self.spec.restart.lower()])
 
             # Add Disk
             exec_mounts = []
             if 'volumes' in self.spec:
                 for vol in self.spec.volumes:
-                    exec_mounts.append(ExecutableMount(vol.execName, vol.mountPath, vol.subPath))
+                    exec_mounts.append(
+                        ExecutableMount(vol.execName, vol.mountPath,
+                                        vol.subPath))
+
             if len(exec_mounts) > 0:
                 provision_config = add_mount_volume_provision_config(
-                    provision_config, __componentName, device, exec_mounts)
+                    provision_config, component_name, device, exec_mounts)
 
-        provision_config.set_component_alias(__componentName, self.metadata.name)
+        provision_config.set_component_alias(component_name,
+                                             self.metadata.name)
 
         if os.environ.get('DEBUG'):
             print(provision_config)
+
         deployment = pkg.provision(self.metadata.name, provision_config)
 
         try:
             deployment.poll_deployment_till_ready()
         except DeploymentNotRunningException as e:
             raise Exception(process_deployment_errors(e)) from e
         except Exception as e:
             raise e
 
         deployment.get_status()
+
         return deployment
 
     def update_object(self, client: Client, obj: typing.Any) -> typing.Any:
-        if 'depends' in self.spec:
-            pass
         pass
 
     def delete_object(self, client: Client, obj: typing.Any) -> typing.Any:
         obj.deprovision()
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
@@ -320,15 +363,15 @@
 
     @staticmethod
     def validate(data):
         """
         Validates if deployment data is matching with its corresponding schema
         """
         schema = load_schema('deployment')
-        validate_manifest(instance=data, schema=schema)
+        schema.validate(data)
 
 
 def process_deployment_errors(e: DeploymentNotRunningException):
     errors = e.deployment_status.errors
     err_fmt = '[{}] {}\nAction: {}'
     support_action = ('Report the issue together with the relevant'
                       ' details to the support team')
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/deployment/run.py` & `rapyuta-io-cli-3.0.0/riocli/deployment/run.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/deployment/ssh.py` & `rapyuta-io-cli-3.0.0/riocli/deployment/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/deployment/status.py` & `rapyuta-io-cli-3.0.0/riocli/deployment/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/deployment/util.py` & `rapyuta-io-cli-3.0.0/riocli/deployment/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/deployment/wait.py` & `rapyuta-io-cli-3.0.0/riocli/deployment/wait.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/device/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from riocli.device.inspect import inspect_device
 from riocli.device.label import device_labels
 from riocli.device.list import list_devices
 from riocli.device.metric import device_metrics
 from riocli.device.onboard import device_onboard
 from riocli.device.tools import tools
 from riocli.device.topic import device_topics
+from riocli.device.vpn import toggle_vpn
 
 
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
     help_headers_color='yellow',
     help_options_color='green',
@@ -38,20 +39,21 @@
 def device():
     """
     Devices on Rapyuta.io
     """
     pass
 
 
+device.add_command(create_device)
 device.add_command(execute_command)
 device.add_command(delete_device)
 device.add_command(device_config)
 device.add_command(device_onboard)
-device.add_command(list_deployments)
 device.add_command(device_labels)
 device.add_command(device_metrics)
 device.add_command(device_topics)
-device.add_command(list_devices)
-device.add_command(inspect_device)
-device.add_command(create_device)
 device.add_command(device_uploads)
+device.add_command(inspect_device)
+device.add_command(list_deployments)
+device.add_command(list_devices)
 device.add_command(tools)
+device.add_command(toggle_vpn)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/config.py` & `rapyuta-io-cli-3.0.0/riocli/device/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/create.py` & `rapyuta-io-cli-3.0.0/riocli/device/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/delete.py` & `rapyuta-io-cli-3.0.0/riocli/device/delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,14 @@
     """
     Deletes the device from the Platform
     """
     if not force:
         click.confirm('Deleting device {} ({})'.format(device_name, device_guid), abort=True)
 
     try:
-        client = new_client(with_project=False)
+        client = new_client(with_project=True)
         with click_spinner.spinner():
             client.delete_device(device_id=device_guid)
         click.secho('Device deleted successfully!', fg='green')
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/deployment.py` & `rapyuta-io-cli-3.0.0/riocli/device/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/execute.py` & `rapyuta-io-cli-3.0.0/riocli/device/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/files.py` & `rapyuta-io-cli-3.0.0/riocli/device/files.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/inspect.py` & `rapyuta-io-cli-3.0.0/riocli/device/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/label.py` & `rapyuta-io-cli-3.0.0/riocli/device/label.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/list.py` & `rapyuta-io-cli-3.0.0/riocli/device/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/metric.py` & `rapyuta-io-cli-3.0.0/riocli/device/metric.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/model.py` & `rapyuta-io-cli-3.0.0/riocli/device/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 from rapyuta_io import Client
 from rapyuta_io.clients.device import Device as v1Device, DevicePythonVersion
 
+from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
-from riocli.jsonschema.validate import validate_manifest, load_schema
 
 
 class Device(Model):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
@@ -67,8 +67,8 @@
 
     @staticmethod
     def validate(data):
         """
         Validates if device data is matching with its corresponding schema
         """
         schema = load_schema('device')
-        validate_manifest(instance=data, schema=schema)
+        schema.validate(data)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/onboard.py` & `rapyuta-io-cli-3.0.0/riocli/device/onboard.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/tools/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/device/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/tools/device_init.py` & `rapyuta-io-cli-3.0.0/riocli/device/tools/device_init.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/tools/forward.py` & `rapyuta-io-cli-3.0.0/riocli/device/tools/forward.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/tools/rapyuta_logs.py` & `rapyuta-io-cli-3.0.0/riocli/device/tools/rapyuta_logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/tools/scp.py` & `rapyuta-io-cli-3.0.0/riocli/device/tools/scp.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/tools/service.py` & `rapyuta-io-cli-3.0.0/riocli/device/tools/service.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/tools/ssh.py` & `rapyuta-io-cli-3.0.0/riocli/device/tools/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/tools/util.py` & `rapyuta-io-cli-3.0.0/riocli/device/tools/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/topic.py` & `rapyuta-io-cli-3.0.0/riocli/device/topic.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/device/util.py` & `rapyuta-io-cli-3.0.0/riocli/device/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/disk/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/disk/create.py` & `rapyuta-io-cli-3.0.0/riocli/disk/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/disk/delete.py` & `rapyuta-io-cli-3.0.0/riocli/disk/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/disk/list.py` & `rapyuta-io-cli-3.0.0/riocli/disk/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/disk/model.py` & `rapyuta-io-cli-3.0.0/riocli/disk/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import click
 import click_spinner
 from munch import munchify
 from rapyuta_io import Client
 from rapyuta_io.utils.rest_client import HttpMethod
 
 from riocli.disk.util import _api_call
+from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
-from riocli.jsonschema.validate import load_schema, validate_manifest
 
 
 class Disk(Model):
     def find_object(self, client: Client) -> typing.Any:
         _, disk = self.rc.find_depends({'kind': 'disk', 'nameOrGUID': self.metadata.name})
         if not disk:
             return False
@@ -76,8 +76,8 @@
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
     @staticmethod
     def validate(data):
         schema = load_schema('disk')
-        validate_manifest(data, schema)
+        schema.validate(data)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/disk/util.py` & `rapyuta-io-cli-3.0.0/riocli/disk/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/exceptions/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/jsonschema/validate.py` & `rapyuta-io-cli-3.0.0/riocli/static_route/open.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-# Copyright 2023 Rapyuta Robotics
+# Copyright 2021 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import click
 
-from functools import lru_cache
-from pathlib import Path
+from riocli.config import new_client
+from riocli.static_route.util import name_to_guid
 
-import yaml
 
-import jsonschema
-
-
-@lru_cache(maxsize=None)
-def load_schema(resource: str) -> dict:
-    """
-    Reads JSON schema yaml and returns a dict.
-    """
-    schema_dir = Path(__file__).parent.joinpath('schemas')
-    with open(schema_dir.joinpath(resource + "-schema.yaml")) as f:
-        return yaml.safe_load(f)
-
-
-def validate_manifest(instance, schema) -> None:
+@click.command('open')
+@click.argument('static-route', type=str)
+@name_to_guid
+def open_static_route(static_route, static_route_guid) -> None:
     """
-    Validates a manifest against a JSON schema.
+    Opens the static route in the default browser
     """
-    jsonschema.validate(instance, schema)
+    try:
+        client = new_client()
+        route = client.get_static_route(static_route_guid)
+        click.launch(url='https://{}'.format(route.urlString), wait=False)
+    except Exception as e:
+        click.secho(str(e), fg='red')
+        raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/managedservice/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/managedservice/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_help_colors import HelpColorsGroup
 
+from riocli.managedservice.delete import delete_instance
 from riocli.managedservice.inspect import inspect_instance
 from riocli.managedservice.list import list_instances
 from riocli.managedservice.list_providers import list_providers
 
 
 @click.group(
     invoke_without_command=False,
@@ -31,10 +32,11 @@
 
     With managed services on rapyuta.io, you can provision services
     like elasticsearch, etc. on-demand and use them with your deployments.
     """
     pass
 
 
+managedservice.add_command(delete_instance)
 managedservice.add_command(list_providers)
 managedservice.add_command(list_instances)
 managedservice.add_command(inspect_instance)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/managedservice/inspect.py` & `rapyuta-io-cli-3.0.0/riocli/managedservice/inspect.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import click
+from munch import unmunchify
 
-from riocli.managedservice.util import ManagedServicesClient
+from riocli.config import new_v2_client
 from riocli.utils import inspect_with_format
 
 
 @click.command('inspect')
 @click.option('--format', '-f', 'format_type', default='yaml',
               type=click.Choice(['json', 'yaml'], case_sensitive=False))
 @click.argument('instance-name', required=True)
-def inspect_instance(format_type: str, instance_name: str) -> None:
+def inspect_instance(format_type: str, instance_name: str):
     """
     Inspect a managedservice instance
     """
     try:
-        client = ManagedServicesClient()
+        client = new_v2_client()
         instance = client.get_instance(instance_name)
-        inspect_with_format(instance, format_type)
+        inspect_with_format(unmunchify(instance), format_type)
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/managedservice/list.py` & `rapyuta-io-cli-3.0.0/riocli/managedservice/delete.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,33 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import typing
 
 import click
 
-from riocli.managedservice.util import ManagedServicesClient
-from riocli.utils import tabulate_data
+from riocli.config import new_v2_client
 
 
-@click.command('list')
-def list_instances() -> None:
+@click.command('delete')
+@click.argument('instance-name', required=True)
+def delete_instance(instance_name: str):
     """
-    List all the managedservice instances
+    Delete a managedservice instance
     """
     try:
-        client = ManagedServicesClient()
-        instances = client.list_instances()
-        _display_instances(instances)
+        client = new_v2_client()
+        r = client.delete_instance(instance_name)
+        if r.get('success', None):
+            click.secho("✅ Deleted instance '{}'".format(instance_name), fg='green')
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
-
-
-def _display_instances(instances: typing.Any):
-    headers = ("Provider", "Name", "Created At", "Labels")
-
-    data = []
-    for i in instances:
-        m = i['metadata']
-        data.append([
-            i['spec']['provider'],
-            m['name'],
-            m['created_at'],
-            m['labels']
-        ])
-
-    tabulate_data(data, headers)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/managedservice/list_providers.py` & `rapyuta-io-cli-3.0.0/riocli/managedservice/list_providers.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,36 +10,36 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
 import click
-from riocli.utils import tabulate_data
 
-from riocli.managedservice.util import ManagedServicesClient
+from riocli.config import new_v2_client
+from riocli.utils import tabulate_data
 
 
 @click.command('providers')
-def list_providers() -> None:
+def list_providers():
     """
     List available managedservice providers
     """
     try:
-        client = ManagedServicesClient()
+        client = new_v2_client()
         providers = client.list_providers()
         _display_providers(providers)
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
 
 
 def _display_providers(providers: typing.Any):
     headers = ['Provider Name']
 
     data = []
     for provider in providers:
-        if provider['name'] == 'dummy':
+        if provider.name == 'dummy':
             continue
-        data.append([provider['name']])
+        data.append([provider.name])
 
     tabulate_data(data, headers)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/managedservice/model.py` & `rapyuta-io-cli-3.0.0/riocli/managedservice/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,54 +9,57 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
-from munch import munchify
+from munch import munchify, unmunchify
 from rapyuta_io import Client
 
-from riocli.managedservice.util import ManagedServicesClient
+from riocli.config import new_v2_client
+from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
-from riocli.jsonschema.validate import load_schema, validate_manifest
 
 
 class ManagedService(Model):
     def find_object(self, client: Client) -> typing.Any:
         name = self.metadata.name
-        client = ManagedServicesClient()
+        client = new_v2_client()
 
         try:
             instance = client.get_instance(name)
             return munchify(instance)
         except Exception:
             return False
 
     def create_object(self, client: Client) -> typing.Any:
-        client = ManagedServicesClient()
-        result = client.create_instance(self)
+        client = new_v2_client()
+
+        ms = unmunchify(self)
+        ms.pop('rc', None)
+        result = client.create_instance(ms)
         return munchify(result)
 
     def update_object(self, client: Client, obj: typing.Any) -> typing.Any:
         pass
 
     def delete_object(self, client: Client, obj: typing.Any) -> typing.Any:
-        client = ManagedServicesClient()
+        client = new_v2_client()
         client.delete_instance(obj.metadata.name)
 
     @staticmethod
     def list_instances():
-        client = ManagedServicesClient()
+        client = new_v2_client()
         return client.list_instances()
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
     @staticmethod
     def validate(data):
         """
         Validates if managedservice data is matching with its corresponding schema
         """
         schema = load_schema('managedservice')
-        validate_manifest(instance=data, schema=schema)
+        schema.validate(data)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/marketplace/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/project/features/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,29 +10,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_help_colors import HelpColorsGroup
 
-from riocli.marketplace.inspect import inspect_marketplace
-from riocli.marketplace.install import install_product
-from riocli.marketplace.list import list_marketplace
+from riocli.project.features.vpn import vpn
 
 
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
     help_headers_color='yellow',
     help_options_color='green',
-    hidden=True,
 )
-def marketplace():
+def features():
     """
-    Marketplace of the packages
+    Toggle features on a project
     """
     pass
 
 
-marketplace.add_command(list_marketplace)
-marketplace.add_command(inspect_marketplace)
-marketplace.add_command(install_product)
+features.add_command(vpn)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/marketplace/inspect.py` & `rapyuta-io-cli-3.0.0/riocli/secret/inspect.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,37 +7,43 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 import click
-from rapyuta_io.utils.rest_client import HttpMethod
+from rapyuta_io import Secret
 
-from riocli.marketplace.util import api_call
+from riocli.config import new_client
+from riocli.secret.util import name_to_guid
 from riocli.utils import inspect_with_format
 
-_SKU_URL_FMT = 'marketplace/sku/{}@{}/detail'
-_PRODUCT_FMT = 'marketplace/product/{}/detail'
-
 
 @click.command('inspect')
 @click.option('--format', '-f', 'format_type', default='yaml',
               type=click.Choice(['json', 'yaml'], case_sensitive=False))
-@click.argument('rrn')
-@click.argument('version', required=False)
-def inspect_marketplace(format_type: str, rrn: str, version: str = None) -> None:
+@click.argument('secret-name', type=str)
+@name_to_guid
+def inspect_secret(format_type: str, secret_name: str, secret_guid: str) -> None:
     """
-    Inspect the marketplace package
+    Inspect the secret resource
     """
     try:
-        if version is not None:
-            url_format = _SKU_URL_FMT.format(rrn, version)
-        else:
-            url_format = _PRODUCT_FMT.format(rrn)
-        package = api_call(url_format, HttpMethod.GET)
-        inspect_with_format(package, format_type=format_type)
+        client = new_client()
+        secret = client.get_secret(secret_guid)
+        data = make_secret_inspectable(secret)
+        inspect_with_format(data, format_type)
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
+
+
+def make_secret_inspectable(obj: Secret) -> dict:
+    return {
+        'created_at': obj.created_at,
+        'creator': obj.creator,
+        'guid': obj.guid,
+        'name': obj.name,
+        'project': obj.project_guid,
+        'secret_type': obj.secret_type.value,
+    }
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/marketplace/list.py` & `rapyuta-io-cli-3.0.0/riocli/parameter/delete.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,33 +11,32 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import click
 from rapyuta_io.utils.rest_client import HttpMethod
 
-from riocli.marketplace.util import api_call
+from riocli.parameter.utils import _api_call
 
-_LIST_URL_FMT = 'marketplace/products'
 
-
-@click.command('list')
-def list_marketplace() -> None:
+@click.command('delete')
+@click.option('-f', '--force', '--silent', 'silent', is_flag=True, default=False,
+              help="Skip confirmation")
+@click.argument('tree', type=click.STRING)
+def delete_configurations(tree: str, silent: bool = False) -> None:
     """
-    List the marketplace packages
+    Deletes the Configuration Parameter Tree.
     """
+    click.secho('Configuration Parameter {} will be deleted'.format(tree))
+
+    if not silent:
+        click.confirm('Do you want to proceed?', default=True, abort=True)
+
     try:
-        packages = api_call(_LIST_URL_FMT, HttpMethod.GET)
-        display_marketplace_list(packages=packages, show_header=True)
-    except Exception as e:
+        data = _api_call(HttpMethod.DELETE, name=tree)
+        if data.get('data') != 'ok':
+            raise Exception('Something went wrong!')
+
+    except IOError as e:
+        click.secho(str(e.__traceback__), fg='red')
         click.secho(str(e), fg='red')
         raise SystemExit(1)
-
-
-def display_marketplace_list(packages: list, show_header: bool = True) -> None:
-    if show_header:
-        click.secho('{:35} {:<35} {:<24} {:40}'.format('RRN', 'Name', 'Publisher', 'Categories'), fg='yellow')
-
-    for package in packages:
-        categories = ', '.join([category['category_name'] for category in package['categories']])
-        click.secho('{:35} {:<35} {:<24} {:40}'.format(package['rrn'], package['name'], package['publisher']['name'],
-                                                       categories))
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/model/base.py` & `rapyuta-io-cli-3.0.0/riocli/model/base.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/network/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/network/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/network/create.py` & `rapyuta-io-cli-3.0.0/riocli/network/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/network/delete.py` & `rapyuta-io-cli-3.0.0/riocli/network/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/network/inspect.py` & `rapyuta-io-cli-3.0.0/riocli/network/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/network/list.py` & `rapyuta-io-cli-3.0.0/riocli/network/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/network/logs.py` & `rapyuta-io-cli-3.0.0/riocli/network/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/network/model.py` & `rapyuta-io-cli-3.0.0/riocli/network/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 from typing import Union, Any, Dict
 
 from rapyuta_io import Client
-from rapyuta_io.clients.native_network import NativeNetwork, Parameters as NativeNetworkParameters
-from rapyuta_io.clients.routed_network import RoutedNetwork, Parameters as RoutedNetworkParameters
 from rapyuta_io.clients.common_models import Limits
+from rapyuta_io.clients.native_network import NativeNetwork, \
+    Parameters as NativeNetworkParameters
+from rapyuta_io.clients.routed_network import RoutedNetwork, \
+    Parameters as RoutedNetworkParameters
 
+from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
 from riocli.network.util import find_network_name, NetworkNotFound
-from riocli.jsonschema.validate import validate_manifest, load_schema
 
 
 class Network(Model):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
@@ -98,8 +100,8 @@
 
     @staticmethod
     def validate(data):
         """
         Validates if network data is matching with its corresponding schema
         """
         schema = load_schema('network')
-        validate_manifest(instance=data, schema=schema)
+        schema.validate(data)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/network/native_network.py` & `rapyuta-io-cli-3.0.0/riocli/network/native_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/network/routed_network.py` & `rapyuta-io-cli-3.0.0/riocli/network/routed_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/network/util.py` & `rapyuta-io-cli-3.0.0/riocli/network/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/package/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/package/create.py` & `rapyuta-io-cli-3.0.0/riocli/package/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/package/delete.py` & `rapyuta-io-cli-3.0.0/riocli/package/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/package/deployment.py` & `rapyuta-io-cli-3.0.0/riocli/package/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/package/inspect.py` & `rapyuta-io-cli-3.0.0/riocli/package/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/package/list.py` & `rapyuta-io-cli-3.0.0/riocli/package/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/package/model.py` & `rapyuta-io-cli-3.0.0/riocli/package/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 import os
 import typing
 
 from munch import munchify
 from rapyuta_io import Client
 from rapyuta_io.clients.package import RestartPolicy
 
+from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
-from riocli.jsonschema.validate import validate_manifest, load_schema
 
 
 class Package(Model):
     RESTART_POLICY = {
         'always': RestartPolicy.Always,
         'never': RestartPolicy.Never,
         'onfailure': RestartPolicy.OnFailure
@@ -155,16 +155,15 @@
                 component_obj.ros.services = list(self._get_rosendpoint_struct(self.spec.ros.rosEndpoints, 'service'))
                 component_obj.ros.actions = list(self._get_rosendpoint_struct(self.spec.ros.rosEndpoints, 'action'))
 
         if 'rosBagJobs' in self.spec:
             component_obj.rosBagJobDefs = self.spec.rosBagJobs
 
         pkg_object.plans[0].components = [component_obj]
-        # return package
-        # print(json.dumps(pkg_object))
+
         return client.create_package(pkg_object)
 
     def update_object(self, client: Client, obj: typing.Any) -> typing.Any:
         pass
 
     def delete_object(self, client: Client, obj: typing.Any) -> typing.Any:
         client.delete_package(obj.packageId)
@@ -195,15 +194,15 @@
 
         if 'limits' in exec:
             exec_object.limits = {
                 "cpu": exec.limits.cpu,
                 "memory": exec.limits.memory
             }
 
-        if exec.runAsBash:
+        if exec.get('runAsBash'):
             if 'command' in exec:
                 exec_object.cmd = ['/bin/bash', '-c', exec.command]
         else:
             # TODO verify this is right for secret?
             if 'command' in exec:
                 exec_object.cmd = [exec.command]
 
@@ -245,8 +244,8 @@
 
     @staticmethod
     def validate(data):
         """
         Validates if package data is matching with its corresponding schema
         """
         schema = load_schema('package')
-        validate_manifest(instance=data, schema=schema)
+        schema.validate(data)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/package/util.py` & `rapyuta-io-cli-3.0.0/riocli/package/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/parameter/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/parameter/apply.py` & `rapyuta-io-cli-3.0.0/riocli/parameter/apply.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 @click.command('apply')
 @click.option('--devices', type=click.STRING, multiple=True, default=(),
               help='Device names to apply configurations')
 @click.option('--tree-names', type=click.STRING, multiple=True, default=None,
               help='Tree names to apply')
 @click.option('--retry-limit', type=click.INT, default=0,
               help='Retry limit')
-@click.option('--silent', type=click.BOOL, default=False, help="Skip confirmation")
+@click.option('-f', '--force', '--silent', 'silent', is_flag=True, type=click.BOOL, default=False,
+              help="Skip confirmation")
 def apply_configurations(devices: typing.List, tree_names: str = None, retry_limit: int = 0,
                          silent: bool = False) -> None:
     """
     Apply a set of configurations to a list of devices
     """
     try:
         client = new_client()
@@ -39,24 +40,21 @@
         device_map = {d.name: d for d in online_devices}
 
         if devices:
             device_ids = {device_map[d].uuid: d for d in devices if d in device_map}
         else:
             device_ids = {v.uuid: k for k, v in device_map.items()}
 
-        if len(device_ids) == 0:
+        if not device_ids:
             click.secho("invalid devices or no device is currently online", fg='red')
             raise SystemExit(1)
 
         click.secho('Online Devices: {}'.format(','.join(device_ids.values())), fg='green')
 
-        printable_tree_names = "*all*"
-        if len(tree_names) > 0:
-            printable_tree_names = ','.join(tree_names)
-
+        printable_tree_names = ','.join(tree_names) if tree_names != "" else "*all*"
         click.secho('Config Trees: {}'.format(printable_tree_names), fg='green')
 
         if not silent:
             click.confirm(
                 "Do you want to apply the configurations?",
                 default=True, abort=True)
 
@@ -72,8 +70,8 @@
             success = device['success'] or "Partial"
             result.append([device_name, success])
 
         tabulate_data(result, headers=["Device", "Success"])
     except IOError as e:
         click.secho(str(e.__traceback__), fg='red')
         click.secho(str(e), fg='red')
-        raise SystemExit(1)
+        raise SystemExit(1) from e
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/parameter/delete.py` & `rapyuta-io-cli-3.0.0/riocli/parameter/upload.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,53 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import typing
+
 import click
-from rapyuta_io.utils.rest_client import HttpMethod
+from click_spinner import spinner
 
-from riocli.parameter.utils import _api_call
+from riocli.config import new_client
+from riocli.parameter.utils import filter_trees, display_trees
 
 
-@click.command('delete')
-@click.option('-f', '--force', '--silent', 'silent', is_flag=True, default=False,
-              help="Skip confirmation")
-@click.argument('tree', type=click.STRING)
-def delete_configurations(tree: str, silent: bool = False) -> None:
+@click.command('upload')
+@click.option('--tree-names', type=click.STRING, multiple=True, default=[], help='Directory names to upload')
+@click.option('--recreate', '--delete-existing', 'delete_existing', is_flag=True,
+              help='Overwrite existing parameter tree')
+@click.option('-f', '--force', '--silent', 'silent', is_flag=True, default=False, help="Skip confirmation")
+@click.argument('path', type=click.Path(exists=True))
+def upload_configurations(path: str, tree_names: typing.Tuple[str] = None, delete_existing: bool = False,
+                          silent: bool = False) -> None:
     """
-    Deletes the Configuration Parameter Tree.
+    Upload a set of Configuration Parameter directory trees.
     """
-    click.secho('Configuration Parameter {} will be deleted'.format(tree))
+    trees = filter_trees(path, tree_names)
+
+    click.secho('Following Trees will be uploaded')
+    click.secho('')
+    display_trees(path, trees)
 
     if not silent:
         click.confirm('Do you want to proceed?', default=True, abort=True)
 
     try:
-        data = _api_call(HttpMethod.DELETE, name=tree)
-        if data.get('data') != 'ok':
-            raise Exception('Something went wrong!')
+        client = new_client()
+        with spinner():
+            client.upload_configurations(rootdir=path, tree_names=trees, delete_existing_trees=delete_existing,
+                                         as_folder=True)
 
-    except IOError as e:
-        click.secho(str(e.__traceback__), fg='red')
+        click.secho('✅ Configuration parameters uploaded successfully', fg='green')
+    except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/parameter/diff.py` & `rapyuta-io-cli-3.0.0/riocli/parameter/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 # limitations under the License.
 # -----------------------------------------------------------------------------
 #
 # Configurations
 # Args
 #    path,  tree_names,  delete_existing=True|False
 # -----------------------------------------------------------------------------
-import filecmp
 import os.path
-import typing
 from difflib import unified_diff
 from filecmp import dircmp
 from tempfile import TemporaryDirectory
 from typing import Tuple
 
 import click
 from rapyuta_io.utils.error import APIError, InternalServerError
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/parameter/download.py` & `rapyuta-io-cli-3.0.0/riocli/static_route/delete.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,41 @@
-# Copyright 2023 Rapyuta Robotics
+# Copyright 2021 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import typing
-from tempfile import mkdtemp
-from xmlrpc.client import Boolean
-
 import click
 from click_spinner import spinner
 
 from riocli.config import new_client
-from riocli.parameter.utils import display_trees
-
-
-# -----------------------------------------------------------------------------
-#
-# Configurations
-# Args
-#    path,  tree_names,  delete_existing=True|False
-# -----------------------------------------------------------------------------
+from riocli.static_route.util import name_to_guid
 
 
-@click.command('download')
-@click.option('--tree-names', type=click.STRING, multiple=True, default=None, help='Tree names to fetch')
-@click.option('--overwrite', '--delete-existing', 'delete_existing', is_flag=True,
-              help='Overwrite existing parameter tree')
-@click.argument('path', type=click.Path(exists=True), required=False)
-def download_configurations(path: str, tree_names: typing.Tuple[str] = None, delete_existing: Boolean = False) -> None:
+@click.command('delete')
+@click.option('--force', '-f', is_flag=True, default=False, help='Skip confirmation')
+@click.argument('static-route', type=str)
+@name_to_guid
+def delete_static_route(static_route: str, static_route_guid: str, force: bool) -> None:
     """
-    Download the Configuration Parameter trees.
+    Deletes the static route resource from the Platform
     """
-    if path is None:
-        # Not using the Context Manager because we need to persist the Temporary directory.
-        path = mkdtemp()
 
-    click.secho('Downloading at {}'.format(path))
+    if not force:
+        click.confirm('Deleting static route {} ({})'.format(static_route, static_route_guid),
+                      abort=True)
 
     try:
         client = new_client()
-
         with spinner():
-            client.download_configurations(path, tree_names=list(tree_names),
-                                           delete_existing_trees=delete_existing)
-
-        click.secho('✅ Configuration Parameters downloaded successfully', fg='green')
+            client.delete_static_route(static_route_guid)
+        click.secho('Static Route deleted successfully!', fg='green')
     except Exception as e:
-        click.secho(e, fg='red')
+        click.secho(str(e), fg='red')
         raise SystemExit(1)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/parameter/list.py` & `rapyuta-io-cli-3.0.0/riocli/managedservice/list.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,45 @@
-# Copyright 2023 Rapyuta Robotics
+# Copyright 2022 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import typing
+
 import click
-from rapyuta_io.utils.rest_client import HttpMethod
+from munch import unmunchify
 
-from riocli.parameter.utils import _api_call
+from riocli.config import new_v2_client
 from riocli.utils import tabulate_data
 
 
 @click.command('list')
-def list_configuration_trees() -> None:
+def list_instances():
     """
-    List the Configuration Parameter Trees.
+    List all the managedservice instances
     """
     try:
-        data = _api_call(HttpMethod.GET)
-        if 'data' not in data:
-            raise Exception('Something went wrong!')
-
-        trees = [[tree] for tree in data['data']]
-
-        tabulate_data(trees, headers=['Tree Name'])
-
+        client = new_v2_client()
+        instances = client.list_instances()
+        _display_instances(instances)
     except Exception as e:
         click.secho(str(e), fg='red')
         raise SystemExit(1)
+
+
+def _display_instances(instances: typing.Any):
+    headers = ["Provider", "Name", "Created At", "Labels"]
+
+    data = []
+    for i in instances:
+        m = i.metadata
+        data.append([i.spec.provider, m.name, m.createdAt, unmunchify(m.labels)])
+
+    tabulate_data(data, headers)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/parameter/upload.py` & `rapyuta-io-cli-3.0.0/riocli/shell/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,74 @@
-# Copyright 2023 Rapyuta Robotics
+# Copyright 2022 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-import typing
+import os
 
 import click
-from click_spinner import spinner
+from click_help_colors import HelpColorsCommand
+from click_repl import repl
+from prompt_toolkit.history import FileHistory, ThreadedHistory
+
+from riocli.config import Configuration
+from riocli.shell.prompt import prompt_callback
+
 
-from riocli.config import new_client
-from riocli.parameter.utils import filter_trees, display_trees
+@click.command(
+    cls=HelpColorsCommand,
+    help_headers_color='yellow',
+    help_options_color='green',
+)
+@click.pass_context
+def shell(ctx: click.Context):
+    """
+    Interactive Shell for Rapyuta.io
+    """
+    start_shell(ctx)
 
 
-@click.command('upload')
-@click.option('--tree-names', type=click.STRING, multiple=True, default=[], help='Directory names to upload')
-@click.option('--recreate', '--delete-existing', 'delete_existing', is_flag=True,
-              help='Overwrite existing parameter tree')
-@click.option('-f', '--force', '--silent', 'silent', is_flag=True, default=False, help="Skip confirmation")
-@click.argument('path', type=click.Path(exists=True))
-def upload_configurations(path: str, tree_names: typing.Tuple[str] = None, delete_existing: bool = False,
-                          silent: bool = False) -> None:
+@click.command(
+    'repl',
+    cls=HelpColorsCommand,
+    help_headers_color='yellow',
+    help_options_color='green',
+    hidden=True
+)
+@click.pass_context
+def deprecated_repl(ctx: click.Context):
     """
-    Upload a set of Configuration Parameter directory trees.
+    [Deprecated] Use "rio shell" instead
     """
-    trees = filter_trees(path, tree_names)
+    start_shell(ctx)
+
+
+def start_shell(ctx: click.Context):
+    prompt_config = _parse_config(ctx.obj)
+    while True:
+        try:
+            repl(click.get_current_context(), prompt_kwargs=prompt_config)
+        except Exception as e:
+            click.secho(str(e), fg='red')
+        else:
+            break
+
+
+def _parse_config(config: Configuration) -> dict:
+    history_path = os.path.join(click.get_app_dir(config.APP_NAME), "history")
+    default_prompt_kwargs = {
+        'history': ThreadedHistory(FileHistory(history_path)),
+        'message': prompt_callback,
+        'enable_suspend': True
+    }
+
+    shell_config = config.data.get('shell', {})
 
-    click.secho('Following Trees will be uploaded')
-    click.secho('')
-    display_trees(path, trees)
-
-    if not silent:
-        click.confirm('Do you want to proceed?', default=True, abort=True)
-
-    try:
-        client = new_client()
-        with spinner():
-            client.upload_configurations(rootdir=path, tree_names=trees, delete_existing_trees=delete_existing,
-                                         as_folder=True)
-
-        click.secho('✅ Configuration parameters uploaded successfully', fg='green')
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
+    return {**default_prompt_kwargs, **shell_config}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/parameter/utils.py` & `rapyuta-io-cli-3.0.0/riocli/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/project/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/project/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_help_colors import HelpColorsGroup
 
 from riocli.project.create import create_project
 from riocli.project.delete import delete_project
+from riocli.project.features import features
 from riocli.project.inspect import inspect_project
 from riocli.project.list import list_project
 from riocli.project.select import select_project
 
 
 @click.group(
     invoke_without_command=False,
@@ -35,7 +36,8 @@
 
 
 project.add_command(list_project)
 project.add_command(create_project)
 project.add_command(delete_project)
 project.add_command(select_project)
 project.add_command(inspect_project)
+project.add_command(features)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/project/delete.py` & `rapyuta-io-cli-3.0.0/riocli/project/features/vpn.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,49 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
-from click_spinner import spinner
 
-from riocli.config import new_client
+from riocli.config import new_v2_client
 from riocli.project.util import name_to_guid
 
 
-@click.command('delete')
-@click.option('--force', '-f', 'force', is_flag=True, help='Skip confirmation')
+@click.command('vpn')
 @click.argument('project-name', type=str)
+@click.argument('enable', type=bool)
 @name_to_guid
-def delete_project(force: bool, project_name: str, project_guid: str) -> None:
+def vpn(project_name: str, project_guid: str, enable: bool) -> None:
     """
-    Deletes the project from the Platform
+    Enable or disable VPN on a project
+
+    Example: rio project features vpn "my-project" true
     """
-    if not force:
-        click.confirm('Deleting project {} ({})'.format(project_name, project_guid), abort=True)
+    client = new_v2_client(with_project=False)
+
+    body = {
+        "metadata": {
+            "projectGUID": project_guid
+        },
+        "spec": {
+            "features": {
+                "vpn": enable
+            }
+        }
+    }
 
     try:
-        client = new_client(with_project=False)
-        with spinner():
-            client.delete_project(project_guid)
-        click.secho('Project deleted successfully!', fg='green')
+        r = client.update_project(project_guid, body)
     except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
+        click.secho("❌ Failed: {}".format(e), fg='red')
+        raise SystemExit(1) from e
+
+    click.secho("✅ VPN has been {}".format("enabled" if enable else "disabled"), fg='green')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/project/list.py` & `rapyuta-io-cli-3.0.0/riocli/project/select.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,51 +7,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import typing
-
 import click
-from rapyuta_io import Project
 
-from riocli.config import new_client
-from riocli.utils import tabulate_data
+from riocli.project.util import name_to_guid
+from riocli.utils.context import get_root_context
 
 
-@click.command('list')
+@click.command('select')
+@click.argument('project-name', type=str)
+@name_to_guid
 @click.pass_context
-def list_project(ctx: click.Context) -> None:
+def select_project(ctx: click.Context, project_name: str,
+                   project_guid: str) -> None:
     """
-    List all the projects you are part of
+    Sets the given project in the CLI context. All other resources use this project to act upon.
     """
-    try:
-        client = new_client(with_project=False)
-        projects = client.list_projects()
-        projects = sorted(projects, key=lambda p: p.name.lower())
-        current = ctx.obj.data.get('project_id', None)
-        _display_project_list(projects, current, show_header=True)
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
-
-
-def _display_project_list(projects: typing.List[Project], current: str = None, show_header: bool = True) -> None:
-    headers = []
-    if show_header:
-        headers = ('Project ID', 'Project Name', 'Created At', 'Creator')
-
-    data = []
-    for project in projects:
-        fg = None
-        if project.guid == current:
-            fg = 'green'
-
-        data.append([
-            click.style(v, fg=fg)
-            for v in (project.guid, project.name,
-                      project.created_at, project.creator)
-        ])
-
-    tabulate_data(data, headers)
+    ctx = get_root_context(ctx)
+    ctx.obj.data['project_id'] = project_guid
+    ctx.obj.data['project_name'] = project_name
+    ctx.obj.save()
+    click.secho(
+        'Project {} ({}) is selected!'.format(project_name, project_guid),
+        fg='green')
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/project/model.py` & `rapyuta-io-cli-3.0.0/riocli/static_route/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,50 +9,47 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
 
-from rapyuta_io import Project as v1Project, Client
+from rapyuta_io import Client
+from rapyuta_io.clients.static_route import StaticRoute as v1StaticRoute
 
+from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
-from riocli.jsonschema.validate import validate_manifest, load_schema
 
 
-class Project(Model):
-
+class StaticRoute(Model):
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
-        guid, obj = self.rc.find_depends(
-            {"kind": "project", "nameOrGUID": self.metadata.name})
-        if not guid:
+        _, static_route = self.rc.find_depends({'kind': 'staticroute',
+                                                'nameOrGUID': self.metadata.name})
+        if not static_route:
             return False
 
-        return obj
+        return static_route
 
-    def create_object(self, client: Client) -> v1Project:
-        project = client.create_project(self.to_v1())
-        return project
+    def create_object(self, client: Client) -> v1StaticRoute:
+        static_route = client.create_static_route(self.metadata.name)
+        return static_route
 
-    def update_object(self, client: Client, obj: typing.Any) -> typing.Any:
+    def update_object(self, client: Client, obj: typing.Any) -> None:
         pass
 
-    def delete_object(self, client: Client, obj: typing.Any) -> typing.Any:
-        obj.delete()
-
-    def to_v1(self) -> v1Project:
-        return v1Project(self.metadata.name)
+    def delete_object(self, client: Client, obj: typing.Any):
+        client.delete_static_route(obj.guid)
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
     @staticmethod
     def validate(data):
         """
-        Validates if project data is matching with its corresponding schema
+        Validates if static route data is matching with its corresponding schema
         """
-        schema = load_schema('project')
-        validate_manifest(instance=data, schema=schema)
+        schema = load_schema('static_route')
+        schema.validate(data)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/project/select.py` & `rapyuta-io-cli-3.0.0/riocli/organization/select.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,46 @@
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2023 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 
-from riocli.project.util import name_to_guid
+from riocli.auth.util import select_project
+from riocli.project.util import name_to_organization_guid
 from riocli.utils.context import get_root_context
 
 
 @click.command('select')
-@click.argument('project-name', type=str)
-@name_to_guid
+@click.argument('organization-name', type=str)
 @click.pass_context
-def select_project(ctx: click.Context, project_name: str, project_guid: str) -> None:
+@name_to_organization_guid
+def select_organization(ctx: click.Context, organization_name: str, organization_guid: str) -> None:
     """
-    Sets the given project in the CLI context. All other resources use this project to act upon.
+    Sets the current organization to the one provided
+    in the argument and prompts you to select a new project
+    in the changed organization
+
+    Example:
+
+        rio organization select other-org
     """
     ctx = get_root_context(ctx)
-    ctx.obj.data['project_id'] = project_guid
-    ctx.obj.data['project_name'] = project_name
+
+    if ctx.obj.data['organization_id'] == organization_guid:
+        click.secho("You are already in the '{}' organization".format(organization_name), fg='green')
+        return
+
+    ctx.obj.data['organization_id'] = organization_guid
+    ctx.obj.data['organization_name'] = organization_name
+
+    select_project(ctx.obj, organization=organization_guid)
+
     ctx.obj.save()
-    click.secho('Project {} ({}) is selected!'.format(project_name, project_guid), fg='green')
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/project/util.py` & `rapyuta-io-cli-3.0.0/riocli/project/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 # limitations under the License.
 import functools
 import typing
 
 import click
 from rapyuta_io import Client
 
-from riocli.config import new_client
+from riocli.config import new_client, new_v2_client
 from riocli.utils.selector import show_selection
+from riocli.v2client import Client as v2Client
 
 
 def name_to_guid(f: typing.Callable) -> typing.Callable:
     @functools.wraps(f)
     def decorated(**kwargs: typing.Any):
-        client = new_client(with_project=False)
+        client = new_v2_client(with_project=False)
         name = kwargs.pop('project_name')
         guid = None
 
         if name.startswith('project-'):
             guid = name
             name = None
 
@@ -45,58 +46,62 @@
         kwargs['project_name'] = name
         kwargs['project_guid'] = guid
         f(**kwargs)
 
     return decorated
 
 
-def find_project_guid(client: Client, name: str) -> str:
-    projects = client.list_projects()
+def find_project_guid(client: v2Client, name: str,
+                      organization: str = None) -> str:
+    projects = client.list_projects(organization_guid=organization)
     for project in projects:
-        if project.name == name:
-            return project.guid
+        if project.metadata.name == name:
+            return project.metadata.guid
 
     raise ProjectNotFound()
 
 
-def get_project_name(client: Client, guid: str) -> str:
+def get_project_name(client: v2Client, guid: str) -> str:
     project = client.get_project(guid)
-    return project.name
+    return project.metadata.name
 
 
 def find_organization_guid(client: Client, name: str) -> str:
     organizations = client.get_user_organizations()
     options = {}
 
     for organization in organizations:
         if organization.name == name:
-            options[organization.guid] = '{} ({})'.format(organization.name, organization.url)
+            options[organization.guid] = '{} ({})'.format(organization.name,
+                                                          organization.url)
 
     if len(options) == 1:
         return list(options.keys())[0]
 
     if len(options) == 0:
         raise Exception("User is not part of organization: {}".format(name))
 
-    choice = show_selection(options, header='Following packages were found with the same name')
+    choice = show_selection(options,
+                            header='Following packages were found with the same name')
     return choice
 
 
 def get_organization_name(client: Client, guid: str) -> str:
     organizations = client.get_user_organizations()
     for organization in organizations:
         if organization.guid == guid:
             return organization.name
 
-    raise OrganizationNotFound("User is not part of organization with guid: {}".format(guid))
+    raise OrganizationNotFound(
+        "User is not part of organization with guid: {}".format(guid))
 
 
 def name_to_organization_guid(f: typing.Callable) -> typing.Callable:
     @functools.wraps(f)
-    def decorated(**kwargs: typing.Any):
+    def decorated(*args: typing.Any, **kwargs: typing.Any):
         client = new_client(with_project=False)
         name = kwargs.get('organization_name')
         guid = None
 
         if name:
             try:
                 if name.startswith('org-'):
@@ -105,15 +110,15 @@
                 else:
                     guid = find_organization_guid(client, name)
             except Exception as e:
                 click.secho(str(e), fg='red')
                 raise SystemExit(1)
         kwargs['organization_name'] = name
         kwargs['organization_guid'] = guid
-        f(**kwargs)
+        f(*args, **kwargs)
 
     return decorated
 
 
 class ProjectNotFound(Exception):
     def __init__(self, message='project not found'):
         self.message = message
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/rosbag/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/rosbag/blob.py` & `rapyuta-io-cli-3.0.0/riocli/rosbag/blob.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/rosbag/job.py` & `rapyuta-io-cli-3.0.0/riocli/rosbag/job.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/secret/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/secret/create.py` & `rapyuta-io-cli-3.0.0/riocli/secret/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/secret/delete.py` & `rapyuta-io-cli-3.0.0/riocli/secret/delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from click_spinner import spinner
 
 from riocli.config import new_client
 from riocli.secret.util import name_to_guid
 
 
 @click.command('delete')
-@click.option('--force', '-f', 'force', is_flag=True, default=False, help='Skip confirmation')
+@click.option('--force', '-f', '--silent', 'force', is_flag=True,
+              default=False, help='Skip confirmation')
 @click.argument('secret-name', type=str)
 @name_to_guid
 def delete_secret(force: str, secret_name: str, secret_guid: str) -> None:
     """
     Deletes the secret resource from the Platform
     """
     if not force:
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/secret/docker_secret.py` & `rapyuta-io-cli-3.0.0/riocli/secret/docker_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/secret/import_secret.py` & `rapyuta-io-cli-3.0.0/riocli/secret/import_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/secret/list.py` & `rapyuta-io-cli-3.0.0/riocli/secret/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/secret/model.py` & `rapyuta-io-cli-3.0.0/riocli/secret/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 import typing
 
 from rapyuta_io import Secret as v1Secret, SecretConfigDocker, \
     SecretConfigSourceBasicAuth, \
     SecretConfigSourceSSHAuth, Client
 
+from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
-from riocli.jsonschema.validate import load_schema, validate_manifest
 
 
 class Secret(Model):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
@@ -75,8 +75,8 @@
 
     @staticmethod
     def validate(data):
         """
         Validates if secret data is matching with its corresponding schema
         """
         schema = load_schema('secret')
-        validate_manifest(instance=data, schema=schema)
+        schema.validate(data)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/secret/source_secret.py` & `rapyuta-io-cli-3.0.0/riocli/secret/source_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/secret/util.py` & `rapyuta-io-cli-3.0.0/riocli/secret/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/shell/prompt.py` & `rapyuta-io-cli-3.0.0/riocli/utils/context.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,13 +7,21 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import click
+from click import Context
 
 
-@click.pass_context
-def prompt_callback(ctx: click.Context) -> str:
-    return '{} > '.format(ctx.obj.data['project_name'])
+def get_root_context(ctx: Context) -> Context:
+    """
+    get_root_context figures out the top-level Context from the given context by walking down the linked-list.
+
+    https://click.palletsprojects.com/en/8.0.x/complex/#contexts
+    """
+    while True:
+        if ctx.parent is None:
+            return ctx
+
+        ctx = ctx.parent
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/static_route/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/static_route/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/static_route/create.py` & `rapyuta-io-cli-3.0.0/riocli/static_route/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/static_route/delete.py` & `rapyuta-io-cli-3.0.0/riocli/static_route/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,35 +7,75 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import functools
+import typing
+
 import click
-from click_spinner import spinner
+from rapyuta_io import Client
+from rapyuta_io.clients.static_route import StaticRoute
 
 from riocli.config import new_client
-from riocli.static_route.util import name_to_guid
-
 
-@click.command('delete')
-@click.option('--force', '-f', is_flag=True, default=False, help='Skip confirmation')
-@click.argument('static-route', type=str)
-@name_to_guid
-def delete_static_route(static_route: str, static_route_guid: str, force: bool) -> None:
-    """
-    Deletes the static route resource from the Platform
-    """
-
-    if not force:
-        click.confirm('Deleting static route {} ({})'.format(static_route, static_route_guid),
-                      abort=True)
 
-    try:
+def name_to_guid(f: typing.Callable) -> typing.Callable:
+    @functools.wraps(f)
+    def decorated(**kwargs: typing.Any):
         client = new_client()
-        with spinner():
-            client.delete_static_route(static_route_guid)
-        click.secho('Static Route deleted successfully!', fg='green')
-    except Exception as e:
-        click.secho(str(e), fg='red')
-        raise SystemExit(1)
+        name = kwargs.pop('static_route')
+        guid = None
+
+        if name.startswith('staticroute-'):
+            guid = name
+            name = None
+
+        if name is None:
+            name = get_static_route_name(client, guid)
+
+        if guid is None:
+            guid = find_static_route_guid(client, name)
+
+        kwargs['static_route'] = name
+        kwargs['static_route_guid'] = guid
+        f(**kwargs)
+
+    return decorated
+
+
+def get_static_route_name(client: Client, guid: str) -> str:
+    static_route = client.get_static_route(guid)
+    return static_route.urlPrefix.split("-")[0]
+
+
+def find_static_route_guid(client: Client, name: str) -> str:
+    routes = client.get_all_static_routes()
+    for route in routes:
+        if route.urlPrefix == name or route.urlString == name:
+            return route.guid
+
+    raise StaticRouteNotFound()
+
+
+def repr_static_routes(routes: typing.List[StaticRoute]) -> None:
+    header = '{:<36} {:<25} {:36} {:36} {:32}'.format(
+        'Static Route ID',
+        'Name',
+        'Full URL',
+        'Creator',
+        'Created At',
+    )
+    click.echo(click.style(header, fg='yellow'))
+    for route in routes:
+        click.secho(
+            '{:<36} {:<25} {:36} {:36} {:32}'.
+            format(route.guid, route.urlPrefix, route.urlString, route.creator,
+                   route.CreatedAt))
+
+
+class StaticRouteNotFound(Exception):
+    def __init__(self, message='secret not found'):
+        self.message = message
+        super().__init__(self.message)
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/static_route/inspect.py` & `rapyuta-io-cli-3.0.0/riocli/static_route/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/static_route/list.py` & `rapyuta-io-cli-3.0.0/riocli/static_route/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/utils/__init__.py` & `rapyuta-io-cli-3.0.0/riocli/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,38 +24,56 @@
 import yaml
 from click_help_colors import HelpColorsGroup
 from tabulate import tabulate
 
 
 def inspect_with_format(obj: typing.Any, format_type: str):
     if format_type == 'json':
-        click.echo(json.dumps(obj, indent=4))
+        click.echo_via_pager(json.dumps(obj, indent=4))
     elif format_type == 'yaml':
-        click.echo(yaml.dump(obj, allow_unicode=True))
+        click.echo_via_pager(yaml.dump(obj, allow_unicode=True))
     else:
         raise Exception('Invalid format')
 
 
 def dump_all_yaml(objs: typing.List):
     """
     Dump multiple documents as YAML separated by triple dash (---)
     """
-    click.echo(yaml.safe_dump_all(objs, allow_unicode=True,
-                                  explicit_start=True))
+    click.echo_via_pager(
+        yaml.safe_dump_all(
+            documents=objs,
+            allow_unicode=True,
+            explicit_start=True
+        )
+    )
 
 
-def run_bash(cmd, bg=False):
+def run_bash_with_return_code(cmd, bg=False) -> (str, int):
     cmd_parts = shlex.split(cmd)
 
     if bg is True:
-        bg_output = subprocess.Popen(cmd_parts)
-        output = str(bg_output.stdout).strip()
+        output = subprocess.Popen(cmd_parts)
+        stdout = str(output.stdout).strip()
+        ret_code = output.returncode
     else:
-        output = subprocess.run(cmd_parts, stdout=subprocess.PIPE).stdout.decode('utf-8')
-    return output.strip()
+        output = subprocess.run(cmd_parts, stdout=subprocess.PIPE)
+        stdout = output.stdout.decode('utf-8')
+        ret_code = output.returncode
+
+    return stdout.strip(), ret_code
+
+
+def run_bash(cmd, bg=False) -> str:
+    """
+    Runs a bash command and returns the output only
+    """
+    output, _ = run_bash_with_return_code(cmd, bg)
+
+    return output
 
 
 riocli_group_opts = {
     'invoke_without_command': True,
     'cls': HelpColorsGroup,
     'help_headers_color': 'yellow',
     'help_options_color': 'green'
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/utils/execute.py` & `rapyuta-io-cli-3.0.0/riocli/utils/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from riocli.config import Configuration, new_client
 
 _CLOUD_RUN_REMOTE_COMMAND = '{}/serviceinstance/{}/cmd'
 
 
 def run_on_cloud(deployment_guid: str, comp_id: str, exec_id: str, pod_name: str, command: typing.List[str]) -> (
-str, str):
+        str, str):
     """
     run_on_cloud uses the RunCommand API of the IOBroker to execute arbitrary commands on the cloud deployment
     containers.
     """
     config = Configuration()
     rest = RestClient(_run_cloud_url(config, deployment_guid)).headers(config.get_auth_header()).method(HttpMethod.PUT)
     resp = rest.execute(payload=_run_cloud_data(comp_id, exec_id, pod_name, command))
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/utils/mermaid.py` & `rapyuta-io-cli-3.0.0/riocli/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/utils/selector.py` & `rapyuta-io-cli-3.0.0/riocli/utils/selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     fmt = '{}\n{}'.format(fmt, prompt)
     choice = click.prompt(fmt, type=types.IntParamType())
     return ranger[choice - 1]
 
 
 def _show_selection_dict(ranger: dict, header: str, prompt: str):
     options = []
-    fmt = header
+    fmt = click.style(header, fg='yellow')
     for idx, key in enumerate(ranger):
         options.append(key)
         fmt = '{}\n{}) {} - {}'.format(fmt, idx + 1, key, ranger[key])
 
-    fmt = '{}\n{}'.format(fmt, prompt)
+    fmt = '{}\n{}'.format(fmt, click.style(prompt, fg='blue'))
     choice = click.prompt(fmt, type=types.IntParamType())
     return options[choice - 1]
```

### Comparing `rapyuta-io-cli-2.0.2/riocli/utils/spinner.py` & `rapyuta-io-cli-3.0.0/riocli/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/riocli/utils/ssh_tunnel.py` & `rapyuta-io-cli-3.0.0/riocli/utils/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-2.0.2/setup.py` & `rapyuta-io-cli-3.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 
 from setuptools import setup, find_packages
 
 version = re.search(
     '^__version__\s*=\s*"(.*)"', open("riocli/bootstrap.py").read(), re.M
 ).group(1)
 
-
 with open("README.md", "rb") as f:
     long_descr = f.read().decode("utf-8")
 
-
 setup(
     name="rapyuta-io-cli",
     packages=find_packages(),
     package_data={
         'riocli': [
             'apply/manifests/*.yaml',
             'jsonschema/schemas/*.yaml'
@@ -54,11 +52,12 @@
         "setuptools",
         "six>=1.13.0",
         "tabulate>=0.8.0",
         "urllib3>=1.23",
         "pyrfc3339>=1.1",
         "directory-tree>=0.0.3.1",
         "yaspin>=2.3.0",
-        "jsonschema>=4.0.0"
+        "jsonschema>=4.0.0",
+        "waiting>=1.4.1"
     ],
     setup_requires=["flake8"],
 )
```

