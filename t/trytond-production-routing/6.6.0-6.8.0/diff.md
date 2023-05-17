# Comparing `tmp/trytond_production_routing-6.6.0.tar.gz` & `tmp/trytond_production_routing-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_production_routing-6.6.0.tar", last modified: Mon Oct 31 16:28:59 2022, max compression
+gzip compressed data, was "trytond_production_routing-6.8.0.tar", last modified: Mon May  1 11:39:26 2023, max compression
```

## Comparing `trytond_production_routing-6.6.0.tar` & `trytond_production_routing-6.8.0.tar`

### file list

```diff
@@ -1,76 +1,73 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:59.176223 trytond_production_routing-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_production_routing-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_production_routing-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-31 16:28:57.000000 trytond_production_routing-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_production_routing-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1184 2022-10-31 16:28:57.000000 trytond_production_routing-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      721 2022-10-31 16:28:56.000000 trytond_production_routing-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_production_routing-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2672 2022-10-31 16:28:59.176223 trytond_production_routing-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2021-12-11 16:59:33.000000 trytond_production_routing-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:59.172890 trytond_production_routing-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:59.169556 trytond_production_routing-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1806 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1613 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1710 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1779 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1621 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1502 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1691 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1697 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1657 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1710 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1506 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1719 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1863 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1710 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1745 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1708 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1746 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1502 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1799 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1689 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1686 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1502 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1712 2022-10-29 07:50:33.000000 trytond_production_routing-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      749 2022-10-11 19:49:58.000000 trytond_production_routing-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2089 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1632 2022-04-10 15:40:35.000000 trytond_production_routing-6.6.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1650 2022-10-11 19:49:58.000000 trytond_production_routing-6.6.0/routing.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5490 2021-03-24 12:34:22.000000 trytond_production_routing-6.6.0/routing.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:28:59.176223 trytond_production_routing-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5293 2022-10-29 07:39:11.000000 trytond_production_routing-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:59.169556 trytond_production_routing-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_production_routing-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2200 2020-07-09 09:37:11.000000 trytond_production_routing-6.6.0/tests/scenario_stock_supply_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2022-04-16 16:30:57.000000 trytond_production_routing-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_production_routing-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2022-10-31 15:10:09.000000 trytond_production_routing-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      153 2022-10-31 16:28:55.000000 trytond_production_routing-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:59.176223 trytond_production_routing-6.6.0/trytond_production_routing.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2672 2022-10-31 16:28:58.000000 trytond_production_routing-6.6.0/trytond_production_routing.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2358 2022-10-31 16:28:59.000000 trytond_production_routing-6.6.0/trytond_production_routing.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:28:58.000000 trytond_production_routing-6.6.0/trytond_production_routing.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2022-10-31 16:28:58.000000 trytond_production_routing-6.6.0/trytond_production_routing.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:50.000000 trytond_production_routing-6.6.0/trytond_production_routing.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      131 2022-10-31 16:28:58.000000 trytond_production_routing-6.6.0/trytond_production_routing.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:28:58.000000 trytond_production_routing-6.6.0/trytond_production_routing.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:59.172890 trytond_production_routing-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/view/operation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2019-10-11 23:09:48.000000 trytond_production_routing-6.6.0/view/operation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/view/product_bom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/view/product_bom_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      324 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/view/production_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/view/production_lead_time_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/view/production_lead_time_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      311 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/view/production_lead_time_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/view/routing_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2019-10-11 23:09:48.000000 trytond_production_routing-6.6.0/view/routing_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2019-02-13 10:09:35.000000 trytond_production_routing-6.6.0/view/routing_step_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      266 2019-10-11 23:09:48.000000 trytond_production_routing-6.6.0/view/routing_step_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2019-10-11 23:09:48.000000 trytond_production_routing-6.6.0/view/routing_step_list_sequence.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:26.044132 trytond_production_routing-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1347 2023-05-01 10:59:44.000000 trytond_production_routing-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      721 2023-05-01 10:59:44.000000 trytond_production_routing-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production_routing-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2661 2023-05-01 11:39:26.044132 trytond_production_routing-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-01-16 14:00:21.000000 trytond_production_routing-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:26.040799 trytond_production_routing-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-01-16 14:00:21.000000 trytond_production_routing-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:26.037465 trytond_production_routing-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1806 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1613 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1710 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1779 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1621 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1502 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1691 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1697 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1710 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1506 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1719 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1863 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1710 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1708 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1746 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1502 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1799 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1689 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1686 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1502 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1712 2023-04-29 08:02:40.000000 trytond_production_routing-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      749 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2089 2023-01-16 14:00:21.000000 trytond_production_routing-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1632 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-01-16 14:00:20.000000 trytond_production_routing-6.8.0/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1650 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/routing.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5490 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/routing.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:39:26.044132 trytond_production_routing-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4479 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:26.037465 trytond_production_routing-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2200 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/tests/scenario_stock_supply_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      153 2023-05-01 10:59:39.000000 trytond_production_routing-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:26.044132 trytond_production_routing-6.8.0/trytond_production_routing.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2661 2023-05-01 11:39:25.000000 trytond_production_routing-6.8.0/trytond_production_routing.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2332 2023-05-01 11:39:25.000000 trytond_production_routing-6.8.0/trytond_production_routing.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:39:25.000000 trytond_production_routing-6.8.0/trytond_production_routing.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-05-01 11:39:25.000000 trytond_production_routing-6.8.0/trytond_production_routing.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_production_routing-6.8.0/trytond_production_routing.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      131 2023-05-01 11:39:25.000000 trytond_production_routing-6.8.0/trytond_production_routing.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:39:25.000000 trytond_production_routing-6.8.0/trytond_production_routing.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:26.040799 trytond_production_routing-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-30 10:46:36.000000 trytond_production_routing-6.8.0/view/operation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/view/operation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-01-16 14:00:21.000000 trytond_production_routing-6.8.0/view/product_bom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-01-16 14:00:21.000000 trytond_production_routing-6.8.0/view/product_bom_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-01-16 14:00:21.000000 trytond_production_routing-6.8.0/view/production_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-01-16 14:00:21.000000 trytond_production_routing-6.8.0/view/production_lead_time_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-01-16 14:00:21.000000 trytond_production_routing-6.8.0/view/production_lead_time_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-01-16 14:00:21.000000 trytond_production_routing-6.8.0/view/production_lead_time_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-01-16 14:00:21.000000 trytond_production_routing-6.8.0/view/routing_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/view/routing_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:21.000000 trytond_production_routing-6.8.0/view/routing_step_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/view/routing_step_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-04-15 07:12:15.000000 trytond_production_routing-6.8.0/view/routing_step_list_sequence.xml
```

### Comparing `trytond_production_routing-6.6.0/CHANGELOG` & `trytond_production_routing-6.8.0/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.10
```

### Comparing `trytond_production_routing-6.6.0/COPYRIGHT` & `trytond_production_routing-6.8.0/COPYRIGHT`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2015-2022 Cédric Krier.
-Copyright (C) 2015-2022 B2CK SPRL.
+Copyright (C) 2015-2023 Cédric Krier.
+Copyright (C) 2015-2023 B2CK SPRL.
 Copyright (C) 2013-2015 NaN·tic.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_production_routing-6.6.0/LICENSE` & `trytond_production_routing-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/PKG-INFO` & `trytond_production_routing-6.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_production_routing
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for production routing
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
-Project-URL: Source Code, https://hg.tryton.org/modules/production_routing
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton production routing
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
 
 Production Routing Module
 #########################
 
 The production routing module defines the routings for production: Routing,
```

### Comparing `trytond_production_routing-6.6.0/__init__.py` & `trytond_production_routing-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/bg.po` & `trytond_production_routing-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/ca.po` & `trytond_production_routing-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/cs.po` & `trytond_production_routing-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/de.po` & `trytond_production_routing-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/es.po` & `trytond_production_routing-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/es_419.po` & `trytond_production_routing-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/et.po` & `trytond_production_routing-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/fa.po` & `trytond_production_routing-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/fi.po` & `trytond_production_routing-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/fr.po` & `trytond_production_routing-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/hu.po` & `trytond_production_routing-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/id.po` & `trytond_production_routing-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/it.po` & `trytond_production_routing-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/lo.po` & `trytond_production_routing-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/lt.po` & `trytond_production_routing-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/nl.po` & `trytond_production_routing-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/pl.po` & `trytond_production_routing-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/pt.po` & `trytond_production_routing-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/ro.po` & `trytond_production_routing-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/ru.po` & `trytond_production_routing-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/sl.po` & `trytond_production_routing-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/tr.po` & `trytond_production_routing-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/uk.po` & `trytond_production_routing-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/locale/zh_CN.po` & `trytond_production_routing-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/product.py` & `trytond_production_routing-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/product.xml` & `trytond_production_routing-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/production.py` & `trytond_production_routing-6.8.0/production.py`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/routing.py` & `trytond_production_routing-6.8.0/routing.py`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/routing.xml` & `trytond_production_routing-6.8.0/routing.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/setup.py` & `trytond_production_routing-6.8.0/setup.py`

 * *Files 13% similar despite different names*

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
@@ -34,63 +31,44 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_production_routing'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
 if minor_version % 2:
-    version = '%s.%s.dev0' % (major_version, minor_version)
-    download_url = (
-        'hg+http://hg.tryton.org/modules/%s#egg=%s-%s' % (
-            name[8:], name, version))
-local_version = []
-if os.environ.get('CI_JOB_ID'):
-    local_version.append(os.environ['CI_JOB_ID'])
+    download_url = ''
 else:
-    for build in ['CI_BUILD_NUMBER', 'CI_JOB_NUMBER']:
-        if os.environ.get(build):
-            local_version.append(os.environ[build])
-        else:
-            local_version = []
-            break
-if local_version:
-    version += '+' + '.'.join(local_version)
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-sql >= 0.4']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
     get_require_version('proteus'),
     get_require_version('trytond_stock_supply_production'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for production routing',
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
-        "Source Code": 'https://hg.tryton.org/modules/production_routing',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton production routing',
     package_dir={'trytond.modules.production_routing': '.'},
     packages=(
         ['trytond.modules.production_routing']
         + ['trytond.modules.production_routing.%s' % p
             for p in find_packages()]
@@ -128,27 +106,26 @@
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
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     production_routing = trytond.modules.production_routing
     """,
     )
```

### Comparing `trytond_production_routing-6.6.0/tests/scenario_stock_supply_production.rst` & `trytond_production_routing-6.8.0/tests/scenario_stock_supply_production.rst`

 * *Files identical despite different names*

### Comparing `trytond_production_routing-6.6.0/trytond_production_routing.egg-info/PKG-INFO` & `trytond_production_routing-6.8.0/trytond_production_routing.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-production-routing
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for production routing
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
-Project-URL: Source Code, https://hg.tryton.org/modules/production_routing
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton production routing
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
 
 Production Routing Module
 #########################
 
 The production routing module defines the routings for production: Routing,
```

### Comparing `trytond_production_routing-6.6.0/trytond_production_routing.egg-info/SOURCES.txt` & `trytond_production_routing-6.8.0/trytond_production_routing.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-.drone.yml
-.flake8
-.hgtags
-.isort.cfg
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 product.py
@@ -62,14 +58,15 @@
 ./view/production_lead_time_list.xml
 ./view/production_lead_time_list_sequence.xml
 ./view/routing_form.xml
 ./view/routing_list.xml
 ./view/routing_step_form.xml
 ./view/routing_step_list.xml
 ./view/routing_step_list_sequence.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_production_routing-6.6.0/view/routing_form.xml` & `trytond_production_routing-6.8.0/view/routing_form.xml`

 * *Files identical despite different names*

