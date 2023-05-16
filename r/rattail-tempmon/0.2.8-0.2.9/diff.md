# Comparing `tmp/rattail-tempmon-0.2.8.tar.gz` & `tmp/rattail-tempmon-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/lance/src/rattail-tempmon/dist/.tmp-61fp2ggs/rattail-tempmon-0.2.8.tar", last modified: Sun Feb 12 17:22:26 2023, max compression
+gzip compressed data, was "rattail-tempmon-0.2.9.tar", last modified: Tue May 16 22:40:56 2023, max compression
```

## Comparing `rattail-tempmon-0.2.8.tar` & `rattail-tempmon-0.2.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/
--rw-r--r--   0 lance     (1000) lance     (1000)     4412 2023-02-12 17:22:01.000000 rattail-tempmon-0.2.8/CHANGES.rst
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 04:36:35.000000 rattail-tempmon-0.2.8/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      252 2016-12-11 04:16:13.000000 rattail-tempmon-0.2.8/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     1096 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      371 2017-07-07 04:37:44.000000 rattail-tempmon-0.2.8/README.rst
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon/
--rw-r--r--   0 lance     (1000) lance     (1000)     1008 2017-07-07 04:37:15.000000 rattail-tempmon-0.2.8/rattail_tempmon/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-02-12 17:22:03.000000 rattail-tempmon-0.2.8/rattail_tempmon/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7834 2023-02-12 04:24:45.000000 rattail-tempmon-0.2.8/rattail_tempmon/client.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5401 2017-11-19 04:01:12.000000 rattail-tempmon-0.2.8/rattail_tempmon/commands.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2076 2017-07-07 04:36:51.000000 rattail-tempmon-0.2.8/rattail_tempmon/config.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/
--rw-r--r--   0 lance     (1000) lance     (1000)     1082 2017-07-07 04:37:01.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2015-01-27 18:37:50.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/README
--rw-r--r--   0 lance     (1000) lance     (1000)     1958 2017-08-08 23:46:47.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/env.py
--rw-r--r--   0 lance     (1000) lance     (1000)      640 2017-08-05 17:53:32.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/script.py.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/
--rw-r--r--   0 lance     (1000) lance     (1000)      728 2018-09-28 17:24:26.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/34041e1032a2_add_client_probe_notes.py
--rw-r--r--   0 lance     (1000) lance     (1000)      600 2018-09-29 00:08:14.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/5f2b87474433_add_client_disk_type.py
--rw-r--r--   0 lance     (1000) lance     (1000)      639 2017-08-05 17:53:37.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/75c09e11543c_grow_degrees.py
--rw-r--r--   0 lance     (1000) lance     (1000)      587 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/76d52bb064b8_add_client_delay.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1383 2018-10-19 22:29:06.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/796084026e5b_add_appliance.py
--rw-rw-r--   0 lance     (1000) lance     (1000)     3462 2016-12-05 21:23:41.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/7c7d205787b0_initial_tables.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1039 2018-10-20 00:16:00.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/a2676d3dfc1e_add_appliance_images.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1847 2018-10-19 18:52:07.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/b02c531caca5_add_more_timeouts.py
--rw-r--r--   0 lance     (1000) lance     (1000)      778 2018-09-28 17:18:35.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/e9eb7fc0a451_add_client_archived.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2695 2019-01-26 00:47:51.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/fd1df160539a_make_enabled_datetime.py
--rw-r--r--   0 lance     (1000) lance     (1000)    16559 2023-02-08 16:54:09.000000 rattail-tempmon-0.2.8/rattail_tempmon/db/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5516 2019-06-13 17:06:43.000000 rattail-tempmon-0.2.8/rattail_tempmon/emails.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon/hotcooler/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.8/rattail_tempmon/hotcooler/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon/hotcooler/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.8/rattail_tempmon/hotcooler/importing/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5156 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.8/rattail_tempmon/hotcooler/importing/tempmon.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2095 2019-01-26 00:39:09.000000 rattail-tempmon-0.2.8/rattail_tempmon/problems.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13667 2019-05-05 16:34:10.000000 rattail-tempmon-0.2.8/rattail_tempmon/server.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2729 2018-10-23 15:22:14.000000 rattail-tempmon-0.2.8/rattail_tempmon/settings.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon/templates/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/
--rw-r--r--   0 lance     (1000) lance     (1000)      249 2018-02-07 23:48:07.000000 rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/tempmon_client_offline.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1260 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/tempmon_critical_high_temp.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1260 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/tempmon_critical_low_temp.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      873 2018-09-11 23:41:05.000000 rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/tempmon_disabled_probes.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      339 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/tempmon_error.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      268 2016-12-10 18:35:21.000000 rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/tempmon_good_temp.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      573 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/tempmon_high_temp.html.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      573 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/tempmon_low_temp.html.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1096 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)     2036 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      449 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       24 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       16 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/rattail_tempmon.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2023-02-12 17:22:26.000000 rattail-tempmon-0.2.8/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     4291 2023-02-08 16:53:08.000000 rattail-tempmon-0.2.8/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.794132 rattail-tempmon-0.2.9/
+-rw-r--r--   0 lance     (1000) lance     (1000)     4505 2023-05-16 22:40:30.000000 rattail-tempmon-0.2.9/CHANGES.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 04:36:35.000000 rattail-tempmon-0.2.9/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      252 2016-12-11 04:16:13.000000 rattail-tempmon-0.2.9/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     1096 2023-05-16 22:40:56.794132 rattail-tempmon-0.2.9/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      371 2017-07-07 04:37:44.000000 rattail-tempmon-0.2.9/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.754131 rattail-tempmon-0.2.9/rattail_tempmon/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1008 2017-07-07 04:37:15.000000 rattail-tempmon-0.2.9/rattail_tempmon/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-05-16 22:40:33.000000 rattail-tempmon-0.2.9/rattail_tempmon/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7834 2023-02-12 04:24:45.000000 rattail-tempmon-0.2.9/rattail_tempmon/client.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5401 2017-11-19 04:01:12.000000 rattail-tempmon-0.2.9/rattail_tempmon/commands.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2076 2017-07-07 04:36:51.000000 rattail-tempmon-0.2.9/rattail_tempmon/config.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.754131 rattail-tempmon-0.2.9/rattail_tempmon/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1082 2017-07-07 04:37:01.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.758131 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/
+-rw-r--r--   0 lance     (1000) lance     (1000)       38 2015-01-27 18:37:50.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/README
+-rw-r--r--   0 lance     (1000) lance     (1000)     1958 2017-08-08 23:46:47.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/env.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      640 2017-08-05 17:53:32.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/script.py.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.774131 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/
+-rw-r--r--   0 lance     (1000) lance     (1000)      728 2018-09-28 17:24:26.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/34041e1032a2_add_client_probe_notes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      600 2018-09-29 00:08:14.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/5f2b87474433_add_client_disk_type.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      639 2017-08-05 17:53:37.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/75c09e11543c_grow_degrees.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      587 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/76d52bb064b8_add_client_delay.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1383 2018-10-19 22:29:06.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/796084026e5b_add_appliance.py
+-rw-rw-r--   0 lance     (1000) lance     (1000)     3462 2016-12-05 21:23:41.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/7c7d205787b0_initial_tables.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1039 2018-10-20 00:16:00.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/a2676d3dfc1e_add_appliance_images.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1847 2018-10-19 18:52:07.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/b02c531caca5_add_more_timeouts.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      778 2018-09-28 17:18:35.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/e9eb7fc0a451_add_client_archived.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2695 2019-01-26 00:47:51.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/fd1df160539a_make_enabled_datetime.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    16559 2023-02-08 16:54:09.000000 rattail-tempmon-0.2.9/rattail_tempmon/db/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5516 2019-06-13 17:06:43.000000 rattail-tempmon-0.2.9/rattail_tempmon/emails.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.778131 rattail-tempmon-0.2.9/rattail_tempmon/hotcooler/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/hotcooler/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.778131 rattail-tempmon-0.2.9/rattail_tempmon/hotcooler/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/hotcooler/importing/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5156 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/hotcooler/importing/tempmon.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2095 2019-01-26 00:39:09.000000 rattail-tempmon-0.2.9/rattail_tempmon/problems.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13667 2019-05-05 16:34:10.000000 rattail-tempmon-0.2.9/rattail_tempmon/server.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2729 2018-10-23 15:22:14.000000 rattail-tempmon-0.2.9/rattail_tempmon/settings.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.742131 rattail-tempmon-0.2.9/rattail_tempmon/templates/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.794132 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/
+-rw-r--r--   0 lance     (1000) lance     (1000)      249 2018-02-07 23:48:07.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_client_offline.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1260 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_critical_high_temp.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1260 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_critical_low_temp.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      873 2018-09-11 23:41:05.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_disabled_probes.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      339 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_error.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      268 2016-12-10 18:35:21.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_good_temp.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      573 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_high_temp.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      573 2017-07-06 21:38:38.000000 rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_low_temp.html.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-16 22:40:56.754131 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1096 2023-05-16 22:40:56.000000 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)     2046 2023-05-16 22:40:56.000000 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-05-16 22:40:56.000000 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      449 2023-05-16 22:40:56.000000 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       24 2023-05-16 22:40:56.000000 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       16 2023-05-16 22:40:56.000000 rattail-tempmon-0.2.9/rattail_tempmon.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1295 2023-05-16 22:40:56.794132 rattail-tempmon-0.2.9/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     1015 2023-05-16 18:21:17.000000 rattail-tempmon-0.2.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rattail-tempmon-0.2.8/CHANGES.rst` & `rattail-tempmon-0.2.9/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 
 CHANGELOG
 =========
 
+0.2.9 (2023-05-16)
+------------------
+
+* Replace ``setup.py`` contents with ``setup.cfg``.
+
+
 0.2.8 (2023-02-12)
 ------------------
 
 * Refactor ``Query.get()`` => ``Session.get()`` per SQLAlchemy 1.4.
 
 
 0.2.7 (2023-02-10)
```

### Comparing `rattail-tempmon-0.2.8/COPYING.txt` & `rattail-tempmon-0.2.9/COPYING.txt`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/PKG-INFO` & `rattail-tempmon-0.2.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-tempmon
-Version: 0.2.8
+Version: 0.2.9
 Summary: Retail Software Framework - Temperature monitoring add-on
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/__init__.py` & `rattail-tempmon-0.2.9/rattail_tempmon/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/client.py` & `rattail-tempmon-0.2.9/rattail_tempmon/client.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/commands.py` & `rattail-tempmon-0.2.9/rattail_tempmon/commands.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/config.py` & `rattail-tempmon-0.2.9/rattail_tempmon/config.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/__init__.py` & `rattail-tempmon-0.2.9/rattail_tempmon/db/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/env.py` & `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/env.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/script.py.mako` & `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/34041e1032a2_add_client_probe_notes.py` & `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/34041e1032a2_add_client_probe_notes.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/5f2b87474433_add_client_disk_type.py` & `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/5f2b87474433_add_client_disk_type.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/75c09e11543c_grow_degrees.py` & `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/75c09e11543c_grow_degrees.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/76d52bb064b8_add_client_delay.py` & `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/76d52bb064b8_add_client_delay.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/796084026e5b_add_appliance.py` & `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/796084026e5b_add_appliance.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/7c7d205787b0_initial_tables.py` & `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/7c7d205787b0_initial_tables.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/a2676d3dfc1e_add_appliance_images.py` & `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/a2676d3dfc1e_add_appliance_images.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/b02c531caca5_add_more_timeouts.py` & `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/b02c531caca5_add_more_timeouts.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/e9eb7fc0a451_add_client_archived.py` & `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/e9eb7fc0a451_add_client_archived.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/alembic/versions/fd1df160539a_make_enabled_datetime.py` & `rattail-tempmon-0.2.9/rattail_tempmon/db/alembic/versions/fd1df160539a_make_enabled_datetime.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/db/model.py` & `rattail-tempmon-0.2.9/rattail_tempmon/db/model.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/emails.py` & `rattail-tempmon-0.2.9/rattail_tempmon/emails.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/hotcooler/importing/tempmon.py` & `rattail-tempmon-0.2.9/rattail_tempmon/hotcooler/importing/tempmon.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/problems.py` & `rattail-tempmon-0.2.9/rattail_tempmon/problems.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/server.py` & `rattail-tempmon-0.2.9/rattail_tempmon/server.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/settings.py` & `rattail-tempmon-0.2.9/rattail_tempmon/settings.py`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/tempmon_critical_high_temp.html.mako` & `rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_critical_high_temp.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/tempmon_critical_low_temp.html.mako` & `rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_critical_low_temp.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/tempmon_disabled_probes.html.mako` & `rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_disabled_probes.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/tempmon_high_temp.html.mako` & `rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_high_temp.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon/templates/mail/tempmon_low_temp.html.mako` & `rattail-tempmon-0.2.9/rattail_tempmon/templates/mail/tempmon_low_temp.html.mako`

 * *Files identical despite different names*

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon.egg-info/PKG-INFO` & `rattail-tempmon-0.2.9/rattail_tempmon.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-tempmon
-Version: 0.2.8
+Version: 0.2.9
 Summary: Retail Software Framework - Temperature monitoring add-on
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rattail-tempmon-0.2.8/rattail_tempmon.egg-info/SOURCES.txt` & `rattail-tempmon-0.2.9/rattail_tempmon.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CHANGES.rst
 COPYING.txt
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 rattail_tempmon/__init__.py
 rattail_tempmon/_version.py
 rattail_tempmon/client.py
 rattail_tempmon/commands.py
 rattail_tempmon/config.py
 rattail_tempmon/emails.py
```

