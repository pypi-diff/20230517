# Comparing `tmp/episoder-0.9.1.tar.gz` & `tmp/episoder-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/episoder-0.9.1.tar", last modified: Sun Oct 11 01:28:23 2020, max compression
+gzip compressed data, was "dist/episoder-0.9.2.tar", last modified: Fri Jan  1 12:45:48 2021, max compression
```

## Comparing `episoder-0.9.1.tar` & `episoder-0.9.2.tar`

### file list

```diff
@@ -1,37 +1,74 @@
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2020-10-11 01:28:23.037130 episoder-0.9.1/
--rw-r--r--   0 stefan    (1027) stefan    (1027)       31 2018-11-19 01:09:10.000000 episoder-0.9.1/AUTHORS
--rw-r--r--   0 stefan    (1027) stefan    (1027)     8106 2020-10-11 01:27:32.000000 episoder-0.9.1/CHANGELOG
--rw-r--r--   0 stefan    (1027) stefan    (1027)    35147 2018-11-19 01:09:10.000000 episoder-0.9.1/COPYING
--rw-r--r--   0 stefan    (1027) stefan    (1027)      841 2020-10-11 01:28:23.036130 episoder-0.9.1/PKG-INFO
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1618 2020-10-11 01:18:15.000000 episoder-0.9.1/README.md
--rwxr-xr-x   0 stefan    (1027) stefan    (1027)    13313 2020-03-28 21:52:38.000000 episoder-0.9.1/episoder
--rw-r--r--   0 stefan    (1027) stefan    (1027)     9425 2020-03-28 21:52:38.000000 episoder-0.9.1/episoder.1
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2020-10-11 01:28:23.032130 episoder-0.9.1/episoder.egg-info/
--rw-r--r--   0 stefan    (1027) stefan    (1027)      841 2020-10-11 01:28:22.000000 episoder-0.9.1/episoder.egg-info/PKG-INFO
--rw-r--r--   0 stefan    (1027) stefan    (1027)      613 2020-10-11 01:28:23.000000 episoder-0.9.1/episoder.egg-info/SOURCES.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)        1 2020-10-11 01:28:22.000000 episoder-0.9.1/episoder.egg-info/dependency_links.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)       38 2020-10-11 01:28:22.000000 episoder-0.9.1/episoder.egg-info/requires.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)       11 2020-10-11 01:28:22.000000 episoder-0.9.1/episoder.egg-info/top_level.txt
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2020-10-11 01:28:23.032130 episoder-0.9.1/examples/
--rw-r--r--   0 stefan    (1027) stefan    (1027)      950 2020-03-28 21:27:06.000000 episoder-0.9.1/examples/home.episoder
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2020-10-11 01:28:23.033130 episoder-0.9.1/pyepisoder/
--rw-r--r--   0 stefan    (1027) stefan    (1027)        0 2020-10-10 23:22:31.000000 episoder-0.9.1/pyepisoder/__init__.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     3767 2020-10-11 01:18:15.000000 episoder-0.9.1/pyepisoder/database.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     8092 2020-10-11 01:18:15.000000 episoder-0.9.1/pyepisoder/episoder.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     5167 2020-10-11 01:18:15.000000 episoder-0.9.1/pyepisoder/output.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)    11174 2020-10-11 01:18:15.000000 episoder-0.9.1/pyepisoder/sources.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)      762 2020-10-11 01:27:32.000000 episoder-0.9.1/pyepisoder/version.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)       38 2020-10-11 01:28:23.037130 episoder-0.9.1/setup.cfg
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1765 2020-10-11 01:27:32.000000 episoder-0.9.1/setup.py
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2020-10-11 01:28:23.036130 episoder-0.9.1/test/
--rw-r--r--   0 stefan    (1027) stefan    (1027)    14912 2020-10-11 01:18:15.000000 episoder-0.9.1/test/test_database.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)    14578 2020-10-11 01:18:15.000000 episoder-0.9.1/test/test_epguides_parser.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     2690 2020-10-11 01:18:15.000000 episoder-0.9.1/test/test_episode.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1103 2020-10-11 01:18:15.000000 episoder-0.9.1/test/test_metainfo.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)    12034 2020-10-11 01:18:15.000000 episoder-0.9.1/test/test_migration.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     8670 2020-10-11 01:18:15.000000 episoder-0.9.1/test/test_notify.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     6774 2020-10-11 01:18:15.000000 episoder-0.9.1/test/test_output.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     2681 2020-10-11 01:18:15.000000 episoder-0.9.1/test/test_show.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1521 2020-10-11 01:18:15.000000 episoder-0.9.1/test/test_sources.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1241 2020-10-11 01:18:15.000000 episoder-0.9.1/test/test_tvcom.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)    13429 2020-10-11 01:18:15.000000 episoder-0.9.1/test/test_tvdb.py
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2021-01-01 12:45:48.000000 episoder-0.9.2/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       12 2015-09-26 00:30:25.000000 episoder-0.9.2/.gitignore
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     2414 2021-01-01 12:37:21.000000 episoder-0.9.2/.gitlab-ci.yml
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       31 2015-09-26 00:30:25.000000 episoder-0.9.2/AUTHORS
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     8378 2021-01-01 12:44:38.000000 episoder-0.9.2/CHANGELOG
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    35147 2015-09-26 00:30:25.000000 episoder-0.9.2/COPYING
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      841 2021-01-01 12:45:48.000000 episoder-0.9.2/PKG-INFO
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1760 2021-01-01 12:37:21.000000 episoder-0.9.2/README.md
+-rwxr-xr-x   0 stefan    (1027) stefan    (1027)    13300 2021-01-01 12:37:21.000000 episoder-0.9.2/episoder
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     9387 2021-01-01 12:37:21.000000 episoder-0.9.2/episoder.1
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2021-01-01 12:45:48.000000 episoder-0.9.2/episoder.egg-info/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      841 2021-01-01 12:45:48.000000 episoder-0.9.2/episoder.egg-info/PKG-INFO
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1950 2021-01-01 12:45:48.000000 episoder-0.9.2/episoder.egg-info/SOURCES.txt
+-rw-r--r--   0 stefan    (1027) stefan    (1027)        1 2021-01-01 12:45:48.000000 episoder-0.9.2/episoder.egg-info/dependency_links.txt
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       38 2021-01-01 12:45:48.000000 episoder-0.9.2/episoder.egg-info/requires.txt
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       11 2021-01-01 12:45:48.000000 episoder-0.9.2/episoder.egg-info/top_level.txt
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2021-01-01 12:45:48.000000 episoder-0.9.2/examples/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      950 2020-09-21 10:29:57.000000 episoder-0.9.2/examples/home.episoder
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2021-01-01 12:45:48.000000 episoder-0.9.2/pyepisoder/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)        0 2015-09-26 00:30:25.000000 episoder-0.9.2/pyepisoder/__init__.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     3767 2021-01-01 12:37:21.000000 episoder-0.9.2/pyepisoder/database.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     8092 2021-01-01 12:37:21.000000 episoder-0.9.2/pyepisoder/episoder.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     5150 2021-01-01 12:37:21.000000 episoder-0.9.2/pyepisoder/output.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    11456 2021-01-01 12:37:21.000000 episoder-0.9.2/pyepisoder/sources.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      762 2021-01-01 12:44:38.000000 episoder-0.9.2/pyepisoder/version.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       38 2021-01-01 12:45:48.000000 episoder-0.9.2/setup.cfg
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1765 2021-01-01 12:37:16.000000 episoder-0.9.2/setup.py
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2021-01-01 12:45:48.000000 episoder-0.9.2/test/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)        0 2020-09-21 10:29:57.000000 episoder-0.9.2/test/__init__.py
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2021-01-01 12:45:48.000000 episoder-0.9.2/test/fixtures/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    37502 2015-11-07 02:49:50.000000 episoder-0.9.2/test/fixtures/epguides_48_hours_mistery.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)   113934 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/epguides_american_idol.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    32726 2015-11-07 02:27:36.000000 episoder-0.9.2/test/fixtures/epguides_bsg.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    46828 2015-09-26 00:30:25.000000 episoder-0.9.2/test/fixtures/epguides_buzzcocks.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    98137 2021-01-01 12:37:21.000000 episoder-0.9.2/test/fixtures/epguides_doctor_who.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    22460 2015-11-07 02:47:59.000000 episoder-0.9.2/test/fixtures/epguides_eureka.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    31378 2015-11-07 02:43:24.000000 episoder-0.9.2/test/fixtures/epguides_futurama.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    37156 2015-11-07 02:46:18.000000 episoder-0.9.2/test/fixtures/epguides_house.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    13603 2015-09-26 00:30:25.000000 episoder-0.9.2/test/fixtures/epguides_kr2008.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    33005 2015-11-07 02:19:47.000000 episoder-0.9.2/test/fixtures/epguides_lost.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    57390 2021-01-01 12:37:16.000000 episoder-0.9.2/test/fixtures/epguides_lost_html.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    16252 2021-01-01 12:37:16.000000 episoder-0.9.2/test/fixtures/epguides_lower_decks.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    27052 2015-11-07 02:44:50.000000 episoder-0.9.2/test/fixtures/epguides_midsomer_murders.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     6429 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/epguides_test_iso_8859_1.html
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       35 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_error_404.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      756 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_search_frasier.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1367 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_search_friends.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       75 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_260.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      329 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_260_1_eps.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       53 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_261.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      403 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_261_1_eps.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      399 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_261_2_eps.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      290 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_261_3_eps.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       53 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_262.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      315 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_262_1_eps.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       53 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_263.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      706 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_268156.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    18991 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_268156_1_eps.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       67 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_73739.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      217 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_73739_1_eps.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       78 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_75397.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     2759 2020-09-21 10:29:57.000000 episoder-0.9.2/test/fixtures/tvdb_test_show_75397_1_eps.json
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    14912 2021-01-01 12:37:21.000000 episoder-0.9.2/test/test_database.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    16381 2021-01-01 12:37:21.000000 episoder-0.9.2/test/test_epguides_parser.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     2690 2021-01-01 12:37:21.000000 episoder-0.9.2/test/test_episode.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1103 2021-01-01 12:37:21.000000 episoder-0.9.2/test/test_metainfo.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    12034 2021-01-01 12:37:21.000000 episoder-0.9.2/test/test_migration.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     8670 2021-01-01 12:37:21.000000 episoder-0.9.2/test/test_notify.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     8917 2021-01-01 12:37:21.000000 episoder-0.9.2/test/test_output.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     2681 2021-01-01 12:37:21.000000 episoder-0.9.2/test/test_show.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1521 2021-01-01 12:37:21.000000 episoder-0.9.2/test/test_sources.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1241 2021-01-01 12:37:21.000000 episoder-0.9.2/test/test_tvcom.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    13429 2021-01-01 12:37:21.000000 episoder-0.9.2/test/test_tvdb.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1660 2021-01-01 12:37:21.000000 episoder-0.9.2/test/util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `episoder-0.9.1/CHANGELOG` & `episoder-0.9.2/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+== 0.9.2 (1 Jan 2021) ==
+ * Fix a crash when trying to render episodes without production number
+ * Use appropriate colors when showing episodes from a past date
+ * Fix formatting of show names in list of shows
+ * Accept empty episode lines in epguide HTML format parser
+
 == 0.9.1 (11 Oct 2020) ==
  * Fix setup.py
 
 == 0.9.0 (11 Oct 2020) ==
  * Add support for new HTML format on epguides.com (thanks to Jethro Beekman)
 
 == 0.8.5 (28 Mar 2020) ==
```

### Comparing `episoder-0.9.1/COPYING` & `episoder-0.9.2/COPYING`

 * *Files identical despite different names*

### Comparing `episoder-0.9.1/PKG-INFO` & `episoder-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: episoder
-Version: 0.9.1
+Version: 0.9.2
 Summary: TV episode notifier
 Home-page: https://code.ott.net/episoder
 Author: Stefan Ott
 Author-email: stefan@ott.net
 License: GPLv3
 Description: episoder is a tool to tell you about new episodes of your favourite TV shows
 Platform: UNKNOWN
```

### Comparing `episoder-0.9.1/README.md` & `episoder-0.9.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 
 ## Dependencies
 
 In order to use episoder, you will need python installed on your system. In
 addition to the default distribution, the `requests`, `sqlalchemy` and `bs4`
 modules are required.
 
+## Downloading
+
+The official website, bug tracker etc. for episoder can be found at
+[code.ott.net/episoder](https://code.ott.net/episoder/).
+
 ## Installation
 
 You can install episoder through [pypi](https://pypi.python.org/pypi/episoder)
 (using `easy_install` or `pip`) or by running `setup.py` from the downloaded and
 extracted tarball.
 
 ## Configuration
```

### Comparing `episoder-0.9.1/episoder` & `episoder-0.9.2/episoder`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 # episoder, https://code.ott.net/episoder
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -364,20 +364,19 @@
 		enabled_strings = ["Disabled", "Enabled"]
 
 		for show in database.get_shows():
 
 			if self._args.active and show.status == Show.ENDED:
 				continue
 
-			name = show.name.encode("utf8")
 			status = status_strings[show.status or 0]
 			enabled = enabled_strings[show.enabled]
 
 			print("[%4d] %s" % (show.id, show.url))
-			print("       %s, %s, %s" % (name, status, enabled))
+			print("       %s, %s, %s" % (show.name, status, enabled))
 			print("       Last update: %s" % (show.updated))
 			print("       Episodes: %d" % len(show.episodes))
 
 	def notify(self):
 
 		opt = self._args
 
@@ -422,15 +421,15 @@
 			n_days = self._args.days
 
 		if self._args.search:
 			episodes = database.search(self._args.search)
 		else:
 			episodes = database.get_episodes(startdate, n_days)
 
-		out.render(episodes, not self._args.nocolor)
+		out.render(episodes, self._args.date, not self._args.nocolor)
 
 	def search(self):
 
 		tvdb = TVDB()
 		tvdb.login(self._args)
 
 		try:
```

### Comparing `episoder-0.9.1/episoder.1` & `episoder-0.9.2/episoder.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .TH EPISODER 1
 .SH NAME
 episoder \- TV show episode reminder.
 .SH SYNOPSIS
 .B episoder
 [global options] [command] [command-specific options]
 .SH COPYRIGHT
-episoder is Copyright (C) 2004-2020 by Stefan Ott
+episoder is Copyright (C) 2004-2021 by Stefan Ott
 .SH DESCRIPTION
 episoder is a tool to tell you about new episodes of your favourite TV shows
 .SH GLOBAL OPTIONS
 .TP
 .B \-h
 Show help and quit.
 .TP
@@ -129,23 +129,23 @@
 .B episoder \fR[options] \fBnotify \fR[notify-options]
 .PP
 Send e-mail notifications about recently discovered episodes. You can run this command after \fBepisoder update \fRin order to get a friendly reminder about upcoming episodes to your INBOX.
 .PP
 The \fBnotify \fRcommand knows the following extra options:
 .TP
 .B \-d \fIDATE\fR
-Only report episodes that air prior to \fIDATE\fR. You can either specify an absolute date as \fIYYYY-MM-DD\fR or a relative date by passing the number of days back. The default is TODO.
+Only report episodes that air prior to \fIDATE\fR. You can either specify an absolute date as \fIYYYY-MM-DD\fR or a relative date by passing the number of days back.
 .TP
 .B \-n \fIDAYS\fB, \-\-days \fIDAYS\fR
-The number of days to include. Any episodes that are more than \fIDAYS\fR days in the future will be ignored. The default value is TODO (2?).
+The number of days to include. Any episodes that are more than \fIDAYS\fR days in the future will be ignored. The default value is 2.
 .TP
 .B \-s \fIID\fB, \-\-show \fIID\fR
 Only send notifications about episodes that belong to the show with the id \fIID\fR.
 .TP
-Note that you will need to configure your e-mail settings in the configuration file (see below for details).
+Note that you will need to configure your e-mail settings in the configuration file (see above for details).
 .SH EXAMPLES
 Find a show on TheTVDB.com:
 .IP
 .B episoder search dexter
 .IP
 The output will look like this:
 .IP
@@ -186,15 +186,15 @@
 .LP
 The configuration file contains default settings for episoder.
 .TP
 .B agent=foo
 Set the user-agent string to be used when fetching data. This is only used for shows on epguides.com.
 .TP
 .B data=/path/to/file
-Path to episoder's data file. If, instead of a file, you supply a database url (as expected by sqlalchemy, eg. 'mysql://localhost/episoder'), episoder is going to use that database for storage instead.
+Path to episoder's data file. If, instead of a file, you supply a database url as expected by sqlalchemy, eg. 'mysql://localhost/episoder', episoder will use that database for storage instead.
 .TP
 .B format=unquoted format string
 This allows you to customize episoder's output. Available fields are:
 .PP
         %airdate     The episode's airdate as YYYY-MM-DD
         %show        Name of the show
         %season      Current season
```

### Comparing `episoder-0.9.1/episoder.egg-info/PKG-INFO` & `episoder-0.9.2/episoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: episoder
-Version: 0.9.1
+Version: 0.9.2
 Summary: TV episode notifier
 Home-page: https://code.ott.net/episoder
 Author: Stefan Ott
 Author-email: stefan@ott.net
 License: GPLv3
 Description: episoder is a tool to tell you about new episodes of your favourite TV shows
 Platform: UNKNOWN
```

### Comparing `episoder-0.9.1/examples/home.episoder` & `episoder-0.9.2/examples/home.episoder`

 * *Files identical despite different names*

### Comparing `episoder-0.9.1/pyepisoder/database.py` & `episoder-0.9.2/pyepisoder/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # episoder, https://code.ott.net/episoder
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `episoder-0.9.1/pyepisoder/episoder.py` & `episoder-0.9.2/pyepisoder/episoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # episoder, https://code.ott.net/episoder
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `episoder-0.9.1/pyepisoder/output.py` & `episoder-0.9.2/pyepisoder/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # episoder, https://code.ott.net/episoder
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -34,15 +34,15 @@
         airdate = episode.airdate.strftime(self._dateformat)
         string = string.replace("%airdate", airdate)
         string = string.replace("%show", episode.show.name)
         string = string.replace("%season", str(episode.season))
         string = string.replace("%epnum", "%02d" % episode.episode)
         string = string.replace("%eptitle", str(episode.title))
         string = string.replace("%totalep", str(episode.totalnum))
-        string = string.replace("%prodnum", episode.prodnum)
+        string = string.replace("%prodnum", str(episode.prodnum))
 
         return string
 
 
 class ConsoleRenderer(FormattingRenderer):
 
     RED = "\033[31;1m"
@@ -73,17 +73,16 @@
 
         self._dest.write("%s\n" % (string))
 
     def _render(self, episode, render, color):
 
         render(self.format(episode), color)
 
-    def render(self, episodes, use_colors=True):
+    def render(self, episodes, today, use_colors=True):
 
-        today = date.today()
         yesterday = today - timedelta(1)
         tomorrow = today + timedelta(1)
 
         if use_colors:
             render = self._render_color
         else:
             render = self._render_no_color
```

### Comparing `episoder-0.9.1/pyepisoder/sources.py` & `episoder-0.9.2/pyepisoder/sources.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # episoder, https://code.ott.net/episoder
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -335,30 +335,39 @@
                 return ""
             else:
                 return field.contents[0].strip()
 
         line = BeautifulSoup(line, "html.parser")
         epinfos = line.find_all("td", class_="epinfo")
 
+        # We expect 3 cells, otherwise we refuse to go on
+        if len(epinfos) < 3:
+            return None
+
         total = contents(epinfos[0]).split(".",1)[0]
         try:
             total = int(total)
         except ValueError:
             # Some shows have specials (numbered separately)
             total = -1
-        [season, epnum] = contents(epinfos[1]).split("-")
+
+        details = contents(epinfos[1]).split("-")
+        if len(details) < 2:
+            return None
+
+        [season, epnum] = details
         day = contents(epinfos[2])
         if not day:
-            # Some episodes don't have dates
-            day = "01 Jan 70"
+            # Drop episodes without date
+            return None
 
         title = contents(line.find("td", class_="eptitle").find("a"))
 
-        prodnum = None
-        return (total, season, epnum, prodnum, day, title)
+        # prodnum is None, we dont' have those
+        return (total, season, epnum, None, day, title)
 
     def _parse_line(self, line, show, db):
 
         # Name of the show
         res = search(r"<title>(.*)</title>", line)
         if res:
             title = res.groups()[0]
@@ -381,17 +390,20 @@
         if res:
             text = res.groups()[0]
             if "ended" in text:
                 show.status = Show.ENDED
             else:
                 show.status = Show.RUNNING
 
-        res = search(r"<td class=.epinfo", line)
-        if res:
-            (total, season, epnum, prodnum, day, title) = self._html_line(line)
+        if search(r"<td class=.epinfo", line):
+            fields = self._html_line(line)
+            if fields:
+                (total, season, epnum, prodnum, day, title) = fields
+            else:
+                return
 
         # Known formatting supported by this fine regex:
         # 4.     1-4        19 Jun 02  <a [..]>title</a>
         #   1.  19- 1   01-01    5 Jan 88  <a [..]>title</a>
         # 23     3-05       27/Mar/98  <a [..]>title</a>
         # 65.   17-10       23 Apr 05  <a [..]>title</a>
         # 101.   5-15       09 May 09  <a [..]>title</a>
```

### Comparing `episoder-0.9.1/pyepisoder/version.py` & `episoder-0.9.2/pyepisoder/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # episoder, https://code.ott.net/episoder
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
```

### Comparing `episoder-0.9.1/setup.py` & `episoder-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `episoder-0.9.1/test/test_database.py` & `episoder-0.9.2/test/test_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # episoder, https://code.ott.net/episoder
 # -*- coding: utf8 -*-
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `episoder-0.9.1/test/test_epguides_parser.py` & `episoder-0.9.2/test/test_epguides_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # episoder, https://code.ott.net/episoder
 # -*- coding: utf8 -*-
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -415,7 +415,54 @@
         self.assertEqual(date(2020, 9, 8), episode.airdate)
 
         episode = episodes[10]
         self.assertEqual(1, episode.season)
         self.assertEqual(10, episode.episode)
         self.assertEqual("No Small Parts", episode.title)
         self.assertEqual(date(2020, 10, 8), episode.airdate)
+
+    def test_empty_episode_lines_in_html_shows(self):
+
+        # This page has some epinfo table cells that should contain
+        # episode data but don't
+
+        url = u"http://epguides.com/doctor_who"
+        show = self.db.add_show(Show(u"none", url=url))
+        self.parser.parse(show, self.db, self.args)
+
+        self.assertEqual("Doctor Who (2005)", show.name)
+        self.assertEqual(Show.RUNNING, show.status)
+
+        episodes = self.db.get_episodes(date(2005,3,26), 99999)
+        self.assertEqual(161, len(episodes))
+
+        episode = episodes[0]
+        self.assertEqual(1, episode.season)
+        self.assertEqual(1, episode.episode)
+        self.assertEqual("Rose", episode.title)
+        self.assertEqual(date(2005, 3, 26), episode.airdate)
+
+        episode = episodes[12]
+        self.assertEqual(1, episode.season)
+        self.assertEqual(13, episode.episode)
+        self.assertEqual("The Parting of the Ways", episode.title)
+        self.assertEqual(date(2005, 6, 18), episode.airdate)
+
+        episode = episodes[13]
+        self.assertEqual(1, episode.season)
+        self.assertEqual(0, episode.episode)
+        self.assertEqual("Born Again", episode.title)
+        self.assertEqual(date(2005, 11, 18), episode.airdate)
+
+        episode = episodes[14]
+        self.assertEqual(2, episode.season)
+        self.assertEqual(0, episode.episode)
+        # both are acceptable
+        self.assertIn(episode.title, ["The Christmas Invasion",
+                "Attack of the Graske"])
+        self.assertEqual(date(2005, 12, 25), episode.airdate)
+
+        episode = episodes[15]
+        self.assertEqual(2, episode.season)
+        self.assertEqual(1, episode.episode)
+        self.assertEqual("New Earth", episode.title)
+        self.assertEqual(date(2006, 4, 15), episode.airdate)
```

### Comparing `episoder-0.9.1/test/test_episode.py` & `episoder-0.9.2/test/test_episode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # episoder, https://code.ott.net/episoder
 # -*- coding: utf8 -*-
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `episoder-0.9.1/test/test_metainfo.py` & `episoder-0.9.2/test/test_metainfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # episoder, https://code.ott.net/episoder
 # -*- coding: utf8 -*-
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `episoder-0.9.1/test/test_migration.py` & `episoder-0.9.2/test/test_migration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # episoder, https://code.ott.net/episoder
 # -*- coding: utf8 -*-
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `episoder-0.9.1/test/test_notify.py` & `episoder-0.9.2/test/test_notify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # episoder, https://code.ott.net/episoder
 # -*- coding: utf8 -*-
-# # Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# # Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `episoder-0.9.1/test/test_output.py` & `episoder-0.9.2/test/test_output.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # episoder, https://code.ott.net/episoder
 # -*- coding: utf8 -*-
-# # Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# # Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -50,144 +50,193 @@
         self.assertEqual(str(renderer), "ConsoleRenderer")
         self.assertEqual(repr(renderer),
             'ConsoleRenderer("%show", "%Y%m%d", <..>)')
 
     def test_render_airdate(self):
 
         renderer = ConsoleRenderer("%airdate", "%Y%m%d", self.io)
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"20080101\n")
 
         self.episode.airdate = date(2015, 2, 3)
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"20080101\n20150203\n")
 
     def test_render_show_name(self):
 
         renderer = ConsoleRenderer("%show", "", self.io)
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"Test show 36\n")
 
         self.show.name = "Test 55"
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"Test show 36\nTest 55\n")
 
     def test_render_season_number(self):
 
         renderer = ConsoleRenderer("%season", "", self.io)
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"2\n")
 
         self.episode.season = 12
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"2\n12\n")
 
     def test_render_episode_number(self):
 
         renderer = ConsoleRenderer("%epnum", "", self.io)
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"05\n")
 
         self.episode.episode = 22
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"05\n22\n")
 
     def test_render_episode_title(self):
 
         renderer = ConsoleRenderer("%eptitle", "", self.io)
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"Episode 41\n")
 
         self.episode.title = "Episode 8"
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"Episode 41\nEpisode 8\n")
 
     def test_render_episode_without_title(self):
 
         renderer = ConsoleRenderer("%eptitle", "", self.io)
         self.episode.title = None
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"None\n")
 
     def test_render_total_episode_number(self):
 
         renderer = ConsoleRenderer("%totalep", "", self.io)
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"3\n")
 
         self.episode.totalnum = 90
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"3\n90\n")
 
     def test_render_prodnum(self):
 
         renderer = ConsoleRenderer("%prodnum", "", self.io)
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"NX01\n")
 
         self.episode.prodnum = "ABCD"
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
         self.assertEqual(self.io.getvalue(), u"NX01\nABCD\n")
 
+    def test_render_episode_without_prodnum(self):
+
+        renderer = ConsoleRenderer("%prodnum", "", self.io)
+        renderer.render([self.episode], date.today(), False)
+        self.assertEqual(self.io.getvalue(), u"NX01\n")
+
+        self.episode.prodnum = None
+        renderer.render([self.episode], date.today(), False)
+        self.assertEqual(self.io.getvalue(), u"NX01\nNone\n")
+
     def test_render_combined(self):
 
         self.show.name = "Frasier"
         self.episode.airdate = date(1998, 9, 24)
         self.episode.season = 6
         self.episode.episode = 1
         self.episode.title = "Good Grief"
 
         fmt="%airdate: %show %seasonx%epnum - %eptitle"
         renderer = ConsoleRenderer(fmt, "%Y-%m-%d", self.io)
-        renderer.render([self.episode], False)
+        renderer.render([self.episode], date.today(), False)
 
         out=self.io.getvalue()
         self.assertEqual(out, "1998-09-24: Frasier 6x01 - Good Grief\n")
 
     def test_render_colors(self):
 
         today = date.today()
 
         # Two days ago -> grey
         io = StringIO()
         renderer = ConsoleRenderer("%airdate", "%Y", io)
         then = today - timedelta(2)
         self.episode.airdate = then
         expect = "\033[30;0m%s\033[30;0m\n" % then.strftime("%Y")
-        renderer.render([self.episode], True)
+        renderer.render([self.episode], today, True)
         self.assertEqual(expect, io.getvalue())
 
         # Yesterday -> red
         io = StringIO()
         renderer = ConsoleRenderer("%airdate", "%Y", io)
         then = today - timedelta(1)
         self.episode.airdate = then
         expect = "\033[31;1m%s\033[30;0m\n" % then.strftime("%Y")
-        renderer.render([self.episode], True)
+        renderer.render([self.episode], today, True)
         self.assertEqual(expect, io.getvalue())
 
         # Today -> yellow
         io = StringIO()
         renderer = ConsoleRenderer("%airdate", "%Y", io)
         then = today
         self.episode.airdate = then
         expect = "\033[33;1m%s\033[30;0m\n" % then.strftime("%Y")
-        renderer.render([self.episode], True)
+        renderer.render([self.episode], today, True)
         self.assertEqual(expect, io.getvalue())
 
         # Tomorrow -> green
         io = StringIO()
         renderer = ConsoleRenderer("%airdate", "%Y", io)
         then = today + timedelta(1)
         self.episode.airdate = then
         expect = "\033[32;1m%s\033[30;0m\n" % then.strftime("%Y")
-        renderer.render([self.episode], True)
+        renderer.render([self.episode], today, True)
         self.assertEqual(expect, io.getvalue())
 
         # The future -> cyan
         io = StringIO()
         renderer = ConsoleRenderer("%airdate", "%Y", io)
         then = today + timedelta(2)
         self.episode.airdate = then
         expect = "\033[36;1m%s\033[30;0m\n" % then.strftime("%Y")
-        renderer.render([self.episode], True)
+        renderer.render([self.episode], today, True)
         self.assertEqual(expect, io.getvalue())
+
+    def test_render_colors_different_date(self):
+
+        today = date(2001, 7, 10)
+
+        # Two days ago -> grey
+        io = StringIO()
+        renderer = ConsoleRenderer("%airdate", "%Y", io)
+        self.episode.airdate = date(2001, 7, 8)
+        renderer.render([self.episode], today, True)
+        self.assertEqual("\033[30;0m2001\033[30;0m\n", io.getvalue())
+
+        # Yesterday -> red
+        io = StringIO()
+        renderer = ConsoleRenderer("%airdate", "%Y", io)
+        self.episode.airdate = date(2001, 7, 9)
+        renderer.render([self.episode], today, True)
+        self.assertEqual("\033[31;1m2001\033[30;0m\n", io.getvalue())
+
+        # Today -> yellow
+        io = StringIO()
+        renderer = ConsoleRenderer("%airdate", "%Y", io)
+        self.episode.airdate = date(2001, 7, 10)
+        renderer.render([self.episode], today, True)
+        self.assertEqual("\033[33;1m2001\033[30;0m\n", io.getvalue())
+
+        # Tomorrow -> green
+        io = StringIO()
+        renderer = ConsoleRenderer("%airdate", "%Y", io)
+        self.episode.airdate = date(2001, 7, 11)
+        renderer.render([self.episode], today, True)
+        self.assertEqual("\033[32;1m2001\033[30;0m\n", io.getvalue())
+
+        # The future -> cyan
+        io = StringIO()
+        renderer = ConsoleRenderer("%airdate", "%Y", io)
+        self.episode.airdate = date(2001, 7, 12)
+        renderer.render([self.episode], today, True)
+        self.assertEqual("\033[36;1m2001\033[30;0m\n", io.getvalue())
```

### Comparing `episoder-0.9.1/test/test_show.py` & `episoder-0.9.2/test/test_show.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # episoder, https://code.ott.net/episoder
 # -*- coding: utf8 -*-
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `episoder-0.9.1/test/test_sources.py` & `episoder-0.9.2/test/test_sources.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # episoder, https://code.ott.net/episoder
 # -*- coding: utf8 -*-
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `episoder-0.9.1/test/test_tvcom.py` & `episoder-0.9.2/test/test_tvcom.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # episoder, https://code.ott.net/episoder
 # -*- coding: utf8 -*-
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `episoder-0.9.1/test/test_tvdb.py` & `episoder-0.9.2/test/test_tvdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # episoder, https://code.ott.net/episoder
 # -*- coding: utf8 -*-
 #
-# Copyright (C) 2004-2020 Stefan Ott. All rights reserved.
+# Copyright (C) 2004-2021 Stefan Ott. All rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

