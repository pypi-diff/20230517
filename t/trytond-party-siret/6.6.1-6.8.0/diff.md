# Comparing `tmp/trytond_party_siret-6.6.1.tar.gz` & `tmp/trytond_party_siret-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_party_siret-6.6.1.tar", last modified: Wed May 17 20:53:45 2023, max compression
+gzip compressed data, was "trytond_party_siret-6.8.0.tar", last modified: Mon May  1 11:49:15 2023, max compression
```

## Comparing `trytond_party_siret-6.6.1.tar` & `trytond_party_siret-6.8.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:53:45.251544 trytond_party_siret-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2289 2023-05-17 20:53:42.000000 trytond_party_siret-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-17 20:53:42.000000 trytond_party_siret-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_party_siret-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2361 2023-05-17 20:53:45.251544 trytond_party_siret-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      109 2022-12-19 12:02:49.000000 trytond_party_siret-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3328 2023-05-04 17:40:39.000000 trytond_party_siret-6.6.1/address.py
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/address.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:53:45.248211 trytond_party_siret-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2023-04-08 09:35:50.000000 trytond_party_siret-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      109 2022-12-19 12:02:49.000000 trytond_party_siret-6.6.1/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:53:45.248211 trytond_party_siret-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1257 2023-05-04 17:40:39.000000 trytond_party_siret-6.6.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-17 20:53:45.251544 trytond_party_siret-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4238 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:53:45.248211 trytond_party_siret-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:53:45.251544 trytond_party_siret-6.6.1/trytond_party_siret.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2361 2023-05-17 20:53:44.000000 trytond_party_siret-6.6.1/trytond_party_siret.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1393 2023-05-17 20:53:45.000000 trytond_party_siret-6.6.1/trytond_party_siret.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:53:44.000000 trytond_party_siret-6.6.1/trytond_party_siret.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-05-17 20:53:44.000000 trytond_party_siret-6.6.1/trytond_party_siret.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:53:44.000000 trytond_party_siret-6.6.1/trytond_party_siret.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       42 2023-05-17 20:53:44.000000 trytond_party_siret-6.6.1/trytond_party_siret.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-17 20:53:44.000000 trytond_party_siret-6.6.1/trytond_party_siret.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:53:45.248211 trytond_party_siret-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/view/address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-04-13 16:52:41.000000 trytond_party_siret-6.6.1/view/party_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:15.134775 trytond_party_siret-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2415 2023-05-01 11:06:10.000000 trytond_party_siret-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:06:10.000000 trytond_party_siret-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_party_siret-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_party_siret-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2357 2023-05-01 11:49:15.131442 trytond_party_siret-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      109 2023-04-15 07:12:15.000000 trytond_party_siret-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_party_siret-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3385 2023-04-30 10:46:36.000000 trytond_party_siret-6.8.0/address.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-04-15 07:12:15.000000 trytond_party_siret-6.8.0/address.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:15.131442 trytond_party_siret-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_party_siret-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      109 2023-04-15 07:12:15.000000 trytond_party_siret-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:15.128109 trytond_party_siret-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-29 08:02:45.000000 trytond_party_siret-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1314 2023-04-30 10:46:36.000000 trytond_party_siret-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_party_siret-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:49:15.134775 trytond_party_siret-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4206 2023-04-15 07:12:15.000000 trytond_party_siret-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:15.128109 trytond_party_siret-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_party_siret-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_party_siret-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_party_siret-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-05-01 11:06:04.000000 trytond_party_siret-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:15.131442 trytond_party_siret-6.8.0/trytond_party_siret.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2357 2023-05-01 11:49:14.000000 trytond_party_siret-6.8.0/trytond_party_siret.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1393 2023-05-01 11:49:15.000000 trytond_party_siret-6.8.0/trytond_party_siret.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:49:14.000000 trytond_party_siret-6.8.0/trytond_party_siret.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-05-01 11:49:14.000000 trytond_party_siret-6.8.0/trytond_party_siret.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_party_siret-6.8.0/trytond_party_siret.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       42 2023-05-01 11:49:14.000000 trytond_party_siret-6.8.0/trytond_party_siret.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:49:14.000000 trytond_party_siret-6.8.0/trytond_party_siret.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:15.131442 trytond_party_siret-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_party_siret-6.8.0/view/address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-04-15 07:12:15.000000 trytond_party_siret-6.8.0/view/party_tree.xml
```

### Comparing `trytond_party_siret-6.6.1/CHANGELOG` & `trytond_party_siret-6.8.0/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 
-Version 6.6.1 - 2023-05-17
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Manage dereferenced name in SIREN and SIRET identifier clause
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_party_siret-6.6.1/COPYRIGHT` & `trytond_party_siret-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_party_siret-6.6.1/LICENSE` & `trytond_party_siret-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_party_siret-6.6.1/PKG-INFO` & `trytond_party_siret-6.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_party_siret
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to add SIRET/SIREN on parties
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/party_siret
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton party siret siren
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,20 +39,20 @@
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 
 Party SIRET Module
 ##################
 
 The party siret module adds the SIREN and SIRET on party and address.
```

### Comparing `trytond_party_siret-6.6.1/address.py` & `trytond_party_siret-6.8.0/address.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,17 +64,18 @@
         for identifier in self.identifiers:
             if identifier.type == 'fr_siret':
                 return identifier.id
 
     @classmethod
     def search_siret(cls, name, clause):
         _, operator, value = clause
+        nested = clause[0][len(name) + 1:]
         domain = [
             ('identifiers', 'where', [
-                    ('code', operator, value),
+                    (nested or 'rec_name', operator, value),
                     ('type', '=', 'fr_siren'),
                     ]),
             ]
         # Add party without tax identifier
         if ((operator == '=' and value is None)
                 or (operator == 'in' and None in value)):
             domain = ['OR',
```

### Comparing `trytond_party_siret-6.6.1/doc/conf.py` & `trytond_party_siret-6.8.0/doc/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,18 @@
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     info['name'] = result.stdout.decode('utf-8').strip()
 
     result = subprocess.run(
         [sys.executable, 'setup.py', '--version'],
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     version = result.stdout.decode('utf-8').strip()
-    if 'dev' in version:
+    major_version, minor_version, _ = version.split('.', 2)
+    major_version = int(major_version)
+    minor_version = int(minor_version)
+    if minor_version % 2:
         info['series'] = 'latest'
     else:
         info['series'] = '.'.join(version.split('.', 2)[:2])
 
     for key in {'depends', 'extras_depend'}:
         info[key] = info.get(key, '').strip().splitlines()
     info['modules'] = set(info['depends'] + info['extras_depend'])
```

### Comparing `trytond_party_siret-6.6.1/party.py` & `trytond_party_siret-6.8.0/party.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,17 +15,18 @@
         for identifier in self.identifiers:
             if identifier.type == 'fr_siren':
                 return identifier.id
 
     @classmethod
     def search_siren(cls, name, clause):
         _, operator, value = clause
+        nested = clause[0][len(name) + 1:]
         domain = [
             ('identifiers', 'where', [
-                    ('code', operator, value),
+                    (nested or 'rec_name', operator, value),
                     ('type', '=', 'fr_siren'),
                     ]),
             ]
         # Add party without tax identifier
         if ((operator == '=' and value is None)
                 or (operator == 'in' and None in value)):
             domain = ['OR',
```

### Comparing `trytond_party_siret-6.6.1/setup.py` & `trytond_party_siret-6.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 def read(fname):
     return io.open(
         os.path.join(os.path.dirname(__file__), fname),
         'r', encoding='utf-8').read()
 
 
 def get_require_version(name):
-    if minor_version % 2:
-        require = '%s >= %s.%s.dev0, < %s.%s'
-    else:
-        require = '%s >= %s.%s, < %s.%s'
+    require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
 
 
 config = ConfigParser()
 config.read_file(open(os.path.join(os.path.dirname(__file__), 'tryton.cfg')))
@@ -34,36 +31,39 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_party_siret'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 setup(name=name,
     version=version,
     description='Tryton module to add SIRET/SIREN on parties',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/party_siret',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton party siret siren',
     package_dir={'trytond.modules.party_siret': '.'},
     packages=(
         ['trytond.modules.party_siret']
         + ['trytond.modules.party_siret.%s' % p for p in find_packages()]
         ),
@@ -100,23 +100,23 @@
         'Natural Language :: Russian',
         'Natural Language :: Slovenian',
         'Natural Language :: Spanish',
         'Natural Language :: Turkish',
         'Natural Language :: Ukrainian',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Office/Business',
         ],
     license='GPL-3',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=requires,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     party_siret = trytond.modules.party_siret
     """,
     )
```

### Comparing `trytond_party_siret-6.6.1/tox.ini` & `trytond_party_siret-6.8.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 commands =
-    coverage run --include=./**/party_siret/* -m unittest discover -s tests
-    coverage report --include=./**/party_siret/* --omit=*/tests/*
+    coverage run --omit=*/tests/* -m xmlrunner discover -s tests {posargs}
+commands_post =
+    coverage report
+    coverage xml
 deps =
     coverage
+    unittest-xml-reporting
     postgresql: psycopg2 >= 2.7.0
 passenv = *
 setenv =
     sqlite: TRYTOND_DATABASE_URI={env:SQLITE_URI:sqlite://}
     postgresql: TRYTOND_DATABASE_URI={env:POSTGRESQL_URI:postgresql://}
     sqlite: DB_NAME={env:DB_NAME::memory:}
     postgresql: DB_NAME={env:DB_NAME:test}
```

### Comparing `trytond_party_siret-6.6.1/trytond_party_siret.egg-info/PKG-INFO` & `trytond_party_siret-6.8.0/trytond_party_siret.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-party-siret
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to add SIRET/SIREN on parties
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/party_siret
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton party siret siren
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,20 +39,20 @@
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 
 Party SIRET Module
 ##################
 
 The party siret module adds the SIREN and SIRET on party and address.
```

### Comparing `trytond_party_siret-6.6.1/trytond_party_siret.egg-info/SOURCES.txt` & `trytond_party_siret-6.8.0/trytond_party_siret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

