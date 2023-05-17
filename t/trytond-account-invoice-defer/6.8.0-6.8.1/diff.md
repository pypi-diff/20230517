# Comparing `tmp/trytond_account_invoice_defer-6.8.0.tar.gz` & `tmp/trytond_account_invoice_defer-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_defer-6.8.0.tar", last modified: Mon May  1 12:02:48 2023, max compression
+gzip compressed data, was "trytond_account_invoice_defer-6.8.1.tar", last modified: Wed May 17 20:57:47 2023, max compression
```

## Comparing `trytond_account_invoice_defer-6.8.0.tar` & `trytond_account_invoice_defer-6.8.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:48.081531 trytond_account_invoice_defer-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      597 2023-05-01 11:15:38.000000 trytond_account_invoice_defer-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-05-01 11:15:37.000000 trytond_account_invoice_defer-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2493 2023-05-01 12:02:48.081531 trytond_account_invoice_defer-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18427 2023-04-29 11:01:18.000000 trytond_account_invoice_defer-6.8.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8380 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:48.078197 trytond_account_invoice_defer-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1844 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:48.071530 trytond_account_invoice_defer-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5844 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6073 2023-04-30 10:46:36.000000 trytond_account_invoice_defer-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5849 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5961 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4801 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5896 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1240 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:02:48.081531 trytond_account_invoice_defer-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4610 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:48.074864 trytond_account_invoice_defer-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3858 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/tests/scenario_account_invoice_defer.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1769 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      120 2023-05-01 11:15:31.000000 trytond_account_invoice_defer-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:48.081531 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2493 2023-05-01 12:02:47.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1811 2023-05-01 12:02:48.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:02:47.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-05-01 12:02:47.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      130 2023-05-01 12:02:47.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:02:47.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:48.074864 trytond_account_invoice_defer-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      964 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/view/invoice_deferred_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/view/invoice_deferred_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/view/invoice_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:57:47.954470 trytond_account_invoice_defer-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      698 2023-05-17 20:57:44.000000 trytond_account_invoice_defer-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-05-17 20:57:44.000000 trytond_account_invoice_defer-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2493 2023-05-17 20:57:47.954470 trytond_account_invoice_defer-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18527 2023-05-13 22:06:18.000000 trytond_account_invoice_defer-6.8.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8380 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:57:47.947803 trytond_account_invoice_defer-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1844 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:57:47.941136 trytond_account_invoice_defer-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5844 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6073 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5849 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5961 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4801 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5896 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1240 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-17 20:57:47.954470 trytond_account_invoice_defer-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4610 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:57:47.944470 trytond_account_invoice_defer-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3858 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/tests/scenario_account_invoice_defer.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1769 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      120 2023-05-01 12:18:02.000000 trytond_account_invoice_defer-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:57:47.951137 trytond_account_invoice_defer-6.8.1/trytond_account_invoice_defer.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2493 2023-05-17 20:57:47.000000 trytond_account_invoice_defer-6.8.1/trytond_account_invoice_defer.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1811 2023-05-17 20:57:47.000000 trytond_account_invoice_defer-6.8.1/trytond_account_invoice_defer.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:57:47.000000 trytond_account_invoice_defer-6.8.1/trytond_account_invoice_defer.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-05-17 20:57:47.000000 trytond_account_invoice_defer-6.8.1/trytond_account_invoice_defer.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:57:47.000000 trytond_account_invoice_defer-6.8.1/trytond_account_invoice_defer.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      130 2023-05-17 20:57:47.000000 trytond_account_invoice_defer-6.8.1/trytond_account_invoice_defer.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-17 20:57:47.000000 trytond_account_invoice_defer-6.8.1/trytond_account_invoice_defer.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:57:47.947803 trytond_account_invoice_defer-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      964 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/view/invoice_deferred_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/view/invoice_deferred_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-05-01 12:17:30.000000 trytond_account_invoice_defer-6.8.1/view/invoice_line_form.xml
```

### Comparing `trytond_account_invoice_defer-6.8.0/CHANGELOG` & `trytond_account_invoice_defer-6.8.1/CHANGELOG`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 6.8.1 - 2023-05-17
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 3.7
 * Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
```

### Comparing `trytond_account_invoice_defer-6.8.0/COPYRIGHT` & `trytond_account_invoice_defer-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/LICENSE` & `trytond_account_invoice_defer-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/PKG-INFO` & `trytond_account_invoice_defer-6.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_defer
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module to defer expense and revenue
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_invoice_defer-6.8.0/__init__.py` & `trytond_account_invoice_defer-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/account.py` & `trytond_account_invoice_defer-6.8.1/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,24 +160,28 @@
     @classmethod
     def _journal_types(cls, type):
         if type == 'out':
             return ['revenue']
         else:
             return ['expense']
 
+    @fields.depends(methods=['set_journal'])
+    def on_change_type(self):
+        self.set_journal()
+
     @fields.depends('type')
-    def on_change_with_journal(self, pattern=None):
+    def set_journal(self, pattern=None):
         pool = Pool()
         Journal = pool.get('account.journal')
         pattern = pattern.copy() if pattern is not None else {}
         pattern.setdefault('type', {
                 'out': 'revenue',
                 'in': 'expense',
                 }.get(self.type))
-        return Journal.find(pattern)
+        self.journal = Journal.find(pattern)
 
     @fields.depends('invoice_line', 'start_date', 'company')
     def on_change_invoice_line(self):
         pool = Pool()
         Currency = pool.get('currency.currency')
         if self.invoice_line:
             if not self.start_date:
```

### Comparing `trytond_account_invoice_defer-6.8.0/account.xml` & `trytond_account_invoice_defer-6.8.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/doc/conf.py` & `trytond_account_invoice_defer-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/doc/design.rst` & `trytond_account_invoice_defer-6.8.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/bg.po` & `trytond_account_invoice_defer-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/ca.po` & `trytond_account_invoice_defer-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/cs.po` & `trytond_account_invoice_defer-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/de.po` & `trytond_account_invoice_defer-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/es.po` & `trytond_account_invoice_defer-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/es_419.po` & `trytond_account_invoice_defer-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/et.po` & `trytond_account_invoice_defer-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/fa.po` & `trytond_account_invoice_defer-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/fi.po` & `trytond_account_invoice_defer-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/fr.po` & `trytond_account_invoice_defer-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/hu.po` & `trytond_account_invoice_defer-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/id.po` & `trytond_account_invoice_defer-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/it.po` & `trytond_account_invoice_defer-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/lo.po` & `trytond_account_invoice_defer-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/lt.po` & `trytond_account_invoice_defer-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/nl.po` & `trytond_account_invoice_defer-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/pl.po` & `trytond_account_invoice_defer-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/pt.po` & `trytond_account_invoice_defer-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/ro.po` & `trytond_account_invoice_defer-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/ru.po` & `trytond_account_invoice_defer-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/sl.po` & `trytond_account_invoice_defer-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/tr.po` & `trytond_account_invoice_defer-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/uk.po` & `trytond_account_invoice_defer-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/locale/zh_CN.po` & `trytond_account_invoice_defer-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/message.xml` & `trytond_account_invoice_defer-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/setup.py` & `trytond_account_invoice_defer-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/tests/scenario_account_invoice_defer.rst` & `trytond_account_invoice_defer-6.8.1/tests/scenario_account_invoice_defer.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/tests/tools.py` & `trytond_account_invoice_defer-6.8.1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/tox.ini` & `trytond_account_invoice_defer-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/PKG-INFO` & `trytond_account_invoice_defer-6.8.1/trytond_account_invoice_defer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-account-invoice-defer
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module to defer expense and revenue
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/SOURCES.txt` & `trytond_account_invoice_defer-6.8.1/trytond_account_invoice_defer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.8.0/view/invoice_deferred_form.xml` & `trytond_account_invoice_defer-6.8.1/view/invoice_deferred_form.xml`

 * *Files identical despite different names*

