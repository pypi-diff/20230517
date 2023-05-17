# Comparing `tmp/trytond_account-6.8.0.tar.gz` & `tmp/trytond_account-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account-6.8.0.tar", last modified: Mon May  1 11:44:33 2023, max compression
+gzip compressed data, was "trytond_account-6.8.1.tar", last modified: Wed May 17 21:00:08 2023, max compression
```

## Comparing `trytond_account-6.8.0.tar` & `trytond_account-6.8.1.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.691283 trytond_account-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)    10071 2023-05-01 11:03:09.000000 trytond_account-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-01 11:03:09.000000 trytond_account-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-05-01 11:44:33.691283 trytond_account-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:14.000000 trytond_account-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3898 2023-04-21 08:36:08.000000 trytond_account-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)   125458 2023-04-30 10:46:36.000000 trytond_account-6.8.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    47195 2023-04-15 07:12:14.000000 trytond_account-6.8.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    51736 2023-01-16 14:00:20.000000 trytond_account-6.8.0/aged_balance.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)     6318 2023-04-15 07:12:14.000000 trytond_account-6.8.0/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1088 2023-04-15 07:12:14.000000 trytond_account-6.8.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9401 2023-04-21 08:36:08.000000 trytond_account-6.8.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-04-15 07:12:14.000000 trytond_account-6.8.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.674616 trytond_account-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/configuration.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.681283 trytond_account-6.8.0/doc/design/
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/account.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3062 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/fiscal-year.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      198 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2124 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/journal.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6736 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4330 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4793 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/design/template.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1558 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2410 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/setup.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.681283 trytond_account-6.8.0/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)     3763 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/close.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1984 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/create.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      220 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      770 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2858 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/report.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1327 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/structure.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2092 2023-04-15 07:12:14.000000 trytond_account-6.8.0/doc/usage/view.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1612 2023-04-15 07:12:14.000000 trytond_account-6.8.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25810 2023-04-28 07:46:16.000000 trytond_account-6.8.0/fiscalyear.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7617 2023-04-15 07:12:14.000000 trytond_account-6.8.0/fiscalyear.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    52160 2023-04-15 07:12:14.000000 trytond_account-6.8.0/general_journal.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    81553 2023-04-15 07:12:14.000000 trytond_account-6.8.0/general_ledger.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.684616 trytond_account-6.8.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:14.000000 trytond_account-6.8.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-6.8.0/icons/tryton-account-block.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:14.000000 trytond_account-6.8.0/icons/tryton-account-close.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:14.000000 trytond_account-6.8.0/icons/tryton-account-open.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-01-16 14:00:20.000000 trytond_account-6.8.0/icons/tryton-account.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    13471 2023-04-15 07:12:14.000000 trytond_account-6.8.0/journal.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11585 2023-04-21 08:36:08.000000 trytond_account-6.8.0/journal.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.644616 trytond_account-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)   129951 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)   128941 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)   112944 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)   132434 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)   129284 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)   117838 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125584 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)   136808 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)   116831 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)   131223 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   124036 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)   115678 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)   121715 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)   141931 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)   133225 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   129526 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   120919 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   124236 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   127368 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)   131779 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)   121797 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   112776 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   146125 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125354 2023-04-30 10:46:36.000000 trytond_account-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1494 2023-04-15 07:12:14.000000 trytond_account-6.8.0/localize.xsl
--rw-r--r--   0 ced       (1000) ced       (1000)    16493 2023-04-28 07:46:16.000000 trytond_account-6.8.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22110 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11303 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11052 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11058 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11004 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11069 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11050 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11083 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11090 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11405 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11056 2023-04-15 07:12:14.000000 trytond_account-6.8.0/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   114131 2023-04-21 08:36:08.000000 trytond_account-6.8.0/move.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27017 2023-04-21 08:36:08.000000 trytond_account-6.8.0/move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14747 2023-04-28 07:46:16.000000 trytond_account-6.8.0/move_template.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6825 2023-04-15 07:12:14.000000 trytond_account-6.8.0/move_template.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14382 2023-04-15 07:12:14.000000 trytond_account-6.8.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4226 2023-04-15 07:12:14.000000 trytond_account-6.8.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    15701 2023-04-21 08:36:08.000000 trytond_account-6.8.0/period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4677 2023-04-15 07:12:14.000000 trytond_account-6.8.0/period.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:44:33.691283 trytond_account-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4529 2023-04-15 07:12:14.000000 trytond_account-6.8.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    70888 2023-04-21 08:36:08.000000 trytond_account-6.8.0/tax.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24586 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tax.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.651282 trytond_account-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4654 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_account_active.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3732 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_account_reconcile.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2456 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_account_reconcile_automatic.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6220 2023-04-21 08:36:08.000000 trytond_account-6.8.0/tests/scenario_account_reconciliation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3390 2023-04-21 08:36:08.000000 trytond_account-6.8.0/tests/scenario_account_reconciliation_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4119 2023-04-21 08:36:08.000000 trytond_account-6.8.0/tests/scenario_account_reconciliation_alternate_currency_write_off.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4815 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_close_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4337 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_move_cancel.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2951 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_move_line_delegate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5029 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_move_line_group.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4919 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_move_line_reschedule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3981 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_move_template.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2276 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    10880 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_reports.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2670 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/scenario_tax_code.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    73136 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4788 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:14.000000 trytond_account-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)    47972 2023-04-15 07:12:14.000000 trytond_account-6.8.0/trial_balance.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-05-01 11:03:03.000000 trytond_account-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.687950 trytond_account-6.8.0/trytond_account.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-05-01 11:44:32.000000 trytond_account-6.8.0/trytond_account.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    11872 2023-05-01 11:44:33.000000 trytond_account-6.8.0/trytond_account.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:44:32.000000 trytond_account-6.8.0/trytond_account.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-05-01 11:44:32.000000 trytond_account-6.8.0/trytond_account.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account-6.8.0/trytond_account.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-05-01 11:44:32.000000 trytond_account-6.8.0/trytond_account.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:44:32.000000 trytond_account-6.8.0/trytond_account.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    54595 2023-04-15 07:12:14.000000 trytond_account-6.8.0/type_statement.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:33.674616 trytond_account-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_balance_sheet_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      598 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_deferral_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_deferral_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2841 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_income_statement_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_list_balance_sheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1074 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1283 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1103 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_type_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_type_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_type_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/account_type_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/aged_balance_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/aged_balance_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/balance_sheet_context_comparison_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/balance_sheet_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1334 2023-04-21 08:36:08.000000 trytond_account-6.8.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/create_chart_account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/create_chart_properties_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/create_chart_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/fiscalyear_balance_non_deferral_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/fiscalyear_create_periods_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      910 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/fiscalyear_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/fiscalyear_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      700 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/general_ledger_account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-28 07:46:16.000000 trytond_account-6.8.0/view/general_ledger_account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/general_ledger_account_party_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/general_ledger_line_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      783 2023-04-28 07:46:16.000000 trytond_account-6.8.0/view/general_ledger_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1138 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/income_statement_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/journal_list_cash.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/journal_open_cash_context.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/journal_period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/journal_period_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/journal_period_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/journal_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_cancel_default_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1075 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_delegate_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1724 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1241 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_form_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_group_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_list_payable_receivable.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-21 08:36:08.000000 trytond_account-6.8.0/view/move_line_list_reconcile.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_receivable_payable_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_reschedule_preview_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_reschedule_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_reschedule_term_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/move_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1025 2023-04-28 07:46:16.000000 trytond_account-6.8.0/view/move_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      640 2023-04-28 07:46:16.000000 trytond_account-6.8.0/view/move_line_tree_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_reconciliation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_reconciliation_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/move_template_create_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      927 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/move_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/move_template_keyword_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/move_template_keyword_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/move_template_keyword_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/open_journal_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1161 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/party_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      747 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/period_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/period_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/reconcile_lines_writeoff_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      755 2023-04-21 08:36:08.000000 trytond_account-6.8.0/view/reconcile_show_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/reconcile_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      576 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/renew_fiscalyear_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      555 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_code_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1122 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_code_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_code_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_code_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_code_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_code_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      843 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_code_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_code_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_code_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_code_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2193 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_group_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_line_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_rule_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_rule_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2101 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/tax_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/tax_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      250 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/update_chart_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/update_chart_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-01-16 14:00:20.000000 trytond_account-6.8.0/view/writeoff_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:14.000000 trytond_account-6.8.0/view/writeoff_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 21:00:08.926169 trytond_account-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10172 2023-05-17 21:00:05.000000 trytond_account-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-17 21:00:05.000000 trytond_account-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:30.000000 trytond_account-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:30.000000 trytond_account-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-05-17 21:00:08.926169 trytond_account-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-05-01 12:17:30.000000 trytond_account-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3898 2023-05-01 12:17:30.000000 trytond_account-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   125458 2023-05-01 12:17:30.000000 trytond_account-6.8.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    47195 2023-05-01 12:17:30.000000 trytond_account-6.8.1/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    51736 2023-05-01 12:17:30.000000 trytond_account-6.8.1/aged_balance.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)     6318 2023-05-01 12:17:30.000000 trytond_account-6.8.1/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1088 2023-05-01 12:17:30.000000 trytond_account-6.8.1/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9401 2023-05-01 12:17:30.000000 trytond_account-6.8.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-05-01 12:17:30.000000 trytond_account-6.8.1/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 21:00:08.896169 trytond_account-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/configuration.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 21:00:08.902836 trytond_account-6.8.1/doc/design/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/design/account.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/design/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3062 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/design/fiscal-year.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      198 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/design/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2124 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/design/journal.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6736 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/design/move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4330 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/design/tax.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4793 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/design/template.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1558 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2410 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/setup.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 21:00:08.912836 trytond_account-6.8.1/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3763 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/usage/close.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1984 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/usage/create.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      220 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      770 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/usage/process.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2858 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/usage/report.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1327 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/usage/structure.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2092 2023-05-01 12:17:30.000000 trytond_account-6.8.1/doc/usage/view.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1612 2023-05-01 12:17:30.000000 trytond_account-6.8.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25810 2023-05-01 12:17:30.000000 trytond_account-6.8.1/fiscalyear.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7617 2023-05-01 12:17:30.000000 trytond_account-6.8.1/fiscalyear.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    52160 2023-05-01 12:17:30.000000 trytond_account-6.8.1/general_journal.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    81553 2023-05-01 12:17:30.000000 trytond_account-6.8.1/general_ledger.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 21:00:08.912836 trytond_account-6.8.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:30.000000 trytond_account-6.8.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-05-01 12:17:30.000000 trytond_account-6.8.1/icons/tryton-account-block.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-05-01 12:17:30.000000 trytond_account-6.8.1/icons/tryton-account-close.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-05-01 12:17:30.000000 trytond_account-6.8.1/icons/tryton-account-open.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-05-01 12:17:30.000000 trytond_account-6.8.1/icons/tryton-account.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    13471 2023-05-01 12:17:30.000000 trytond_account-6.8.1/journal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11585 2023-05-01 12:17:30.000000 trytond_account-6.8.1/journal.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 21:00:08.742834 trytond_account-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)   129951 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   128941 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   112944 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   132434 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   129284 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   117838 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125584 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   136808 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   116831 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   131223 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   124036 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   115678 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   121715 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   141931 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   133225 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   129526 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   120919 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   124236 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   127368 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   131779 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   121797 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   112776 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   146125 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125354 2023-05-01 12:17:30.000000 trytond_account-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1494 2023-05-01 12:17:30.000000 trytond_account-6.8.1/localize.xsl
+-rw-r--r--   0 ced       (1000) ced       (1000)    16493 2023-05-01 12:17:30.000000 trytond_account-6.8.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22110 2023-05-01 12:17:30.000000 trytond_account-6.8.1/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11303 2023-05-01 12:17:30.000000 trytond_account-6.8.1/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11052 2023-05-01 12:17:30.000000 trytond_account-6.8.1/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11058 2023-05-01 12:17:30.000000 trytond_account-6.8.1/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11004 2023-05-01 12:17:30.000000 trytond_account-6.8.1/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11069 2023-05-01 12:17:30.000000 trytond_account-6.8.1/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11050 2023-05-01 12:17:30.000000 trytond_account-6.8.1/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11083 2023-05-01 12:17:30.000000 trytond_account-6.8.1/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11090 2023-05-01 12:17:30.000000 trytond_account-6.8.1/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11405 2023-05-01 12:17:30.000000 trytond_account-6.8.1/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11056 2023-05-01 12:17:30.000000 trytond_account-6.8.1/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   114201 2023-05-13 22:22:57.000000 trytond_account-6.8.1/move.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27017 2023-05-01 12:17:30.000000 trytond_account-6.8.1/move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14747 2023-05-01 12:17:30.000000 trytond_account-6.8.1/move_template.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6825 2023-05-01 12:17:30.000000 trytond_account-6.8.1/move_template.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14382 2023-05-01 12:17:30.000000 trytond_account-6.8.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4226 2023-05-01 12:17:30.000000 trytond_account-6.8.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15701 2023-05-01 12:17:30.000000 trytond_account-6.8.1/period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4677 2023-05-01 12:17:30.000000 trytond_account-6.8.1/period.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-17 21:00:08.926169 trytond_account-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4529 2023-05-01 12:17:30.000000 trytond_account-6.8.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    70888 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tax.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24586 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tax.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 21:00:08.769501 trytond_account-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4654 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_account_active.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3732 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_account_reconcile.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2456 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_account_reconcile_automatic.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6220 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_account_reconciliation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3390 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_account_reconciliation_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4119 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_account_reconciliation_alternate_currency_write_off.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4815 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_close_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4337 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_move_cancel.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2951 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_move_line_delegate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5029 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_move_line_group.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4919 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_move_line_reschedule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3981 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_move_template.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2276 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    10880 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_reports.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2670 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/scenario_tax_code.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    73136 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4788 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:30.000000 trytond_account-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)    47972 2023-05-01 12:17:30.000000 trytond_account-6.8.1/trial_balance.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-05-01 12:18:02.000000 trytond_account-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 21:00:08.919503 trytond_account-6.8.1/trytond_account.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2511 2023-05-17 21:00:07.000000 trytond_account-6.8.1/trytond_account.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    11872 2023-05-17 21:00:08.000000 trytond_account-6.8.1/trytond_account.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 21:00:07.000000 trytond_account-6.8.1/trytond_account.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-05-17 21:00:07.000000 trytond_account-6.8.1/trytond_account.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 21:00:07.000000 trytond_account-6.8.1/trytond_account.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-05-17 21:00:07.000000 trytond_account-6.8.1/trytond_account.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-17 21:00:07.000000 trytond_account-6.8.1/trytond_account.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    54595 2023-05-01 12:17:30.000000 trytond_account-6.8.1/type_statement.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 21:00:08.889502 trytond_account-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_balance_sheet_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      598 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_deferral_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_deferral_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2841 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_income_statement_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_list_balance_sheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1074 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1283 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1103 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_type_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_type_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_type_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/account_type_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/aged_balance_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/aged_balance_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/balance_sheet_context_comparison_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/balance_sheet_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1334 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/create_chart_account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/create_chart_properties_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/create_chart_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/fiscalyear_balance_non_deferral_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/fiscalyear_create_periods_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      910 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/fiscalyear_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/fiscalyear_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      700 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/general_ledger_account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/general_ledger_account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/general_ledger_account_party_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/general_ledger_line_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      783 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/general_ledger_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1138 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/income_statement_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/journal_list_cash.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/journal_open_cash_context.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/journal_period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/journal_period_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/journal_period_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/journal_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_cancel_default_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1075 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_delegate_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1724 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1241 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_form_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_group_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_list_payable_receivable.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_list_reconcile.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_receivable_payable_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_reschedule_preview_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_reschedule_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_reschedule_term_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1025 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      640 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_line_tree_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_reconciliation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_reconciliation_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_template_create_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      927 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_template_keyword_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_template_keyword_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_template_keyword_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/open_journal_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1161 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/party_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      747 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/period_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/period_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/reconcile_lines_writeoff_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      755 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/reconcile_show_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/reconcile_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/renew_fiscalyear_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      555 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_code_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1122 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_code_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_code_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_code_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_code_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_code_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      843 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_code_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_code_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_code_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_code_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2193 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_group_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_rule_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_rule_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_rule_line_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_rule_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_rule_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_rule_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_rule_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_rule_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2101 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/tax_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      250 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/update_chart_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/update_chart_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/writeoff_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-05-01 12:17:30.000000 trytond_account-6.8.1/view/writeoff_tree.xml
```

### Comparing `trytond_account-6.8.0/CHANGELOG` & `trytond_account-6.8.1/CHANGELOG`

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
 * Support reconcile lines with currency exchange
 * Add reconcile and unreconcile from general ledger lines
 * Always raise exception when fiscal year or period are not found
 * Remove support for Python 3.7
```

### Comparing `trytond_account-6.8.0/COPYRIGHT` & `trytond_account-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/LICENSE` & `trytond_account-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/PKG-INFO` & `trytond_account-6.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for accounting
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account-6.8.0/__init__.py` & `trytond_account-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/account.py` & `trytond_account-6.8.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/account.xml` & `trytond_account-6.8.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/aged_balance.fodt` & `trytond_account-6.8.1/aged_balance.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/common.py` & `trytond_account-6.8.1/common.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/company.py` & `trytond_account-6.8.1/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/configuration.py` & `trytond_account-6.8.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/configuration.xml` & `trytond_account-6.8.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/conf.py` & `trytond_account-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/configuration.rst` & `trytond_account-6.8.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/design/account.rst` & `trytond_account-6.8.1/doc/design/account.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/design/configuration.rst` & `trytond_account-6.8.1/doc/design/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/design/fiscal-year.rst` & `trytond_account-6.8.1/doc/design/fiscal-year.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/design/journal.rst` & `trytond_account-6.8.1/doc/design/journal.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/design/move.rst` & `trytond_account-6.8.1/doc/design/move.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/design/tax.rst` & `trytond_account-6.8.1/doc/design/tax.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/design/template.rst` & `trytond_account-6.8.1/doc/design/template.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/reference.rst` & `trytond_account-6.8.1/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/setup.rst` & `trytond_account-6.8.1/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/usage/close.rst` & `trytond_account-6.8.1/doc/usage/close.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/usage/create.rst` & `trytond_account-6.8.1/doc/usage/create.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/usage/process.rst` & `trytond_account-6.8.1/doc/usage/process.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/usage/report.rst` & `trytond_account-6.8.1/doc/usage/report.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/usage/structure.rst` & `trytond_account-6.8.1/doc/usage/structure.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/doc/usage/view.rst` & `trytond_account-6.8.1/doc/usage/view.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/exceptions.py` & `trytond_account-6.8.1/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/fiscalyear.py` & `trytond_account-6.8.1/fiscalyear.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/fiscalyear.xml` & `trytond_account-6.8.1/fiscalyear.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/general_journal.fodt` & `trytond_account-6.8.1/general_journal.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/general_ledger.fodt` & `trytond_account-6.8.1/general_ledger.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/icons/LICENSE` & `trytond_account-6.8.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/journal.py` & `trytond_account-6.8.1/journal.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/journal.xml` & `trytond_account-6.8.1/journal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/bg.po` & `trytond_account-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/ca.po` & `trytond_account-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/cs.po` & `trytond_account-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/de.po` & `trytond_account-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/es.po` & `trytond_account-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/es_419.po` & `trytond_account-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/et.po` & `trytond_account-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/fa.po` & `trytond_account-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/fi.po` & `trytond_account-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/fr.po` & `trytond_account-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/hu.po` & `trytond_account-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/id.po` & `trytond_account-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/it.po` & `trytond_account-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/lo.po` & `trytond_account-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/lt.po` & `trytond_account-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/nl.po` & `trytond_account-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/pl.po` & `trytond_account-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/pt.po` & `trytond_account-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/ro.po` & `trytond_account-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/ru.po` & `trytond_account-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/sl.po` & `trytond_account-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/tr.po` & `trytond_account-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/uk.po` & `trytond_account-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/locale/zh_CN.po` & `trytond_account-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/localize.xsl` & `trytond_account-6.8.1/localize.xsl`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/message.xml` & `trytond_account-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/minimal_chart.xml` & `trytond_account-6.8.1/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/minimal_chart_bg.xml` & `trytond_account-6.8.1/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/minimal_chart_ca.xml` & `trytond_account-6.8.1/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/minimal_chart_de.xml` & `trytond_account-6.8.1/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/minimal_chart_en.xml` & `trytond_account-6.8.1/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/minimal_chart_es.xml` & `trytond_account-6.8.1/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/minimal_chart_fr.xml` & `trytond_account-6.8.1/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/minimal_chart_nl.xml` & `trytond_account-6.8.1/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/minimal_chart_pt.xml` & `trytond_account-6.8.1/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/minimal_chart_ru.xml` & `trytond_account-6.8.1/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/minimal_chart_sl.xml` & `trytond_account-6.8.1/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/move.py` & `trytond_account-6.8.1/move.py`

 * *Files 0% similar despite different names*

```diff
@@ -2201,16 +2201,17 @@
                     return 'end'
         if self.start.automatic or self.start.only_balanced:
             lines = self._default_lines()
             if lines and self.start.automatic:
                 while lines:
                     Line.reconcile(lines)
                     lines = self._default_lines()
-                if not self.get_parties(
-                        self.show.account, party=self.show.party):
+                if not self.get_currencies(
+                        self.show.account, self.show.party,
+                        currency=self.show.currency):
                     return 'next_'
             elif not lines and self.start.only_balanced:
                 return 'next_'
         return 'show'
 
     def default_show(self, fields):
         pool = Pool()
@@ -2393,20 +2394,20 @@
         states={
             'invisible': _write_off_states['invisible'],
             })
 
     @fields.depends('lines', 'currency', 'company')
     def on_change_lines(self):
         amount = Decimal(0)
-        for line in self.lines:
-            if line.second_currency == self.currency:
-                amount += line.amount_second_currency
-            elif line.currency == self.currency:
-                amount += line.debit - line.credit
         if self.currency:
+            for line in self.lines:
+                if line.second_currency == self.currency:
+                    amount += line.amount_second_currency
+                elif line.currency == self.currency:
+                    amount += line.debit - line.credit
             amount = self.currency.round(amount)
         self.write_off_amount = amount
 
 
 class CancelMoves(Wizard):
     'Cancel Moves'
     __name__ = 'account.move.cancel'
```

### Comparing `trytond_account-6.8.0/move.xml` & `trytond_account-6.8.1/move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/move_template.py` & `trytond_account-6.8.1/move_template.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/move_template.xml` & `trytond_account-6.8.1/move_template.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/party.py` & `trytond_account-6.8.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/party.xml` & `trytond_account-6.8.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/period.py` & `trytond_account-6.8.1/period.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/period.xml` & `trytond_account-6.8.1/period.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/setup.py` & `trytond_account-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tax.py` & `trytond_account-6.8.1/tax.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tax.xml` & `trytond_account-6.8.1/tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_account_active.rst` & `trytond_account-6.8.1/tests/scenario_account_active.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_account_reconcile.rst` & `trytond_account-6.8.1/tests/scenario_account_reconcile.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_account_reconcile_automatic.rst` & `trytond_account-6.8.1/tests/scenario_account_reconcile_automatic.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_account_reconciliation.rst` & `trytond_account-6.8.1/tests/scenario_account_reconciliation.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_account_reconciliation_alternate_currency.rst` & `trytond_account-6.8.1/tests/scenario_account_reconciliation_alternate_currency.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_account_reconciliation_alternate_currency_write_off.rst` & `trytond_account-6.8.1/tests/scenario_account_reconciliation_alternate_currency_write_off.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_close_fiscalyear.rst` & `trytond_account-6.8.1/tests/scenario_close_fiscalyear.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_move_cancel.rst` & `trytond_account-6.8.1/tests/scenario_move_cancel.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_move_line_delegate.rst` & `trytond_account-6.8.1/tests/scenario_move_line_delegate.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_move_line_group.rst` & `trytond_account-6.8.1/tests/scenario_move_line_group.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_move_line_reschedule.rst` & `trytond_account-6.8.1/tests/scenario_move_line_reschedule.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_move_template.rst` & `trytond_account-6.8.1/tests/scenario_move_template.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_renew_fiscalyear.rst` & `trytond_account-6.8.1/tests/scenario_renew_fiscalyear.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_reports.rst` & `trytond_account-6.8.1/tests/scenario_reports.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/scenario_tax_code.rst` & `trytond_account-6.8.1/tests/scenario_tax_code.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/test_module.py` & `trytond_account-6.8.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tests/tools.py` & `trytond_account-6.8.1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/tox.ini` & `trytond_account-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/trial_balance.fodt` & `trytond_account-6.8.1/trial_balance.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/trytond_account.egg-info/PKG-INFO` & `trytond_account-6.8.1/trytond_account.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-account
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for accounting
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account-6.8.0/trytond_account.egg-info/SOURCES.txt` & `trytond_account-6.8.1/trytond_account.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/type_statement.fodt` & `trytond_account-6.8.1/type_statement.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/account_deferral_form.xml` & `trytond_account-6.8.1/view/account_deferral_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/account_form.xml` & `trytond_account-6.8.1/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/account_template_form.xml` & `trytond_account-6.8.1/view/account_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/account_type_form.xml` & `trytond_account-6.8.1/view/account_type_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/account_type_template_form.xml` & `trytond_account-6.8.1/view/account_type_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/aged_balance_context_form.xml` & `trytond_account-6.8.1/view/aged_balance_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/configuration_form.xml` & `trytond_account-6.8.1/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/fiscalyear_create_periods_start_form.xml` & `trytond_account-6.8.1/view/fiscalyear_create_periods_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/fiscalyear_form.xml` & `trytond_account-6.8.1/view/fiscalyear_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/general_ledger_account_context_form.xml` & `trytond_account-6.8.1/view/general_ledger_account_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/general_ledger_account_list.xml` & `trytond_account-6.8.1/view/general_ledger_account_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/general_ledger_line_list.xml` & `trytond_account-6.8.1/view/general_ledger_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/income_statement_context_form.xml` & `trytond_account-6.8.1/view/income_statement_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/journal_form.xml` & `trytond_account-6.8.1/view/journal_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/move_form.xml` & `trytond_account-6.8.1/view/move_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/move_line_form.xml` & `trytond_account-6.8.1/view/move_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/move_line_form_move.xml` & `trytond_account-6.8.1/view/move_line_form_move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/move_line_list_payable_receivable.xml` & `trytond_account-6.8.1/view/move_line_list_payable_receivable.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/move_line_reschedule_start_form.xml` & `trytond_account-6.8.1/view/move_line_reschedule_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/move_line_template_form.xml` & `trytond_account-6.8.1/view/move_line_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/move_line_tree.xml` & `trytond_account-6.8.1/view/move_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/move_line_tree_move.xml` & `trytond_account-6.8.1/view/move_line_tree_move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/move_template_form.xml` & `trytond_account-6.8.1/view/move_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/move_template_keyword_form.xml` & `trytond_account-6.8.1/view/move_template_keyword_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/move_tree.xml` & `trytond_account-6.8.1/view/move_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/party_form.xml` & `trytond_account-6.8.1/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/period_form.xml` & `trytond_account-6.8.1/view/period_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/reconcile_show_form.xml` & `trytond_account-6.8.1/view/reconcile_show_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/renew_fiscalyear_start_form.xml` & `trytond_account-6.8.1/view/renew_fiscalyear_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/tax_code_context_form.xml` & `trytond_account-6.8.1/view/tax_code_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/tax_code_form.xml` & `trytond_account-6.8.1/view/tax_code_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/tax_code_template_form.xml` & `trytond_account-6.8.1/view/tax_code_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/tax_form.xml` & `trytond_account-6.8.1/view/tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/tax_rule_form.xml` & `trytond_account-6.8.1/view/tax_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/tax_rule_line_form.xml` & `trytond_account-6.8.1/view/tax_rule_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/tax_rule_line_template_form.xml` & `trytond_account-6.8.1/view/tax_rule_line_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/tax_template_form.xml` & `trytond_account-6.8.1/view/tax_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/tax_test_form.xml` & `trytond_account-6.8.1/view/tax_test_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-6.8.0/view/writeoff_form.xml` & `trytond_account-6.8.1/view/writeoff_form.xml`

 * *Files identical despite different names*

