# Comparing `tmp/ayugespidertools-2.1.0.tar.gz` & `tmp/ayugespidertools-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-2.1.0.tar", max compression
+gzip compressed data, was "ayugespidertools-3.0.1.tar", max compression
```

## Comparing `ayugespidertools-2.1.0.tar` & `ayugespidertools-3.0.1.tar`

### file list

```diff
@@ -1,117 +1,85 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-2.1.0/LICENSE
--rw-r--r--   0        0        0    13798 2023-04-27 03:19:49.000000 ayugespidertools-2.1.0/README.md
--rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-2.1.0/ayugespidertools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-2.1.0/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0      158 2023-04-25 08:54:15.594268 ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      536 2023-04-25 08:55:28.881319 ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc
--rw-r--r--   0        0        0      685 2023-04-25 08:54:15.595268 ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
--rw-r--r--   0        0        0     2860 2023-05-06 06:33:53.042068 ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
--rw-r--r--   0        0        0     1086 2023-04-25 08:54:15.618268 ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
--rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-2.1.0/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     4039 2023-05-06 06:32:50.000000 ayugespidertools-2.1.0/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-2.1.0/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0     3704 2023-04-21 05:52:41.000000 ayugespidertools-2.1.0/ayugespidertools/common/encryption.py
--rw-r--r--   0        0        0     6622 2023-04-25 02:55:24.000000 ayugespidertools-2.1.0/ayugespidertools/common/expend.py
--rw-r--r--   0        0        0     6885 2023-05-05 06:09:23.000000 ayugespidertools-2.1.0/ayugespidertools/common/mongodbpipe.py
--rw-r--r--   0        0        0    11765 2023-04-27 08:36:37.000000 ayugespidertools-2.1.0/ayugespidertools/common/multiplexing.py
--rw-r--r--   0        0        0    13474 2023-04-25 02:55:56.000000 ayugespidertools-2.1.0/ayugespidertools/common/mysqlerrhandle.py
--rw-r--r--   0        0        0    32707 2023-04-26 06:59:16.000000 ayugespidertools-2.1.0/ayugespidertools/common/params.py
--rw-r--r--   0        0        0     4264 2023-04-25 02:56:33.000000 ayugespidertools-2.1.0/ayugespidertools/common/spiderdbconf.py
--rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-2.1.0/ayugespidertools/common/sqlformat.py
--rw-r--r--   0        0        0     2368 2023-04-27 03:08:07.000000 ayugespidertools-2.1.0/ayugespidertools/common/typevars.py
--rw-r--r--   0        0        0    11325 2023-04-26 08:38:41.000000 ayugespidertools-2.1.0/ayugespidertools/common/utils.py
--rw-r--r--   0        0        0     3693 2023-04-25 02:57:48.000000 ayugespidertools-2.1.0/ayugespidertools/common/yidungap.py
--rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-2.1.0/ayugespidertools/config.py
--rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-2.1.0/ayugespidertools/formatdata.py
--rw-r--r--   0        0        0     7681 2023-04-25 03:03:41.000000 ayugespidertools-2.1.0/ayugespidertools/imgoperation.py
--rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-2.1.0/ayugespidertools/items.py
--rw-r--r--   0        0        0      898 2023-04-24 02:31:51.000000 ayugespidertools-2.1.0/ayugespidertools/middlewares.py
--rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-2.1.0/ayugespidertools/mongoclient.py
--rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-2.1.0/ayugespidertools/mysqlclient.py
--rw-r--r--   0        0        0     5431 2023-04-25 03:03:58.000000 ayugespidertools-2.1.0/ayugespidertools/oss.py
--rw-r--r--   0        0        0      802 2023-05-09 03:25:16.000000 ayugespidertools-2.1.0/ayugespidertools/pipelines.py
--rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/processmanager.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-2.1.0/ayugespidertools/request.py
--rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-2.1.0/ayugespidertools/rpa.py
--rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/runjs.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0      356 2023-04-26 08:48:02.859698 ayugespidertools-2.1.0/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1442 2023-04-25 08:54:13.045266 ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1068 2023-04-27 08:45:17.819120 ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
--rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0     1195 2023-04-24 02:25:23.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0      981 2023-04-25 08:58:10.179432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2248 2023-04-25 08:58:10.180432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc
--rw-r--r--   0        0        0     1742 2023-04-25 02:58:16.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0      374 2023-04-24 02:00:59.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/__init__.py
--rw-r--r--   0        0        0      475 2023-04-25 08:58:10.180432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7677 2023-04-27 07:35:53.380544 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc
--rw-r--r--   0        0        0     2200 2023-04-25 08:58:10.182432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc
--rw-r--r--   0        0        0    10519 2023-04-27 07:35:00.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
--rw-r--r--   0        0        0     4331 2023-04-25 02:58:59.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/requestslib.py
--rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0      481 2023-04-25 08:58:10.183432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3911 2023-04-25 08:58:10.184432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc
--rw-r--r--   0        0        0     3056 2023-04-26 08:48:05.030700 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc
--rw-r--r--   0        0        0     7795 2023-04-25 08:58:10.186432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc
--rw-r--r--   0        0        0     4228 2023-04-25 02:59:18.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2876 2023-04-26 02:43:33.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/private.py
--rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0      885 2023-04-25 08:58:19.202438 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/download/image.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0      173 2023-04-25 08:58:19.202438 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2624 2023-05-05 08:55:33.703084 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/__pycache__/asynced.cpython-38.pyc
--rw-r--r--   0        0        0     2971 2023-05-05 08:55:33.673084 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc
--rw-r--r--   0        0        0     1820 2023-04-25 08:58:19.205438 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc
--rw-r--r--   0        0        0     2114 2023-05-05 07:48:47.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/asynced.py
--rw-r--r--   0        0        0     2872 2023-05-04 09:09:37.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     1356 2023-04-25 03:00:42.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0    13396 2023-04-25 03:01:05.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0    11209 2023-04-25 08:58:19.207438 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4205 2023-05-09 01:56:17.338129 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc
--rw-r--r--   0        0        0      717 2023-04-25 08:58:19.219438 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc
--rw-r--r--   0        0        0     1998 2023-05-04 07:33:52.883359 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc
--rw-r--r--   0        0        0     3619 2023-04-25 08:58:19.223438 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc
--rw-r--r--   0        0        0     4379 2023-05-05 08:25:40.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2842 2023-05-04 02:07:52.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3794 2023-04-25 03:02:20.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     6737 2023-04-25 03:02:38.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0     4569 2023-04-25 08:54:13.141266 ayugespidertools-2.1.0/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      760 2023-04-25 08:54:14.345267 ayugespidertools-2.1.0/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
--rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-2.1.0/ayugespidertools/spiders.py
--rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/.gitignore
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      613 2023-04-25 05:46:03.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     4093 2023-04-25 04:01:51.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-2.1.0/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     6409 2023-04-25 08:46:25.000000 ayugespidertools-2.1.0/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1941 2023-04-25 08:47:57.000000 ayugespidertools-2.1.0/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-2.1.0/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-2.1.0/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.1.0/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0      155 2023-04-25 08:55:31.774321 ayugespidertools-2.1.0/ayugespidertools/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5350 2023-05-09 01:56:20.922134 ayugespidertools-2.1.0/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc
--rw-r--r--   0        0        0     5943 2023-05-09 01:54:08.000000 ayugespidertools-2.1.0/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-2.1.0/ayugespidertools/verificationcode.py
--rw-r--r--   0        0        0     3135 2023-05-09 01:05:39.000000 ayugespidertools-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    15541 1970-01-01 00:00:00.000000 ayugespidertools-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-3.0.1/LICENSE
+-rw-r--r--   0        0        0    13919 2023-05-17 08:57:35.000000 ayugespidertools-3.0.1/README.md
+-rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-3.0.1/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-3.0.1/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-3.0.1/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     3880 2023-05-12 03:27:33.000000 ayugespidertools-3.0.1/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-3.0.1/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0     3704 2023-04-21 05:52:41.000000 ayugespidertools-3.0.1/ayugespidertools/common/encryption.py
+-rw-r--r--   0        0        0     6622 2023-04-25 02:55:24.000000 ayugespidertools-3.0.1/ayugespidertools/common/expend.py
+-rw-r--r--   0        0        0     6407 2023-05-16 02:31:54.000000 ayugespidertools-3.0.1/ayugespidertools/common/mongodbpipe.py
+-rw-r--r--   0        0        0    15755 2023-05-17 02:27:54.000000 ayugespidertools-3.0.1/ayugespidertools/common/multiplexing.py
+-rw-r--r--   0        0        0    13558 2023-05-15 09:13:35.000000 ayugespidertools-3.0.1/ayugespidertools/common/mysqlerrhandle.py
+-rw-r--r--   0        0        0    32707 2023-04-26 06:59:16.000000 ayugespidertools-3.0.1/ayugespidertools/common/params.py
+-rw-r--r--   0        0        0     4264 2023-04-25 02:56:33.000000 ayugespidertools-3.0.1/ayugespidertools/common/spiderdbconf.py
+-rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-3.0.1/ayugespidertools/common/sqlformat.py
+-rw-r--r--   0        0        0     2368 2023-04-27 03:08:07.000000 ayugespidertools-3.0.1/ayugespidertools/common/typevars.py
+-rw-r--r--   0        0        0    11325 2023-05-17 02:11:53.000000 ayugespidertools-3.0.1/ayugespidertools/common/utils.py
+-rw-r--r--   0        0        0     3693 2023-04-25 02:57:48.000000 ayugespidertools-3.0.1/ayugespidertools/common/yidungap.py
+-rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-3.0.1/ayugespidertools/config.py
+-rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-3.0.1/ayugespidertools/formatdata.py
+-rw-r--r--   0        0        0     7681 2023-04-25 03:03:41.000000 ayugespidertools-3.0.1/ayugespidertools/imgoperation.py
+-rw-r--r--   0        0        0     4994 2023-05-16 09:33:56.000000 ayugespidertools-3.0.1/ayugespidertools/items.py
+-rw-r--r--   0        0        0      898 2023-04-24 02:31:51.000000 ayugespidertools-3.0.1/ayugespidertools/middlewares.py
+-rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-3.0.1/ayugespidertools/mongoclient.py
+-rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-3.0.1/ayugespidertools/mysqlclient.py
+-rw-r--r--   0        0        0     5431 2023-04-25 03:03:58.000000 ayugespidertools-3.0.1/ayugespidertools/oss.py
+-rw-r--r--   0        0        0      802 2023-05-10 05:50:47.000000 ayugespidertools-3.0.1/ayugespidertools/pipelines.py
+-rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/processmanager.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-3.0.1/ayugespidertools/request.py
+-rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-3.0.1/ayugespidertools/rpa.py
+-rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/runjs.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0     1195 2023-04-24 02:25:23.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0     1742 2023-04-25 02:58:16.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0      374 2023-04-24 02:00:59.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/netlib/__init__.py
+-rw-r--r--   0        0        0    10519 2023-04-27 07:35:00.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
+-rw-r--r--   0        0        0     4331 2023-04-25 02:58:59.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/netlib/requestslib.py
+-rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0     4228 2023-04-25 02:59:18.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2876 2023-04-26 02:43:33.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/private.py
+-rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/download/image.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0     2055 2023-05-16 09:34:33.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/asynced.py
+-rw-r--r--   0        0        0     2877 2023-05-16 08:50:58.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1361 2023-05-16 08:56:28.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0    12469 2023-05-16 08:48:07.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0     4371 2023-05-16 08:51:08.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2842 2023-05-04 02:07:52.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3854 2023-05-16 08:50:14.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     7167 2023-05-17 01:13:17.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-3.0.1/ayugespidertools/spiders.py
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      613 2023-05-11 03:15:22.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     1337 2023-05-14 07:20:40.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-3.0.1/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     6327 2023-05-17 06:24:21.000000 ayugespidertools-3.0.1/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1829 2023-05-17 06:32:25.000000 ayugespidertools-3.0.1/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-3.0.1/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-3.0.1/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.0.1/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0     5943 2023-05-09 01:54:08.000000 ayugespidertools-3.0.1/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-3.0.1/ayugespidertools/verificationcode.py
+-rw-r--r--   0        0        0     3074 2023-05-17 08:47:49.000000 ayugespidertools-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    15659 1970-01-01 00:00:00.000000 ayugespidertools-3.0.1/PKG-INFO
```

### Comparing `ayugespidertools-2.1.0/LICENSE` & `ayugespidertools-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/README.md` & `ayugespidertools-3.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 使用方法示例 `GIF` 如下：
 
 ![ayugespidertools.gif](https://raw.githubusercontent.com/shengchenyang/AyugeSpiderTools/main/examples/ayugespidertools-use.gif)
 
 对以上 `GIF` 中的步骤进行解释：
 
 ```shell
-# 注：更推荐使用 ayuge 的 cli 名称，输入体验更友好，（ayugespidertools 的 cli 则会在下一大版本中会剔除）。
+# 注：ayugespidertools 的 cli 已剔除，现只能使用 ayuge。
 
 # 查看库版本
 ayuge version
 
 # 创建项目
 ayuge startproject <project_name>
 
@@ -67,48 +67,51 @@
 
 # 替换(覆盖)为真实的配置 .conf 文件；
 # 这里是为了演示方便，正常情况是直接在 VIT 路径下的 .conf 配置文件填上相关配置即可
 cp /root/mytemp/.conf DemoSpider/VIT/.conf
 
 # 运行脚本
 scrapy crawl <spider_name>
+# 注：也可以使用 ayuge crawl <spider_name>
 ```
 
 具体使用方法请在 [DemoSpider 之 AyugeSpiderTools 工具应用示例](https://github.com/shengchenyang/DemoSpider) 项目中查看，目前已适配以下场景：
 
 ```diff
 # 采集数据存入 `Mysql` 的场景：
-- 1).demo_one: 配置根据本地 `settings` 的 `LOCAL_MYSQL_CONFIG` 中取值
++ 1).demo_one: 配置根据本地 `settings` 的 `LOCAL_MYSQL_CONFIG` 中取值
 + 3).demo_three: 配置根据 `consul` 的应用管理中心中取值
 + 5).demo_five: 异步存入 `Mysql` 的场景
 
 # 采集数据存入 `MongoDB` 的场景：
-- 2).demo_two: 采集数据存入 `MongoDB` 的场景（配置根据本地 `settings` 的 `LOCAL_MONGODB_CONFIG` 中取值）
++ 2).demo_two: 采集数据存入 `MongoDB` 的场景（配置根据本地 `settings` 的 `LOCAL_MONGODB_CONFIG` 中取值）
 + 4).demo_four: 采集数据存入 `MongoDB` 的场景（配置根据 `consul` 的应用管理中心中取值）
 + 6).demo_six: 异步存入 `MongoDB` 的场景
 
 # 将 `Scrapy` 的 `Request`，`FormRequest` 替换为其它工具实现的场景
 - 以上为使用 scrapy Request 的场景
 + 7).demo_seven: scrapy Request 替换为 requests 请求的场景(一般情况下不推荐使用，同步库
 + 会拖慢 scrapy 速度，可用于测试场景)
 
 + 8).demo_eight: 同时存入 Mysql 和 MongoDB 的场景
 
-- 9).demo_aiohttp_example: scrapy Request 替换为 aiohttp 请求的场景，提供了各种请求场景示例（GET,POST）
++ 9).demo_aiohttp_example: scrapy Request 替换为 aiohttp 请求的场景，提供了各种请求场景示例（GET,POST）
 + 10).demo_aiohttp_test: scrapy aiohttp 在具体项目中的使用方法示例
 
 + 11).demo_proxy_one: 快代理动态隧道代理示例
 + 12).demo_proxy_two: 测试快代理独享代理
 
 +13).demo_AyuTurboMysqlPipeline: mysql 同步连接池的示例
 +14).demo_crawl: 支持 scrapy CrawlSpider 的示例
 
 # 本库中给出支持 Item Loaders 特性的示例(文档地址：https://ayugespidertools.readthedocs.io/en/latest/topics/loaders.html)
-+15).demo_item_loader: 本库 ScrapyClassicItem 及原生 scrapy item 动态添加 item 字段及支持 Item Loaders 的示例
-+16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例
++15).demo_item_loader: 本库中使用 Item Loaders 的示例
+-16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例，此示例已删除，可查看上个 demo_item_loader 中的示例，目标已经可以很方便的使用 Item Loaders 功能了
+
++17).demo_mongo_async: asyncio 版本存储 mongoDB 的 pipelines 示例
 ```
 
 注：具体内容及时效性请以 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 项目中描述为准。
 
 ### 2.2. 开发场景
 
 > 这里不再一一列举所有功能，大概介绍下包含的大致功能。
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/commands/startproject.py` & `ayugespidertools-3.0.1/ayugespidertools/commands/startproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 from scrapy.utils.template import render_templatefile, string_camelcase
 
 import ayugespidertools
 from ayugespidertools.common.params import Param
 
 # 添加需要的自定义配置文件
 TEMPLATES_TO_RENDER = (
-    (".gitignore",),
     ("pyproject.toml",),
     ("README.md",),
     ("requirements.txt",),
-    (".gitignore",),
     ("scrapy.cfg",),
     ("${project_name}", "settings.py.tmpl"),
     ("${project_name}", "items.py.tmpl"),
     ("${project_name}", "pipelines.py.tmpl"),
     ("${project_name}", "middlewares.py.tmpl"),
     # 添加 run.py 总运行文件
     ("${project_name}", "run.py.tmpl"),
@@ -60,28 +58,26 @@
                     string.Template(s).substitute(project_name=project_name)
                     for s in paths
                 ),
             )
             render_templatefile(
                 tplfile,
                 project_name=project_name,
-                # 这个 py 就只为了处理模板中 .gitignore 多余的 $py 干扰
-                py="$py",
                 ProjectName=string_camelcase(project_name),
             )
 
         # 添加执行 shell 文件 run.sh 的生成
         if _has_project_dir_args:
             run_shell_path = f"{project_dir}/{project_name}/run.sh.tmpl"
         else:
             run_shell_path = f"{project_dir}/{project_dir}/run.sh.tmpl"
         run_shell_abspath = Path(project_dir).resolve()
         # 如果是 windows 环境的话，就不生成 shell 文件了，没啥必要
         if Param.IS_WINDOWS:
-            print("Info: The run.sh file is no longer generated under windows")
+            print("Info: The run.sh file is no longer generated under windows.")
             del_file = Path(run_shell_path)
             if Path.exists(del_file):
                 del_file.unlink()
 
         else:
             render_templatefile(
                 run_shell_path,
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/commands/version.py` & `ayugespidertools-3.0.1/ayugespidertools/commands/version.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/common/encryption.py` & `ayugespidertools-3.0.1/ayugespidertools/common/encryption.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/common/expend.py` & `ayugespidertools-3.0.1/ayugespidertools/common/expend.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/common/mongodbpipe.py` & `ayugespidertools-3.0.1/ayugespidertools/common/mongodbpipe.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+from typing import Union
 
 from itemadapter import ItemAdapter
 
 from ayugespidertools.common.multiplexing import ReuseOperation
 from ayugespidertools.common.params import Param
 
 __all__ = [
@@ -34,92 +35,79 @@
         assert (
             " " not in full_collection_name
         ), "集合名不能含空格，请检查 MONGODB_COLLECTION_PREFIX 参数和 item 中的 table 参数"
         return full_collection_name
 
     def _get_insert_data(
         self,
-        item_dict: ItemAdapter,
+        item_dict: Union[ItemAdapter, dict],
     ) -> dict:
         """
         获取要插入的数据，将 item 中的存储数据提取出来
         Args:
-            item_dict: item ItemAdapter 格式数据，可像字典一样操作
+            item_dict: item ItemAdapter 或者 dict 格式数据，可像字典一样操作
 
         Returns:
             None
         """
-        insert_data = item_dict.get("alldata")
-        # 如果有 alldata 字段，则其为推荐格式
-        if all([insert_data, isinstance(insert_data, dict)]):
-            judge_item = next(iter(insert_data.values()))
-            # 判断数据中中的 alldata 的格式：
-            #     1.推荐：是嵌套 dict，就像 AyuMysqlPipeline 一样 -- 这是为了通用写法风格；
-            #     2.是单层的 dict
-            # 是 namedtuple 类型
-            if ReuseOperation.is_namedtuple_instance(judge_item):
-                insert_data = {v: insert_data[v].key_value for v in insert_data.keys()}
-            # 如果是嵌套 dict 格式的话，需要再转化为正常格式
-            elif isinstance(judge_item, dict):
-                insert_data = {
-                    v: insert_data[v]["key_value"] for v in insert_data.keys()
-                }
-
-        # 否则为旧格式
-        else:
-            insert_data = ReuseOperation.get_items_except_keys(
-                dict_conf=item_dict,
-                key_list=["table", "item_mode", "mongo_update_rule"],
-            )
+        insert_data = ReuseOperation.get_items_except_keys(
+            dict_conf=item_dict,
+            key_list=["_table", "_item_mode", "_mongo_update_rule"],
+        )
+        judge_item = next(iter(insert_data.values()))
+        # 是 namedtuple 类型
+        if ReuseOperation.is_namedtuple_instance(judge_item):
+            insert_data = {v: insert_data[v].key_value for v in insert_data.keys()}
+        # 是普通的 dict 格式，则直接为 insert_data
         return insert_data
 
     def process_item_template(
         self,
-        item_dict: ItemAdapter,
+        item_dict: Union[ItemAdapter, dict],
         db: Param.PymongoDataBase,
         collection_prefix: str = "",
     ) -> None:
         """
         模板方法，用于处理 mongodb pipeline 存储的模板方法类
         Args:
-            item_dict: item ItemAdapter 格式数据
+            item_dict: item ItemAdapter 或 dict 格式数据
             db: mongodb 数据库连接
             collection_prefix: 集合前缀
 
         Returns:
             None
         """
         insert_data = self._get_insert_data(item_dict)
         # 真实的集合名称为：集合前缀名 + 集合名称
         collection_name = self._get_collection_name(
-            table=item_dict["table"],
+            table=item_dict["_table"],
             collection_prefix=collection_prefix,
         )
         self._data_storage_logic(
             db=db,
             item_dict=item_dict,
             collection_name=collection_name,
             insert_data=insert_data,
         )
 
     @abstractmethod
     def _data_storage_logic(
         self,
         db: Param.PymongoDataBase,
-        item_dict: ItemAdapter,
+        item_dict: Union[ItemAdapter, dict],
         collection_name: str,
         insert_data: dict,
         *args,
         **kwargs,
     ) -> None:
         """
         数据存储逻辑，需要子类实现
         Args:
             db: mongodb 数据库连接
-            item_dict: item ItemAdapter 格式数据
+            item_dict: item ItemAdapter 或 dict 格式数据
             collection_name: 集合名称
             insert_data: 要插入的数据
             *args: 可变参数
             **kwargs:关键字参数
 
         Returns:
             None
@@ -131,95 +119,95 @@
     """
     pipeline 同步执行 mongodb 存储的场景
     """
 
     def _data_storage_logic(
         self,
         db: Param.PymongoDataBase,
-        item_dict: ItemAdapter,
+        item_dict: Union[ItemAdapter, dict],
         collection_name: str,
         insert_data: dict,
         *args,
         **kwargs,
     ) -> None:
         # 如果没有查重字段时，就直接插入数据（不去重）
-        if not item_dict.get("mongo_update_rule"):
+        if not item_dict.get("_mongo_update_rule"):
             db[collection_name].insert(insert_data)
         else:
             db[collection_name].update(
-                item_dict["mongo_update_rule"], {"$set": insert_data}, True
+                item_dict["_mongo_update_rule"], {"$set": insert_data}, True
             )
 
 
 class TwistedAsynchronous(AbstractClass):
     """
     pipeline twisted 异步执行 mongodb 存储的场景
     """
 
     def _data_storage_logic(
         self,
         db: Param.PymongoDataBase,
-        item_dict: ItemAdapter,
+        item_dict: Union[ItemAdapter, dict],
         collection_name: str,
         insert_data: dict,
         *args,
         **kwargs,
     ) -> None:
-        if not item_dict.get("mongo_update_rule"):
+        if not item_dict.get("_mongo_update_rule"):
             db[collection_name].insert(insert_data)
         else:
             db[collection_name].update(
-                item_dict["mongo_update_rule"], {"$set": insert_data}, True
+                item_dict["_mongo_update_rule"], {"$set": insert_data}, True
             )
 
 
 class AsyncioAsynchronous(AbstractClass):
     """
     pipeline asyncio 异步执行 mongodb 存储的场景 - 使用 motor 实现
     """
 
     async def _data_storage_logic(
         self,
         db: Param.PymongoDataBase,
-        item_dict: ItemAdapter,
+        item_dict: Union[ItemAdapter, dict],
         collection_name: str,
         insert_data: dict,
         *args,
         **kwargs,
     ) -> None:
-        if not item_dict.get("mongo_update_rule"):
+        if not item_dict.get("_mongo_update_rule"):
             await db[collection_name].insert_one(insert_data)
         else:
             await db[collection_name].update_many(
-                item_dict["mongo_update_rule"], {"$set": insert_data}, True
+                item_dict["_mongo_update_rule"], {"$set": insert_data}, True
             )
 
     async def process_item_template(
         self,
-        item_dict: ItemAdapter,
+        item_dict: Union[ItemAdapter, dict],
         db: Param.PymongoDataBase,
         collection_prefix: str = "",
     ) -> None:
         insert_data = self._get_insert_data(item_dict)
         # 真实的集合名称为：集合前缀名 + 集合名称
         collection_name = self._get_collection_name(
-            table=item_dict["table"],
+            table=item_dict["_table"],
             collection_prefix=collection_prefix,
         )
         await self._data_storage_logic(
             db=db,
             item_dict=item_dict,
             collection_name=collection_name,
             insert_data=insert_data,
         )
 
 
 def mongodb_pipe(
     abstract_class: AbstractClass,
-    item_dict: ItemAdapter,
+    item_dict: Union[ItemAdapter, dict],
     db: Param.PymongoDataBase,
     collection_prefix: str = "",
 ) -> None:
     """
     mongodb pipeline 存储的通用调用方法
     """
     abstract_class.process_item_template(
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/common/multiplexing.py` & `ayugespidertools-3.0.1/ayugespidertools/formatdata.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,374 +1,287 @@
-import asyncio
-import json
-import os
-import random
+import datetime
 import re
-from typing import Any, List, Union
+import time
+from typing import Optional
+from urllib.parse import urljoin
 
-import cv2
-import numpy as np
-import pymysql
-from scrapy.settings import Settings
-from twisted.internet.defer import Deferred
-
-from ayugespidertools.common.typevars import MysqlConfig
-from ayugespidertools.config import logger
+import html2text
+from w3lib.html import remove_tags, replace_entities
 
 __all__ = [
-    "ReuseOperation",
+    "DataHandle",
 ]
 
 
-class ReuseOperation(object):
-    """
-    用于存放经常复用的一些操作
-    """
+class DataHandle(object):
+    """数据处理相关方法"""
 
     @staticmethod
-    def as_deferred(f):
+    def get_full_url(domain_name: str, deal_url: str) -> str:
         """
-        transform a Twisted Deferred to an Asyncio Future
+        根据域名 domain_name 拼接 deal_url 来获得完整链接
         Args:
-            f: async function
+            domain_name: 域名链接
+            deal_url: 需要拼接的 url
 
         Returns:
-            1).Deferred
+            1). 拼接完整的链接
         """
-        return Deferred.fromFuture(asyncio.ensure_future(f))
+        return urljoin(domain_name, deal_url)
 
     @staticmethod
-    def is_namedtuple_instance(x: Any) -> bool:
+    def click_point_deal(decimal: float, decimal_places=2) -> float:
         """
-        判断 x 是否为 namedtuple 类型
+        将小数 decimal 保留小数点后 decimal_places 位，结果四舍五入
         Args:
-            x: 需要判断的参数
+            decimal: 需要处理的小数
+            decimal_places: 需要保留的小数点位数
 
         Returns:
-            1). 是否符合 namedtuple 类型
+            decimal(float): 四舍五入后的小数点
         """
-        return isinstance(x, tuple) and hasattr(x, "_fields")
+        # 先拼接需要保留的位数
+        decimal_deal = f"%.{decimal_places}f"
+        return float(decimal_deal % decimal)
 
     @staticmethod
-    def get_file_name_by_url(file_url: str) -> str:
+    def judge_utc_time(local_time: str) -> bool:
         """
-        根据文件链接取出文件的名称
+        判断 local_time 是否为 utc 格式的时间
         Args:
-            file_url: 文件链接
+            local_time: 需要判断的时间参数，比如：Thu Jul 21 17:59:44 2022 或 Fri, 22 Jul 2022 01:43:06 +0800 等等
 
         Returns:
-            1). 文件名称
+            1): 是否为 utc 格式的数据
         """
-        pattern = re.compile(r""".*/(.*?)\..*?""")
-        if file_name_list := pattern.findall(file_url):
-            return file_name_list[0]
-        return ""
+        pattern = re.compile(r"""mon|tues|wed|thu|fri|sat|sun""")
+        return bool(pattern.findall(local_time.lower()))
 
     @staticmethod
-    def get_files_from_path(path: str) -> list:
-        """
-        获取 path 文件夹下的所有文件，而且输出以 path 为根目录的相对路径
-        Args:
-            path: 需要判断的文件夹路径
-
-        Returns:
-            file_list: path 文件夹下的文件列表
-        """
-        return [f.path for f in os.scandir(path) if f.is_file()]
+    def judge_include_letter(local_time: str) -> bool:
+        pattern = re.compile(r"""[a-zA-Z]""")
+        return bool(pattern.findall(local_time.lower()))
 
     @staticmethod
-    def get_bytes_by_file(file_path: str) -> bytes:
-        """
-        获取媒体文件的 bytes 内容
-        Args:
-            file_path: 对应文件的路径
-
-        Returns:
-            file_bytes: file_path 对应文件的 bytes 内容
-        """
-        with open(file_path, "rb") as f:
-            file_bytes = f.read()
-        return file_bytes
+    def _get_format_t(
+        date_style: str = "",
+        date_is_full: bool = False,
+        specific_date_conn: str = " ",
+        hms_conn: str = ":",
+    ) -> str:
+        """
+        将需要格式化的数据用 date_style 标识来拼接起来，如果 date_is_full 为 True 时，则需要补齐"时分秒"位
+        Args:
+            date_style: 将格式化符拼接时需要的标识，比如：-
+            date_is_full: 是否需要完整的时间格式化（即是否需要补齐"时分秒"单位）
+            specific_date_conn: 年月日与时分秒拼接的方式
+            hms_conn: 时分秒拼接的方式
+
+        Returns:
+            1).最终的格式化拼接结果，比如：%Y-%m-%d %H-%M-%S
+        """
+        # 年月日
+        _y_m_d = ["%Y", "%m", "%d"]
+        _y_m_d_format = date_style.join(_y_m_d)
+
+        if date_is_full:
+            # 时分秒
+            _h_m_s = ["%H", "%M", "%S"]
+            # 时分秒大都为":"连接
+            _h_m_s_format = hms_conn.join(_h_m_s)
+            return specific_date_conn.join([_y_m_d_format, _h_m_s_format])
+        return _y_m_d_format
 
     @staticmethod
-    def read_image_data(
-        bg: Union[bytes, str],
-        tp: Union[bytes, str],
-    ) -> (np.ndarray, np.ndarray):
+    def _time_format(date_str) -> str:
         """
-        用 opencv 读取图片数据
+        判断时间是什么格式的，比如：xxxx-xx-xx 或 xxxx.xx.xx
         Args:
-            bg: 背景图片信息
-            tp: 滑块图
+            date_str: 需要判断格式的时间
 
         Returns:
-            bg_cv: opencv 读取背景图片的数据
-            tp_cv: opencv 读取滑块图片的数据
+            1): 时间格式的标识，比如：-，若没有就返回空字符
         """
-        assert type(bg) in [str, bytes], "带缺口的背景图参数需要是全路径图片或 bytes 数据"
-        assert type(tp) in [str, bytes], "滑块图参数需要是全路径图片或 bytes 数据"
+        format_styles = ["-", ".", "/", "年"]
+        return next(
+            (
+                format_style
+                for format_style in format_styles
+                if format_style in date_str
+            ),
+            "",
+        )
 
-        if isinstance(bg, bytes):
-            bg_buf = np.frombuffer(bg, np.uint8)
-            bg_cv = cv2.imdecode(bg_buf, cv2.IMREAD_ANYCOLOR)
-        else:
-            # 读取图片，读进来直接是 BGR 格式数据格式在 0~255
-            bg_cv = cv2.imread(bg)
+    @classmethod
+    def normal_to_stamp(
+        cls,
+        normal_time: str,
+        _format_t: str = None,
+        date_is_full: bool = True,
+        specific_date_conn: str = " ",
+        hms_conn: str = ":",
+    ) -> int:
+        """
+        将网页正常时间转为时间戳
+        Args:
+            normal_time: 需要转换的时间
+            _format_t: 时间格式化符，默认不填。除非在英文时间的参数出错时可指定 _format_t 的值
+            date_is_full: 是否包含"时分秒"单位的完整格式
+            specific_date_conn: 年月日与时分秒拼接的方式
+            hms_conn: 时分秒拼接的方式
+
+        Returns:
+            stamp: 返回的时间戳
+        """
+        # 判断 normal_time 是否是特殊模式
+        is_utc_time = cls.judge_utc_time(normal_time)
+        is_letter_time = cls.judge_include_letter(normal_time)
+        # stamp = None
+        if any([is_utc_time, is_letter_time]):
+            # 如果不传递时间的格式符参数
+            if not _format_t:
+                if "," in normal_time:
+                    _format_t = "%a, %d %b %Y %H:%M:%S +0800"
+                else:
+                    _format_t = "%a %b %d %H:%M:%S %Y"
+            standard_time = datetime.datetime.strptime(normal_time, _format_t)
+            stamp = time.mktime(
+                time.strptime(str(standard_time), cls._get_format_t("-", True))
+            )
 
-        if isinstance(tp, bytes):
-            tp_buf = np.frombuffer(tp, np.uint8)
-            tp_cv = cv2.imdecode(tp_buf, cv2.IMREAD_ANYCOLOR)
         else:
-            # 0 表示采用黑白的方式读取图片
-            tp_cv = cv2.imread(tp, 0)
-
-        return bg_cv, tp_cv
+            # 先判断正常时间的格式
+            date_style = cls._time_format(normal_time)
+            # standard_time_format = _get_format_t(date_style, date_is_full).replace('%m', '%b').replace('-', '/')
+            standard_time_format = cls._get_format_t(
+                date_style, date_is_full, specific_date_conn, hms_conn
+            )
+            stamp = time.mktime(time.strptime(normal_time, standard_time_format))
+        return int(stamp)
 
     @staticmethod
-    def random_weight(weight_data: list):
+    def timestamp_to_normal(timestamp_data: int) -> str:
         """
-        带权重的随机取值，即在带权重的列表数据中根据权重随机取一个值
+        将时间戳转为正常时间 xxxx-xx-xx xx:xx:xx 的格式
         Args:
-            weight_data: 带权重的列表信息，示例：
-                [{'username': 'xxxx', 'password': '******', 'weight': 8}, ...]
+            timestamp_data: 需要处理的时间格式
 
         Returns:
-            ret: 返回当前权重列表 account_arr 中的一个值
+            1). 转换后的时间结果
         """
-        total = sum(item["weight"] for item in weight_data)
-        # 在 0 与权重和之间获取一个随机数
-        ra = random.uniform(0, total)
-        curr_sum = 0
-        ret = None
-        for data in weight_data:
-            # 在遍历中，累加当前权重值
-            curr_sum += data["weight"]
-            # 当随机数 <= 当前权重和时，返回权重 key
-            if ra <= curr_sum:
-                ret = data
-                break
-        return ret
+        if len(str(timestamp_data)) > 10:
+            timestamp_data = int(str(timestamp_data[:-3]))
 
-    @classmethod
-    def is_dict_meet_min_limit(cls, dict_conf: dict, key_list: List[str]) -> bool:
-        """
-        判断 dict_conf 是否满足 key_list 中的 key 值限定
-        Args:
-            dict_conf: 需要判断的参数
-            key_list: dict_conf 中需要包含的 key 值列表，示例为：['proxy', 'username', 'password']
+        time_array = time.localtime(timestamp_data)
+        return time.strftime("%Y-%m-%d %H:%M:%S", time_array)
 
-        Returns:
-            1). 是否满足 key 值限制
+    @staticmethod
+    def remove_all_tags(func):
         """
-        if any([not dict_conf, not isinstance(dict_conf, dict)]):
-            return False
-
-        return all(key in dict_conf for key in key_list)
-
-    @classmethod
-    def get_items_by_keys(
-        cls,
-        dict_conf: dict,
-        key_list: List[str],
-    ) -> dict:
+        去除所有标签
         """
-        获取 dict_conf 中的含有 key_list 的 key 的字段
-        Args:
-            dict_conf: 需要处理的参数
-            key_list: 需要取的 key 值列表
 
-        Returns:
-            1). 取值后的 dict，或不满足请求的 False 值
-        """
-        # 参数先要满足最小限定，然后再取出限定的参数值；否则返回空字典
-        return (
-            {k: dict_conf[k] for k in key_list}
-            if cls.is_dict_meet_min_limit(dict_conf=dict_conf, key_list=key_list)
-            else {}
-        )
+        def inner(*args, **kwargs):
+            func_res = func(*args, **kwargs)
+            func_res = remove_tags(func_res)
+            return func_res
 
-    @classmethod
-    def get_items_except_keys(cls, dict_conf, key_list: List[str]) -> dict:
-        """
-        获取 dict_conf 中的不含有 key_list 的 key 的字段
-        Args:
-            dict_conf: 需要处理的参数
-            key_list: 需要排除的 key 值列表
+        return inner
 
-        Returns:
-            1). dict_conf 排除 key_list 中的键值后的值
+    @staticmethod
+    def normal_display(func):
         """
-        return {k: dict_conf[k] for k in dict_conf if k not in key_list}
-
-    @classmethod
-    def create_database(cls, mysql_conf: MysqlConfig) -> None:
+        去除掉网页的注释(将网页中的特殊字符的源码改成正常显示)
         """
-        创建数据库
-        由于这是在连接数据库，报数据库不存在错误时的场景，则需要新建(不指定数据库)连接创建好所需数据库即可
-        Args:
-            mysql_conf: pymysql 的数据库连接配置
 
-        Returns:
-            None
-        """
-        conn = pymysql.connect(
-            user=mysql_conf.user,
-            password=mysql_conf.password,
-            host=mysql_conf.host,
-            port=mysql_conf.port,
-            charset=mysql_conf.charset,
-        )
-        cursor = conn.cursor()
-        cursor.execute(
-            f"CREATE DATABASE `{mysql_conf.database}` character set {mysql_conf.charset};"
-        )
-        conn.close()
-        logger.info(
-            f"创建数据库 {mysql_conf.database} 成功，其 charset 类型是：{mysql_conf.charset}!"
-        )
+        def inner(*args, **kwargs):
+            func_res = func(*args, **kwargs)
+            func_res = replace_entities(func_res)
+            return func_res
 
-    @classmethod
-    def dict_keys_to_lower(cls, deal_dict: dict) -> dict:
-        """
-        将 dict 中 str 类型的 key 值变成小写
-        Args:
-            deal_dict: 需要处理的 dict
+        return inner
 
-        Returns:
-            1).处理后的 dict 值
+    @staticmethod
+    def simple_deal_for_extract(func):
         """
-        str_key_to_lower_dict = {
-            k.lower(): v for k, v in deal_dict.items() if isinstance(k, str)
-        }
-        not_str_key_dict = {
-            k: v for k, v in deal_dict.items() if not isinstance(k, str)
-        }
-        # python 3.9+ 可优化为：str_key_to_lower_dict |= not_str_key_dict
-        str_key_to_lower_dict.update(not_str_key_dict)
-        return str_key_to_lower_dict
-
-    @classmethod
-    def dict_keys_to_upper(cls, deal_dict: dict) -> dict:
+        将 xpath, css 或 json 提取的数据做简单处理；提取的数据若非数组数据，则统一返回字符类型
         """
-        将 dict 中 str 类型的 key 值变成大写
-        Args:
-            deal_dict: 需要处理的 dict
 
-        Returns:
-            1).处理后的 dict 值
-        """
-        # 找出 str 类型的 key 字段数据，并将其大写
-        str_key_to_upper_dict = {
-            k.upper(): v for k, v in deal_dict.items() if isinstance(k, str)
-        }
-        # 找出非 str 类型的数据
-        not_str_key_dict = {
-            k: v for k, v in deal_dict.items() if not isinstance(k, str)
-        }
-        # 将大写处理的字典加上非 str 类型的 key 字段数据
-        str_key_to_upper_dict.update(not_str_key_dict)
-        return str_key_to_upper_dict
+        def inner(*args, **kwargs):
+            func_res = func(*args, **kwargs)
+            if type(func_res) in [str, int, float, bool]:
+                # 这里可添加一些通用的数据处理
+                return str(func_res).strip()
+            else:
+                return func_res
 
-    @classmethod
-    def get_consul_conf(cls, settings: Settings) -> dict:
-        """
-        获取项目中的 consul 配置，且要根据项目整体情况来取出满足最少要求的 consul 配置
-        Args:
-            settings: scrapy 的 settings 信息
-
-        Returns:
-            consul_conf_dict_min: 满足要求的最少要求的 consul 配置
-        """
-        consul_conf_dict = settings.get("CONSUL_CONFIG", {})
-        return cls.get_items_by_keys(
-            dict_conf=consul_conf_dict, key_list=["token", "url", "format"]
-        )
+        return inner
 
     @classmethod
-    def judge_str_is_json(cls, judge_str: str) -> bool:
-        """
-        判断字符串是否为 json 格式
-        Args:
-            judge_str: 需要判断的字符串
-
-        Returns:
-            1）.是否为 json 格式
-        """
-        if not isinstance(judge_str, str):
-            return False
-
-        try:
-            json.loads(judge_str)
-        except Exception:
-            return False
-        else:
-            return True
-
-    @staticmethod
-    def get_ck_dict_from_headers(headers_ck_str: str) -> dict:
+    def _extract_table_rule(
+        cls, html_txt: str, h_obj: Optional[html2text.HTML2Text] = None
+    ):
         """
-        从 headers 中的 ck str 格式转化为 dict 格式
+        根据 html2text 来处理 html 中的 table 表格内容
         Args:
-            headers_ck_str: request headers ck 的 str 格式
+            html_txt: 网页内容
+            h_obj: html2text 对象句柄
 
         Returns:
-            1). 转化 dict 格式后的 ck
+            1).转换后的结果
         """
-        # 也可以这样写，但不推荐
-        # dict(line.split("=", 1) for line in headers_ck_str.split("; "))
-        return {
-            x.split("=", 1)[0].strip(): x.split("=", 1)[1].strip()
-            for x in headers_ck_str.split(";")
-        }
+        if not h_obj:
+            h_obj = html2text.HTML2Text()
 
-    @staticmethod
-    def get_req_dict_from_scrapy(req_body_data_str: str) -> dict:
-        """
-        将 scrapy 请求中的 body 对象转为 dict 格式
-        Args:
-            req_body_data_str: scrapy 中的 body 参数
-
-        Returns:
-            1). 转化 dict 格式后的 body
-        """
-        return {
-            x.split("=", 1)[0]: x.split("=", 1)[1] for x in req_body_data_str.split("&")
-        }
-
-    @staticmethod
-    def get_array_dimension(array: Union[frozenset, list, set, tuple]) -> int:
-        """
-        获取 array 的维度
-        Args:
-            array: 数组
-
-        Returns:
-            1).层级数
-        """
-        # 其实直接返回 len(array) 即可
-        return len(np.array(array).shape)
+        h_obj.protect_links = True
+        h_obj.body_width = 0
+        h_obj.ignore_links = True
+        h_obj.bypass_tables = False
+        return h_obj.handle(html_txt)
 
     @classmethod
-    def get_array_depth(cls, array: list) -> int:
-        """
-        获取 array 的最大层级，深度
-        Args:
-            array: 数组
-
-        Returns:
-            1).最大层级，深度
-        """
-
-        """1 + max(map(depthCount,x)) if x and isinstance(x,list) else 0"""
-        # 先判断是否为数组类型的元素
-        judge_array = isinstance(
-            array,
-            (
-                frozenset,
-                list,
-                set,
-                tuple,
-            ),
-        )
-        return (
-            int(judge_array) and len(array) and 1 + max(map(cls.get_array_depth, array))
-        )
+    def extract_html_to_md(
+        cls, html_txt: str, h_obj: Optional[html2text.HTML2Text] = None
+    ) -> str:
+        """
+        将 html 内容转化为 markdown 内容
+
+        更多、更详细的配置参数请查看文档内容: https://github.com/Alir3z4/html2text/blob/master/html2text/cli.py
+        Args:
+            html_txt: 网页内容（一般是带标签的内容）
+            h_obj: html2text 对象句柄
+
+        Returns:
+            1).转换后的结果
+        """
+        if not h_obj:
+            h_obj = html2text.HTML2Text()
+
+        # 以下步骤先处理通用部分，先不处理 table 内容
+        h_obj.body_width = 0
+        # h_obj.protect_links = True
+        h_obj.bypass_tables = True
+        # h_obj.unicode_snob = True
+        h_obj.ignore_links = True
+        content = h_obj.handle(html_txt)
+
+        # 先处理表格 <table> 标签中格式
+        table_pattern = re.compile(r"(<table.*?</table>)", flags=re.S)
+        if table_res_list := table_pattern.findall(content):
+            for table_res in table_res_list:
+                table_deal = cls._extract_table_rule(html_txt=table_res, h_obj=h_obj)
+                # 将 table 转换时去除多余的换行和空白字符等内容
+                table_deal = re.sub(r"\|\s*\n", "| ", table_deal, flags=re.S)
+                table_deal = re.sub(r"\n\s*\|", "| ", table_deal, flags=re.S)
+                table_deal = re.sub(r"\n\s*\n", "\n\n", table_deal, flags=re.S)
+                table_deal = re.sub(r"\r\n", "\n", table_deal, flags=re.S)
+                table_deal = re.sub(r"[\n]{1,}", "\n", table_deal, flags=re.S)
+
+                content = re.sub(
+                    r"(<table.*?</table>)", table_deal + "\n", content, 1, re.S
+                )
+
+        # TODO: 可以添加上通用处理的装饰器
+        # 将三个以上换行改为两个换行
+        content = re.sub(r"[\n]{3,}", "\n\n", content)
+        content = content.strip()
+        return content
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/common/mysqlerrhandle.py` & `ayugespidertools-3.0.1/ayugespidertools/common/mysqlerrhandle.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,53 +20,53 @@
 
     def _create_table(
         self,
         cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
         table_name: str,
         charset: str,
         collate: str,
-        tabel_notes: str = "",
+        table_notes: str = "",
         demand_code: str = "",
     ) -> None:
         """
         创建数据库表
         Args:
             cursor: mysql connect cursor，参数选择有：
                 1). 类型为 pymysql.cursors.Cursor，在同步 pipelines 中使用；
                 2). dbpool.runInteraction() 方法会将数据库连接的游标对象作为参数传入
                 回调函数中，而游标对象的类型可能是不同的，比如 DictCursor 或 Cursor 类型，在
                 异步 pipelines 中使用；
             table_name: 创建表的名称
             charset: charset
             collate: collate
-            tabel_notes: 创建表的注释
+            table_notes: 创建表的注释
             demand_code: 创建表的需求对应的 code 值，用于和需求中的任务对应
 
         Returns:
             None
         """
-        # 用于表格 comment 的参数生成(即 tabel_notes 参数)
+        # 用于表格 comment 的参数生成(即 table_notes 参数)
         if demand_code != "":
-            tabel_notes = f"{demand_code}_{tabel_notes}"
+            table_notes = f"{demand_code}_{table_notes}"
 
         sql = f"""
         CREATE TABLE IF NOT EXISTS `{table_name}`
         (`id` int(32) NOT NULL AUTO_INCREMENT COMMENT 'id', PRIMARY KEY (`id`))
-        ENGINE=InnoDB DEFAULT CHARSET={charset} COLLATE={collate} COMMENT='{tabel_notes}';
+        ENGINE=InnoDB DEFAULT CHARSET={charset} COLLATE={collate} COMMENT='{table_notes}';
         """
 
         try:
             # 执行 sql 查询，获取数据
             data = cursor.execute(sql)
             if any([data == 0, not data]):
-                logger.info(f"创建数据表 {tabel_notes}: {table_name} 成功！")
+                logger.info(f"创建数据表 {table_notes}: {table_name} 成功！")
 
         except Exception as e:
             logger.error(
-                f"创建表失败，tabel_notes：{tabel_notes}，table_name：{table_name}，error：{e}"
+                f"创建表失败，table_notes：{table_notes}，table_name：{table_name}，error：{e}"
             )
 
     def _get_column_type(
         self,
         cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
         database: str,
         table: str,
@@ -145,14 +145,16 @@
                 table_enum=table_enum,
             )
             self._create_table(
                 cursor=cursor,
                 table_name=table_name,
                 charset=charset,
                 collate=collate,
+                table_notes=table_notes,
+                demand_code=demand_code,
             )
 
         elif "1406" in err_msg:
             sql, possible_err = self.deal_1406_error(
                 err_msg=err_msg,
                 cursor=cursor,
                 database=database,
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/common/params.py` & `ayugespidertools-3.0.1/ayugespidertools/common/params.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/common/spiderdbconf.py` & `ayugespidertools-3.0.1/ayugespidertools/common/spiderdbconf.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/common/sqlformat.py` & `ayugespidertools-3.0.1/ayugespidertools/common/sqlformat.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/common/typevars.py` & `ayugespidertools-3.0.1/ayugespidertools/common/typevars.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/common/utils.py` & `ayugespidertools-3.0.1/ayugespidertools/common/utils.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/common/yidungap.py` & `ayugespidertools-3.0.1/ayugespidertools/common/yidungap.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/imgoperation.py` & `ayugespidertools-3.0.1/ayugespidertools/imgoperation.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/middlewares.py` & `ayugespidertools-3.0.1/ayugespidertools/middlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/mongoclient.py` & `ayugespidertools-3.0.1/ayugespidertools/mongoclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/mysqlclient.py` & `ayugespidertools-3.0.1/ayugespidertools/mysqlclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/oss.py` & `ayugespidertools-3.0.1/ayugespidertools/oss.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/pipelines.py` & `ayugespidertools-3.0.1/ayugespidertools/pipelines.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/rpa.py` & `ayugespidertools-3.0.1/ayugespidertools/rpa.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/runjs.py` & `ayugespidertools-3.0.1/ayugespidertools/runjs.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/form.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/http/request/form.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/requestslib.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/netlib/requestslib.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/private.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/private.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/__init__.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/download/file.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/download/file.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/download/image.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/download/image.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/asynced.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/asynced.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import asyncio
 import urllib.parse
 
 import motor.motor_asyncio
 
 from ayugespidertools.common.mongodbpipe import AsyncioAsynchronous
 from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.common.utils import ToolsForAyu
 
 
 class AsyncMongoPipeline(object):
     """
     通过 motor 实现异步写入 MongoDB 的存储管道
     """
 
@@ -45,16 +44,16 @@
         self.client = motor.motor_asyncio.AsyncIOMotorClient(self.mongo_uri)
         self.db = self.client[spider.mongodb_conf.database]
 
     async def close_spider(self, spider):
         self.client.close()
 
     async def process_item(self, item, spider):
-        item_dict = ToolsForAyu.convert_items_to_dict(item)
-        if item_dict["item_mode"] == "MongoDB":
+        item_dict = ReuseOperation.item_to_dict(item)
+        if item_dict["_item_mode"] == "MongoDB":
             await asyncio.shield(
                 AsyncioAsynchronous().process_item_template(
                     item_dict=item_dict,
                     db=self.db,
                     collection_prefix=self.collection_prefix,
                 )
             )
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ayugespidertools.common.mongodbpipe import Synchronize, mongodb_pipe
-from ayugespidertools.common.utils import ToolsForAyu
+from ayugespidertools.common.multiplexing import ReuseOperation
 from ayugespidertools.mongoclient import MongoDbBase
 
 __all__ = [
     "AyuFtyMongoPipeline",
 ]
 
 
@@ -66,17 +66,17 @@
         Args:
             item: scrapy item
             spider: scrapy spider
 
         Returns:
             item: scrapy item
         """
-        item_dict = ToolsForAyu.convert_items_to_dict(item)
+        item_dict = ReuseOperation.item_to_dict(item)
         # 先查看存储场景是否匹配
-        if item_dict["item_mode"] == "MongoDB":
+        if item_dict["_item_mode"] == "MongoDB":
             mongodb_pipe(
                 Synchronize(),
                 item_dict=item_dict,
                 db=self.db,
                 collection_prefix=self.collection_prefix,
             )
         return item
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/twisted.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/twisted.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from twisted.internet import defer, reactor
 
 from ayugespidertools.common.mongodbpipe import TwistedAsynchronous, mongodb_pipe
-from ayugespidertools.common.utils import ToolsForAyu
+from ayugespidertools.common.multiplexing import ReuseOperation
 from ayugespidertools.scraper.pipelines.mongo.fantasy import AyuFtyMongoPipeline
 
 __all__ = [
     "AyuTwistedMongoPipeline",
 ]
 
 
@@ -25,17 +25,17 @@
     def process_item(self, item, spider):
         out = defer.Deferred()
         reactor.callInThread(self.db_insert, item, out)
         yield out
         defer.returnValue(item)
 
     def db_insert(self, item, out):
-        item_dict = ToolsForAyu.convert_items_to_dict(item)
+        item_dict = ReuseOperation.item_to_dict(item)
         # 先查看存储场景是否匹配
-        if item_dict["item_mode"] == "MongoDB":
+        if item_dict["_item_mode"] == "MongoDB":
             mongodb_pipe(
                 TwistedAsynchronous(),
                 item_dict=item_dict,
                 db=self.db,
                 collection_prefix=self.collection_prefix,
             )
             reactor.callFromThread(out.callback, item_dict)
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 import warnings
-from typing import Optional, Tuple, Type
+from typing import Any, Dict, Optional, Tuple, Type
 
 import pymysql
 from retrying import retry
 
 from ayugespidertools.common.expend import MysqlPipeEnhanceMixin
 from ayugespidertools.common.multiplexing import ReuseOperation
 from ayugespidertools.common.mysqlerrhandle import Synchronize, deal_mysql_err
@@ -90,66 +90,50 @@
 
         # 最终的数据表名不能含有空格
         assert (
             " " not in full_table_name
         ), "数据表名不能含空格，请检查 MYSQL_TABLE_PREFIX 参数和 item 中的 table 参数"
         return full_table_name
 
-    def get_new_item(self, item) -> AlterItem:
+    def get_new_item(self, item_dict: Dict[str, Any]) -> AlterItem:
         """
         重新整合 item
         Args:
-            item: scrapy item
+            item_dict: dict 类型的 item
 
         Returns:
             1). 整合后的 item
         """
         new_item = {}
         notes_dic = {}
-        # 如果是 ayugespidertools.Items 中的各个自封装类型时
-        # alldata 可以认为是关键字，需要判断其是否存在，且是否为 dict。
-        # 若其存在且为 dict，则默认其为 Items 中的 alldata 数据类型而非单一字段值
-        insert_data = item.get("alldata")
-        if all([insert_data, isinstance(insert_data, dict)]):
-            judge_item = next(iter(insert_data.values()))
-            # 是 namedtuple 类型
-            if ReuseOperation.is_namedtuple_instance(judge_item):
-                for key, value in insert_data.items():
-                    new_item[key] = value.key_value
-                    notes_dic[key] = value.notes
-            # 是双层 dict 格式
-            elif isinstance(judge_item, dict):
-                for key, value in insert_data.items():
-                    new_item[key] = value.get("key_value", "")
-                    notes_dic[key] = value["notes"]
-            # 其它默认为单层 dict 格式
-            else:
-                for key, value in insert_data.items():
-                    new_item[key] = value
-                    notes_dic[key] = key
 
-        # 兼容旧写法，直接 dict 格式的 item 即可
+        insert_data = ReuseOperation.get_items_except_keys(
+            dict_conf=item_dict, key_list=["_item_mode", "_table"]
+        )
+        judge_item = next(iter(insert_data.values()))
+        # 是 namedtuple 类型
+        if ReuseOperation.is_namedtuple_instance(judge_item):
+            for key, value in insert_data.items():
+                new_item[key] = value.key_value
+                notes_dic[key] = value.notes
+        # 是普通的 dict 类型
         else:
-            # 将存入表的无关字段给去掉
-            save_data_item = ReuseOperation.get_items_except_keys(
-                dict_conf=item, key_list=["table", "item_mode"]
-            )
-            for key, value in save_data_item.items():
+            for key, value in insert_data.items():
                 new_item[key] = value
-                notes_dic[key] = key
+                notes_dic[key] = ""
 
         return AlterItem(new_item=new_item, notes_dic=notes_dic)
 
     def process_item(self, item, spider):
-        item_dict = ToolsForAyu.convert_items_to_dict(item)
+        item_dict = ReuseOperation.item_to_dict(item)
         # 先查看存储场景是否匹配
-        if item_dict["item_mode"] == "Mysql":
+        if item_dict["_item_mode"] == "Mysql":
             self.insert_item(
                 alter_item=self.get_new_item(item_dict),
-                table=self.get_table_name(item_dict["table"]),
+                table=self.get_table_name(item_dict["_table"]),
             )
         return item
 
     def insert_item(self, alter_item: AlterItem, table: str):
         """
         通用插入数据，将 item 数据存入 Mysql 中，item 中的 key 需要跟 Mysql 数据中的字段名称一致
         Args:
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/asynced.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,23 +36,23 @@
             password=self.mysql_conf.password,
             db=self.mysql_conf.database,
             charset=self.mysql_conf.charset,
             cursorclass=aiomysql.DictCursor,
         )
 
     async def process_item(self, item, spider):
-        item_dict = ToolsForAyu.convert_items_to_dict(item)
-        if item_dict["item_mode"] == "Mysql":
+        item_dict = ReuseOperation.item_to_dict(item)
+        if item_dict["_item_mode"] == "Mysql":
             async with self.db.cursor() as cursor:
                 async with self.lock:
                     alter_item = super(AsyncNormalMysqlPipeline, self).get_new_item(
                         item_dict
                     )
                     table = super(AsyncNormalMysqlPipeline, self).get_table_name(
-                        item_dict["table"]
+                        item_dict["_table"]
                     )
                     new_item = alter_item.new_item
                     sql = self._get_sql_by_item(table=table, item=new_item)
                     await cursor.execute(sql, tuple(new_item.values()) * 2)
                     await self.db.commit()
         return item
 
@@ -90,21 +90,21 @@
             # 连接池最大连接数
             maxsize=10,
             # 连接池最小连接数
             minsize=1,
         )
 
     async def process_item(self, item, spider):
-        item_dict = ToolsForAyu.convert_items_to_dict(item)
-        if item_dict["item_mode"] == "Mysql":
+        item_dict = ReuseOperation.item_to_dict(item)
+        if item_dict["_item_mode"] == "Mysql":
             async with self.pool.acquire() as conn:
                 async with conn.cursor() as cursor:
                     alter_item = super(AsyncMysqlPipeline, self).get_new_item(item_dict)
                     table = super(AsyncMysqlPipeline, self).get_table_name(
-                        item_dict["table"]
+                        item_dict["_table"]
                     )
                     new_item = alter_item.new_item
                     sql = self._get_sql_by_item(table=table, item=new_item)
                     await asyncio.shield(
                         cursor.execute(sql, tuple(new_item.values()) * 2)
                     )
         return item
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/twisted.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pymysql import cursors
 from twisted.enterprise import adbapi
 
+from ayugespidertools.common.multiplexing import ReuseOperation
 from ayugespidertools.common.mysqlerrhandle import TwistedAsynchronous, deal_mysql_err
 from ayugespidertools.common.utils import ToolsForAyu
 from ayugespidertools.scraper.pipelines.mysql import AyuMysqlPipeline
 
 __all__ = [
     "AyuTwistedMysqlPipeline",
 ]
@@ -50,24 +51,24 @@
     def db_create(self, cursor):
         pass
 
     def db_create_err(self, failure):
         self.slog.error(f"创建数据表失败: {failure}")
 
     def process_item(self, item, spider):
-        item_dict = ToolsForAyu.convert_items_to_dict(item)
+        item_dict = ReuseOperation.item_to_dict(item)
         # 先查看存储场景是否匹配
-        if item_dict["item_mode"] == "Mysql":
+        if item_dict["_item_mode"] == "Mysql":
             query = self.dbpool.runInteraction(self.db_insert, item_dict)
             query.addErrback(self.handle_error, item)
         return item
 
     def db_insert(self, cursor, item):
         alter_item = super(AyuTwistedMysqlPipeline, self).get_new_item(item)
-        table = super(AyuTwistedMysqlPipeline, self).get_table_name(item["table"])
+        table = super(AyuTwistedMysqlPipeline, self).get_table_name(item["_table"])
 
         if not (new_item := alter_item.new_item):
             return
 
         note_dic = alter_item.notes_dic
         sql = self._get_sql_by_item(table=table, item=new_item)
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-3.0.1/ayugespidertools/scraper/spiders/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,14 +138,22 @@
         settings_type = getattr(cls, "settings_type", "common")
         # 根据 settings_type 参数取出对应的 inner_settings 配置
         inner_settings = getattr(cls, f"custom_{settings_type}_settings", {})
 
         if custom_table_enum:
             inner_settings["DATA_ENUM"] = custom_table_enum
 
+        if vit_dir := settings.get("VIT_DIR", None):
+            # 根据 vit_dir 配置，获取对应的 inner_settings 配置
+            inner_settings = ReuseOperation.get_conf_by_settings(
+                vit_dir=vit_dir, inner_settings=inner_settings
+            )
+
+        else:
+            logger.warning("请在 settings.py 中配置 VIT_DIR 的路径参数，用于本库运行所需配置 .conf 的读取！")
         # 内置配置 inner_settings 优先级介于 project 和 spider 之间
         # 即优先级顺序：settings < inner_settings < custom_settings
         settings.setdict(inner_settings, priority="project")
         settings.setdict(cls.custom_settings or {}, priority="spider")
 
     @classmethod
     def from_crawler(cls, crawler, *args, **kwargs):
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/templates/project/module/VIT/.conf` & `ayugespidertools-3.0.1/ayugespidertools/templates/project/module/VIT/.conf`

 * *Files 17% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 00000080: 3d2a 2a2a 0d0a 6175 7468 736f 7572 6365  =***..authsource
 00000090: 3d2a 2a2a 0d0a 7573 6572 3d2a 2a2a 0d0a  =***..user=***..
 000000a0: 7061 7373 776f 7264 3d2a 2a2a 0d0a 0d0a  password=***....
 000000b0: 5b63 6f6e 7375 6c5d 0d0a 746f 6b65 6e3d  [consul]..token=
 000000c0: 0d0a 7572 6c3d 6874 7470 3a2f 2f68 6f73  ..url=http://hos
 000000d0: 743a 706f 7274 2f76 312f 6b76 2f2e 2e2e  t:port/v1/kv/...
 000000e0: 3f64 633d 6463 310d 0a66 6f72 6d61 743d  ?dc=dc1..format=
-000000f0: 6a73 6f6e 0d0a 0d0a 5b6b 646c 5f64 796e  json....[kdl_dyn
-00000100: 616d 6963 5f70 726f 7879 5d0d 0a70 726f  amic_proxy]..pro
-00000110: 7879 3d6f 3636 382e 6b64 6c74 7073 2e63  xy=o668.kdltps.c
-00000120: 6f6d 3a31 3538 3138 0d0a 7573 6572 6e61  om:15818..userna
-00000130: 6d65 3d2a 2a2a 0d0a 7061 7373 776f 7264  me=***..password
-00000140: 3d2a 2a2a 0d0a 0d0a 5b6b 646c 5f65 7863  =***....[kdl_exc
-00000150: 6c75 7369 7665 5f70 726f 7879 5d0d 0a70  lusive_proxy]..p
-00000160: 726f 7879 3d68 7474 703a 2f2f 6b70 732e  roxy=http://kps.
-00000170: 6b64 6c61 7069 2e63 6f6d 2f61 7069 2f67  kdlapi.com/api/g
-00000180: 6574 6b70 733f 6f72 6465 7269 643d 2a2a  etkps?orderid=**
-00000190: 2a26 6e75 6d3d 3130 3026 666f 726d 6174  *&num=100&format
-000001a0: 3d6a 736f 6e0d 0a75 7365 726e 616d 653d  =json..username=
-000001b0: 2a2a 2a0d 0a70 6173 7377 6f72 643d 2a2a  ***..password=**
-000001c0: 2a0d 0a69 6e64 6578 3d31 0d0a 0d0a 5b61  *..index=1....[a
-000001d0: 6c69 5f6f 7373 5d0d 0a6f 7373 6163 6365  li_oss]..ossacce
-000001e0: 7373 6b65 7969 643d 4c54 412a 2a2a 2a2a  sskeyid=LTA*****
-000001f0: 2a0d 0a6f 7373 6163 6365 7373 6b65 7973  *..ossaccesskeys
-00000200: 6563 7265 743d 2a2a 2a2a 2a2a 0d0a 656e  ecret=******..en
-00000210: 6470 6f69 6e74 3d68 7474 7073 3a2f 2f6f  dpoint=https://o
-00000220: 7373 2d63 6e2d 2a2a 2a2a 2a2a 2e61 6c69  ss-cn-******.ali
-00000230: 7975 6e63 732e 636f 6d0d 0a65 7861 6d70  yuncs.com..examp
-00000240: 6c65 6275 636b 6574 3d2a 2a2a 2a2a 2a0d  lebucket=******.
-00000250: 0a6f 7065 7261 7465 646f 633d 2a2a 2a2a  .operatedoc=****
+000000f0: 6a73 6f6e 0d0a 0d0a 5b77 7862 6f74 5d0d  json....[wxbot].
+00000100: 0a6b 6579 3d2a 2a2a 0d0a 0d0a 5b6b 646c  .key=***....[kdl
+00000110: 5f64 796e 616d 6963 5f70 726f 7879 5d0d  _dynamic_proxy].
+00000120: 0a70 726f 7879 3d6f 3636 382e 6b64 6c74  .proxy=o668.kdlt
+00000130: 7073 2e63 6f6d 3a31 3538 3138 0d0a 7573  ps.com:15818..us
+00000140: 6572 6e61 6d65 3d2a 2a2a 0d0a 7061 7373  ername=***..pass
+00000150: 776f 7264 3d2a 2a2a 0d0a 0d0a 5b6b 646c  word=***....[kdl
+00000160: 5f65 7863 6c75 7369 7665 5f70 726f 7879  _exclusive_proxy
+00000170: 5d0d 0a70 726f 7879 3d68 7474 703a 2f2f  ]..proxy=http://
+00000180: 6b70 732e 6b64 6c61 7069 2e63 6f6d 2f61  kps.kdlapi.com/a
+00000190: 7069 2f67 6574 6b70 733f 6f72 6465 7269  pi/getkps?orderi
+000001a0: 643d 2a2a 2a26 6e75 6d3d 3130 3026 666f  d=***&num=100&fo
+000001b0: 726d 6174 3d6a 736f 6e0d 0a75 7365 726e  rmat=json..usern
+000001c0: 616d 653d 2a2a 2a0d 0a70 6173 7377 6f72  ame=***..passwor
+000001d0: 643d 2a2a 2a0d 0a69 6e64 6578 3d31 0d0a  d=***..index=1..
+000001e0: 0d0a 5b61 6c69 5f6f 7373 5d0d 0a61 6363  ..[ali_oss]..acc
+000001f0: 6573 736b 6579 6964 3d4c 5441 2a2a 2a2a  esskeyid=LTA****
+00000200: 2a2a 0d0a 6163 6365 7373 6b65 7973 6563  **..accesskeysec
+00000210: 7265 743d 2a2a 2a2a 2a2a 0d0a 656e 6470  ret=******..endp
+00000220: 6f69 6e74 3d68 7474 7073 3a2f 2f6f 7373  oint=https://oss
+00000230: 2d63 6e2d 2a2a 2a2a 2a2a 2e61 6c69 7975  -cn-******.aliyu
+00000240: 6e63 732e 636f 6d0d 0a62 7563 6b65 743d  ncs.com..bucket=
+00000250: 2a2a 2a2a 2a2a 0d0a 646f 633d 2a2a 2a2a  ******..doc=****
 00000260: 2a2a 2a0d 0a                             ***..
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/templates/project/module/items.py.tmpl` & `ayugespidertools-3.0.1/ayugespidertools/templates/project/module/items.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-3.0.1/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-3.0.1/ayugespidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-3.0.1/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files 6% similar despite different names*

```diff
@@ -92,26 +92,21 @@
                 json_data=curr_data,
                 query="favorCount")
 
             nick_name = ToolsForAyu.extract_with_json(
                 json_data=curr_data,
                 query="nickName")
 
-            # 这是需要存储的字段信息
-            article_info = {
-                "article_detail_url": DataItem(article_detail_url, "文章详情链接"),
-                "article_title": DataItem(article_title, "文章标题"),
-                "comment_count": DataItem(comment_count, "文章评论数量"),
-                "favor_count": DataItem(favor_count, "文章赞成数量"),
-                "nick_name": DataItem(nick_name, "文章作者昵称"),
-            }
-
             ArticleInfoMysqlItem = MysqlDataItem(
-                alldata=article_info,
-                table=TableEnum.article_list_table.value["value"],
+                article_detail_url=DataItem(article_detail_url, "文章详情链接"),
+                article_title=DataItem(article_title, "文章标题"),
+                comment_count=DataItem(comment_count, "文章评论数量"),
+                favor_count=DataItem(favor_count, "文章赞成数量"),
+                nick_name=DataItem(nick_name, "文章作者昵称"),
+                _table=TableEnum.article_list_table.value["value"],
             )
             self.slog.info(f"ArticleInfoMysqlItem: {ArticleInfoMysqlItem}")
 
             # 数据入库逻辑，你可以使用 mysql_engine 来去重或自定义规则
             try:
                 save_table = f'{self.custom_settings.get("MYSQL_TABLE_PREFIX", "")}{TableEnum.article_list_table.value["value"]}'
                 sql = f'''select `id` from `{save_table}` where `article_detail_url` = "{article_detail_url}" limit 1'''
@@ -129,15 +124,17 @@
                 if any(["1146" in str(e), "1054" in str(e), "doesn't exist" in str(e)]):
                     yield ArticleInfoMysqlItem
                 else:
                     self.slog.error(f"请查看数据库链接或网络是否通畅！Error: {e}")
 
             # 这是 MongoDB 存储场景的示例
             ArticleInfoMongoItem = MongoDataItem(
-                # alldata 用于存储 mongo 的 Document 文档所需要的字段映射
-                alldata=article_info,
-                # table 为 mongo 的存储 Collection 集合的名称
-                table=TableEnum.article_list_table.value["value"],
-                # mongo_update_rule 为查询数据是否存在的规则
-                mongo_update_rule={"article_detail_url": article_detail_url},
+                article_detail_url=article_detail_url,
+                article_title=article_title,
+                comment_count=comment_count,
+                favor_count=favor_count,
+                nick_name=nick_name,
+                _table=TableEnum.article_list_table.value["value"],
+                # 这里表示以 article_detail_url 为去重规则，若存在则更新，不存在则新增
+                _mongo_update_rule={"article_detail_url": article_detail_url},
             )
             yield ArticleInfoMongoItem
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-3.0.1/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files 11% similar despite different names*

```diff
@@ -38,16 +38,12 @@
 
     def parse_item(self, response):
         # 获取图书名称 - （获取的是详情页中的图书名称）
         book_name_list = response.xpath('//div[@class="book-name"]//text()').extract()
         book_name = "".join(book_name_list).strip()
         self.slog.debug(f"book_name: {book_name}")
 
-        novel_info = {
-            "book_name": {"key_value": book_name, "notes": "图书名称"},
-        }
-
         NovelInfoItem = MysqlDataItem(
-            alldata=novel_info,
-            table=TableEnum.article_list_table.value["value"],
+            book_name=book_name,
+            _table=TableEnum.article_list_table.value["value"],
         )
         yield NovelInfoItem
```

### Comparing `ayugespidertools-2.1.0/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-3.0.1/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-3.0.1/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/utils/cmdline.py` & `ayugespidertools-3.0.1/ayugespidertools/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/ayugespidertools/verificationcode.py` & `ayugespidertools-3.0.1/ayugespidertools/verificationcode.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.1.0/pyproject.toml` & `ayugespidertools-3.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "2.1.0"
+version = "3.0.1"
 description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
@@ -40,15 +40,14 @@
 toml = "^0.10.2"
 python-hcl2 = "^4.3.0"
 motor = "2.5.1"
 urllib3 = "~1.26.15"
 
 [tool.poetry.scripts]
 ayuge = "ayugespidertools.utils.cmdline:execute"
-ayugespidertools = "ayugespidertools.utils.cmdline:execute"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^23.1.0"
 isort = "^5.12.0"
 sphinx-rtd-theme = "1.2.0"
 coverage = "^7.2.2"
```

### Comparing `ayugespidertools-2.1.0/PKG-INFO` & `ayugespidertools-3.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayugespidertools
-Version: 2.1.0
+Version: 3.0.1
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。
 Home-page: https://www.ayuge.top/mkdocs-material/
 Keywords: crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
@@ -93,15 +93,15 @@
 使用方法示例 `GIF` 如下：
 
 ![ayugespidertools.gif](https://raw.githubusercontent.com/shengchenyang/AyugeSpiderTools/main/examples/ayugespidertools-use.gif)
 
 对以上 `GIF` 中的步骤进行解释：
 
 ```shell
-# 注：更推荐使用 ayuge 的 cli 名称，输入体验更友好，（ayugespidertools 的 cli 则会在下一大版本中会剔除）。
+# 注：ayugespidertools 的 cli 已剔除，现只能使用 ayuge。
 
 # 查看库版本
 ayuge version
 
 # 创建项目
 ayuge startproject <project_name>
 
@@ -113,48 +113,51 @@
 
 # 替换(覆盖)为真实的配置 .conf 文件；
 # 这里是为了演示方便，正常情况是直接在 VIT 路径下的 .conf 配置文件填上相关配置即可
 cp /root/mytemp/.conf DemoSpider/VIT/.conf
 
 # 运行脚本
 scrapy crawl <spider_name>
+# 注：也可以使用 ayuge crawl <spider_name>
 ```
 
 具体使用方法请在 [DemoSpider 之 AyugeSpiderTools 工具应用示例](https://github.com/shengchenyang/DemoSpider) 项目中查看，目前已适配以下场景：
 
 ```diff
 # 采集数据存入 `Mysql` 的场景：
-- 1).demo_one: 配置根据本地 `settings` 的 `LOCAL_MYSQL_CONFIG` 中取值
++ 1).demo_one: 配置根据本地 `settings` 的 `LOCAL_MYSQL_CONFIG` 中取值
 + 3).demo_three: 配置根据 `consul` 的应用管理中心中取值
 + 5).demo_five: 异步存入 `Mysql` 的场景
 
 # 采集数据存入 `MongoDB` 的场景：
-- 2).demo_two: 采集数据存入 `MongoDB` 的场景（配置根据本地 `settings` 的 `LOCAL_MONGODB_CONFIG` 中取值）
++ 2).demo_two: 采集数据存入 `MongoDB` 的场景（配置根据本地 `settings` 的 `LOCAL_MONGODB_CONFIG` 中取值）
 + 4).demo_four: 采集数据存入 `MongoDB` 的场景（配置根据 `consul` 的应用管理中心中取值）
 + 6).demo_six: 异步存入 `MongoDB` 的场景
 
 # 将 `Scrapy` 的 `Request`，`FormRequest` 替换为其它工具实现的场景
 - 以上为使用 scrapy Request 的场景
 + 7).demo_seven: scrapy Request 替换为 requests 请求的场景(一般情况下不推荐使用，同步库
 + 会拖慢 scrapy 速度，可用于测试场景)
 
 + 8).demo_eight: 同时存入 Mysql 和 MongoDB 的场景
 
-- 9).demo_aiohttp_example: scrapy Request 替换为 aiohttp 请求的场景，提供了各种请求场景示例（GET,POST）
++ 9).demo_aiohttp_example: scrapy Request 替换为 aiohttp 请求的场景，提供了各种请求场景示例（GET,POST）
 + 10).demo_aiohttp_test: scrapy aiohttp 在具体项目中的使用方法示例
 
 + 11).demo_proxy_one: 快代理动态隧道代理示例
 + 12).demo_proxy_two: 测试快代理独享代理
 
 +13).demo_AyuTurboMysqlPipeline: mysql 同步连接池的示例
 +14).demo_crawl: 支持 scrapy CrawlSpider 的示例
 
 # 本库中给出支持 Item Loaders 特性的示例(文档地址：https://ayugespidertools.readthedocs.io/en/latest/topics/loaders.html)
-+15).demo_item_loader: 本库 ScrapyClassicItem 及原生 scrapy item 动态添加 item 字段及支持 Item Loaders 的示例
-+16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例
++15).demo_item_loader: 本库中使用 Item Loaders 的示例
+-16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例，此示例已删除，可查看上个 demo_item_loader 中的示例，目标已经可以很方便的使用 Item Loaders 功能了
+
++17).demo_mongo_async: asyncio 版本存储 mongoDB 的 pipelines 示例
 ```
 
 注：具体内容及时效性请以 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 项目中描述为准。
 
 ### 2.2. 开发场景
 
 > 这里不再一一列举所有功能，大概介绍下包含的大致功能。
```

