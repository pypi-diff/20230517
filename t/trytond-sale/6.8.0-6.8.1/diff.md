# Comparing `tmp/trytond_sale-6.8.0.tar.gz` & `tmp/trytond_sale-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale-6.8.0.tar", last modified: Mon May  1 12:01:27 2023, max compression
+gzip compressed data, was "trytond_sale-6.8.1.tar", last modified: Wed May 17 20:47:33 2023, max compression
```

## Comparing `trytond_sale-6.8.0.tar` & `trytond_sale-6.8.1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.907202 trytond_sale-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     6223 2023-05-01 11:14:41.000000 trytond_sale-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-01 11:14:41.000000 trytond_sale-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2664 2023-05-01 12:01:27.907202 trytond_sale-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2345 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5173 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2425 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.900536 trytond_sale-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9118 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.903869 trytond_sale-6.8.0/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1985 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/usage/presales.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4006 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/usage/reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1618 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/doc/usage/returns.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.903869 trytond_sale-6.8.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-01-16 14:00:21.000000 trytond_sale-6.8.0/icons/tryton-sale.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5255 2023-04-21 08:36:08.000000 trytond_sale-6.8.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1800 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.890535 trytond_sale-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    42111 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42743 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37074 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    43431 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42922 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35457 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40621 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    45323 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37035 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    43294 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41625 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38328 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39740 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41170 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41661 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42791 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38642 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39960 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    43083 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42203 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39643 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37026 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34909 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37290 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4405 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4574 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3022 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9820 2023-04-21 08:36:08.000000 trytond_sale-6.8.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2671 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    76266 2023-04-28 07:46:16.000000 trytond_sale-6.8.0/sale.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    81894 2023-04-30 10:46:36.000000 trytond_sale-6.8.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24722 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    39881 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/sale_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    56250 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/sale_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:01:27.907202 trytond_sale-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4515 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7402 2023-04-21 08:36:08.000000 trytond_sale-6.8.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3013 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.893869 trytond_sale-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20162 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/scenario_sale.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/scenario_sale_default_methods.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/scenario_sale_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2969 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/scenario_sale_modify_header.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    12999 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/scenario_sale_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2526 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-05-01 11:14:35.000000 trytond_sale-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.907202 trytond_sale-6.8.0/trytond_sale.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2664 2023-05-01 12:01:27.000000 trytond_sale-6.8.0/trytond_sale.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4921 2023-05-01 12:01:27.000000 trytond_sale-6.8.0/trytond_sale.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:01:27.000000 trytond_sale-6.8.0/trytond_sale.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2023-05-01 12:01:27.000000 trytond_sale-6.8.0/trytond_sale.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_sale-6.8.0/trytond_sale.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-05-01 12:01:27.000000 trytond_sale-6.8.0/trytond_sale.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:01:27.000000 trytond_sale-6.8.0/trytond_sale.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:27.900536 trytond_sale-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-01-16 14:00:21.000000 trytond_sale-6.8.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/handle_invoice_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/handle_shipment_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-01-16 14:00:21.000000 trytond_sale-6.8.0/view/modify_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      844 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/product_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/product_list_sale_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/product_sale_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/return_sale_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3721 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1554 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_country_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_customer_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_customer_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_customer_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_customer_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_customer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_main_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-04-28 07:46:16.000000 trytond_sale-6.8.0/view/sale_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_main_time_series_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-28 07:46:16.000000 trytond_sale-6.8.0/view/sale_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_product_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_product_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_product_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_product_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_reporting_region_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/sale_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      935 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_sale-6.8.0/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:33.140392 trytond_sale-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6324 2023-05-17 20:47:30.000000 trytond_sale-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-17 20:47:29.000000 trytond_sale-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2664 2023-05-17 20:47:33.140392 trytond_sale-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2345 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5173 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2425 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:33.127058 trytond_sale-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9118 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:33.130392 trytond_sale-6.8.1/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1985 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/doc/usage/presales.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4006 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/doc/usage/process.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      726 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/doc/usage/reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1618 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/doc/usage/returns.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:33.133725 trytond_sale-6.8.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/icons/tryton-sale.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5255 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1800 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:33.080391 trytond_sale-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    42111 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42743 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37074 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43431 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42922 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35457 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40621 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    45323 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37035 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43294 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41625 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38328 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39740 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41170 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41661 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42791 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38642 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39960 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43083 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42203 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39643 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37026 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34909 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37290 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4405 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4574 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3022 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9820 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2671 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    76266 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/sale.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    81865 2023-05-13 22:06:18.000000 trytond_sale-6.8.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24722 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    39881 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/sale_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    56250 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/sale_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-17 20:47:33.140392 trytond_sale-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4515 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7402 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3013 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:33.087058 trytond_sale-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20162 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/tests/scenario_sale.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/tests/scenario_sale_default_methods.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/tests/scenario_sale_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2969 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/tests/scenario_sale_modify_header.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    12999 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/tests/scenario_sale_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2526 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-05-01 12:18:02.000000 trytond_sale-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:33.137059 trytond_sale-6.8.1/trytond_sale.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2664 2023-05-17 20:47:32.000000 trytond_sale-6.8.1/trytond_sale.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4921 2023-05-17 20:47:32.000000 trytond_sale-6.8.1/trytond_sale.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:47:32.000000 trytond_sale-6.8.1/trytond_sale.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       46 2023-05-17 20:47:32.000000 trytond_sale-6.8.1/trytond_sale.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:47:32.000000 trytond_sale-6.8.1/trytond_sale.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-05-17 20:47:32.000000 trytond_sale-6.8.1/trytond_sale.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-17 20:47:32.000000 trytond_sale-6.8.1/trytond_sale.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:47:33.123725 trytond_sale-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/handle_invoice_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/handle_shipment_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/modify_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      844 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/product_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/product_list_sale_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/product_sale_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/return_sale_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3721 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1554 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_country_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_customer_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_customer_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_customer_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_customer_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_customer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_main_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_main_time_series_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_product_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_product_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_product_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_product_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_reporting_region_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/sale_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      935 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-05-01 12:17:31.000000 trytond_sale-6.8.1/view/template_tree.xml
```

### Comparing `trytond_sale-6.8.0/CHANGELOG` & `trytond_sale-6.8.1/CHANGELOG`

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

### Comparing `trytond_sale-6.8.0/COPYRIGHT` & `trytond_sale-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/LICENSE` & `trytond_sale-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/PKG-INFO` & `trytond_sale-6.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for sale
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale-6.8.0/__init__.py` & `trytond_sale-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/configuration.py` & `trytond_sale-6.8.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/configuration.xml` & `trytond_sale-6.8.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/doc/conf.py` & `trytond_sale-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/doc/design.rst` & `trytond_sale-6.8.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/doc/usage/presales.rst` & `trytond_sale-6.8.1/doc/usage/presales.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/doc/usage/process.rst` & `trytond_sale-6.8.1/doc/usage/process.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/doc/usage/reporting.rst` & `trytond_sale-6.8.1/doc/usage/reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/doc/usage/returns.rst` & `trytond_sale-6.8.1/doc/usage/returns.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/icons/LICENSE` & `trytond_sale-6.8.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/invoice.py` & `trytond_sale-6.8.1/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/invoice.xml` & `trytond_sale-6.8.1/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/bg.po` & `trytond_sale-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/ca.po` & `trytond_sale-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/cs.po` & `trytond_sale-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/de.po` & `trytond_sale-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/es.po` & `trytond_sale-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/es_419.po` & `trytond_sale-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/et.po` & `trytond_sale-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/fa.po` & `trytond_sale-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/fi.po` & `trytond_sale-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/fr.po` & `trytond_sale-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/hu.po` & `trytond_sale-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/id.po` & `trytond_sale-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/it.po` & `trytond_sale-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/lo.po` & `trytond_sale-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/lt.po` & `trytond_sale-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/nl.po` & `trytond_sale-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/pl.po` & `trytond_sale-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/pt.po` & `trytond_sale-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/ro.po` & `trytond_sale-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/ru.po` & `trytond_sale-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/sl.po` & `trytond_sale-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/tr.po` & `trytond_sale-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/uk.po` & `trytond_sale-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/locale/zh_CN.po` & `trytond_sale-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/message.xml` & `trytond_sale-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/party.py` & `trytond_sale-6.8.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/party.xml` & `trytond_sale-6.8.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/product.py` & `trytond_sale-6.8.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/product.xml` & `trytond_sale-6.8.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/sale.fodt` & `trytond_sale-6.8.1/sale.fodt`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/sale.py` & `trytond_sale-6.8.1/sale.py`

 * *Files 0% similar despite different names*

```diff
@@ -852,15 +852,15 @@
             company=self.company,
             type='out',
             party=party,
             invoice_address=self.invoice_address,
             currency=self.currency,
             account=party.account_receivable_used,
             )
-        invoice.journal = invoice.on_change_with_journal()
+        invoice.set_journal()
         invoice.payment_term = self.payment_term
         return invoice
 
     def create_invoice(self):
         'Create and return an invoice'
         if self.invoice_method == 'manual':
             return
```

### Comparing `trytond_sale-6.8.0/sale.xml` & `trytond_sale-6.8.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/sale_reporting.py` & `trytond_sale-6.8.1/sale_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/sale_reporting.xml` & `trytond_sale-6.8.1/sale_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/setup.py` & `trytond_sale-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/stock.py` & `trytond_sale-6.8.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/stock.xml` & `trytond_sale-6.8.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/tests/scenario_sale.rst` & `trytond_sale-6.8.1/tests/scenario_sale.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/tests/scenario_sale_default_methods.rst` & `trytond_sale-6.8.1/tests/scenario_sale_default_methods.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/tests/scenario_sale_empty.rst` & `trytond_sale-6.8.1/tests/scenario_sale_empty.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/tests/scenario_sale_modify_header.rst` & `trytond_sale-6.8.1/tests/scenario_sale_modify_header.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/tests/scenario_sale_reporting.rst` & `trytond_sale-6.8.1/tests/scenario_sale_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/tests/test_module.py` & `trytond_sale-6.8.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/tox.ini` & `trytond_sale-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/trytond_sale.egg-info/PKG-INFO` & `trytond_sale-6.8.1/trytond_sale.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-sale
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for sale
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale-6.8.0/trytond_sale.egg-info/SOURCES.txt` & `trytond_sale-6.8.1/trytond_sale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/view/configuration_form.xml` & `trytond_sale-6.8.1/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/view/party_form.xml` & `trytond_sale-6.8.1/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/view/product_list_sale_line.xml` & `trytond_sale-6.8.1/view/product_list_sale_line.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/view/product_sale_context_form.xml` & `trytond_sale-6.8.1/view/product_sale_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/view/sale_form.xml` & `trytond_sale-6.8.1/view/sale_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/view/sale_line_form.xml` & `trytond_sale-6.8.1/view/sale_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/view/sale_line_tree.xml` & `trytond_sale-6.8.1/view/sale_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/view/sale_line_tree_sequence.xml` & `trytond_sale-6.8.1/view/sale_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/view/sale_reporting_context_form.xml` & `trytond_sale-6.8.1/view/sale_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/view/sale_reporting_customer_category_list.xml` & `trytond_sale-6.8.1/view/sale_reporting_customer_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/view/sale_reporting_product_category_list.xml` & `trytond_sale-6.8.1/view/sale_reporting_product_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/view/sale_tree.xml` & `trytond_sale-6.8.1/view/sale_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-6.8.0/view/template_form.xml` & `trytond_sale-6.8.1/view/template_form.xml`

 * *Files identical despite different names*

