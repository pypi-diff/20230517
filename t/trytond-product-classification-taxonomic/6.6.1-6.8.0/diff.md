# Comparing `tmp/trytond_product_classification_taxonomic-6.6.1.tar.gz` & `tmp/trytond_product_classification_taxonomic-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_classification_taxonomic-6.6.1.tar", last modified: Wed May 17 20:51:16 2023, max compression
+gzip compressed data, was "trytond_product_classification_taxonomic-6.8.0.tar", last modified: Mon May  1 11:54:09 2023, max compression
```

## Comparing `trytond_product_classification_taxonomic-6.6.1.tar` & `trytond_product_classification_taxonomic-6.8.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:51:16.456417 trytond_product_classification_taxonomic-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-05-17 20:51:13.000000 trytond_product_classification_taxonomic-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-17 20:51:13.000000 trytond_product_classification_taxonomic-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-13 16:52:41.000000 trytond_product_classification_taxonomic-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2752 2023-05-17 20:51:16.456417 trytond_product_classification_taxonomic-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      588 2022-12-19 12:02:49.000000 trytond_product_classification_taxonomic-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-13 16:52:41.000000 trytond_product_classification_taxonomic-6.6.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:51:16.456417 trytond_product_classification_taxonomic-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2023-04-08 09:35:50.000000 trytond_product_classification_taxonomic-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      588 2022-12-19 12:02:49.000000 trytond_product_classification_taxonomic-6.6.1/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:51:16.449751 trytond_product_classification_taxonomic-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3299 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3096 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3007 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3119 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3117 2022-12-19 12:02:49.000000 trytond_product_classification_taxonomic-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3044 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3296 2022-12-19 12:02:49.000000 trytond_product_classification_taxonomic-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2968 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3116 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3202 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2883 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3146 2022-12-19 12:02:49.000000 trytond_product_classification_taxonomic-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3238 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3007 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3117 2023-04-13 16:52:41.000000 trytond_product_classification_taxonomic-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3149 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3178 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2845 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3290 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3180 2022-12-19 12:02:49.000000 trytond_product_classification_taxonomic-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3220 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-04-13 16:52:41.000000 trytond_product_classification_taxonomic-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3163 2022-12-19 12:02:49.000000 trytond_product_classification_taxonomic-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2167 2023-05-04 17:14:05.000000 trytond_product_classification_taxonomic-6.6.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8421 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-17 20:51:16.456417 trytond_product_classification_taxonomic-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4352 2023-04-13 16:52:41.000000 trytond_product_classification_taxonomic-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:51:16.449751 trytond_product_classification_taxonomic-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-13 16:52:41.000000 trytond_product_classification_taxonomic-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-13 16:52:41.000000 trytond_product_classification_taxonomic-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-04-13 16:52:41.000000 trytond_product_classification_taxonomic-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       87 2023-04-13 16:52:41.000000 trytond_product_classification_taxonomic-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:51:16.456417 trytond_product_classification_taxonomic-6.6.1/trytond_product_classification_taxonomic.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2752 2023-05-17 20:51:15.000000 trytond_product_classification_taxonomic-6.6.1/trytond_product_classification_taxonomic.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2023-05-17 20:51:16.000000 trytond_product_classification_taxonomic-6.6.1/trytond_product_classification_taxonomic.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:51:15.000000 trytond_product_classification_taxonomic-6.6.1/trytond_product_classification_taxonomic.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      102 2023-05-17 20:51:15.000000 trytond_product_classification_taxonomic-6.6.1/trytond_product_classification_taxonomic.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:51:15.000000 trytond_product_classification_taxonomic-6.6.1/trytond_product_classification_taxonomic.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       59 2023-05-17 20:51:15.000000 trytond_product_classification_taxonomic-6.6.1/trytond_product_classification_taxonomic.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-17 20:51:15.000000 trytond_product_classification_taxonomic-6.6.1/trytond_product_classification_taxonomic.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:51:16.453084 trytond_product_classification_taxonomic-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2022-12-19 12:02:49.000000 trytond_product_classification_taxonomic-6.6.1/view/cultivar_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/view/cultivar_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/view/cultivar_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/view/cultivar_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/view/taxon_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2022-12-19 12:02:49.000000 trytond_product_classification_taxonomic-6.6.1/view/taxon_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2022-12-19 12:02:50.000000 trytond_product_classification_taxonomic-6.6.1/view/taxon_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:09.471762 trytond_product_classification_taxonomic-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1310 2023-05-01 11:09:32.000000 trytond_product_classification_taxonomic-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:09:32.000000 trytond_product_classification_taxonomic-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2727 2023-05-01 11:54:09.471762 trytond_product_classification_taxonomic-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      588 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:09.468428 trytond_product_classification_taxonomic-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      588 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:09.465095 trytond_product_classification_taxonomic-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3299 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3096 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3007 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3119 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3117 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3044 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3296 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2968 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3116 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3202 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2883 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3146 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3238 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3007 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3117 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3149 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3178 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3290 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3180 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3220 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3163 2023-04-29 08:02:47.000000 trytond_product_classification_taxonomic-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2167 2023-04-30 10:46:36.000000 trytond_product_classification_taxonomic-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8421 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:54:09.471762 trytond_product_classification_taxonomic-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4284 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:09.465095 trytond_product_classification_taxonomic-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       87 2023-05-01 11:09:27.000000 trytond_product_classification_taxonomic-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:09.471762 trytond_product_classification_taxonomic-6.8.0/trytond_product_classification_taxonomic.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2727 2023-05-01 11:54:08.000000 trytond_product_classification_taxonomic-6.8.0/trytond_product_classification_taxonomic.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2023-05-01 11:54:09.000000 trytond_product_classification_taxonomic-6.8.0/trytond_product_classification_taxonomic.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:54:08.000000 trytond_product_classification_taxonomic-6.8.0/trytond_product_classification_taxonomic.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      102 2023-05-01 11:54:08.000000 trytond_product_classification_taxonomic-6.8.0/trytond_product_classification_taxonomic.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_product_classification_taxonomic-6.8.0/trytond_product_classification_taxonomic.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       59 2023-05-01 11:54:08.000000 trytond_product_classification_taxonomic-6.8.0/trytond_product_classification_taxonomic.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:54:08.000000 trytond_product_classification_taxonomic-6.8.0/trytond_product_classification_taxonomic.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:09.468428 trytond_product_classification_taxonomic-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-6.8.0/view/cultivar_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-6.8.0/view/cultivar_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_product_classification_taxonomic-6.8.0/view/cultivar_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-6.8.0/view/cultivar_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-6.8.0/view/taxon_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-6.8.0/view/taxon_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-01-16 14:00:20.000000 trytond_product_classification_taxonomic-6.8.0/view/taxon_tree.xml
```

### Comparing `trytond_product_classification_taxonomic-6.6.1/CHANGELOG` & `trytond_product_classification_taxonomic-6.8.0/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
-Version 6.6.1 - 2023-05-17
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

### Comparing `trytond_product_classification_taxonomic-6.6.1/COPYRIGHT` & `trytond_product_classification_taxonomic-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/LICENSE` & `trytond_product_classification_taxonomic-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/PKG-INFO` & `trytond_product_classification_taxonomic-6.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_product_classification_taxonomic
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to implement product classification taxonomic
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
-Project-URL: Source Code, https://hg.tryton.org/modules/product_classification_taxonomic
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product classification taxonomic
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: Bulgarian
@@ -36,21 +36,21 @@
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
 
 Product Classification Taxonomic Module
 #######################################
 
 The Product Classification Taxonomic module adds the taxonomic classification
 to the products.
```

### Comparing `trytond_product_classification_taxonomic-6.6.1/README.rst` & `trytond_product_classification_taxonomic-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/doc/conf.py` & `trytond_product_classification_taxonomic-6.8.0/doc/conf.py`

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

### Comparing `trytond_product_classification_taxonomic-6.6.1/doc/index.rst` & `trytond_product_classification_taxonomic-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/bg.po` & `trytond_product_classification_taxonomic-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/ca.po` & `trytond_product_classification_taxonomic-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/cs.po` & `trytond_product_classification_taxonomic-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/de.po` & `trytond_product_classification_taxonomic-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/es.po` & `trytond_product_classification_taxonomic-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/es_419.po` & `trytond_product_classification_taxonomic-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/et.po` & `trytond_product_classification_taxonomic-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/fa.po` & `trytond_product_classification_taxonomic-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/fi.po` & `trytond_product_classification_taxonomic-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/fr.po` & `trytond_product_classification_taxonomic-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/hu.po` & `trytond_product_classification_taxonomic-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/id.po` & `trytond_product_classification_taxonomic-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/it.po` & `trytond_product_classification_taxonomic-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/lo.po` & `trytond_product_classification_taxonomic-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/lt.po` & `trytond_product_classification_taxonomic-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/nl.po` & `trytond_product_classification_taxonomic-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/pl.po` & `trytond_product_classification_taxonomic-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/pt.po` & `trytond_product_classification_taxonomic-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/ro.po` & `trytond_product_classification_taxonomic-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/ru.po` & `trytond_product_classification_taxonomic-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/sl.po` & `trytond_product_classification_taxonomic-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/tr.po` & `trytond_product_classification_taxonomic-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/uk.po` & `trytond_product_classification_taxonomic-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/locale/zh_CN.po` & `trytond_product_classification_taxonomic-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/product.py` & `trytond_product_classification_taxonomic-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/product.xml` & `trytond_product_classification_taxonomic-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_classification_taxonomic-6.6.1/setup.py` & `trytond_product_classification_taxonomic-6.8.0/setup.py`

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
@@ -34,37 +31,39 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_product_classification_taxonomic'
 
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
     description='Tryton module to implement product classification taxonomic',
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
-        "Source Code": (
-            'https://hg.tryton.org/modules/product_classification_taxonomic'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton product classification taxonomic',
     package_dir={'trytond.modules.product_classification_taxonomic': '.'},
     packages=(
         ['trytond.modules.product_classification_taxonomic']
         + ['trytond.modules.product_classification_taxonomic.%s' % p
             for p in find_packages()]
@@ -100,23 +99,23 @@
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
     product_classification_taxonomic = trytond.modules.product_classification_taxonomic
     """,  # noqa: E501
     )
```

### Comparing `trytond_product_classification_taxonomic-6.6.1/trytond_product_classification_taxonomic.egg-info/PKG-INFO` & `trytond_product_classification_taxonomic-6.8.0/trytond_product_classification_taxonomic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-product-classification-taxonomic
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to implement product classification taxonomic
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
-Project-URL: Source Code, https://hg.tryton.org/modules/product_classification_taxonomic
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product classification taxonomic
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: Bulgarian
@@ -36,21 +36,21 @@
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
 
 Product Classification Taxonomic Module
 #######################################
 
 The Product Classification Taxonomic module adds the taxonomic classification
 to the products.
```

### Comparing `trytond_product_classification_taxonomic-6.6.1/trytond_product_classification_taxonomic.egg-info/SOURCES.txt` & `trytond_product_classification_taxonomic-6.8.0/trytond_product_classification_taxonomic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

