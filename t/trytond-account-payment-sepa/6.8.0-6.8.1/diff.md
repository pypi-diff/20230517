# Comparing `tmp/trytond_account_payment_sepa-6.8.0.tar.gz` & `tmp/trytond_account_payment_sepa-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_sepa-6.8.0.tar", last modified: Mon May  1 11:58:50 2023, max compression
+gzip compressed data, was "trytond_account_payment_sepa-6.8.1.tar", last modified: Wed May 17 20:56:01 2023, max compression
```

## Comparing `trytond_account_payment_sepa-6.8.0.tar` & `trytond_account_payment_sepa-6.8.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.125244 trytond_account_payment_sepa-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2688 2023-05-01 11:12:50.000000 trytond_account_payment_sepa-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:12:50.000000 trytond_account_payment_sepa-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4200 2023-05-01 11:58:50.125244 trytond_account_payment_sepa-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1915 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      803 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1948 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1056 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.118578 trytond_account_payment_sepa-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1915 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.098577 trytond_account_payment_sepa-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14910 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16985 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14377 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17220 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16868 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13739 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16064 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17244 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14360 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17008 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14691 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14237 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16454 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15217 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14491 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16939 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14648 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16059 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13793 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14999 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15868 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14360 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13739 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14512 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    81515 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/mandate.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)     1891 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4832 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    34292 2023-04-21 08:36:08.000000 trytond_account_payment_sepa-6.8.0/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15511 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4236 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/sepa_handler.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:58:50.125244 trytond_account_payment_sepa-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4535 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.101911 trytond_account_payment_sepa-6.8.0/template/
--rw-r--r--   0 ced       (1000) ced       (1000)     4112 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/base.003.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4330 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/base.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4970 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/pain.001.001.03.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4356 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/pain.001.001.05.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3590 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/pain.001.003.03.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5513 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/pain.008.001.02.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4824 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/pain.008.001.04.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4286 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/pain.008.003.02.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.115244 trytond_account_payment_sepa-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.01.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    54092 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.01.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     1394 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.02.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    63410 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.02.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2090 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.03.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    88101 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.03.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2159 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.04.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    86922 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.04.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    44938 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/pain.001.001.03.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    45912 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/pain.001.001.05.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    19514 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/pain.001.003.03.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    43173 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/pain.008.001.02.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    44121 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/pain.008.001.04.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    25935 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/pain.008.003.02.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    15710 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-05-01 11:12:44.000000 trytond_account_payment_sepa-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.121911 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4200 2023-05-01 11:58:49.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2023-05-01 11:58:50.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:58:49.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-05-01 11:58:49.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-05-01 11:58:49.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:58:49.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.118578 trytond_account_payment_sepa-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1044 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/view/mandate_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/mandate_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/message_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/view/message_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/party_identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/party_reception_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      776 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/payment_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/payment_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1027 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/payment_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:56:01.593188 trytond_account_payment_sepa-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2789 2023-05-17 20:55:58.000000 trytond_account_payment_sepa-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-17 20:55:58.000000 trytond_account_payment_sepa-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4200 2023-05-17 20:56:01.589855 trytond_account_payment_sepa-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1915 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      803 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1948 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1056 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:56:01.576521 trytond_account_payment_sepa-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1915 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:56:01.433186 trytond_account_payment_sepa-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14910 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16985 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14377 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17220 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16868 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13739 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16064 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17244 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14360 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17008 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14691 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14237 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16454 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15217 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14491 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16939 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14648 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16059 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13793 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14999 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15868 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14360 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13739 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14512 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    81515 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/mandate.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1891 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4832 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    34424 2023-05-04 17:42:26.000000 trytond_account_payment_sepa-6.8.1/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15511 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4236 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/sepa_handler.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-17 20:56:01.593188 trytond_account_payment_sepa-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4535 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:56:01.456519 trytond_account_payment_sepa-6.8.1/template/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4112 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/template/base.003.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4330 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/template/base.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4970 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/template/pain.001.001.03.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4356 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/template/pain.001.001.05.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3590 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/template/pain.001.003.03.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5513 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/template/pain.008.001.02.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4824 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/template/pain.008.001.04.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4286 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/template/pain.008.003.02.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:56:01.533187 trytond_account_payment_sepa-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/camt.054.001.01.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    54092 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/camt.054.001.01.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     1394 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/camt.054.001.02.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    63410 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/camt.054.001.02.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2090 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/camt.054.001.03.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    88101 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/camt.054.001.03.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2159 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/camt.054.001.04.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    86922 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/camt.054.001.04.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    44938 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/pain.001.001.03.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    45912 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/pain.001.001.05.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    19514 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/pain.001.003.03.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    43173 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/pain.008.001.02.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    44121 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/pain.008.001.04.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    25935 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/pain.008.003.02.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    15710 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-05-01 12:18:02.000000 trytond_account_payment_sepa-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:56:01.589855 trytond_account_payment_sepa-6.8.1/trytond_account_payment_sepa.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4200 2023-05-17 20:56:00.000000 trytond_account_payment_sepa-6.8.1/trytond_account_payment_sepa.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2023-05-17 20:56:01.000000 trytond_account_payment_sepa-6.8.1/trytond_account_payment_sepa.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:56:00.000000 trytond_account_payment_sepa-6.8.1/trytond_account_payment_sepa.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-05-17 20:56:00.000000 trytond_account_payment_sepa-6.8.1/trytond_account_payment_sepa.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:56:00.000000 trytond_account_payment_sepa-6.8.1/trytond_account_payment_sepa.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-05-17 20:56:00.000000 trytond_account_payment_sepa-6.8.1/trytond_account_payment_sepa.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-17 20:56:00.000000 trytond_account_payment_sepa-6.8.1/trytond_account_payment_sepa.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:56:01.566521 trytond_account_payment_sepa-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1044 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/view/mandate_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/view/mandate_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/view/message_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/view/message_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/view/party_identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/view/party_reception_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      776 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/view/payment_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/view/payment_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1027 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-05-01 12:17:30.000000 trytond_account_payment_sepa-6.8.1/view/payment_list.xml
```

### Comparing `trytond_account_payment_sepa-6.8.0/CHANGELOG` & `trytond_account_payment_sepa-6.8.1/CHANGELOG`

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

### Comparing `trytond_account_payment_sepa-6.8.0/COPYRIGHT` & `trytond_account_payment_sepa-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/LICENSE` & `trytond_account_payment_sepa-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/PKG-INFO` & `trytond_account_payment_sepa-6.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_sepa
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for SEPA payment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_payment_sepa-6.8.0/README.rst` & `trytond_account_payment_sepa-6.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/__init__.py` & `trytond_account_payment_sepa-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/account.py` & `trytond_account_payment_sepa-6.8.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/account.xml` & `trytond_account_payment_sepa-6.8.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/doc/conf.py` & `trytond_account_payment_sepa-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/doc/index.rst` & `trytond_account_payment_sepa-6.8.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/bg.po` & `trytond_account_payment_sepa-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/ca.po` & `trytond_account_payment_sepa-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/cs.po` & `trytond_account_payment_sepa-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/de.po` & `trytond_account_payment_sepa-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/es.po` & `trytond_account_payment_sepa-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/es_419.po` & `trytond_account_payment_sepa-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/et.po` & `trytond_account_payment_sepa-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/fa.po` & `trytond_account_payment_sepa-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/fi.po` & `trytond_account_payment_sepa-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/fr.po` & `trytond_account_payment_sepa-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/hu.po` & `trytond_account_payment_sepa-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/id.po` & `trytond_account_payment_sepa-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/it.po` & `trytond_account_payment_sepa-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/lo.po` & `trytond_account_payment_sepa-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/lt.po` & `trytond_account_payment_sepa-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/nl.po` & `trytond_account_payment_sepa-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/pl.po` & `trytond_account_payment_sepa-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/pt.po` & `trytond_account_payment_sepa-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/ro.po` & `trytond_account_payment_sepa-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/ru.po` & `trytond_account_payment_sepa-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/sl.po` & `trytond_account_payment_sepa-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/tr.po` & `trytond_account_payment_sepa-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/uk.po` & `trytond_account_payment_sepa-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/locale/zh_CN.po` & `trytond_account_payment_sepa-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/mandate.fodt` & `trytond_account_payment_sepa-6.8.1/mandate.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/message.xml` & `trytond_account_payment_sepa-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/party.py` & `trytond_account_payment_sepa-6.8.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/party.xml` & `trytond_account_payment_sepa-6.8.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/payment.py` & `trytond_account_payment_sepa-6.8.1/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,18 +231,20 @@
         for payment in self.payments:
             if not payment.sepa_bank_account_number:
                 raise ProcessError(
                     gettext('account_payment_sepa'
                         '.msg_payment_process_no_iban',
                         payment=payment.rec_name))
             if not payment.sepa_bank_account_number.account.bank:
+                bank_account = payment.sepa_bank_account_number.account
                 raise ProcessError(
                     gettext('account_payment_sepa'
                         '.msg_payment_process_no_bank',
-                        payment=payment.rec_name))
+                        payment=payment.rec_name,
+                        bank_account=bank_account.rec_name))
         to_write = []
         for key, payments in self.sepa_payments:
             to_write.append(payments)
             to_write.append({
                     'sepa_info_id': self.sepa_group_payment_id(key),
                     })
         if to_write:
```

### Comparing `trytond_account_payment_sepa-6.8.0/payment.xml` & `trytond_account_payment_sepa-6.8.1/payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/sepa_handler.py` & `trytond_account_payment_sepa-6.8.1/sepa_handler.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/setup.py` & `trytond_account_payment_sepa-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/template/base.003.xml` & `trytond_account_payment_sepa-6.8.1/template/base.003.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/template/base.xml` & `trytond_account_payment_sepa-6.8.1/template/base.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/template/pain.001.001.03.xml` & `trytond_account_payment_sepa-6.8.1/template/pain.001.001.03.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/template/pain.001.001.05.xml` & `trytond_account_payment_sepa-6.8.1/template/pain.001.001.05.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/template/pain.001.003.03.xml` & `trytond_account_payment_sepa-6.8.1/template/pain.001.003.03.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/template/pain.008.001.02.xml` & `trytond_account_payment_sepa-6.8.1/template/pain.008.001.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/template/pain.008.001.04.xml` & `trytond_account_payment_sepa-6.8.1/template/pain.008.001.04.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/template/pain.008.003.02.xml` & `trytond_account_payment_sepa-6.8.1/template/pain.008.003.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.01.xml` & `trytond_account_payment_sepa-6.8.1/tests/camt.054.001.01.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.01.xsd` & `trytond_account_payment_sepa-6.8.1/tests/camt.054.001.01.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.02.xml` & `trytond_account_payment_sepa-6.8.1/tests/camt.054.001.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.02.xsd` & `trytond_account_payment_sepa-6.8.1/tests/camt.054.001.02.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.03.xml` & `trytond_account_payment_sepa-6.8.1/tests/camt.054.001.03.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.03.xsd` & `trytond_account_payment_sepa-6.8.1/tests/camt.054.001.03.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.04.xml` & `trytond_account_payment_sepa-6.8.1/tests/camt.054.001.04.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.04.xsd` & `trytond_account_payment_sepa-6.8.1/tests/camt.054.001.04.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/pain.001.001.03.xsd` & `trytond_account_payment_sepa-6.8.1/tests/pain.001.001.03.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/pain.001.001.05.xsd` & `trytond_account_payment_sepa-6.8.1/tests/pain.001.001.05.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/pain.001.003.03.xsd` & `trytond_account_payment_sepa-6.8.1/tests/pain.001.003.03.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/pain.008.001.02.xsd` & `trytond_account_payment_sepa-6.8.1/tests/pain.008.001.02.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/pain.008.001.04.xsd` & `trytond_account_payment_sepa-6.8.1/tests/pain.008.001.04.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/pain.008.003.02.xsd` & `trytond_account_payment_sepa-6.8.1/tests/pain.008.003.02.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tests/test_module.py` & `trytond_account_payment_sepa-6.8.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/tox.ini` & `trytond_account_payment_sepa-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/PKG-INFO` & `trytond_account_payment_sepa-6.8.1/trytond_account_payment_sepa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-account-payment-sepa
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for SEPA payment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/SOURCES.txt` & `trytond_account_payment_sepa-6.8.1/trytond_account_payment_sepa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/view/mandate_form.xml` & `trytond_account_payment_sepa-6.8.1/view/mandate_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/view/message_form.xml` & `trytond_account_payment_sepa-6.8.1/view/message_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/view/payment_form.xml` & `trytond_account_payment_sepa-6.8.1/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.8.0/view/payment_journal_form.xml` & `trytond_account_payment_sepa-6.8.1/view/payment_journal_form.xml`

 * *Files identical despite different names*

