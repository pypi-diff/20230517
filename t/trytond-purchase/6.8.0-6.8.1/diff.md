# Comparing `tmp/trytond_purchase-6.8.0.tar.gz` & `tmp/trytond_purchase-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase-6.8.0.tar", last modified: Mon May  1 11:45:48 2023, max compression
+gzip compressed data, was "trytond_purchase-6.8.1.tar", last modified: Wed May 17 20:47:59 2023, max compression
```

## Comparing `trytond_purchase-6.8.0.tar` & `trytond_purchase-6.8.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.248875 trytond_purchase-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     6583 2023-05-01 11:03:55.000000 trytond_purchase-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-01 11:03:55.000000 trytond_purchase-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2736 2023-05-01 11:45:48.245541 trytond_purchase-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1909 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4832 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2554 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.242208 trytond_purchase-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7482 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.242208 trytond_purchase-6.8.0/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      208 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2000 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/usage/prepurchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4855 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2027 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/doc/usage/returns.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.242208 trytond_purchase-6.8.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-01-16 14:00:21.000000 trytond_purchase-6.8.0/icons/tryton-purchase.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5622 2023-04-21 08:36:08.000000 trytond_purchase-6.8.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1761 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.232208 trytond_purchase-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    37471 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37513 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32682 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38008 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37693 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32179 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34342 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39508 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32669 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37860 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36612 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33346 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35879 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37467 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35472 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37911 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33939 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35630 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31956 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37996 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35318 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32660 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30987 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35757 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4104 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3677 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    19452 2023-04-21 08:36:08.000000 trytond_purchase-6.8.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    73107 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/purchase.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    82990 2023-04-30 10:46:36.000000 trytond_purchase-6.8.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    32163 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11720 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/purchase_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24226 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/purchase_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:45:48.248875 trytond_purchase-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4536 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9634 2023-04-21 08:36:08.000000 trytond_purchase-6.8.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4823 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.235541 trytond_purchase-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19171 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/scenario_purchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1676 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/scenario_purchase_copy_product_suppliers.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1332 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/scenario_purchase_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3009 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/scenario_purchase_modify_header.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5192 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/scenario_purchase_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3025 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/scenario_purchase_return_wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4771 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-05-01 11:03:49.000000 trytond_purchase-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.245541 trytond_purchase-6.8.0/trytond_purchase.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2736 2023-05-01 11:45:47.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4760 2023-05-01 11:45:48.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:45:47.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2023-05-01 11:45:47.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-05-01 11:45:47.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:45:47.000000 trytond_purchase-6.8.0/trytond_purchase.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:48.238875 trytond_purchase-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-01-16 14:00:21.000000 trytond_purchase-6.8.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/handle_invoice_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/handle_shipment_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-01-16 14:00:21.000000 trytond_purchase-6.8.0/view/modify_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/move_list_shipment_in.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-01-16 14:00:21.000000 trytond_purchase-6.8.0/view/product_list_purchase_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1048 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/product_supplier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/product_supplier_price_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/product_supplier_price_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/product_supplier_price_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/product_supplier_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/product_supplier_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3481 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1818 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      741 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      544 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_main_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-04-28 07:46:16.000000 trytond_purchase-6.8.0/view/purchase_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_main_time_series_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-28 07:46:16.000000 trytond_purchase-6.8.0/view/purchase_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_reporting_supplier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/purchase_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/return_purchase_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-15 07:12:15.000000 trytond_purchase-6.8.0/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.527377 trytond_purchase-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6684 2023-05-17 20:47:56.000000 trytond_purchase-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-17 20:47:55.000000 trytond_purchase-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2736 2023-05-17 20:47:59.527377 trytond_purchase-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1909 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4832 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2554 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.507377 trytond_purchase-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7482 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.514043 trytond_purchase-6.8.1/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      208 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2000 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/usage/prepurchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4855 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/usage/process.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2027 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/doc/usage/returns.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.514043 trytond_purchase-6.8.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/icons/tryton-purchase.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5622 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1761 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.397375 trytond_purchase-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    37471 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37513 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32682 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38008 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37693 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32179 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34342 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39508 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32669 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37860 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36612 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33346 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35879 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37467 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35472 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37911 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33939 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35630 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31956 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37996 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35318 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32660 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    30987 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35757 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4104 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3677 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    19452 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    73107 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/purchase.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    82961 2023-05-13 22:06:18.000000 trytond_purchase-6.8.1/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    32163 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11720 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/purchase_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24226 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/purchase_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-17 20:47:59.527377 trytond_purchase-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4536 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9634 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4823 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.424042 trytond_purchase-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19171 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/scenario_purchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1676 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/scenario_purchase_copy_product_suppliers.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1332 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/scenario_purchase_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3009 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/scenario_purchase_modify_header.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5192 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/scenario_purchase_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3025 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/scenario_purchase_return_wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4771 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-05-01 12:18:02.000000 trytond_purchase-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.524043 trytond_purchase-6.8.1/trytond_purchase.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2736 2023-05-17 20:47:58.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4760 2023-05-17 20:47:59.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:47:58.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2023-05-17 20:47:58.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:47:58.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-05-17 20:47:58.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-17 20:47:58.000000 trytond_purchase-6.8.1/trytond_purchase.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:59.504043 trytond_purchase-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/handle_invoice_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/handle_shipment_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/modify_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/move_list_shipment_in.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_list_purchase_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1048 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_supplier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_supplier_price_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_supplier_price_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_supplier_price_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_supplier_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/product_supplier_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3481 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1818 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      741 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      544 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_main_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_main_time_series_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_reporting_supplier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/purchase_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/return_purchase_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-05-01 12:17:31.000000 trytond_purchase-6.8.1/view/template_tree.xml
```

### Comparing `trytond_purchase-6.8.0/CHANGELOG` & `trytond_purchase-6.8.1/CHANGELOG`

 * *Files 2% similar despite different names*

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
 * Fill taxes from default account for line without product
 * Add partially shipped to shipment state
 * Add pending, awaiting payment and partially paid to invoice state
 * Remove support for Python 3.7
```

### Comparing `trytond_purchase-6.8.0/COPYRIGHT` & `trytond_purchase-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/LICENSE` & `trytond_purchase-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/PKG-INFO` & `trytond_purchase-6.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase-6.8.0/__init__.py` & `trytond_purchase-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/configuration.py` & `trytond_purchase-6.8.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/configuration.xml` & `trytond_purchase-6.8.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/doc/conf.py` & `trytond_purchase-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/doc/design.rst` & `trytond_purchase-6.8.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/doc/usage/prepurchase.rst` & `trytond_purchase-6.8.1/doc/usage/prepurchase.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/doc/usage/process.rst` & `trytond_purchase-6.8.1/doc/usage/process.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/doc/usage/returns.rst` & `trytond_purchase-6.8.1/doc/usage/returns.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/icons/LICENSE` & `trytond_purchase-6.8.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/invoice.py` & `trytond_purchase-6.8.1/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/invoice.xml` & `trytond_purchase-6.8.1/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/bg.po` & `trytond_purchase-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/ca.po` & `trytond_purchase-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/cs.po` & `trytond_purchase-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/de.po` & `trytond_purchase-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/es.po` & `trytond_purchase-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/es_419.po` & `trytond_purchase-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/et.po` & `trytond_purchase-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/fa.po` & `trytond_purchase-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/fi.po` & `trytond_purchase-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/fr.po` & `trytond_purchase-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/hu.po` & `trytond_purchase-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/id.po` & `trytond_purchase-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/it.po` & `trytond_purchase-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/lo.po` & `trytond_purchase-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/lt.po` & `trytond_purchase-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/nl.po` & `trytond_purchase-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/pl.po` & `trytond_purchase-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/pt.po` & `trytond_purchase-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/ro.po` & `trytond_purchase-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/ru.po` & `trytond_purchase-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/sl.po` & `trytond_purchase-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/tr.po` & `trytond_purchase-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/uk.po` & `trytond_purchase-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/locale/zh_CN.po` & `trytond_purchase-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/message.xml` & `trytond_purchase-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/party.py` & `trytond_purchase-6.8.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/party.xml` & `trytond_purchase-6.8.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/product.py` & `trytond_purchase-6.8.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/product.xml` & `trytond_purchase-6.8.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/purchase.fodt` & `trytond_purchase-6.8.1/purchase.fodt`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/purchase.py` & `trytond_purchase-6.8.1/purchase.py`

 * *Files 0% similar despite different names*

```diff
@@ -797,15 +797,15 @@
             type='in',
             party=party,
             invoice_address=self.invoice_address,
             currency=self.currency,
             account=party.account_payable_used,
             payment_term=self.payment_term,
             )
-        invoice.journal = invoice.on_change_with_journal()
+        invoice.set_journal()
         return invoice
 
     def create_invoice(self):
         'Create an invoice for the purchase and return it'
 
         if self.invoice_method == 'manual':
             return
```

### Comparing `trytond_purchase-6.8.0/purchase.xml` & `trytond_purchase-6.8.1/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/purchase_reporting.py` & `trytond_purchase-6.8.1/purchase_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/purchase_reporting.xml` & `trytond_purchase-6.8.1/purchase_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/setup.py` & `trytond_purchase-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/stock.py` & `trytond_purchase-6.8.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/stock.xml` & `trytond_purchase-6.8.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/tests/scenario_purchase.rst` & `trytond_purchase-6.8.1/tests/scenario_purchase.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/tests/scenario_purchase_copy_product_suppliers.rst` & `trytond_purchase-6.8.1/tests/scenario_purchase_copy_product_suppliers.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/tests/scenario_purchase_empty.rst` & `trytond_purchase-6.8.1/tests/scenario_purchase_empty.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/tests/scenario_purchase_modify_header.rst` & `trytond_purchase-6.8.1/tests/scenario_purchase_modify_header.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/tests/scenario_purchase_reporting.rst` & `trytond_purchase-6.8.1/tests/scenario_purchase_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/tests/scenario_purchase_return_wizard.rst` & `trytond_purchase-6.8.1/tests/scenario_purchase_return_wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/tests/test_module.py` & `trytond_purchase-6.8.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/tox.ini` & `trytond_purchase-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/trytond_purchase.egg-info/PKG-INFO` & `trytond_purchase-6.8.1/trytond_purchase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-purchase
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase-6.8.0/trytond_purchase.egg-info/SOURCES.txt` & `trytond_purchase-6.8.1/trytond_purchase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/view/party_form.xml` & `trytond_purchase-6.8.1/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/view/product_supplier_form.xml` & `trytond_purchase-6.8.1/view/product_supplier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/view/purchase_form.xml` & `trytond_purchase-6.8.1/view/purchase_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/view/purchase_line_form.xml` & `trytond_purchase-6.8.1/view/purchase_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/view/purchase_line_tree.xml` & `trytond_purchase-6.8.1/view/purchase_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/view/purchase_line_tree_sequence.xml` & `trytond_purchase-6.8.1/view/purchase_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/view/purchase_reporting_context_form.xml` & `trytond_purchase-6.8.1/view/purchase_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/view/purchase_tree.xml` & `trytond_purchase-6.8.1/view/purchase_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-6.8.0/view/template_form.xml` & `trytond_purchase-6.8.1/view/template_form.xml`

 * *Files identical despite different names*

