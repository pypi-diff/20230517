# Comparing `tmp/trytond_stock_supply-6.6.3.tar.gz` & `tmp/trytond_stock_supply-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_supply-6.6.3.tar", last modified: Wed May 17 20:42:42 2023, max compression
+gzip compressed data, was "trytond_stock_supply-6.8.0.tar", last modified: Mon May  1 11:49:51 2023, max compression
```

## Comparing `trytond_stock_supply-6.6.3.tar` & `trytond_stock_supply-6.8.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:42:42.456888 trytond_stock_supply-6.6.3/
--rw-r--r--   0 ced       (1000) ced       (1000)     3879 2023-05-17 20:42:39.000000 trytond_stock_supply-6.6.3/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      761 2023-05-17 20:42:39.000000 trytond_stock_supply-6.6.3/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:59.000000 trytond_stock_supply-6.6.3/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4147 2023-05-17 20:42:42.456888 trytond_stock_supply-6.6.3/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1937 2023-04-08 09:35:50.000000 trytond_stock_supply-6.6.3/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:42:42.453554 trytond_stock_supply-6.6.3/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2023-04-08 09:35:50.000000 trytond_stock_supply-6.6.3/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1937 2023-04-08 09:35:50.000000 trytond_stock_supply-6.6.3/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2022-12-19 12:02:59.000000 trytond_stock_supply-6.6.3/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2022-12-19 12:02:59.000000 trytond_stock_supply-6.6.3/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:42:42.450221 trytond_stock_supply-6.6.3/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5635 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6000 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5981 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6050 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4704 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4985 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6098 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6102 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5766 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4701 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4980 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4839 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5825 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5039 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5924 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4611 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5634 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5680 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4597 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4869 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2091 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/location.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2022-12-19 12:02:59.000000 trytond_stock_supply-6.6.3/location.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1357 2022-12-19 12:02:59.000000 trytond_stock_supply-6.6.3/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9085 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/order_point.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4016 2022-12-19 12:02:59.000000 trytond_stock_supply-6.6.3/order_point.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      848 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1637 2022-12-19 12:02:59.000000 trytond_stock_supply-6.6.3/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14341 2023-05-04 17:18:26.000000 trytond_stock_supply-6.6.3/purchase_request.py
--rw-r--r--   0 ced       (1000) ced       (1000)      966 2022-12-19 12:02:59.000000 trytond_stock_supply-6.6.3/purchase_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-17 20:42:42.456888 trytond_stock_supply-6.6.3/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4337 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7696 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/shipment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5068 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1279 2022-12-19 12:02:59.000000 trytond_stock_supply-6.6.3/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:42:42.453554 trytond_stock_supply-6.6.3/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5883 2023-04-08 09:35:50.000000 trytond_stock_supply-6.6.3/tests/scenario_stock_internal_supply.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4349 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/tests/scenario_stock_internal_supply_lead_time.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4578 2023-04-08 09:35:50.000000 trytond_stock_supply-6.6.3/tests/scenario_stock_internal_supply_overflow.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7533 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/tests/scenario_stock_supply_purchase_request.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6265 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      532 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:42:42.456888 trytond_stock_supply-6.6.3/trytond_stock_supply.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4147 2023-05-17 20:42:41.000000 trytond_stock_supply-6.6.3/trytond_stock_supply.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2340 2023-05-17 20:42:42.000000 trytond_stock_supply-6.6.3/trytond_stock_supply.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:42:41.000000 trytond_stock_supply-6.6.3/trytond_stock_supply.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-05-17 20:42:41.000000 trytond_stock_supply-6.6.3/trytond_stock_supply.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:05:32.000000 trytond_stock_supply-6.6.3/trytond_stock_supply.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2023-05-17 20:42:41.000000 trytond_stock_supply-6.6.3/trytond_stock_supply.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-17 20:42:41.000000 trytond_stock_supply-6.6.3/trytond_stock_supply.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:42:42.453554 trytond_stock_supply-6.6.3/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1076 2022-12-19 12:02:59.000000 trytond_stock_supply-6.6.3/view/order_point_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/view/order_point_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2022-12-19 12:02:59.000000 trytond_stock_supply-6.6.3/view/purchase_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-04-13 16:52:41.000000 trytond_stock_supply-6.6.3/view/supply_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:51.255224 trytond_stock_supply-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3740 2023-05-01 11:06:35.000000 trytond_stock_supply-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      761 2023-05-01 11:06:35.000000 trytond_stock_supply-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_supply-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4141 2023-05-01 11:49:51.251891 trytond_stock_supply-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1936 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:51.248557 trytond_stock_supply-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1936 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:51.245224 trytond_stock_supply-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5635 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6000 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5981 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6050 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4704 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4985 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6098 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6102 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5766 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4701 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4980 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4839 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5820 2023-04-30 10:46:36.000000 trytond_stock_supply-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5039 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5924 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4611 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5634 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5680 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4597 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4869 2023-04-29 08:02:45.000000 trytond_stock_supply-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2091 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/location.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-01-16 14:00:21.000000 trytond_stock_supply-6.8.0/location.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1357 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9212 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/order_point.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4016 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/order_point.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      848 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1637 2023-01-16 14:00:21.000000 trytond_stock_supply-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14495 2023-04-30 10:46:36.000000 trytond_stock_supply-6.8.0/purchase_request.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      966 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/purchase_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:49:51.255224 trytond_stock_supply-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4304 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7696 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/shipment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5007 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1279 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:51.245224 trytond_stock_supply-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5764 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/tests/scenario_stock_internal_supply.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4286 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/tests/scenario_stock_internal_supply_lead_time.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4459 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/tests/scenario_stock_internal_supply_overflow.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7516 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/tests/scenario_stock_supply_purchase_request.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6265 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-05-01 11:06:30.000000 trytond_stock_supply-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:51.251891 trytond_stock_supply-6.8.0/trytond_stock_supply.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4141 2023-05-01 11:49:50.000000 trytond_stock_supply-6.8.0/trytond_stock_supply.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2340 2023-05-01 11:49:51.000000 trytond_stock_supply-6.8.0/trytond_stock_supply.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:49:50.000000 trytond_stock_supply-6.8.0/trytond_stock_supply.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-05-01 11:49:50.000000 trytond_stock_supply-6.8.0/trytond_stock_supply.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_stock_supply-6.8.0/trytond_stock_supply.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      217 2023-05-01 11:49:50.000000 trytond_stock_supply-6.8.0/trytond_stock_supply.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:49:50.000000 trytond_stock_supply-6.8.0/trytond_stock_supply.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:51.248557 trytond_stock_supply-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1076 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/view/order_point_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/view/order_point_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/view/purchase_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-04-15 07:12:15.000000 trytond_stock_supply-6.8.0/view/supply_start_form.xml
```

### Comparing `trytond_stock_supply-6.6.3/CHANGELOG` & `trytond_stock_supply-6.8.0/CHANGELOG`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 
-Version 6.6.3 - 2023-05-17
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 6.6.2 - 2023-03-04
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.1 - 2023-02-05
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_stock_supply-6.6.3/COPYRIGHT` & `trytond_stock_supply-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/LICENSE` & `trytond_stock_supply-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/PKG-INFO` & `trytond_stock_supply-6.8.0/trytond_stock_supply.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
-Name: trytond_stock_supply
-Version: 6.6.3
+Name: trytond-stock-supply
+Version: 6.8.0
 Summary: Tryton module for stock supply
 Home-page: http://www.tryton.org/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_supply
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock supply
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
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
 
 Stock Supply Module
 ###################
 
 The Stock Supply module add automatic supply mechanisms and introduce
@@ -64,15 +64,15 @@
 An order point define minimum, maximum and target quantities for a product on a
 location.
 
 * The minimum quantity is the threshold quantity below which the provisioning
   process will be triggered.
 
 * The maximum quantity is the threshold quantity above which the overflowing
-  process will be triggered. 
+  process will be triggered.
 
 * The target quantity is the quantity that will be found in the location after
   the provisioning / overflowing process has been completed.
 
 An order point also define a type which can be:
 
 * Internal
```

### Comparing `trytond_stock_supply-6.6.3/README.rst` & `trytond_stock_supply-6.8.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 An order point define minimum, maximum and target quantities for a product on a
 location.
 
 * The minimum quantity is the threshold quantity below which the provisioning
   process will be triggered.
 
 * The maximum quantity is the threshold quantity above which the overflowing
-  process will be triggered. 
+  process will be triggered.
 
 * The target quantity is the quantity that will be found in the location after
   the provisioning / overflowing process has been completed.
 
 An order point also define a type which can be:
 
 * Internal
```

### Comparing `trytond_stock_supply-6.6.3/__init__.py` & `trytond_stock_supply-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/doc/conf.py` & `trytond_stock_supply-6.8.0/doc/conf.py`

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

### Comparing `trytond_stock_supply-6.6.3/doc/index.rst` & `trytond_stock_supply-6.8.0/doc/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 An order point define minimum, maximum and target quantities for a product on a
 location.
 
 * The minimum quantity is the threshold quantity below which the provisioning
   process will be triggered.
 
 * The maximum quantity is the threshold quantity above which the overflowing
-  process will be triggered. 
+  process will be triggered.
 
 * The target quantity is the quantity that will be found in the location after
   the provisioning / overflowing process has been completed.
 
 An order point also define a type which can be:
 
 * Internal
```

### Comparing `trytond_stock_supply-6.6.3/locale/bg.po` & `trytond_stock_supply-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/ca.po` & `trytond_stock_supply-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/cs.po` & `trytond_stock_supply-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/de.po` & `trytond_stock_supply-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/es.po` & `trytond_stock_supply-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/es_419.po` & `trytond_stock_supply-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/et.po` & `trytond_stock_supply-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/fa.po` & `trytond_stock_supply-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/fi.po` & `trytond_stock_supply-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/fr.po` & `trytond_stock_supply-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/hu.po` & `trytond_stock_supply-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/id.po` & `trytond_stock_supply-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/it.po` & `trytond_stock_supply-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/lo.po` & `trytond_stock_supply-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/lt.po` & `trytond_stock_supply-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/nl.po` & `trytond_stock_supply-6.8.0/locale/nl.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,203 +1,203 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,order_points:"
 msgid "Order Points"
-msgstr "Bestel regels"
+msgstr "Bestel Niveaus"
 
 msgctxt "field:purchase.configuration,supply_period:"
 msgid "Supply Period"
 msgstr "Leveringstermijn"
 
 msgctxt "field:purchase.configuration.supply_period,supply_period:"
 msgid "Supply Period"
 msgstr "Leveringstermijn"
 
 msgctxt "field:stock.location,overflowing_location:"
 msgid "Overflowing Location"
-msgstr "locatie overschot (surplus)"
+msgstr "Overloop Locatie"
 
 msgctxt "field:stock.location,provisioning_location:"
 msgid "Provisioning Location"
-msgstr "provisioning Locatie"
+msgstr "Bevoorrading Locatie"
 
 msgctxt "field:stock.order_point,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
 msgctxt "field:stock.order_point,location:"
 msgid "Location"
-msgstr "Plaats"
+msgstr "Locatie"
 
 msgctxt "field:stock.order_point,max_quantity:"
 msgid "Maximal Quantity"
-msgstr "Maximale hoeveelheid"
+msgstr "Maximale Hoeveelheid"
 
 msgctxt "field:stock.order_point,min_quantity:"
 msgid "Minimal Quantity"
-msgstr "Minimale hoeveelheid"
+msgstr "Minimale Hoeveelheid"
 
 msgctxt "field:stock.order_point,overflowing_location:"
 msgid "Overflowing Location"
-msgstr "Overschot locatie"
+msgstr "Overloop Locatie"
 
 msgctxt "field:stock.order_point,product:"
 msgid "Product"
 msgstr "Product"
 
 msgctxt "field:stock.order_point,provisioning_location:"
 msgid "Provisioning Location"
-msgstr "provisioning Locatie"
+msgstr "Bevoorrading Locatie"
 
 msgctxt "field:stock.order_point,storage_location:"
 msgid "Storage Location"
-msgstr "Opslaglocatie"
+msgstr "Opslag Locatie"
 
 msgctxt "field:stock.order_point,target_quantity:"
 msgid "Target Quantity"
-msgstr "Gewenste hoeveelheid"
+msgstr "Gewenste Hoeveelheid"
 
 msgctxt "field:stock.order_point,type:"
 msgid "Type"
-msgstr "Type"
+msgstr "Soort"
 
 msgctxt "field:stock.order_point,unit:"
 msgid "Unit"
 msgstr "Eenheid"
 
 msgctxt "field:stock.order_point,warehouse_location:"
 msgid "Warehouse Location"
-msgstr "Magazijnlocatie"
+msgstr "Magazijn Locatie"
 
 msgctxt "field:stock.supply.start,warehouses:"
 msgid "Warehouses"
 msgstr "Magazijnen"
 
 msgctxt "help:stock.location,overflowing_location:"
 msgid "Leave empty for no default overflowing."
-msgstr "Laat leeg als er geen opslaglocatie wordt gebruikt voor overschotten."
+msgstr "Laat leeg als er geen locatie wordt gebruikt als overloop."
 
 msgctxt "help:stock.location,provisioning_location:"
 msgid "Leave empty for no default provisioning."
-msgstr "Laat leeg als er geen opslaglocatie wordt gebruikt voor overschotten."
+msgstr "Laat leeg als er geen locatie wordt gebruikt voor bevoorrading."
 
 msgctxt "help:stock.supply.start,warehouses:"
 msgid "If empty all warehouses are used."
 msgstr "Indien leeg worden alle magazijnen gebruikt."
 
 msgctxt "model:ir.action,name:act_order_point_form"
 msgid "Order Points"
-msgstr "Bestel punten"
+msgstr "Bestel Niveaus"
 
 msgctxt "model:ir.action,name:act_order_point_form_relate"
 msgid "Order Points"
-msgstr "Bestel punten"
+msgstr "Bestel Niveaus"
 
 msgctxt "model:ir.action,name:act_order_point_form_relate2"
 msgid "Order Points"
-msgstr "Bestel punten"
+msgstr "Bestel Niveaus"
 
 msgctxt "model:ir.action,name:act_stock_supply"
 msgid "Supply Stock"
-msgstr "voorraad levering"
+msgstr "Voorraad Levering"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_order_point_form_domain_all"
 msgid "All"
 msgstr "Alle"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_order_point_form_domain_internal"
 msgid "Internal"
 msgstr "Intern"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_order_point_form_domain_purchase"
 msgid "Purchase"
-msgstr "Aankoop"
+msgstr "Inkoop"
 
 msgctxt "model:ir.message,text:msg_late_customer_moves"
 msgid "There are some customer moves that are late."
-msgstr "Er zijn enkele klantbewegingen die te laat zijn."
+msgstr "Er zijn enkele klant mutaties die te laat zijn."
 
 msgctxt "model:ir.message,text:msg_late_supplier_moves"
 msgid "There are some supplier moves that are late."
-msgstr "Er zijn enkele leveranciersbewegingen die te laat zijn."
+msgstr "Er zijn enkele leveranciers mutaties die te laat zijn."
 
 msgctxt ""
 "model:ir.message,text:msg_order_point_concurrent_overflowing_location_internal"
 msgid ""
 "You cannot define for the same product two order points with opposite locations\n"
 "(from \"Overflowing Location\" to \"Provisioning Location\" and vice versa)."
 msgstr ""
-"U kunt voor hetzelfde product niet twee bestelpunten met tegenovergestelde locaties definiëren\n"
-"(van \"Overstock locatie\" naar \"provisielocatie\" en vice versa)."
+"U kunt voor hetzelfde product niet twee bestel niveaus met tegenovergestelde locaties definiëren\n"
+"(van \"Overloop Locatie\" naar \"Bevoorrading Locatie\" en vice versa)."
 
 msgctxt ""
 "model:ir.message,text:msg_order_point_concurrent_provisioning_location_internal"
 msgid ""
 "You cannot define for the same product two order points with opposite locations\n"
 "(from \"Storage Location\" to \"Provisioning Location\" and vice versa)."
 msgstr ""
-"U kunt voor hetzelfde product niet twee bestelpunten met tegenovergestelde locaties definiëren\n"
-"(van \"Opslag locatie\" naar \"provisielocatie\" en vice versa)."
+"U kunt voor hetzelfde product niet twee bestel niveaus met tegenovergestelde locaties definiëren\n"
+"(van \"Opslag Locatie\" naar \"Bevoorrading Locatie\" en vice versa)."
 
 msgctxt "model:ir.message,text:msg_order_point_unique"
 msgid "Only one order point is allowed for each product-location pair."
-msgstr "Per product-locatiepaar is slechts één bestelpunt toegestaan."
+msgstr "Per product-locatiepaar is slechts één bestel niveau toegestaan."
 
 msgctxt "model:ir.rule.group,name:rule_group_order_point_companies"
 msgid "User in companies"
-msgstr "Gebruiker in het bedrijf"
+msgstr "Gebruiker in bedrijven"
 
 msgctxt "model:ir.ui.menu,name:menu_order_point_form"
 msgid "Order Points"
-msgstr "Bestel punten"
+msgstr "Bestel Niveaus"
 
 msgctxt "model:ir.ui.menu,name:menu_stock_supply"
 msgid "Supply Stock"
-msgstr "voorraad levering"
+msgstr "Voorraad Levering"
 
 msgctxt "model:purchase.configuration.supply_period,name:"
 msgid "Purchase Configuration Supply Period"
-msgstr "configuratie aankoop verwervingsperiode"
+msgstr "Configuratie Inkoop Levering Periode"
 
 msgctxt "model:stock.order_point,name:"
 msgid "Order Point"
-msgstr "Bestelpunt"
+msgstr "Bestel Niveau"
 
 msgctxt "model:stock.supply.start,name:"
 msgid "Supply Stock"
-msgstr "voorraad levering"
+msgstr "Voorraad Levering"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Supply Stock"
-msgstr "voorraad levering"
+msgstr "Voorraad Levering"
 
 msgctxt "selection:stock.order_point,type:"
 msgid "Internal"
 msgstr "Intern"
 
 msgctxt "selection:stock.order_point,type:"
 msgid "Purchase"
-msgstr "Aankoop"
+msgstr "Inkoop"
 
 msgctxt "view:stock.order_point:"
 msgid "Order Point Type"
-msgstr "Bestelpunttype"
+msgstr "Soort Bestel Niveau"
 
 msgctxt "view:stock.order_point:"
 msgid "Product Info"
-msgstr "Product informatie"
+msgstr "Product Informatie"
 
 msgctxt "view:stock.supply.start:"
 msgid "Supply Stock?"
-msgstr "Voorraad inslaan?"
+msgstr "Voorraad Inslaan?"
 
 msgctxt "wizard_button:stock.supply,start,create_:"
 msgid "Create"
 msgstr "Maken"
 
 msgctxt "wizard_button:stock.supply,start,end:"
 msgid "Cancel"
```

### Comparing `trytond_stock_supply-6.6.3/locale/pl.po` & `trytond_stock_supply-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/pt.po` & `trytond_stock_supply-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/ro.po` & `trytond_stock_supply-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/ru.po` & `trytond_stock_supply-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/sl.po` & `trytond_stock_supply-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/tr.po` & `trytond_stock_supply-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/uk.po` & `trytond_stock_supply-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/locale/zh_CN.po` & `trytond_stock_supply-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/location.py` & `trytond_stock_supply-6.8.0/location.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/message.xml` & `trytond_stock_supply-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/order_point.py` & `trytond_stock_supply-6.8.0/order_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,18 @@
                     [sql_table.target_quantity, sql_table.max_quantity],
                     [sql_table.max_quantity, Null]))
 
     @staticmethod
     def default_type():
         return "purchase"
 
+    @classmethod
+    def default_warehouse_location(cls):
+        return Pool().get('stock.location').get_default_warehouse()
+
     @fields.depends('product', '_parent_product.default_uom')
     def on_change_product(self):
         self.unit = None
         if self.product:
             self.unit = self.product.default_uom
 
     def get_unit(self, name):
```

### Comparing `trytond_stock_supply-6.6.3/order_point.xml` & `trytond_stock_supply-6.8.0/order_point.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/product.py` & `trytond_stock_supply-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/product.xml` & `trytond_stock_supply-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/purchase_request.py` & `trytond_stock_supply-6.8.0/purchase_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,24 @@
 # this repository contains the full copyright notices and license terms.
 import datetime
 import operator
 from collections import defaultdict
 
 from trytond.model import ModelSQL, ValueMixin, fields
 from trytond.pool import Pool, PoolMeta
+from trytond.pyson import TimeDelta
 from trytond.tools import grouped_slice
 from trytond.transaction import Transaction
 
-supply_period = fields.TimeDelta("Supply Period")
+supply_period = fields.TimeDelta(
+    "Supply Period",
+    domain=['OR',
+        ('supply_period', '=', None),
+        ('supply_period', '>=', TimeDelta()),
+        ])
 
 
 class PurchaseConfiguration(metaclass=PoolMeta):
     __name__ = 'purchase.configuration'
     supply_period = fields.MultiValue(supply_period)
```

### Comparing `trytond_stock_supply-6.6.3/purchase_request.xml` & `trytond_stock_supply-6.8.0/purchase_request.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/setup.py` & `trytond_stock_supply-6.8.0/setup.py`

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
@@ -34,37 +31,40 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_supply'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-sql']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module for stock supply',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/stock_supply',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock supply',
     package_dir={'trytond.modules.stock_supply': '.'},
     packages=(
         ['trytond.modules.stock_supply']
         + ['trytond.modules.stock_supply.%s' % p for p in find_packages()]
         ),
@@ -101,23 +101,23 @@
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

### Comparing `trytond_stock_supply-6.6.3/shipment.py` & `trytond_stock_supply-6.8.0/shipment.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/stock.py` & `trytond_stock_supply-6.8.0/stock.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from trytond.i18n import gettext
 from trytond.model import ModelView, fields
 from trytond.pool import Pool
-from trytond.transaction import Transaction
+from trytond.transaction import check_access
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
 from .exceptions import SupplyWarning
 
 
 class Supply(Wizard):
@@ -38,15 +38,15 @@
     def transition_create_(self):
         pool = Pool()
         Move = pool.get('stock.move')
         ShipmentInternal = pool.get('stock.shipment.internal')
         Date = pool.get('ir.date')
         Warning = pool.get('res.user.warning')
         today = Date.today()
-        with Transaction().set_context(_check_access=True):
+        with check_access():
             if Move.search([
                         ('from_location.type', '=', 'supplier'),
                         ('to_location.type', '=', 'storage'),
                         ('state', '=', 'draft'),
                         ('planned_date', '<', today),
                         ], order=[]):
                 name = '%s.supplier@%s' % (self.__name__, today)
@@ -69,15 +69,15 @@
         while created or first:
             created = False
             for type_ in self.types():
                 created |= bool(getattr(self, 'generate_%s' % type_)(first))
             first = False
 
         # Remove transit split of request
-        with Transaction().set_context(_check_access=True):
+        with check_access():
             shipments = ShipmentInternal.search([
                     ('state', '=', 'request'),
                     ])
         Move.delete([m for s in shipments for m in s.moves
                 if m.from_location == s.transit_location])
         for shipment in shipments:
             Move.write([m for m in shipment.moves], {
```

### Comparing `trytond_stock_supply-6.6.3/stock.xml` & `trytond_stock_supply-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/tests/scenario_stock_internal_supply.rst` & `trytond_stock_supply-6.8.0/tests/scenario_stock_internal_supply.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 ===========================
 Stock Shipment Out Scenario
 ===========================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_supply')
 
 Create company::
```

### Comparing `trytond_stock_supply-6.6.3/tests/scenario_stock_internal_supply_lead_time.rst` & `trytond_stock_supply-6.8.0/tests/scenario_stock_internal_supply_lead_time.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ========================================
 Stock Internal Supply Lead Time Scenario
 ========================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
-    >>> tomorrow = today + relativedelta(days=1)
+
+    >>> today = dt.date.today()
+    >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock_supply')
 
 Create customer::
 
@@ -57,15 +57,15 @@
 
 Add lead time between warehouses::
 
     >>> LeadTime = Model.get('stock.location.lead_time')
     >>> lead_time = LeadTime()
     >>> lead_time.warehouse_from = warehouse_loc
     >>> lead_time.warehouse_to = sec_warehouse_loc
-    >>> lead_time.lead_time = datetime.timedelta(1)
+    >>> lead_time.lead_time = dt.timedelta(1)
     >>> lead_time.save()
 
 Create internal order point::
 
     >>> OrderPoint = Model.get('stock.order_point')
     >>> order_point = OrderPoint()
     >>> order_point.product = product
```

### Comparing `trytond_stock_supply-6.6.3/tests/scenario_stock_internal_supply_overflow.rst` & `trytond_stock_supply-6.8.0/tests/scenario_stock_internal_supply_overflow.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 ====================================================
 Stock supply scenario: Internal supply with overflow
 ====================================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_supply')
 
 Create company::
```

### Comparing `trytond_stock_supply-6.6.3/tests/scenario_stock_supply_purchase_request.rst` & `trytond_stock_supply-6.8.0/tests/scenario_stock_supply_purchase_request.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 =========================
 Purchase Request Scenario
 =========================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import (create_chart,
     ...     get_accounts)
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_supply')
 
 Create company::
 
@@ -38,15 +39,15 @@
     >>> supplier = Party(name='Supplier')
     >>> supplier.save()
 
 Configure supply period::
 
     >>> PurchaseConfig = Model.get('purchase.configuration')
     >>> purchase_config = PurchaseConfig(1)
-    >>> purchase_config.supply_period = datetime.timedelta(days=30)
+    >>> purchase_config.supply_period = dt.timedelta(days=30)
     >>> purchase_config.save()
 
 Create stock admin user::
 
     >>> User = Model.get('res.user')
     >>> Group = Model.get('res.group')
     >>> stock_admin_user = User()
@@ -116,15 +117,15 @@
 
 Define a product supplier::
 
     >>> set_user(purchase_user)
     >>> ProductSupplier = Model.get('purchase.product_supplier')
     >>> product_supplier = ProductSupplier(template=template)
     >>> product_supplier.party = supplier
-    >>> product_supplier.lead_time = datetime.timedelta(days=1)
+    >>> product_supplier.lead_time = dt.timedelta(days=1)
     >>> product_supplier.save()
 
 Get stock locations::
 
     >>> set_user(stock_admin_user)
     >>> Location = Model.get('stock.location')
     >>> warehouse_loc, = Location.find([('code', '=', 'WH')])
@@ -151,15 +152,15 @@
     >>> move.to_location = customer_loc
     >>> move.company = company
     >>> move.unit_price = Decimal('1')
     >>> move.currency = company.currency
     >>> shipment_out.click('wait')
 
     >>> shipment_out, = shipment_out.duplicate(
-    ...     default={'planned_date': today + datetime.timedelta(days=10)})
+    ...     default={'planned_date': today + dt.timedelta(days=10)})
     >>> shipment_out.click('wait')
 
 There is no purchase request::
 
     >>> PurchaseRequest = Model.get('purchase.request')
     >>> set_user(purchase_user)
     >>> PurchaseRequest.find([])
```

### Comparing `trytond_stock_supply-6.6.3/tests/test_module.py` & `trytond_stock_supply-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/trytond_stock_supply.egg-info/PKG-INFO` & `trytond_stock_supply-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
-Name: trytond-stock-supply
-Version: 6.6.3
+Name: trytond_stock_supply
+Version: 6.8.0
 Summary: Tryton module for stock supply
 Home-page: http://www.tryton.org/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_supply
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock supply
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
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
 
 Stock Supply Module
 ###################
 
 The Stock Supply module add automatic supply mechanisms and introduce
@@ -64,15 +64,15 @@
 An order point define minimum, maximum and target quantities for a product on a
 location.
 
 * The minimum quantity is the threshold quantity below which the provisioning
   process will be triggered.
 
 * The maximum quantity is the threshold quantity above which the overflowing
-  process will be triggered. 
+  process will be triggered.
 
 * The target quantity is the quantity that will be found in the location after
   the provisioning / overflowing process has been completed.
 
 An order point also define a type which can be:
 
 * Internal
```

### Comparing `trytond_stock_supply-6.6.3/trytond_stock_supply.egg-info/SOURCES.txt` & `trytond_stock_supply-6.8.0/trytond_stock_supply.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-6.6.3/view/order_point_form.xml` & `trytond_stock_supply-6.8.0/view/order_point_form.xml`

 * *Files identical despite different names*

