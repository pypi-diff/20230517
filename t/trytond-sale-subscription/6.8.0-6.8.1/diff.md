# Comparing `tmp/trytond_sale_subscription-6.8.0.tar.gz` & `tmp/trytond_sale_subscription-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_subscription-6.8.0.tar", last modified: Mon May  1 11:53:47 2023, max compression
+gzip compressed data, was "trytond_sale_subscription-6.8.1.tar", last modified: Wed May 17 20:45:00 2023, max compression
```

## Comparing `trytond_sale_subscription-6.8.0.tar` & `trytond_sale_subscription-6.8.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:47.891494 trytond_sale_subscription-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1808 2023-05-01 11:09:19.000000 trytond_sale_subscription-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      686 2023-05-01 11:09:19.000000 trytond_sale_subscription-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_subscription-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     5810 2023-05-01 11:53:47.891494 trytond_sale_subscription-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3531 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1238 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1841 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:47.884827 trytond_sale_subscription-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3531 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:47.888160 trytond_sale_subscription-6.8.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/icons/tryton-sale-subscription.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      737 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:47.874827 trytond_sale_subscription-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18243 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18369 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18386 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14786 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16241 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19172 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18505 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15286 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16546 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16524 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18167 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16783 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17696 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14978 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17576 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14786 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-04-29 08:02:47.000000 trytond_sale_subscription-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1771 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1205 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9310 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/recurrence.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4545 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/recurrence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1014 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/service.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2462 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/service.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:53:47.891494 trytond_sale_subscription-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4438 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    38535 2023-04-29 11:01:18.000000 trytond_sale_subscription-6.8.0/subscription.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14973 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/subscription.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:47.878160 trytond_sale_subscription-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5558 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/tests/scenario_sale_subscription.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5381 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/tests/scenario_sale_subscription_advanced_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4727 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/tests/scenario_sale_subscription_new_line.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      254 2023-05-01 11:09:13.000000 trytond_sale_subscription-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:47.888160 trytond_sale_subscription-6.8.0/trytond_sale_subscription.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     5810 2023-05-01 11:53:46.000000 trytond_sale_subscription-6.8.0/trytond_sale_subscription.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3457 2023-05-01 11:53:47.000000 trytond_sale_subscription-6.8.0/trytond_sale_subscription.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:53:46.000000 trytond_sale_subscription-6.8.0/trytond_sale_subscription.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-05-01 11:53:46.000000 trytond_sale_subscription-6.8.0/trytond_sale_subscription.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_sale_subscription-6.8.0/trytond_sale_subscription.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-05-01 11:53:46.000000 trytond_sale_subscription-6.8.0/trytond_sale_subscription.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:53:46.000000 trytond_sale_subscription-6.8.0/trytond_sale_subscription.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:47.884827 trytond_sale_subscription-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-01-16 14:00:21.000000 trytond_sale_subscription-6.8.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/create_invoice_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/line_consumption_create_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      961 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/recurrence_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/recurrence_rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-01-16 14:00:21.000000 trytond_sale_subscription-6.8.0/view/recurrence_rule_set_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:21.000000 trytond_sale_subscription-6.8.0/view/recurrence_rule_set_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/recurrence_rule_set_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/recurrence_rule_set_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/service_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/service_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2120 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/subscription_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/subscription_line_consumption_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/subscription_line_consumption_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1246 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/subscription_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      527 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/subscription_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/subscription_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-04-15 07:12:15.000000 trytond_sale_subscription-6.8.0/view/subscription_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:45:00.781889 trytond_sale_subscription-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1909 2023-05-17 20:44:57.000000 trytond_sale_subscription-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      686 2023-05-17 20:44:57.000000 trytond_sale_subscription-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     5810 2023-05-17 20:45:00.778555 trytond_sale_subscription-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3531 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1238 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1841 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:45:00.765222 trytond_sale_subscription-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3531 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:45:00.765222 trytond_sale_subscription-6.8.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/icons/tryton-sale-subscription.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      737 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:45:00.665221 trytond_sale_subscription-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18243 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18369 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18386 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14786 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16241 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19172 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18505 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15286 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16546 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16524 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18167 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16783 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17696 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14978 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17576 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14786 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1771 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1205 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9310 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/recurrence.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4545 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/recurrence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1014 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/service.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2462 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/service.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-17 20:45:00.781889 trytond_sale_subscription-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4438 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    38506 2023-05-13 22:06:18.000000 trytond_sale_subscription-6.8.1/subscription.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14973 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/subscription.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:45:00.681887 trytond_sale_subscription-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5558 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/tests/scenario_sale_subscription.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5381 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/tests/scenario_sale_subscription_advanced_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4727 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/tests/scenario_sale_subscription_new_line.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      254 2023-05-01 12:18:02.000000 trytond_sale_subscription-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:45:00.778555 trytond_sale_subscription-6.8.1/trytond_sale_subscription.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5810 2023-05-17 20:44:59.000000 trytond_sale_subscription-6.8.1/trytond_sale_subscription.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3457 2023-05-17 20:45:00.000000 trytond_sale_subscription-6.8.1/trytond_sale_subscription.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:44:59.000000 trytond_sale_subscription-6.8.1/trytond_sale_subscription.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-05-17 20:44:59.000000 trytond_sale_subscription-6.8.1/trytond_sale_subscription.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:44:59.000000 trytond_sale_subscription-6.8.1/trytond_sale_subscription.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-05-17 20:44:59.000000 trytond_sale_subscription-6.8.1/trytond_sale_subscription.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-17 20:44:59.000000 trytond_sale_subscription-6.8.1/trytond_sale_subscription.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:45:00.758555 trytond_sale_subscription-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/create_invoice_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/line_consumption_create_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      961 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/recurrence_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/recurrence_rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/recurrence_rule_set_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/recurrence_rule_set_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/recurrence_rule_set_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/recurrence_rule_set_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/service_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/service_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2120 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/subscription_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/subscription_line_consumption_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/subscription_line_consumption_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1246 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/subscription_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      527 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/subscription_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/subscription_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-05-01 12:17:31.000000 trytond_sale_subscription-6.8.1/view/subscription_list.xml
```

### Comparing `trytond_sale_subscription-6.8.0/CHANGELOG` & `trytond_sale_subscription-6.8.1/CHANGELOG`

 * *Files 8% similar despite different names*

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

### Comparing `trytond_sale_subscription-6.8.0/COPYRIGHT` & `trytond_sale_subscription-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/LICENSE` & `trytond_sale_subscription-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/PKG-INFO` & `trytond_sale_subscription-6.8.1/trytond_sale_subscription.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: trytond_sale_subscription
-Version: 6.8.0
+Name: trytond-sale-subscription
+Version: 6.8.1
 Summary: Tryton module for subscription
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_subscription-6.8.0/README.rst` & `trytond_sale_subscription-6.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/__init__.py` & `trytond_sale_subscription-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/configuration.py` & `trytond_sale_subscription-6.8.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/configuration.xml` & `trytond_sale_subscription-6.8.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/doc/conf.py` & `trytond_sale_subscription-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/doc/index.rst` & `trytond_sale_subscription-6.8.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/icons/LICENSE` & `trytond_sale_subscription-6.8.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/invoice.py` & `trytond_sale_subscription-6.8.1/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/ir.py` & `trytond_sale_subscription-6.8.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/bg.po` & `trytond_sale_subscription-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/ca.po` & `trytond_sale_subscription-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/cs.po` & `trytond_sale_subscription-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/de.po` & `trytond_sale_subscription-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/es.po` & `trytond_sale_subscription-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/es_419.po` & `trytond_sale_subscription-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/et.po` & `trytond_sale_subscription-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/fa.po` & `trytond_sale_subscription-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/fi.po` & `trytond_sale_subscription-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/fr.po` & `trytond_sale_subscription-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/hu.po` & `trytond_sale_subscription-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/id.po` & `trytond_sale_subscription-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/it.po` & `trytond_sale_subscription-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/lo.po` & `trytond_sale_subscription-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/lt.po` & `trytond_sale_subscription-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/nl.po` & `trytond_sale_subscription-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/pl.po` & `trytond_sale_subscription-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/pt.po` & `trytond_sale_subscription-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/ro.po` & `trytond_sale_subscription-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/ru.po` & `trytond_sale_subscription-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/sl.po` & `trytond_sale_subscription-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/tr.po` & `trytond_sale_subscription-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/uk.po` & `trytond_sale_subscription-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/locale/zh_CN.po` & `trytond_sale_subscription-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/message.xml` & `trytond_sale_subscription-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/party.py` & `trytond_sale_subscription-6.8.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/product.py` & `trytond_sale_subscription-6.8.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/recurrence.py` & `trytond_sale_subscription-6.8.1/recurrence.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/recurrence.xml` & `trytond_sale_subscription-6.8.1/recurrence.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/service.py` & `trytond_sale_subscription-6.8.1/service.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/service.xml` & `trytond_sale_subscription-6.8.1/service.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/setup.py` & `trytond_sale_subscription-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/subscription.py` & `trytond_sale_subscription-6.8.1/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,15 @@
             type='out',
             party=party,
             invoice_address=self.invoice_address,
             currency=self.currency,
             account=party.account_receivable_used,
             )
         invoice.invoice_date = self.next_invoice_date
-        invoice.journal = invoice.on_change_with_journal()
+        invoice.set_journal()
         invoice.payment_term = self.payment_term
         return invoice
 
 
 class Line(sequence_ordered(), ModelSQL, ModelView):
     "Subscription Line"
     __name__ = 'sale.subscription.line'
```

### Comparing `trytond_sale_subscription-6.8.0/subscription.xml` & `trytond_sale_subscription-6.8.1/subscription.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/tests/scenario_sale_subscription.rst` & `trytond_sale_subscription-6.8.1/tests/scenario_sale_subscription.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/tests/scenario_sale_subscription_advanced_invoice.rst` & `trytond_sale_subscription-6.8.1/tests/scenario_sale_subscription_advanced_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/tests/scenario_sale_subscription_new_line.rst` & `trytond_sale_subscription-6.8.1/tests/scenario_sale_subscription_new_line.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/tox.ini` & `trytond_sale_subscription-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/trytond_sale_subscription.egg-info/PKG-INFO` & `trytond_sale_subscription-6.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: trytond-sale-subscription
-Version: 6.8.0
+Name: trytond_sale_subscription
+Version: 6.8.1
 Summary: Tryton module for subscription
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_subscription-6.8.0/trytond_sale_subscription.egg-info/SOURCES.txt` & `trytond_sale_subscription-6.8.1/trytond_sale_subscription.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/view/recurrence_rule_form.xml` & `trytond_sale_subscription-6.8.1/view/recurrence_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/view/recurrence_rule_list.xml` & `trytond_sale_subscription-6.8.1/view/recurrence_rule_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/view/subscription_form.xml` & `trytond_sale_subscription-6.8.1/view/subscription_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/view/subscription_line_form.xml` & `trytond_sale_subscription-6.8.1/view/subscription_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/view/subscription_line_list.xml` & `trytond_sale_subscription-6.8.1/view/subscription_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/view/subscription_line_list_sequence.xml` & `trytond_sale_subscription-6.8.1/view/subscription_line_list_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-6.8.0/view/subscription_list.xml` & `trytond_sale_subscription-6.8.1/view/subscription_list.xml`

 * *Files identical despite different names*

