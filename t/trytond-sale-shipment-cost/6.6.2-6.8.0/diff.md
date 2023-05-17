# Comparing `tmp/trytond_sale_shipment_cost-6.6.2.tar.gz` & `tmp/trytond_sale_shipment_cost-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_shipment_cost-6.6.2.tar", last modified: Wed May 17 20:45:36 2023, max compression
+gzip compressed data, was "trytond_sale_shipment_cost-6.8.0.tar", last modified: Mon May  1 11:57:21 2023, max compression
```

## Comparing `trytond_sale_shipment_cost-6.6.2.tar` & `trytond_sale_shipment_cost-6.8.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:45:36.355651 trytond_sale_shipment_cost-6.6.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     3169 2023-05-17 20:45:33.000000 trytond_sale_shipment_cost-6.6.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-05-17 20:45:33.000000 trytond_sale_shipment_cost-6.6.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:57.000000 trytond_sale_shipment_cost-6.6.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2948 2023-05-17 20:45:36.355651 trytond_sale_shipment_cost-6.6.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      837 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:45:36.352317 trytond_sale_shipment_cost-6.6.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2023-04-08 09:35:50.000000 trytond_sale_shipment_cost-6.6.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      240 2022-12-19 12:02:57.000000 trytond_sale_shipment_cost-6.6.2/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:45:36.345651 trytond_sale_shipment_cost-6.6.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3441 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3327 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3358 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3341 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2943 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3053 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3441 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3444 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2909 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3006 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2592 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3289 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2687 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2997 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2592 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2872 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      672 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2030 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1193 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16296 2023-05-04 17:25:41.000000 trytond_sale_shipment_cost-6.6.2/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1456 2022-12-19 12:02:57.000000 trytond_sale_shipment_cost-6.6.2/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-17 20:45:36.355651 trytond_sale_shipment_cost-6.6.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4561 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8406 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      797 2022-12-19 12:02:57.000000 trytond_sale_shipment_cost-6.6.2/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:45:36.348984 trytond_sale_shipment_cost-6.6.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8971 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/tests/scenario_sale_shipment_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3188 2022-12-19 12:02:57.000000 trytond_sale_shipment_cost-6.6.2/tests/scenario_sale_shipment_cost_modify_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3718 2023-04-08 09:35:50.000000 trytond_sale_shipment_cost-6.6.2/tests/scenario_sale_shipment_cost_promotion.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/tests/scenario_sale_shipment_cost_stock.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      544 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      270 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:45:36.355651 trytond_sale_shipment_cost-6.6.2/trytond_sale_shipment_cost.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2948 2023-05-17 20:45:35.000000 trytond_sale_shipment_cost-6.6.2/trytond_sale_shipment_cost.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2252 2023-05-17 20:45:36.000000 trytond_sale_shipment_cost-6.6.2/trytond_sale_shipment_cost.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:45:35.000000 trytond_sale_shipment_cost-6.6.2/trytond_sale_shipment_cost.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-05-17 20:45:35.000000 trytond_sale_shipment_cost-6.6.2/trytond_sale_shipment_cost.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:14:06.000000 trytond_sale_shipment_cost-6.6.2/trytond_sale_shipment_cost.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-05-17 20:45:35.000000 trytond_sale_shipment_cost-6.6.2/trytond_sale_shipment_cost.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-17 20:45:35.000000 trytond_sale_shipment_cost-6.6.2/trytond_sale_shipment_cost.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:45:36.352317 trytond_sale_shipment_cost-6.6.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2022-12-19 12:02:57.000000 trytond_sale_shipment_cost-6.6.2/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2022-12-19 12:02:58.000000 trytond_sale_shipment_cost-6.6.2/view/promotion_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      582 2022-12-19 12:02:57.000000 trytond_sale_shipment_cost-6.6.2/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2022-12-19 12:02:57.000000 trytond_sale_shipment_cost-6.6.2/view/sale_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      480 2023-04-13 16:52:41.000000 trytond_sale_shipment_cost-6.6.2/view/shipment_out_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2022-12-19 12:02:57.000000 trytond_sale_shipment_cost-6.6.2/view/shipment_out_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:21.137473 trytond_sale_shipment_cost-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3189 2023-05-01 11:11:48.000000 trytond_sale_shipment_cost-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-05-01 11:11:48.000000 trytond_sale_shipment_cost-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_shipment_cost-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2937 2023-05-01 11:57:21.134140 trytond_sale_shipment_cost-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      837 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:21.134140 trytond_sale_shipment_cost-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:21.127473 trytond_sale_shipment_cost-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3595 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3572 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2665 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3648 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3587 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3097 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3286 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3729 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2665 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3692 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3063 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2665 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3160 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2665 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2746 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3529 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2841 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3151 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2665 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2746 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3026 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2665 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2665 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2665 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1988 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1193 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16775 2023-04-30 10:46:36.000000 trytond_sale_shipment_cost-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1456 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:57:21.137473 trytond_sale_shipment_cost-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4522 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8403 2023-04-21 08:36:08.000000 trytond_sale_shipment_cost-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      797 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:21.130807 trytond_sale_shipment_cost-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8870 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/tests/scenario_sale_shipment_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3188 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/tests/scenario_sale_shipment_cost_modify_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3599 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/tests/scenario_sale_shipment_cost_promotion.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/tests/scenario_sale_shipment_cost_stock.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      270 2023-05-01 11:11:42.000000 trytond_sale_shipment_cost-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:21.134140 trytond_sale_shipment_cost-6.8.0/trytond_sale_shipment_cost.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2937 2023-05-01 11:57:20.000000 trytond_sale_shipment_cost-6.8.0/trytond_sale_shipment_cost.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2252 2023-05-01 11:57:21.000000 trytond_sale_shipment_cost-6.8.0/trytond_sale_shipment_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:57:20.000000 trytond_sale_shipment_cost-6.8.0/trytond_sale_shipment_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-05-01 11:57:20.000000 trytond_sale_shipment_cost-6.8.0/trytond_sale_shipment_cost.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_sale_shipment_cost-6.8.0/trytond_sale_shipment_cost.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-05-01 11:57:20.000000 trytond_sale_shipment_cost-6.8.0/trytond_sale_shipment_cost.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:57:20.000000 trytond_sale_shipment_cost-6.8.0/trytond_sale_shipment_cost.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:21.130807 trytond_sale_shipment_cost-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-01-16 14:00:21.000000 trytond_sale_shipment_cost-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/view/promotion_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      582 2023-01-16 14:00:21.000000 trytond_sale_shipment_cost-6.8.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-01-16 14:00:21.000000 trytond_sale_shipment_cost-6.8.0/view/sale_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      480 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/view/shipment_out_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-6.8.0/view/shipment_out_list.xml
```

### Comparing `trytond_sale_shipment_cost-6.6.2/CHANGELOG` & `trytond_sale_shipment_cost-6.8.0/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
-Version 6.6.2 - 2023-05-17
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.1 - 2023-02-05
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Require carrier to quote sale with shipment cost method
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_sale_shipment_cost-6.6.2/COPYRIGHT` & `trytond_sale_shipment_cost-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2011-2023 Cédric Krier.
 Copyright (C) 2011-2013 Bertrand Chenal.
-Copyright (C) 2011-2022 Nicolas Évrard.
+Copyright (C) 2011-2023 Nicolas Évrard.
 Copyright (C) 2011-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_sale_shipment_cost-6.6.2/LICENSE` & `trytond_sale_shipment_cost-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-6.6.2/PKG-INFO` & `trytond_sale_shipment_cost-6.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_shipment_cost
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module for sale shipment cost
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_shipment_cost
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale shipment cost
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
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
 Provides-Extra: test
 License-File: LICENSE
 
 Sale Shipment Cost Module
 #########################
 
 The sale_shipment_cost module adds shipment cost for sale.
```

### Comparing `trytond_sale_shipment_cost-6.6.2/README.rst` & `trytond_sale_shipment_cost-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-6.6.2/__init__.py` & `trytond_sale_shipment_cost-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-6.6.2/doc/conf.py` & `trytond_sale_shipment_cost-6.8.0/doc/conf.py`

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

### Comparing `trytond_sale_shipment_cost-6.6.2/doc/index.rst` & `trytond_sale_shipment_cost-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/bg.po` & `trytond_sale_shipment_cost-6.8.0/locale/bg.po`

 * *Files 5% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/ca.po` & `trytond_sale_shipment_cost-6.8.0/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,20 @@
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 "El mètode de cost d'enviament predeterminat per al client.\n"
 "Deixar buit per utilitzar el valor per defecte de la configuració."
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+"Per obtenir un pressupost de la venda \"%(sale)s\" heu d'introduïr un "
+"trasnportista."
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 "Per confirmar la venda \"%(sale)s\" heu de canviar el transportista "
 "\"%(carrier)s\"."
 
 msgctxt ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/cs.po` & `trytond_sale_shipment_cost-6.8.0/locale/cs.po`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/de.po` & `trytond_sale_shipment_cost-6.8.0/locale/de.po`

 * *Files 6% similar despite different names*

```diff
@@ -74,14 +74,20 @@
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 "Die Standard-Lieferkostenmethode für den Kunden.\n"
 "Leer lassen, um den Standardwert aus den Einstellungen zu verwenden."
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+"Damit der Verkauf \"%(sale)s\" in den Status \"Angebot\" gesetzt werden "
+"kann, muss zuerst ein Versanddienstleister erfasst werden."
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 "Damit der Verkauf \"%(sale)s\" bestätigt werden kann, muss der "
 "Versanddienstleister \"%(carrier)s\" geändert werden."
 
 msgctxt ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/es.po` & `trytond_sale_shipment_cost-6.8.0/locale/es.po`

 * *Files 8% similar despite different names*

```diff
@@ -74,14 +74,20 @@
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 "El método de costo de envío predeterminado para el cliente.\n"
 "Dejar en blanco para usar el valor predeterminado de la configuración."
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+"Para obtener un presupuesto de la venta \"%(sale)s\" debe introducir un "
+"transportista."
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 "Para confirmar la venta \"%(sale)s\" debe cambiar el transportista "
 "\"%(carrier)s\"."
 
 msgctxt ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/es_419.po` & `trytond_sale_shipment_cost-6.8.0/locale/es_419.po`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,18 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/et.po` & `trytond_sale_shipment_cost-6.8.0/locale/et.po`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,19 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr "Müügi \"%(sale)s\" kinnitamiseks tuleb muuta vedaja \"%(carrier)s\"."
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr "Müügi \"%(sale)s\" kinnitamiseks tuleb muuta vedaja \"%(carrier)s\"."
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/fa.po` & `trytond_sale_shipment_cost-6.8.0/locale/fa.po`

 * *Files 12% similar despite different names*

```diff
@@ -81,14 +81,21 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+#, fuzzy
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+"برای تأیید فروش :\"%(sale)s\" شما باید حمل کننده :\"%(carrier)s\" را تغییر "
+"دهید."
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 "برای تأیید فروش :\"%(sale)s\" شما باید حمل کننده :\"%(carrier)s\" را تغییر "
 "دهید."
 
 msgctxt ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/fi.po` & `trytond_sale_shipment_cost-6.8.0/locale/fi.po`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/fr.po` & `trytond_sale_shipment_cost-6.8.0/locale/fr.po`

 * *Files 5% similar despite different names*

```diff
@@ -74,14 +74,20 @@
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 "La méthode de coût d'expédition par défaut pour le client.\n"
 "Laissez vide pour utiliser la valeur par défaut de la configuration."
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+"Pour obtenir un devis pour la vente « %(sale)s », vous devez entrer un "
+"transporteur."
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 "Pour confirmer la vente « %(sale)s », vous devez changer le transporteur "
 "« %(carrier)s »."
 
 msgctxt ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/hu.po` & `trytond_sale_shipment_cost-6.8.0/locale/hu.po`

 * *Files 5% similar despite different names*

```diff
@@ -79,14 +79,18 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/id.po` & `trytond_sale_shipment_cost-6.8.0/locale/id.po`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/it.po` & `trytond_sale_shipment_cost-6.8.0/locale/it.po`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/lo.po` & `trytond_sale_shipment_cost-6.8.0/locale/lo.po`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/lt.po` & `trytond_sale_shipment_cost-6.8.0/locale/ru.po`

 * *Files 6% similar despite different names*

```diff
@@ -46,43 +46,47 @@
 msgid "Cost Invoice Line"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,cost_method:"
 msgid "Cost Method"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale:"
 msgid "Cost Sale"
-msgstr ""
+msgstr "Стоимость"
 
-#, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale_currency:"
 msgid "Cost Sale Currency"
-msgstr "Savikainos valiuta"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale_currency_used:"
 msgid "Cost Sale Currency"
-msgstr "Savikainos valiuta"
+msgstr "Стоимость"
 
 #, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale_used:"
 msgid "Cost Sale"
-msgstr "Savikainos valiuta"
+msgstr "Стоимость"
 
 msgctxt "field:stock.shipment.out,shipment_cost_sale_readonly:"
 msgid "Shipment Cost Sale Read Only"
 msgstr ""
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/nl.po` & `trytond_sale_shipment_cost-6.8.0/locale/nl.po`

 * *Files 8% similar despite different names*

```diff
@@ -74,14 +74,20 @@
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 "De standaardverzendkostenmethode voor de klant.\n"
 "Laat leeg om de standaardwaarde uit de configuratie te gebruiken."
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+"Om een offerte voor verkoop \"%(sale)s\" te maken, moet u een koerier "
+"toevoegen."
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 "Om verkoop \"%(sale)s\" te bevestigen, moet u de vervoerder "
 "\"%(carrier)s\"wijzigen."
 
 msgctxt ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/pl.po` & `trytond_sale_shipment_cost-6.8.0/locale/lt.po`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.invoice.line,cost_shipments:"
 msgid "Cost of Shipments"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:party.party,sale_shipment_cost_method:"
 msgid "Shipment Cost Method"
-msgstr "Koszt wysyłki"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:party.party.sale_method,sale_shipment_cost_method:"
 msgid "Sale Shipment Cost Method"
-msgstr "Koszt wysyłki"
+msgstr ""
 
 msgctxt "field:sale.configuration,sale_shipment_cost_method:"
 msgid "Sale Shipment Cost Method"
 msgstr ""
 
 msgctxt "field:sale.configuration.sale_method,sale_shipment_cost_method:"
 msgid "Sale Shipment Cost Method"
 msgstr ""
 
 msgctxt "field:sale.line,shipment_cost:"
 msgid "Shipment Cost"
-msgstr "Koszt wysyłki"
+msgstr ""
 
 msgctxt "field:sale.promotion,amount_shipment_cost_included:"
 msgid "Amount with Shipment Cost Included"
 msgstr ""
 
 msgctxt "field:sale.sale,available_carriers:"
 msgid "Available Carriers"
@@ -48,45 +46,47 @@
 msgid "Cost Invoice Line"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,cost_method:"
 msgid "Cost Method"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale:"
 msgid "Cost Sale"
-msgstr "Koszt"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale_currency:"
 msgid "Cost Sale Currency"
-msgstr "Koszt waluty"
+msgstr "Savikainos valiuta"
 
 #, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale_currency_used:"
 msgid "Cost Sale Currency"
-msgstr "Koszt waluty"
+msgstr "Savikainos valiuta"
 
 #, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale_used:"
 msgid "Cost Sale"
-msgstr "Koszt"
+msgstr "Savikainos valiuta"
 
-#, fuzzy
 msgctxt "field:stock.shipment.out,shipment_cost_sale_readonly:"
 msgid "Shipment Cost Sale Read Only"
-msgstr "Koszt wysyłki"
+msgstr ""
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
@@ -102,11 +102,10 @@
 msgid "On Order"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_cost_method:"
 msgid "On Shipment"
 msgstr ""
 
-#, fuzzy
 msgctxt "view:sale.promotion:"
 msgid "Shipment Cost Included"
-msgstr "Koszt wysyłki"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/pt.po` & `trytond_sale_shipment_cost-6.8.0/locale/pt.po`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,18 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/ro.po` & `trytond_sale_shipment_cost-6.8.0/locale/ro.po`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/ru.po` & `trytond_sale_shipment_cost-6.8.0/locale/tr.po`

 * *Files 2% similar despite different names*

```diff
@@ -46,43 +46,44 @@
 msgid "Cost Invoice Line"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,cost_method:"
 msgid "Cost Method"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale:"
 msgid "Cost Sale"
-msgstr "Стоимость"
+msgstr ""
 
 msgctxt "field:stock.shipment.out,cost_sale_currency:"
 msgid "Cost Sale Currency"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale_currency_used:"
 msgid "Cost Sale Currency"
-msgstr "Стоимость"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale_used:"
 msgid "Cost Sale"
-msgstr "Стоимость"
+msgstr ""
 
 msgctxt "field:stock.shipment.out,shipment_cost_sale_readonly:"
 msgid "Shipment Cost Sale Read Only"
 msgstr ""
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/sl.po` & `trytond_sale_shipment_cost-6.8.0/locale/sl.po`

 * *Files 5% similar despite different names*

```diff
@@ -81,14 +81,18 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/tr.po` & `trytond_sale_shipment_cost-6.8.0/locale/uk.po`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/uk.po` & `trytond_sale_shipment_cost-6.8.0/locale/zh_CN.po`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
```

### Comparing `trytond_sale_shipment_cost-6.6.2/locale/zh_CN.po` & `trytond_sale_shipment_cost-6.8.0/locale/pl.po`

 * *Files 18% similar despite different names*

```diff
@@ -2,33 +2,35 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.invoice.line,cost_shipments:"
 msgid "Cost of Shipments"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:party.party,sale_shipment_cost_method:"
 msgid "Shipment Cost Method"
-msgstr ""
+msgstr "Koszt wysyłki"
 
+#, fuzzy
 msgctxt "field:party.party.sale_method,sale_shipment_cost_method:"
 msgid "Sale Shipment Cost Method"
-msgstr ""
+msgstr "Koszt wysyłki"
 
 msgctxt "field:sale.configuration,sale_shipment_cost_method:"
 msgid "Sale Shipment Cost Method"
 msgstr ""
 
 msgctxt "field:sale.configuration.sale_method,sale_shipment_cost_method:"
 msgid "Sale Shipment Cost Method"
 msgstr ""
 
 msgctxt "field:sale.line,shipment_cost:"
 msgid "Shipment Cost"
-msgstr ""
+msgstr "Koszt wysyłki"
 
 msgctxt "field:sale.promotion,amount_shipment_cost_included:"
 msgid "Amount with Shipment Cost Included"
 msgstr ""
 
 msgctxt "field:sale.sale,available_carriers:"
 msgid "Available Carriers"
@@ -46,40 +48,49 @@
 msgid "Cost Invoice Line"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,cost_method:"
 msgid "Cost Method"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale:"
 msgid "Cost Sale"
-msgstr ""
+msgstr "Koszt"
 
+#, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale_currency:"
 msgid "Cost Sale Currency"
-msgstr ""
+msgstr "Koszt waluty"
 
+#, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale_currency_used:"
 msgid "Cost Sale Currency"
-msgstr ""
+msgstr "Koszt waluty"
 
+#, fuzzy
 msgctxt "field:stock.shipment.out,cost_sale_used:"
 msgid "Cost Sale"
-msgstr ""
+msgstr "Koszt"
 
+#, fuzzy
 msgctxt "field:stock.shipment.out,shipment_cost_sale_readonly:"
 msgid "Shipment Cost Sale Read Only"
-msgstr ""
+msgstr "Koszt wysyłki"
 
 msgctxt "help:party.party,sale_shipment_cost_method:"
 msgid ""
 "The default shipment cost method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_sale_carrier_required_for_quotation"
+msgid "To get a quote for sale \"%(sale)s\" you must enter a carrier."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_sale_invalid_carrier"
 msgid "To confirm sale \"%(sale)s\" you must change the carrier \"%(carrier)s\"."
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_shipment_cost_invoice_missing_account_revenue"
 msgid ""
@@ -95,10 +106,11 @@
 msgid "On Order"
 msgstr ""
 
 msgctxt "selection:sale.sale,shipment_cost_method:"
 msgid "On Shipment"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:sale.promotion:"
 msgid "Shipment Cost Included"
-msgstr ""
+msgstr "Koszt wysyłki"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_shipment_cost-6.6.2/message.xml` & `trytond_sale_shipment_cost-6.8.0/message.xml`

 * *Files 20% similar despite different names*

#### Comparing `trytond_sale_shipment_cost-6.6.2/message.xml` & `trytond_sale_shipment_cost-6.8.0/message.xml`

```diff
@@ -2,12 +2,15 @@
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <tryton>
   <data grouped="1">
     <record model="ir.message" id="msg_sale_invalid_carrier">
       <field name="text">To confirm sale &quot;%(sale)s&quot; you must change the carrier &quot;%(carrier)s&quot;.</field>
     </record>
+    <record model="ir.message" id="msg_sale_carrier_required_for_quotation">
+      <field name="text">To get a quote for sale &quot;%(sale)s&quot; you must enter a carrier.</field>
+    </record>
     <record model="ir.message" id="msg_shipment_cost_invoice_missing_account_revenue">
       <field name="text">To invoice shipment cost of &quot;%(shipment)s&quot;, you must define an account revenue for product &quot;%(product)s&quot;.</field>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_sale_shipment_cost-6.6.2/party.py` & `trytond_sale_shipment_cost-6.8.0/party.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,17 +34,16 @@
 
     @classmethod
     def default_sale_shipment_cost_method(cls, **pattern):
         return 'default'
 
     @classmethod
     def copy(cls, parties, default=None):
-        context = Transaction().context
         default = default.copy() if default else {}
-        if context.get('_check_access'):
+        if Transaction().check_access:
             fields = ['sale_shipment_cost_method']
             default_values = cls.default_get(fields, with_rec_name=False)
             for fname in fields:
                 default.setdefault(fname, default_values.get(fname))
         return super().copy(parties, default=default)
```

### Comparing `trytond_sale_shipment_cost-6.6.2/party.xml` & `trytond_sale_shipment_cost-6.8.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-6.6.2/sale.py` & `trytond_sale_shipment_cost-6.8.0/sale.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # this repository contains the full copyright notices and license terms.
 from decimal import Decimal
 
 from trytond import backend
 from trytond.i18n import gettext
 from trytond.model import ModelView, Workflow, fields
 from trytond.modules.product import price_digits, round_price
-from trytond.modules.sale.exceptions import SaleConfirmError
+from trytond.modules.sale.exceptions import (
+    SaleConfirmError, SaleQuotationError)
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval, If
 from trytond.transaction import Transaction
 
 sale_shipment_cost_method = fields.Selection(
         'get_sale_shipment_cost_methods', "Sale Shipment Cost Method")
 
@@ -149,16 +150,15 @@
 
         if (self.warehouse
                 and self.shipment_address
                 and self.warehouse.address == self.shipment_address):
             return []
 
         pattern = self._get_carrier_selection_pattern()
-        carriers = CarrierSelection.get_carriers(pattern)
-        return [c.id for c in carriers]
+        return CarrierSelection.get_carriers(pattern)
 
     @fields.depends('carrier', methods=['on_change_with_available_carriers'])
     def on_change_party(self):
         super(Sale, self).on_change_party()
         self.available_carriers = self.on_change_with_available_carriers()
         if self.available_carriers and (not self.carrier
                 or self.carrier not in self.available_carriers):
@@ -194,14 +194,27 @@
         self.available_carriers = self.on_change_with_available_carriers()
         if self.available_carriers and (not self.carrier
                 or self.carrier not in self.available_carriers):
             self.carrier = self.available_carriers[0]
         elif not self.available_carriers:
             self.carrier = None
 
+    def check_for_quotation(self):
+        super().check_for_quotation()
+        if self.shipment_cost_method and self.available_carriers:
+            for line in self.lines:
+                if (line.product
+                        and line.product.type != 'service'
+                        and line.quantity >= 0
+                        and not self.carrier):
+                    raise SaleQuotationError(
+                        gettext('sale'
+                            '.msg_sale_carrier_required_for_quotation',
+                            sale=self.rec_name))
+
     @classmethod
     @ModelView.button
     @Workflow.transition('quotation')
     def quote(cls, sales):
         pool = Pool()
         Line = pool.get('sale.line')
         removed = []
@@ -296,16 +309,14 @@
             shipment_cost=shipment_cost,
             )
         cost_line.on_change_product()
         if unit_price is not None:
             cost_line.unit_price = round_price(unit_price)
         else:
             cost_line.unit_price = round_price(cost)
-        if not cost_line.unit_price:
-            cost_line.quantity = 0
         cost_line.amount = cost_line.on_change_with_amount()
         return cost_line
 
     @property
     def _shipment_grouping_fields(self):
         return super()._shipment_grouping_fields + ('cost_method', 'carrier')
```

### Comparing `trytond_sale_shipment_cost-6.6.2/sale.xml` & `trytond_sale_shipment_cost-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-6.6.2/setup.py` & `trytond_sale_shipment_cost-6.8.0/setup.py`

 * *Files 2% similar despite different names*

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
@@ -34,16 +31,19 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_shipment_cost'
 
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
 
@@ -54,22 +54,22 @@
     tests_require.append(get_require_version('trytond_%s' % dep))
 
 setup(name=name,
     version=version,
     description='Tryton module for sale shipment cost',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_shipment_cost',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale shipment cost',
     package_dir={'trytond.modules.sale_shipment_cost': '.'},
     packages=(
         ['trytond.modules.sale_shipment_cost']
         + ['trytond.modules.sale_shipment_cost.%s' % p
             for p in find_packages()]
@@ -107,23 +107,23 @@
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
     extras_require={
         'test': tests_require,
     },
     zip_safe=False,
     entry_points="""
     [trytond.modules]
```

### Comparing `trytond_sale_shipment_cost-6.6.2/stock.py` & `trytond_sale_shipment_cost-6.8.0/stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     @fields.depends(
         'shipment_cost_sale_readonly', 'cost_sale_currency', 'cost_edit',
         methods=['_compute_costs'])
     def on_change_with_cost_sale_currency_used(self, name=None):
         if not self.cost_edit and not self.shipment_cost_sale_readonly:
             return self._compute_costs()['cost_sale_currency']
         elif self.cost_sale_currency:
-            return self.cost_sale_currency.id
+            return self.cost_sale_currency
 
     @classmethod
     def get_cost_methods(cls):
         pool = Pool()
         Sale = pool.get('sale.sale')
         fieldname = 'shipment_cost_method'
         return Sale.fields_get([fieldname])[fieldname]['selection']
```

### Comparing `trytond_sale_shipment_cost-6.6.2/stock.xml` & `trytond_sale_shipment_cost-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-6.6.2/tests/scenario_sale_shipment_cost.rst` & `trytond_sale_shipment_cost-6.8.0/tests/scenario_sale_shipment_cost.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 ===========================
 Sale Shipment Cost Scenario
 ===========================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'sale_shipment_cost',
     ...         'sale',
     ...         'account_invoice',
@@ -65,26 +63,26 @@
     >>> unit, = ProductUom.find([('name', '=', 'Unit')])
 
     >>> template = ProductTemplate()
     >>> template.name = 'Product'
     >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.salable = True
-    >>> template.lead_time = datetime.timedelta(0)
+    >>> template.lead_time = dt.timedelta(0)
     >>> template.list_price = Decimal('20')
     >>> template.account_category = account_category
     >>> template.save()
     >>> product, = template.products
 
     >>> carrier_template = ProductTemplate()
     >>> carrier_template.name = 'Carrier Product'
     >>> carrier_template.default_uom = unit
     >>> carrier_template.type = 'service'
     >>> carrier_template.salable = True
-    >>> carrier_template.lead_time = datetime.timedelta(0)
+    >>> carrier_template.lead_time = dt.timedelta(0)
     >>> carrier_template.list_price = Decimal('3')
     >>> carrier_template.account_category = account_category
     >>> carrier_template.save()
     >>> carrier_product, = carrier_template.products
     >>> carrier_product.cost_price = Decimal('2')
     >>> carrier_product.save()
```

### Comparing `trytond_sale_shipment_cost-6.6.2/tests/scenario_sale_shipment_cost_modify_price.rst` & `trytond_sale_shipment_cost-6.8.0/tests/scenario_sale_shipment_cost_modify_price.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-6.6.2/tests/scenario_sale_shipment_cost_promotion.rst` & `trytond_sale_shipment_cost-6.8.0/tests/scenario_sale_shipment_cost_promotion.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 =====================================
 Sale Shipment Cost Promotion Scenario
 =====================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'sale_shipment_cost',
     ...         'sale',
     ...         'sale_promotion',
```

### Comparing `trytond_sale_shipment_cost-6.6.2/tests/scenario_sale_shipment_cost_stock.rst` & `trytond_sale_shipment_cost-6.8.0/tests/scenario_sale_shipment_cost_stock.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-6.6.2/trytond_sale_shipment_cost.egg-info/PKG-INFO` & `trytond_sale_shipment_cost-6.8.0/trytond_sale_shipment_cost.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-shipment-cost
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module for sale shipment cost
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_shipment_cost
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale shipment cost
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
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
 Provides-Extra: test
 License-File: LICENSE
 
 Sale Shipment Cost Module
 #########################
 
 The sale_shipment_cost module adds shipment cost for sale.
```

### Comparing `trytond_sale_shipment_cost-6.6.2/trytond_sale_shipment_cost.egg-info/SOURCES.txt` & `trytond_sale_shipment_cost-6.8.0/trytond_sale_shipment_cost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-6.6.2/view/sale_form.xml` & `trytond_sale_shipment_cost-6.8.0/view/sale_form.xml`

 * *Files identical despite different names*

