# Comparing `tmp/aioscpy-0.3.8.tar.gz` & `tmp/aioscpy-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioscpy-0.3.8.tar", last modified: Fri Nov  4 05:46:29 2022, max compression
+gzip compressed data, was "aioscpy-0.3.9.tar", last modified: Fri Nov 25 09:36:53 2022, max compression
```

## Comparing `aioscpy-0.3.8.tar` & `aioscpy-0.3.9.tar`

### file list

```diff
@@ -1,118 +1,119 @@
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.188901 aioscpy-0.3.8/
--rw-rw-rw-   0        0        0     1087 2022-03-23 06:54:05.000000 aioscpy-0.3.8/LICENSE
--rw-rw-rw-   0        0        0      148 2022-05-06 10:30:34.000000 aioscpy-0.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6586 2022-11-04 05:46:29.187902 aioscpy-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     4178 2022-10-25 09:35:25.000000 aioscpy-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.104680 aioscpy-0.3.8/aioscpy/
--rw-rw-rw-   0        0        0        7 2022-10-26 06:30:54.000000 aioscpy-0.3.8/aioscpy/VERSION
--rw-rw-rw-   0        0        0      222 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/__init__.py
--rw-rw-rw-   0        0        0       84 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/__main__.py
--rw-rw-rw-   0        0        0     5304 2022-05-23 08:05:47.000000 aioscpy-0.3.8/aioscpy/cmdline.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.119641 aioscpy-0.3.8/aioscpy/commands/
--rw-rw-rw-   0        0        0     5999 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/commands/__init__.py
--rw-rw-rw-   0        0        0     1047 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/commands/crawl.py
--rw-rw-rw-   0        0        0     5263 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/commands/genspider.py
--rw-rw-rw-   0        0        0      910 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/commands/onespider.py
--rw-rw-rw-   0        0        0     2134 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/commands/runspider.py
--rw-rw-rw-   0        0        0     4127 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/commands/startproject.py
--rw-rw-rw-   0        0        0      958 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/commands/version.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.121635 aioscpy-0.3.8/aioscpy/core/
--rw-rw-rw-   0        0        0        0 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/core/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.122632 aioscpy-0.3.8/aioscpy/core/downloader/
--rw-rw-rw-   0        0        0     5809 2022-11-03 01:56:18.000000 aioscpy-0.3.8/aioscpy/core/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.125625 aioscpy-0.3.8/aioscpy/core/downloader/handlers/
--rw-rw-rw-   0        0        0        0 2022-06-10 02:28:33.000000 aioscpy-0.3.8/aioscpy/core/downloader/handlers/__init__.py
--rw-rw-rw-   0        0        0     3141 2022-11-01 09:04:28.000000 aioscpy-0.3.8/aioscpy/core/downloader/handlers/aiohttp.py
--rw-rw-rw-   0        0        0     1953 2022-11-01 09:03:45.000000 aioscpy-0.3.8/aioscpy/core/downloader/handlers/httpx.py
--rw-rw-rw-   0        0        0    10473 2022-11-02 10:18:50.000000 aioscpy-0.3.8/aioscpy/core/engine.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.129617 aioscpy-0.3.8/aioscpy/core/scheduler/
--rw-rw-rw-   0        0        0     1360 2022-08-04 04:06:12.000000 aioscpy-0.3.8/aioscpy/core/scheduler/__init__.py
--rw-rw-rw-   0        0        0      293 2022-05-13 06:12:44.000000 aioscpy-0.3.8/aioscpy/core/scheduler/memory.py
--rw-rw-rw-   0        0        0      619 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/core/scheduler/redis.py
--rw-rw-rw-   0        0        0    10041 2022-10-26 05:55:32.000000 aioscpy-0.3.8/aioscpy/core/scraper.py
--rw-rw-rw-   0        0        0     7386 2022-11-01 09:05:38.000000 aioscpy-0.3.8/aioscpy/crawler.py
--rw-rw-rw-   0        0        0     2101 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.130611 aioscpy-0.3.8/aioscpy/http/
--rw-rw-rw-   0        0        0      277 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/http/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.133607 aioscpy-0.3.8/aioscpy/http/request/
--rw-rw-rw-   0        0        0     3368 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/http/request/__init__.py
--rw-rw-rw-   0        0        0     1174 2022-06-15 02:08:07.000000 aioscpy-0.3.8/aioscpy/http/request/form.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.135598 aioscpy-0.3.8/aioscpy/http/response/
--rw-rw-rw-   0        0        0     5540 2022-06-07 10:04:59.000000 aioscpy-0.3.8/aioscpy/http/response/__init__.py
--rw-rw-rw-   0        0        0     7453 2022-06-15 02:14:29.000000 aioscpy-0.3.8/aioscpy/http/response/text.py
--rw-rw-rw-   0        0        0     6852 2022-10-24 09:41:23.000000 aioscpy-0.3.8/aioscpy/inject.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.137592 aioscpy-0.3.8/aioscpy/libs/
--rw-rw-rw-   0        0        0        0 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.138589 aioscpy-0.3.8/aioscpy/libs/downloadermiddlewares/
--rw-rw-rw-   0        0        0        0 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/libs/downloadermiddlewares/__init__.py
--rw-rw-rw-   0        0        0     2671 2022-05-11 07:02:46.000000 aioscpy-0.3.8/aioscpy/libs/downloadermiddlewares/stats.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.141582 aioscpy-0.3.8/aioscpy/libs/extensions/
--rw-rw-rw-   0        0        0        0 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/libs/extensions/__init__.py
--rw-rw-rw-   0        0        0     1771 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/libs/extensions/corestats.py
--rw-rw-rw-   0        0        0     1975 2022-07-15 09:13:54.000000 aioscpy-0.3.8/aioscpy/libs/extensions/logstats.py
--rw-rw-rw-   0        0        0     2173 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/libs/statscollectors.py
--rw-rw-rw-   0        0        0     3303 2022-05-20 05:38:55.000000 aioscpy-0.3.8/aioscpy/logformatter.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.149277 aioscpy-0.3.8/aioscpy/middleware/
--rw-rw-rw-   0        0        0      304 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/middleware/__init__.py
--rw-rw-rw-   0        0        0     3430 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/middleware/downloader.py
--rw-rw-rw-   0        0        0      341 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/middleware/extension.py
--rw-rw-rw-   0        0        0      663 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/middleware/itempipeline.py
--rw-rw-rw-   0        0        0     4180 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/middleware/manager.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.152266 aioscpy-0.3.8/aioscpy/queue/
--rw-rw-rw-   0        0        0     1715 2022-05-13 08:49:45.000000 aioscpy-0.3.8/aioscpy/queue/__init__.py
--rw-rw-rw-   0        0        0      949 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/queue/compat.py
--rw-rw-rw-   0        0        0     3370 2022-05-11 07:13:42.000000 aioscpy-0.3.8/aioscpy/queue/convert.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.154261 aioscpy-0.3.8/aioscpy/queue/memory/
--rw-rw-rw-   0        0        0      105 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/queue/memory/__init__.py
--rw-rw-rw-   0        0        0     1109 2022-08-04 04:07:58.000000 aioscpy-0.3.8/aioscpy/queue/memory/_queue.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.156256 aioscpy-0.3.8/aioscpy/queue/rabbitmq/
--rw-rw-rw-   0        0        0      128 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/queue/rabbitmq/__init__.py
--rw-rw-rw-   0        0        0     3497 2022-05-17 06:41:35.000000 aioscpy-0.3.8/aioscpy/queue/rabbitmq/_queue.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.159247 aioscpy-0.3.8/aioscpy/queue/redis/
--rw-rw-rw-   0        0        0      258 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/queue/redis/__init__.py
--rw-rw-rw-   0        0        0     2266 2022-05-17 06:41:35.000000 aioscpy-0.3.8/aioscpy/queue/redis/_queue.py
--rw-rw-rw-   0        0        0     3321 2022-08-04 04:04:14.000000 aioscpy-0.3.8/aioscpy/queue/redis/_queue_async.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.162246 aioscpy-0.3.8/aioscpy/settings/
--rw-rw-rw-   0        0        0    16204 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/settings/__init__.py
--rw-rw-rw-   0        0        0     2724 2022-10-19 02:06:17.000000 aioscpy-0.3.8/aioscpy/settings/default_settings.py
--rw-rw-rw-   0        0        0     2471 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/signalmanager.py
--rw-rw-rw-   0        0        0      810 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/signals.py
--rw-rw-rw-   0        0        0     2194 2022-05-11 06:37:07.000000 aioscpy-0.3.8/aioscpy/spider.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.090718 aioscpy-0.3.8/aioscpy/templates/
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.168954 aioscpy-0.3.8/aioscpy/templates/project/
--rw-rw-rw-   0        0        0        0 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/templates/project/__init__.py
--rw-rw-rw-   0        0        0      131 2022-05-23 06:48:39.000000 aioscpy-0.3.8/aioscpy/templates/project/aioscpy.cfg
--rw-rw-rw-   0        0        0     1573 2022-09-29 02:00:21.000000 aioscpy-0.3.8/aioscpy/templates/project/middlewares.py.tmpl
--rw-rw-rw-   0        0        0       97 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/templates/project/pipelines.py.tmpl
--rw-rw-rw-   0        0        0     1680 2022-09-29 01:59:19.000000 aioscpy-0.3.8/aioscpy/templates/project/settings.py.tmpl
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.169951 aioscpy-0.3.8/aioscpy/templates/project/spiders/
--rw-rw-rw-   0        0        0      166 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/templates/project/spiders/__init__.py
--rw-rw-rw-   0        0        0      723 2022-09-29 02:02:35.000000 aioscpy-0.3.8/aioscpy/templates/project/start.py.tmpl
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.171945 aioscpy-0.3.8/aioscpy/templates/spiders/
--rw-rw-rw-   0        0        0      362 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/templates/spiders/basic.tmpl
--rw-rw-rw-   0        0        0      949 2022-07-28 07:27:41.000000 aioscpy-0.3.8/aioscpy/templates/spiders/crawl.tmpl
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.182916 aioscpy-0.3.8/aioscpy/utils/
--rw-rw-rw-   0        0        0        0 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/utils/__init__.py
--rw-rw-rw-   0        0        0     3558 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/utils/common.py
--rw-rw-rw-   0        0        0     4493 2022-06-13 07:23:42.000000 aioscpy-0.3.8/aioscpy/utils/curl.py
--rw-rw-rw-   0        0        0     5334 2022-05-26 03:34:43.000000 aioscpy-0.3.8/aioscpy/utils/log.py
--rw-rw-rw-   0        0        0      896 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/utils/ossignal.py
--rw-rw-rw-   0        0        0     3968 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/utils/othtypes.py
--rw-rw-rw-   0        0        0     2352 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/utils/signal.py
--rw-rw-rw-   0        0        0      874 2022-05-10 09:41:18.000000 aioscpy-0.3.8/aioscpy/utils/template.py
--rw-rw-rw-   0        0        0     9984 2022-07-29 07:34:48.000000 aioscpy-0.3.8/aioscpy/utils/tools.py
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.110664 aioscpy-0.3.8/aioscpy.egg-info/
--rw-rw-rw-   0        0        0     6586 2022-11-04 05:46:28.000000 aioscpy-0.3.8/aioscpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2620 2022-11-04 05:46:28.000000 aioscpy-0.3.8/aioscpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-04 05:46:28.000000 aioscpy-0.3.8/aioscpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2022-11-04 05:46:28.000000 aioscpy-0.3.8/aioscpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-05-06 10:43:15.000000 aioscpy-0.3.8/aioscpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       64 2022-11-04 05:46:28.000000 aioscpy-0.3.8/aioscpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-11-04 05:46:28.000000 aioscpy-0.3.8/aioscpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-04 05:46:29.186905 aioscpy-0.3.8/cegex/
--rw-rw-rw-   0        0        0        0 2022-04-15 02:36:45.000000 aioscpy-0.3.8/cegex/__init__.py
--rw-rw-rw-   0        0        0     1057 2022-11-01 05:42:42.000000 aioscpy-0.3.8/cegex/baidu.py
--rw-rw-rw-   0        0        0      537 2022-07-28 07:15:08.000000 aioscpy-0.3.8/cegex/httpbin.py
--rw-rw-rw-   0        0        0      793 2022-07-28 07:15:45.000000 aioscpy-0.3.8/cegex/httpbin_post.py
--rw-rw-rw-   0        0        0       42 2022-11-04 05:46:29.188901 aioscpy-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     3387 2022-10-26 07:16:00.000000 aioscpy-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.540233 aioscpy-0.3.9/
+-rw-rw-rw-   0        0        0     1087 2022-03-23 06:54:05.000000 aioscpy-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0      148 2022-05-06 10:30:34.000000 aioscpy-0.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6586 2022-11-25 09:36:53.539234 aioscpy-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4178 2022-10-25 09:35:25.000000 aioscpy-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.467425 aioscpy-0.3.9/aioscpy/
+-rw-rw-rw-   0        0        0        7 2022-11-04 05:46:43.000000 aioscpy-0.3.9/aioscpy/VERSION
+-rw-rw-rw-   0        0        0      222 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/__init__.py
+-rw-rw-rw-   0        0        0       84 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/__main__.py
+-rw-rw-rw-   0        0        0     5304 2022-05-23 08:05:47.000000 aioscpy-0.3.9/aioscpy/cmdline.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.480389 aioscpy-0.3.9/aioscpy/commands/
+-rw-rw-rw-   0        0        0     5999 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/commands/__init__.py
+-rw-rw-rw-   0        0        0     1047 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/commands/crawl.py
+-rw-rw-rw-   0        0        0     5263 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/commands/genspider.py
+-rw-rw-rw-   0        0        0      910 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/commands/onespider.py
+-rw-rw-rw-   0        0        0     2134 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/commands/runspider.py
+-rw-rw-rw-   0        0        0     4127 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/commands/startproject.py
+-rw-rw-rw-   0        0        0      958 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/commands/version.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.482384 aioscpy-0.3.9/aioscpy/core/
+-rw-rw-rw-   0        0        0        0 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/core/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.483382 aioscpy-0.3.9/aioscpy/core/downloader/
+-rw-rw-rw-   0        0        0     5809 2022-11-03 01:56:18.000000 aioscpy-0.3.9/aioscpy/core/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.485377 aioscpy-0.3.9/aioscpy/core/downloader/handlers/
+-rw-rw-rw-   0        0        0        0 2022-06-10 02:28:33.000000 aioscpy-0.3.9/aioscpy/core/downloader/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3286 2022-11-25 09:17:58.000000 aioscpy-0.3.9/aioscpy/core/downloader/handlers/aiohttp.py
+-rw-rw-rw-   0        0        0     2114 2022-11-25 09:08:47.000000 aioscpy-0.3.9/aioscpy/core/downloader/handlers/httpx.py
+-rw-rw-rw-   0        0        0    10473 2022-11-02 10:18:50.000000 aioscpy-0.3.9/aioscpy/core/engine.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.488369 aioscpy-0.3.9/aioscpy/core/scheduler/
+-rw-rw-rw-   0        0        0     1360 2022-08-04 04:06:12.000000 aioscpy-0.3.9/aioscpy/core/scheduler/__init__.py
+-rw-rw-rw-   0        0        0      293 2022-05-13 06:12:44.000000 aioscpy-0.3.9/aioscpy/core/scheduler/memory.py
+-rw-rw-rw-   0        0        0      619 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/core/scheduler/redis.py
+-rw-rw-rw-   0        0        0    10041 2022-10-26 05:55:32.000000 aioscpy-0.3.9/aioscpy/core/scraper.py
+-rw-rw-rw-   0        0        0     7439 2022-11-04 06:19:22.000000 aioscpy-0.3.9/aioscpy/crawler.py
+-rw-rw-rw-   0        0        0     2101 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.489367 aioscpy-0.3.9/aioscpy/http/
+-rw-rw-rw-   0        0        0      346 2022-11-25 07:50:15.000000 aioscpy-0.3.9/aioscpy/http/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.492359 aioscpy-0.3.9/aioscpy/http/request/
+-rw-rw-rw-   0        0        0     3322 2022-11-25 09:18:53.000000 aioscpy-0.3.9/aioscpy/http/request/__init__.py
+-rw-rw-rw-   0        0        0     1199 2022-11-25 09:18:41.000000 aioscpy-0.3.9/aioscpy/http/request/form.py
+-rw-rw-rw-   0        0        0      678 2022-11-25 09:18:33.000000 aioscpy-0.3.9/aioscpy/http/request/json.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.494353 aioscpy-0.3.9/aioscpy/http/response/
+-rw-rw-rw-   0        0        0     5540 2022-06-07 10:04:59.000000 aioscpy-0.3.9/aioscpy/http/response/__init__.py
+-rw-rw-rw-   0        0        0     7453 2022-06-15 02:14:29.000000 aioscpy-0.3.9/aioscpy/http/response/text.py
+-rw-rw-rw-   0        0        0     6852 2022-10-24 09:41:23.000000 aioscpy-0.3.9/aioscpy/inject.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.496348 aioscpy-0.3.9/aioscpy/libs/
+-rw-rw-rw-   0        0        0        0 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.498343 aioscpy-0.3.9/aioscpy/libs/downloadermiddlewares/
+-rw-rw-rw-   0        0        0        0 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/libs/downloadermiddlewares/__init__.py
+-rw-rw-rw-   0        0        0     2737 2022-11-25 09:07:10.000000 aioscpy-0.3.9/aioscpy/libs/downloadermiddlewares/stats.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.500337 aioscpy-0.3.9/aioscpy/libs/extensions/
+-rw-rw-rw-   0        0        0        0 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/libs/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1771 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/libs/extensions/corestats.py
+-rw-rw-rw-   0        0        0     1975 2022-07-15 09:13:54.000000 aioscpy-0.3.9/aioscpy/libs/extensions/logstats.py
+-rw-rw-rw-   0        0        0     2173 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/libs/statscollectors.py
+-rw-rw-rw-   0        0        0     3303 2022-05-20 05:38:55.000000 aioscpy-0.3.9/aioscpy/logformatter.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.504327 aioscpy-0.3.9/aioscpy/middleware/
+-rw-rw-rw-   0        0        0      304 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/middleware/__init__.py
+-rw-rw-rw-   0        0        0     3430 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/middleware/downloader.py
+-rw-rw-rw-   0        0        0      341 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/middleware/extension.py
+-rw-rw-rw-   0        0        0      663 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/middleware/itempipeline.py
+-rw-rw-rw-   0        0        0     4180 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/middleware/manager.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.508316 aioscpy-0.3.9/aioscpy/queue/
+-rw-rw-rw-   0        0        0     1715 2022-05-13 08:49:45.000000 aioscpy-0.3.9/aioscpy/queue/__init__.py
+-rw-rw-rw-   0        0        0      949 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/queue/compat.py
+-rw-rw-rw-   0        0        0     3370 2022-05-11 07:13:42.000000 aioscpy-0.3.9/aioscpy/queue/convert.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.510311 aioscpy-0.3.9/aioscpy/queue/memory/
+-rw-rw-rw-   0        0        0      105 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/queue/memory/__init__.py
+-rw-rw-rw-   0        0        0     1109 2022-08-04 04:07:58.000000 aioscpy-0.3.9/aioscpy/queue/memory/_queue.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.512305 aioscpy-0.3.9/aioscpy/queue/rabbitmq/
+-rw-rw-rw-   0        0        0      128 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/queue/rabbitmq/__init__.py
+-rw-rw-rw-   0        0        0     3497 2022-05-17 06:41:35.000000 aioscpy-0.3.9/aioscpy/queue/rabbitmq/_queue.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.515297 aioscpy-0.3.9/aioscpy/queue/redis/
+-rw-rw-rw-   0        0        0      258 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/queue/redis/__init__.py
+-rw-rw-rw-   0        0        0     2266 2022-05-17 06:41:35.000000 aioscpy-0.3.9/aioscpy/queue/redis/_queue.py
+-rw-rw-rw-   0        0        0     3321 2022-08-04 04:04:14.000000 aioscpy-0.3.9/aioscpy/queue/redis/_queue_async.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.517292 aioscpy-0.3.9/aioscpy/settings/
+-rw-rw-rw-   0        0        0    16204 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/settings/__init__.py
+-rw-rw-rw-   0        0        0     2773 2022-11-25 09:20:01.000000 aioscpy-0.3.9/aioscpy/settings/default_settings.py
+-rw-rw-rw-   0        0        0     2471 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/signalmanager.py
+-rw-rw-rw-   0        0        0      810 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/signals.py
+-rw-rw-rw-   0        0        0     2194 2022-05-11 06:37:07.000000 aioscpy-0.3.9/aioscpy/spider.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.453462 aioscpy-0.3.9/aioscpy/templates/
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.522278 aioscpy-0.3.9/aioscpy/templates/project/
+-rw-rw-rw-   0        0        0        0 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/templates/project/__init__.py
+-rw-rw-rw-   0        0        0      131 2022-05-23 06:48:39.000000 aioscpy-0.3.9/aioscpy/templates/project/aioscpy.cfg
+-rw-rw-rw-   0        0        0     1573 2022-09-29 02:00:21.000000 aioscpy-0.3.9/aioscpy/templates/project/middlewares.py.tmpl
+-rw-rw-rw-   0        0        0       97 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/templates/project/pipelines.py.tmpl
+-rw-rw-rw-   0        0        0     1680 2022-09-29 01:59:19.000000 aioscpy-0.3.9/aioscpy/templates/project/settings.py.tmpl
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.523278 aioscpy-0.3.9/aioscpy/templates/project/spiders/
+-rw-rw-rw-   0        0        0      166 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/templates/project/spiders/__init__.py
+-rw-rw-rw-   0        0        0      723 2022-09-29 02:02:35.000000 aioscpy-0.3.9/aioscpy/templates/project/start.py.tmpl
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.525270 aioscpy-0.3.9/aioscpy/templates/spiders/
+-rw-rw-rw-   0        0        0      362 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/templates/spiders/basic.tmpl
+-rw-rw-rw-   0        0        0      949 2022-07-28 07:27:41.000000 aioscpy-0.3.9/aioscpy/templates/spiders/crawl.tmpl
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.535243 aioscpy-0.3.9/aioscpy/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/utils/__init__.py
+-rw-rw-rw-   0        0        0     3558 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/utils/common.py
+-rw-rw-rw-   0        0        0     4493 2022-06-13 07:23:42.000000 aioscpy-0.3.9/aioscpy/utils/curl.py
+-rw-rw-rw-   0        0        0     5334 2022-05-26 03:34:43.000000 aioscpy-0.3.9/aioscpy/utils/log.py
+-rw-rw-rw-   0        0        0      896 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/utils/ossignal.py
+-rw-rw-rw-   0        0        0     3968 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/utils/othtypes.py
+-rw-rw-rw-   0        0        0     2352 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/utils/signal.py
+-rw-rw-rw-   0        0        0      874 2022-05-10 09:41:18.000000 aioscpy-0.3.9/aioscpy/utils/template.py
+-rw-rw-rw-   0        0        0    10188 2022-11-04 06:19:09.000000 aioscpy-0.3.9/aioscpy/utils/tools.py
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.473410 aioscpy-0.3.9/aioscpy.egg-info/
+-rw-rw-rw-   0        0        0     6586 2022-11-25 09:36:52.000000 aioscpy-0.3.9/aioscpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2649 2022-11-25 09:36:52.000000 aioscpy-0.3.9/aioscpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-25 09:36:52.000000 aioscpy-0.3.9/aioscpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2022-11-25 09:36:52.000000 aioscpy-0.3.9/aioscpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-05-06 10:43:15.000000 aioscpy-0.3.9/aioscpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       64 2022-11-25 09:36:52.000000 aioscpy-0.3.9/aioscpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-11-25 09:36:52.000000 aioscpy-0.3.9/aioscpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-11-25 09:36:53.538236 aioscpy-0.3.9/cegex/
+-rw-rw-rw-   0        0        0        0 2022-04-15 02:36:45.000000 aioscpy-0.3.9/cegex/__init__.py
+-rw-rw-rw-   0        0        0     1057 2022-11-01 05:42:42.000000 aioscpy-0.3.9/cegex/baidu.py
+-rw-rw-rw-   0        0        0      537 2022-07-28 07:15:08.000000 aioscpy-0.3.9/cegex/httpbin.py
+-rw-rw-rw-   0        0        0     1445 2022-11-25 09:30:04.000000 aioscpy-0.3.9/cegex/httpbin_post.py
+-rw-rw-rw-   0        0        0       42 2022-11-25 09:36:53.541232 aioscpy-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     3387 2022-10-26 07:16:00.000000 aioscpy-0.3.9/setup.py
```

### Comparing `aioscpy-0.3.8/LICENSE` & `aioscpy-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/PKG-INFO` & `aioscpy-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioscpy
-Version: 0.3.8
+Version: 0.3.9
 Summary: An asyncio + aiolibs crawler imitate scrapy framework
 Home-page: https://github.com/ihandmine/aioscpy
 Author: handmine
 Author-email: handmine@outlook.com
 License: MIT
 Description:
```

### Comparing `aioscpy-0.3.8/README.md` & `aioscpy-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/cmdline.py` & `aioscpy-0.3.9/aioscpy/cmdline.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/commands/__init__.py` & `aioscpy-0.3.9/aioscpy/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/commands/crawl.py` & `aioscpy-0.3.9/aioscpy/commands/crawl.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/commands/genspider.py` & `aioscpy-0.3.9/aioscpy/commands/genspider.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/commands/onespider.py` & `aioscpy-0.3.9/aioscpy/commands/onespider.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/commands/runspider.py` & `aioscpy-0.3.9/aioscpy/commands/runspider.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/commands/startproject.py` & `aioscpy-0.3.9/aioscpy/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/commands/version.py` & `aioscpy-0.3.9/aioscpy/commands/version.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/core/downloader/__init__.py` & `aioscpy-0.3.9/aioscpy/core/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/core/downloader/handlers/aiohttp.py` & `aioscpy-0.3.9/aioscpy/core/downloader/handlers/aiohttp.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,16 +35,20 @@
     def from_crawler(cls, crawler):
         return cls.from_settings(crawler.settings, crawler)
 
     async def download_request(self, request, spider):
         session_kwargs = {
             'timeout': self.settings.get('DOWNLOAD_TIMEOUT'),
             'cookies': dict(request.cookies),
-            'data': request.body or None
         }
+        if isinstance(request.body, dict):
+            session_kwargs['json'] = request.body or None
+        else:
+            session_kwargs['data'] = request.body or None
+        
         headers = request.headers
         if isinstance(headers, Headers):
             headers = headers.to_unicode_dict()
         session_kwargs['headers'] = headers
 
         if request.meta.get('TLS_CIPHERS') or self.settings.get('TLS_CIPHERS'):
             self.context.set_ciphers(generate_cipher())
```

### Comparing `aioscpy-0.3.8/aioscpy/core/downloader/handlers/httpx.py` & `aioscpy-0.3.9/aioscpy/core/downloader/handlers/httpx.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,22 +31,27 @@
             self.context.set_ciphers(generate_cipher())
             httpx_client_session['verify'] = self.context
 
         if request.meta.get("proxy"):
             httpx_client_session['proxies'] = request.meta["proxy"]
             self.logger.debug(f"use {request.meta['proxy']} crawling: {request.url}")
 
+        session_kwargs = {
+            'timeout': self.settings.get('DOWNLOAD_TIMEOUT'),
+            'cookies': dict(request.cookies),
+            'headers': headers,
+            'follow_redirects': True
+        }
+        if isinstance(request.body, dict):
+            session_kwargs['json'] = request.body or None
+        else:
+            session_kwargs['data'] = request.body or None
+        
         async with httpx.AsyncClient(**httpx_client_session) as session:
-            response = await session.request(request.method, request.url, **{
-                'timeout': self.settings.get('DOWNLOAD_TIMEOUT'),
-                'cookies': dict(request.cookies),
-                'data': request.body or None,
-                'headers': headers,
-                'follow_redirects': True
-            })
+            response = await session.request(request.method, request.url, **session_kwargs)
             content = response.read()
 
         return self.di.get("response")(
             str(response.url),
             status=response.status_code,
             headers=response.headers,
             body=content,
```

### Comparing `aioscpy-0.3.8/aioscpy/core/engine.py` & `aioscpy-0.3.9/aioscpy/core/engine.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/core/scheduler/__init__.py` & `aioscpy-0.3.9/aioscpy/core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/core/scheduler/redis.py` & `aioscpy-0.3.9/aioscpy/core/scheduler/redis.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/core/scraper.py` & `aioscpy-0.3.9/aioscpy/core/scraper.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/crawler.py` & `aioscpy-0.3.9/aioscpy/crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,12 +177,13 @@
         signame = signal_names[signum]
         self.logger.info('Received {signame} twice, forcing unclean shutdown',
                     **{'signame': signame})
         asyncio.create_task(self._force_stop_reactor())
 
     def start(self):
         self.di.get("tools").install_event_loop_tips()
+        self.di.get("tools").install_patch_method()
         try:
             anyio.run(self.run, backend='asyncio')
             # asyncio.run(self.run())
         except asyncio.CancelledError:
             pass
```

### Comparing `aioscpy-0.3.8/aioscpy/exceptions.py` & `aioscpy-0.3.9/aioscpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/http/request/__init__.py` & `aioscpy-0.3.9/aioscpy/http/request/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def _get_body(self):
         return self._body
 
     def _set_body(self, body):
         if body is None:
             self._body = b''
         else:
-            self._body = self.di.get("tools").to_bytes(body, self.encoding)
+            self._body = body
 
     body = property(_get_body, _set_body)
 
     @property
     def encoding(self):
         return self._encoding
```

### Comparing `aioscpy-0.3.8/aioscpy/http/request/form.py` & `aioscpy-0.3.9/aioscpy/http/request/form.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
         if formdata:
             items = formdata.items() if isinstance(formdata, dict) else formdata
             querystr = _urlencode(items, self.encoding)
             if self.method == 'POST':
                 self.headers.setdefault(
                     b'Content-Type', [b'application/x-www-form-urlencoded'])
-                self._set_body(querystr)
+                self._set_body(to_bytes(querystr, self.encoding))
             else:
                 self._set_url(
                     self.url + ('&' if '?' in self.url else '?') + querystr)
 
 
 def _urlencode(seq, enc):
     values = [(to_bytes(k, enc), to_bytes(v, enc))
```

### Comparing `aioscpy-0.3.8/aioscpy/http/response/__init__.py` & `aioscpy-0.3.9/aioscpy/http/response/__init__.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/http/response/text.py` & `aioscpy-0.3.9/aioscpy/http/response/text.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/inject.py` & `aioscpy-0.3.9/aioscpy/inject.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/libs/downloadermiddlewares/stats.py` & `aioscpy-0.3.9/aioscpy/libs/downloadermiddlewares/stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     parsed = urlparse_cached(request)
     path = urlunparse(('', '', parsed.path or '/', parsed.params, parsed.query, ''))
     s = to_bytes(request.method) + b" " + to_bytes(path) + b" HTTP/1.1\r\n"
     s += b"Host: " + to_bytes(parsed.hostname or b'') + b"\r\n"
     if request.headers:
         s += request.headers.to_string() + b"\r\n"
     s += b"\r\n"
-    s += request.body
+    s += str(request.body).encode() if isinstance(request.body, dict) else request.body
     return s
 
 
 def get_header_size(headers):
     size = 0
     for key, value in headers.items():
         if isinstance(value, (list, tuple)):
```

### Comparing `aioscpy-0.3.8/aioscpy/libs/extensions/corestats.py` & `aioscpy-0.3.9/aioscpy/libs/extensions/corestats.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/libs/extensions/logstats.py` & `aioscpy-0.3.9/aioscpy/libs/extensions/logstats.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/libs/statscollectors.py` & `aioscpy-0.3.9/aioscpy/libs/statscollectors.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/logformatter.py` & `aioscpy-0.3.9/aioscpy/logformatter.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/middleware/downloader.py` & `aioscpy-0.3.9/aioscpy/middleware/downloader.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/middleware/itempipeline.py` & `aioscpy-0.3.9/aioscpy/middleware/itempipeline.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/middleware/manager.py` & `aioscpy-0.3.9/aioscpy/middleware/manager.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/queue/__init__.py` & `aioscpy-0.3.9/aioscpy/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/queue/compat.py` & `aioscpy-0.3.9/aioscpy/queue/compat.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/queue/convert.py` & `aioscpy-0.3.9/aioscpy/queue/convert.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/queue/memory/_queue.py` & `aioscpy-0.3.9/aioscpy/queue/memory/_queue.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/queue/rabbitmq/_queue.py` & `aioscpy-0.3.9/aioscpy/queue/rabbitmq/_queue.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/queue/redis/_queue.py` & `aioscpy-0.3.9/aioscpy/queue/redis/_queue.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/queue/redis/_queue_async.py` & `aioscpy-0.3.9/aioscpy/queue/redis/_queue_async.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/settings/__init__.py` & `aioscpy-0.3.9/aioscpy/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/settings/default_settings.py` & `aioscpy-0.3.9/aioscpy/settings/default_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     "extension": "aioscpy.middleware.ExtensionManager",
 
 }
 DI_CONFIG_CLS = {
     "request": "aioscpy.http.Request",
     "response": "aioscpy.http.TextResponse",
     "form_request": "aioscpy.http.FormRequest",
+    "json_request": "aioscpy.http.JsonRequest",
     "logger": "aioscpy.utils.log.logger",
     "log": "aioscpy.utils.log",
     "exceptions": "aioscpy.exceptions",
     "tools": "aioscpy.utils.tools",
     'downloader_middleware': 'aioscpy.middleware.DownloaderMiddlewareManager',
     "item_processor": "aioscpy.middleware.ItemPipelineManager",
 }
```

### Comparing `aioscpy-0.3.8/aioscpy/signalmanager.py` & `aioscpy-0.3.9/aioscpy/signalmanager.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/signals.py` & `aioscpy-0.3.9/aioscpy/signals.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/spider.py` & `aioscpy-0.3.9/aioscpy/spider.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/templates/project/middlewares.py.tmpl` & `aioscpy-0.3.9/aioscpy/templates/project/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/templates/project/settings.py.tmpl` & `aioscpy-0.3.9/aioscpy/templates/project/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/templates/project/start.py.tmpl` & `aioscpy-0.3.9/aioscpy/templates/project/start.py.tmpl`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/templates/spiders/crawl.tmpl` & `aioscpy-0.3.9/aioscpy/templates/spiders/crawl.tmpl`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/utils/common.py` & `aioscpy-0.3.9/aioscpy/utils/common.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/utils/curl.py` & `aioscpy-0.3.9/aioscpy/utils/curl.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/utils/log.py` & `aioscpy-0.3.9/aioscpy/utils/log.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/utils/ossignal.py` & `aioscpy-0.3.9/aioscpy/utils/ossignal.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/utils/othtypes.py` & `aioscpy-0.3.9/aioscpy/utils/othtypes.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/utils/signal.py` & `aioscpy-0.3.9/aioscpy/utils/signal.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/utils/template.py` & `aioscpy-0.3.9/aioscpy/utils/template.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/aioscpy/utils/tools.py` & `aioscpy-0.3.9/aioscpy/utils/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import ujson
+import json
 import asyncio
 import weakref
 import sys
 import os
 import pickle
 import warnings
 
@@ -316,7 +318,17 @@
 
 def obsolete_setter(setter, attrname):
     def newsetter(self, value):
         c = self.__class__.__name__
         msg = "%s.%s is not modifiable, use %s.replace() instead" % (c, attrname, c)
         raise AttributeError(msg)
     return newsetter
+
+
+def monkey_patch_json():
+    json.__name__ = 'ujson'
+    json.dumps = ujson.dumps
+    json.loads = ujson.loads
+
+
+def install_patch_method():
+    monkey_patch_json()
```

### Comparing `aioscpy-0.3.8/aioscpy.egg-info/PKG-INFO` & `aioscpy-0.3.9/aioscpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioscpy
-Version: 0.3.8
+Version: 0.3.9
 Summary: An asyncio + aiolibs crawler imitate scrapy framework
 Home-page: https://github.com/ihandmine/aioscpy
 Author: handmine
 Author-email: handmine@outlook.com
 License: MIT
 Description:
```

### Comparing `aioscpy-0.3.8/aioscpy.egg-info/SOURCES.txt` & `aioscpy-0.3.9/aioscpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 aioscpy/core/downloader/handlers/httpx.py
 aioscpy/core/scheduler/__init__.py
 aioscpy/core/scheduler/memory.py
 aioscpy/core/scheduler/redis.py
 aioscpy/http/__init__.py
 aioscpy/http/request/__init__.py
 aioscpy/http/request/form.py
+aioscpy/http/request/json.py
 aioscpy/http/response/__init__.py
 aioscpy/http/response/text.py
 aioscpy/libs/__init__.py
 aioscpy/libs/statscollectors.py
 aioscpy/libs/downloadermiddlewares/__init__.py
 aioscpy/libs/downloadermiddlewares/stats.py
 aioscpy/libs/extensions/__init__.py
```

### Comparing `aioscpy-0.3.8/cegex/baidu.py` & `aioscpy-0.3.9/cegex/baidu.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/cegex/httpbin.py` & `aioscpy-0.3.9/cegex/httpbin.py`

 * *Files identical despite different names*

### Comparing `aioscpy-0.3.8/setup.py` & `aioscpy-0.3.9/setup.py`

 * *Files identical despite different names*

