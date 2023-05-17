# Comparing `tmp/zipreport-lib-1.0.1.tar.gz` & `tmp/zipreport-lib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipreport-lib-1.0.1.tar", last modified: Mon May 15 15:59:25 2023, max compression
+gzip compressed data, was "zipreport-lib-1.0.2.tar", last modified: Wed May 17 16:23:16 2023, max compression
```

## Comparing `zipreport-lib-1.0.1.tar` & `zipreport-lib-1.0.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1088 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/LICENSE
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4883 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3821 2022-05-09 17:32:34.000000 zipreport-lib-1.0.1/README.md
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       38 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/setup.cfg
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2551 2023-05-15 15:58:28.000000 zipreport-lib-1.0.1/setup.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.141871 zipreport-lib-1.0.1/tests/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-07-22 16:58:01.000000 zipreport-lib-1.0.1/tests/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/tests/fileutils/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-07-22 12:25:07.000000 zipreport-lib-1.0.1/tests/fileutils/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5235 2020-07-24 10:35:50.000000 zipreport-lib-1.0.1/tests/fileutils/basefs.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      756 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/fileutils/basezip.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3454 2020-11-22 04:19:51.000000 zipreport-lib-1.0.1/tests/fileutils/test_diskfs.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1339 2020-07-23 10:00:42.000000 zipreport-lib-1.0.1/tests/fileutils/test_pathcache.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2547 2020-07-24 18:01:09.000000 zipreport-lib-1.0.1/tests/fileutils/test_zip.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1539 2020-07-24 10:35:50.000000 zipreport-lib-1.0.1/tests/fileutils/test_zipfs.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/tests/processors/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/processors/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      735 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/processors/base.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2843 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/processors/test_mime.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/tests/render/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      772 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/base.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/tests/render/filters/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/filters/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    16028 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/filters/base.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1968 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/filters/test_jinjafilters.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      590 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/test_jinjaloader.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1673 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/render/test_jinjarender.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/tests/report/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-07-23 07:55:01.000000 zipreport-lib-1.0.1/tests/report/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3281 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/report/test_builder.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2147 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/report/test_job.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1515 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/tests/report/test_loader.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      568 2020-11-22 04:42:34.000000 zipreport-lib-1.0.1/tests/utils.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      135 2022-05-09 17:01:37.000000 zipreport-lib-1.0.1/zipreport/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/cli/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/cli/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5221 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/cli/console.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/cli/debug/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/cli/debug/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     8476 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/cli/debug/server.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/fileutils/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       96 2020-07-23 04:44:59.000000 zipreport-lib-1.0.1/zipreport/fileutils/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/fileutils/backend/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-07-23 04:38:48.000000 zipreport-lib-1.0.1/zipreport/fileutils/backend/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4140 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/fileutils/backend/zip.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4801 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/fileutils/diskfs.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1398 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/fileutils/interface.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3630 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/fileutils/pathcache.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3838 2021-11-14 16:26:47.000000 zipreport-lib-1.0.1/zipreport/fileutils/zipfs.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/misc/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       27 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/misc/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      655 2020-11-22 04:42:34.000000 zipreport-lib-1.0.1/zipreport/misc/html.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/processors/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      200 2021-11-14 16:07:06.000000 zipreport-lib-1.0.1/zipreport/processors/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      143 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/processors/interface.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3001 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/processors/mime.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2211 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/processors/weasyprint.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3075 2021-11-14 16:07:06.000000 zipreport-lib-1.0.1/zipreport/processors/wkhtmltopdf.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4873 2020-10-14 10:13:11.000000 zipreport-lib-1.0.1/zipreport/processors/zipreport.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/report/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      207 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/report/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5827 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/report/builder.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1274 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/report/const.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5884 2020-11-22 04:56:45.000000 zipreport-lib-1.0.1/zipreport/report/job.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2603 2020-10-14 06:19:51.000000 zipreport-lib-1.0.1/zipreport/report/loader.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1901 2020-11-29 15:58:21.000000 zipreport-lib-1.0.1/zipreport/report/reportfile.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/template/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       80 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/template/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport/template/jinja/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/template/jinja/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4985 2022-05-09 17:10:20.000000 zipreport-lib-1.0.1/zipreport/template/jinja/filters.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      913 2020-10-14 06:18:55.000000 zipreport-lib-1.0.1/zipreport/template/jinjaloader.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3242 2020-11-29 15:58:28.000000 zipreport-lib-1.0.1/zipreport/template/jinjarender.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      126 2023-05-15 15:59:08.000000 zipreport-lib-1.0.1/zipreport/version.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3195 2021-11-14 16:07:06.000000 zipreport-lib-1.0.1/zipreport/zipreport.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-15 15:59:25.145871 zipreport-lib-1.0.1/zipreport_lib.egg-info/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4883 2023-05-15 15:59:25.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1929 2023-05-15 15:59:25.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2023-05-15 15:59:25.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       58 2023-05-15 15:59:25.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/entry_points.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2022-05-09 03:05:06.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/not-zip-safe
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       61 2023-05-15 15:59:25.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/requires.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       16 2023-05-15 15:59:25.000000 zipreport-lib-1.0.1/zipreport_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.052072 zipreport-lib-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-17 16:23:16.052072 zipreport-lib-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 16:23:16.052072 zipreport-lib-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.036072 zipreport-lib-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.040072 zipreport-lib-1.0.2/tests/fileutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/basefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/basezip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/test_diskfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/test_pathcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/fileutils/test_zipfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.040072 zipreport-lib-1.0.2/tests/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/processors/test_mime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.040072 zipreport-lib-1.0.2/tests/render/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.040072 zipreport-lib-1.0.2/tests/render/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/filters/test_jinjafilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/test_jinjaloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/render/test_jinjarender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/tests/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/report/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/report/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/report/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/zipreport/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/zipreport/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/cli/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/zipreport/cli/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/cli/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/cli/debug/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/zipreport/fileutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/zipreport/fileutils/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/backend/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/diskfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/pathcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/fileutils/zipfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.044072 zipreport-lib-1.0.2/zipreport/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/misc/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.048072 zipreport-lib-1.0.2/zipreport/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/processors/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/processors/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/processors/weasyprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/processors/wkhtmltopdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/processors/zipreport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.048072 zipreport-lib-1.0.2/zipreport/report/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/report/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/report/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/report/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/report/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/report/reportfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.048072 zipreport-lib-1.0.2/zipreport/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.048072 zipreport-lib-1.0.2/zipreport/template/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/template/jinja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/template/jinja/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/template/jinjaloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/template/jinjarender.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-17 16:23:00.000000 zipreport-lib-1.0.2/zipreport/zipreport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:23:16.052072 zipreport-lib-1.0.2/zipreport_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-17 16:23:15.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-17 16:23:16.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:23:15.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 16:23:15.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:23:15.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-17 16:23:15.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 16:23:15.000000 zipreport-lib-1.0.2/zipreport_lib.egg-info/top_level.txt
```

### Comparing `zipreport-lib-1.0.1/LICENSE` & `zipreport-lib-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/PKG-INFO` & `zipreport-lib-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: zipreport-lib
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python HTML to PDF reporting engine
 Home-page: https://github.com/zipreport/zipreport
 Author: Joao Pinheiro
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://zipreport.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/zipreport/zipreport
 Project-URL: Tracker, https://github.com/zipreport/zipreport/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -128,9 +127,7 @@
 
 
 ### Documentation
 
 Detailed documentation on usage and report building is available on the [project documentation](https://zipreport.readthedocs.io/en/latest/).
 
 
-
-
```

### Comparing `zipreport-lib-1.0.1/README.md` & `zipreport-lib-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/setup.py` & `zipreport-lib-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/fileutils/basefs.py` & `zipreport-lib-1.0.2/tests/fileutils/basefs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/fileutils/basezip.py` & `zipreport-lib-1.0.2/tests/fileutils/basezip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/fileutils/test_diskfs.py` & `zipreport-lib-1.0.2/tests/fileutils/test_diskfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/fileutils/test_pathcache.py` & `zipreport-lib-1.0.2/tests/fileutils/test_pathcache.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/fileutils/test_zip.py` & `zipreport-lib-1.0.2/tests/fileutils/test_zip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/fileutils/test_zipfs.py` & `zipreport-lib-1.0.2/tests/fileutils/test_zipfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/processors/base.py` & `zipreport-lib-1.0.2/tests/processors/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/processors/test_mime.py` & `zipreport-lib-1.0.2/tests/processors/test_mime.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/render/base.py` & `zipreport-lib-1.0.2/tests/render/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/render/filters/base.py` & `zipreport-lib-1.0.2/tests/render/filters/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/render/filters/test_jinjafilters.py` & `zipreport-lib-1.0.2/tests/render/filters/test_jinjafilters.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/render/test_jinjaloader.py` & `zipreport-lib-1.0.2/tests/render/test_jinjaloader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/render/test_jinjarender.py` & `zipreport-lib-1.0.2/tests/render/test_jinjarender.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/report/test_builder.py` & `zipreport-lib-1.0.2/tests/report/test_builder.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/report/test_job.py` & `zipreport-lib-1.0.2/tests/report/test_job.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/report/test_loader.py` & `zipreport-lib-1.0.2/tests/report/test_loader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/tests/utils.py` & `zipreport-lib-1.0.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/cli/console.py` & `zipreport-lib-1.0.2/zipreport/cli/console.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/cli/debug/server.py` & `zipreport-lib-1.0.2/zipreport/cli/debug/server.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/fileutils/backend/zip.py` & `zipreport-lib-1.0.2/zipreport/fileutils/backend/zip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/fileutils/diskfs.py` & `zipreport-lib-1.0.2/zipreport/fileutils/diskfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/fileutils/interface.py` & `zipreport-lib-1.0.2/zipreport/fileutils/interface.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/fileutils/pathcache.py` & `zipreport-lib-1.0.2/zipreport/fileutils/pathcache.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/fileutils/zipfs.py` & `zipreport-lib-1.0.2/zipreport/fileutils/zipfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/misc/html.py` & `zipreport-lib-1.0.2/zipreport/misc/html.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/processors/mime.py` & `zipreport-lib-1.0.2/zipreport/processors/mime.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/processors/weasyprint.py` & `zipreport-lib-1.0.2/zipreport/processors/weasyprint.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/processors/wkhtmltopdf.py` & `zipreport-lib-1.0.2/zipreport/processors/wkhtmltopdf.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/processors/zipreport.py` & `zipreport-lib-1.0.2/zipreport/processors/zipreport.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/report/builder.py` & `zipreport-lib-1.0.2/zipreport/report/builder.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/report/const.py` & `zipreport-lib-1.0.2/zipreport/report/const.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/report/job.py` & `zipreport-lib-1.0.2/zipreport/report/job.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/report/loader.py` & `zipreport-lib-1.0.2/zipreport/report/loader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/report/reportfile.py` & `zipreport-lib-1.0.2/zipreport/report/reportfile.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/template/jinja/filters.py` & `zipreport-lib-1.0.2/zipreport/template/jinja/filters.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/template/jinjaloader.py` & `zipreport-lib-1.0.2/zipreport/template/jinjaloader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/template/jinjarender.py` & `zipreport-lib-1.0.2/zipreport/template/jinjarender.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport/zipreport.py` & `zipreport-lib-1.0.2/zipreport/zipreport.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-1.0.1/zipreport_lib.egg-info/PKG-INFO` & `zipreport-lib-1.0.2/zipreport_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: zipreport-lib
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python HTML to PDF reporting engine
 Home-page: https://github.com/zipreport/zipreport
 Author: Joao Pinheiro
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://zipreport.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/zipreport/zipreport
 Project-URL: Tracker, https://github.com/zipreport/zipreport/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -128,9 +127,7 @@
 
 
 ### Documentation
 
 Detailed documentation on usage and report building is available on the [project documentation](https://zipreport.readthedocs.io/en/latest/).
 
 
-
-
```

### Comparing `zipreport-lib-1.0.1/zipreport_lib.egg-info/SOURCES.txt` & `zipreport-lib-1.0.2/zipreport_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

