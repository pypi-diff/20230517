# Comparing `tmp/trytond_account_invoice-6.8.0.tar.gz` & `tmp/trytond_account_invoice-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice-6.8.0.tar", last modified: Mon May  1 11:45:58 2023, max compression
+gzip compressed data, was "trytond_account_invoice-6.8.1.tar", last modified: Wed May 17 20:58:13 2023, max compression
```

## Comparing `trytond_account_invoice-6.8.0.tar` & `trytond_account_invoice-6.8.1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.909007 trytond_account_invoice-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     7503 2023-05-01 11:04:03.000000 trytond_account_invoice-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-01 11:04:02.000000 trytond_account_invoice-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-05-01 11:45:58.909007 trytond_account_invoice-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1900 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18805 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4994 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.902341 trytond_account_invoice-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      796 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7303 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.902341 trytond_account_invoice-6.8.0/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)     1920 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/usage/amend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3446 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/usage/prepare.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3685 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      869 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.902341 trytond_account_invoice-6.8.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/icons/tryton-invoice.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    83227 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/invoice.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)   130495 2023-04-29 11:01:18.000000 trytond_account_invoice-6.8.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24250 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.885674 trytond_account_invoice-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    36045 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37302 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31162 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37906 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37027 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32038 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35126 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39011 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31136 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37812 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33682 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33571 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34282 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36613 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34940 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37026 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31760 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34582 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35422 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36762 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33969 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31118 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    29853 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35375 2023-04-30 10:46:36.000000 trytond_account_invoice-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6174 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3977 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2389 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    15131 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/payment_term.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5934 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/payment_term.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:45:58.909007 trytond_account_invoice-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4594 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.895674 trytond_account_invoice-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3188 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_cancelling_invoice_move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4029 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_credit_note.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    12415 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5700 2023-04-21 08:36:08.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2856 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_alternate_currency_lower_rate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3472 2023-04-21 08:36:08.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_alternate_currency_rate_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3426 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_alternative_payee.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2713 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_customer_sequential.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4213 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_group_line.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1868 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_in_future.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2606 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_manual_tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3521 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_overpayment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_reschedule_lines.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7417 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_supplier.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3480 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_supplier_post_paid.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3582 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_tax_deductible.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3408 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_invoice_with_credit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3706 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    11545 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      230 2023-05-01 11:03:56.000000 trytond_account_invoice-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.905674 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-05-01 11:45:57.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     5919 2023-05-01 11:45:58.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:45:57.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 11:45:57.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-05-01 11:45:57.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:45:57.000000 trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:58.899007 trytond_account_invoice-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/address_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/contact_mechanism_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/contact_mechanism_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/contact_mechanism_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/credit_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4492 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      694 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      842 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/invoice_sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/invoice_sequence_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/invoice_sequence_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_tax_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/invoice_tax_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-04-28 07:43:48.000000 trytond_account_invoice-6.8.0/view/invoice_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-04-28 07:46:16.000000 trytond_account_invoice-6.8.0/view/move_line_list_payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/move_line_list_to_pay.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-04-21 08:36:08.000000 trytond_account_invoice-6.8.0/view/pay_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-21 08:36:08.000000 trytond_account_invoice-6.8.0/view/pay_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/payment_method_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_method_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-01-16 14:00:20.000000 trytond_account_invoice-6.8.0/view/payment_term_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_line_relativedelta_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_line_relativedelta_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_line_relativedelta_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_account_invoice-6.8.0/view/payment_term_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:58:13.694780 trytond_account_invoice-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7604 2023-05-17 20:58:10.000000 trytond_account_invoice-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-17 20:58:10.000000 trytond_account_invoice-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-05-17 20:58:13.694780 trytond_account_invoice-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1900 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18805 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4994 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:58:13.678113 trytond_account_invoice-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      796 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7303 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:58:13.681447 trytond_account_invoice-6.8.1/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1920 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/doc/usage/amend.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3446 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/doc/usage/prepare.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3685 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/doc/usage/process.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      869 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:58:13.684780 trytond_account_invoice-6.8.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/icons/tryton-invoice.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    83227 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/invoice.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)   130781 2023-05-13 22:06:18.000000 trytond_account_invoice-6.8.1/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24250 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:58:13.614779 trytond_account_invoice-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    36045 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37302 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31162 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37906 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37027 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32038 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35126 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39011 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31136 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37812 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33682 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33571 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34282 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36613 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34940 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37026 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31760 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34582 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35422 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36762 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33969 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31118 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    29853 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35375 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6174 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3977 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2389 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15131 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/payment_term.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5934 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/payment_term.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-17 20:58:13.694780 trytond_account_invoice-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4594 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:58:13.634780 trytond_account_invoice-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3188 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_cancelling_invoice_move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4029 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_credit_note.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    12415 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5700 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2856 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_alternate_currency_lower_rate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3472 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_alternate_currency_rate_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3426 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_alternative_payee.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2713 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_customer_sequential.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4213 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_group_line.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1868 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_in_future.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2606 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_manual_tax.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3521 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_overpayment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_reschedule_lines.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7417 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_supplier.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3480 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_supplier_post_paid.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3582 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_tax_deductible.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3408 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_invoice_with_credit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3706 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    11545 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      230 2023-05-01 12:18:02.000000 trytond_account_invoice-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:58:13.691447 trytond_account_invoice-6.8.1/trytond_account_invoice.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-05-17 20:58:12.000000 trytond_account_invoice-6.8.1/trytond_account_invoice.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     5919 2023-05-17 20:58:13.000000 trytond_account_invoice-6.8.1/trytond_account_invoice.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:58:12.000000 trytond_account_invoice-6.8.1/trytond_account_invoice.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-17 20:58:12.000000 trytond_account_invoice-6.8.1/trytond_account_invoice.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:58:12.000000 trytond_account_invoice-6.8.1/trytond_account_invoice.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-05-17 20:58:12.000000 trytond_account_invoice-6.8.1/trytond_account_invoice.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-17 20:58:12.000000 trytond_account_invoice-6.8.1/trytond_account_invoice.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:58:13.674780 trytond_account_invoice-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/address_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/contact_mechanism_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/contact_mechanism_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/contact_mechanism_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/credit_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4492 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      694 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/invoice_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/invoice_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      842 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/invoice_sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/invoice_sequence_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/invoice_sequence_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/invoice_tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/invoice_tax_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/invoice_tax_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/invoice_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/move_line_list_payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/move_line_list_to_pay.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/pay_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/pay_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/payment_method_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/payment_method_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/payment_term_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/payment_term_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/payment_term_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/payment_term_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/payment_term_line_relativedelta_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/payment_term_line_relativedelta_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/payment_term_line_relativedelta_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/payment_term_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/payment_term_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-05-01 12:17:30.000000 trytond_account_invoice-6.8.1/view/payment_term_tree.xml
```

### Comparing `trytond_account_invoice-6.8.0/CHANGELOG` & `trytond_account_invoice-6.8.1/CHANGELOG`

 * *Files 1% similar despite different names*

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
 * Support payment with currency exchange
 * Remove support for Python 3.7
 * Add support for Python 3.11
 * Warn when cancelling a move related to an invoice
```

### Comparing `trytond_account_invoice-6.8.0/COPYRIGHT` & `trytond_account_invoice-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/LICENSE` & `trytond_account_invoice-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/PKG-INFO` & `trytond_account_invoice-6.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for invoicing
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_invoice-6.8.0/__init__.py` & `trytond_account_invoice-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/account.py` & `trytond_account_invoice-6.8.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/account.xml` & `trytond_account_invoice-6.8.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/company.py` & `trytond_account_invoice-6.8.1/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/doc/conf.py` & `trytond_account_invoice-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/doc/configuration.rst` & `trytond_account_invoice-6.8.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/doc/design.rst` & `trytond_account_invoice-6.8.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/doc/usage/amend.rst` & `trytond_account_invoice-6.8.1/doc/usage/amend.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/doc/usage/prepare.rst` & `trytond_account_invoice-6.8.1/doc/usage/prepare.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/doc/usage/process.rst` & `trytond_account_invoice-6.8.1/doc/usage/process.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/exceptions.py` & `trytond_account_invoice-6.8.1/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/icons/LICENSE` & `trytond_account_invoice-6.8.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/invoice.fodt` & `trytond_account_invoice-6.8.1/invoice.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/invoice.py` & `trytond_account_invoice-6.8.1/invoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,66 +482,75 @@
     def default_company():
         return Transaction().context.get('company')
 
     @fields.depends('company')
     def on_change_with_company_party(self, name=None):
         return self.company.party if self.company else None
 
-    @fields.depends(
-        'state', 'account', 'party', 'type', 'accounting_date', 'invoice_date')
-    def on_change_with_account(self):
-        if self.state != 'draft':
-            return self.account
-        account = None
-        if self.party:
-            with Transaction().set_context(
-                    date=self.accounting_date or self.invoice_date):
-                if self.type == 'out':
-                    account = self.party.account_receivable_used
-                elif self.type == 'in':
-                    account = self.party.account_payable_used
-        return account
+    @fields.depends(methods=['set_journal', 'on_change_party'])
+    def on_change_type(self):
+        self.set_journal()
+        self.on_change_party()
 
     @classmethod
     def _journal_types(cls, invoice_type):
         if invoice_type == 'out':
             return ['revenue']
         else:
             return ['expense']
 
-    @fields.depends('state', 'journal', 'type')
-    def on_change_with_journal(self, pattern=None):
+    @fields.depends('type')
+    def set_journal(self, pattern=None):
         pool = Pool()
         Journal = pool.get('account.journal')
-        if self.state != 'draft':
-            return self.journal
         pattern = pattern.copy() if pattern is not None else {}
         pattern.setdefault('type', {
                 'out': 'revenue',
                 'in': 'expense',
                 }.get(self.type))
-        return Journal.find(pattern)
+        self.journal = Journal.find(pattern)
 
     @classmethod
     def order_accounting_date(cls, tables):
         table, _ = tables[None]
         return [Coalesce(table.accounting_date, table.invoice_date)]
 
-    @fields.depends('party', 'type')
+    @fields.depends('party', 'type', methods=['_update_account'])
     def on_change_party(self):
         self.invoice_address = None
         if self.party:
             self.invoice_address = self.party.address_get(type='invoice')
             self.party_tax_identifier = self.party.tax_identifier
             if self.type == 'out':
+                self.account = self.party.account_receivable_used
                 self.payment_term = self.party.customer_payment_term
             elif self.type == 'in':
+                self.account = self.party.account_payable_used
                 self.payment_term = self.party.supplier_payment_term
         else:
             self.payment_term = None
+            self.account = None
+        self._update_account()
+
+    @fields.depends(methods=['_update_account'])
+    def on_change_accounting_date(self):
+        self._update_account()
+
+    @fields.depends(methods=['_update_account'])
+    def on_change_invoice_date(self):
+        self._update_account()
+
+    @fields.depends('account', 'accounting_date', 'invoice_date')
+    def _update_account(self):
+        "Update account to current account"
+        if self.account:
+            account = self.account.current(
+                date=self.accounting_date or self.invoice_date)
+            if account != self.account:
+                self.account = account
 
     @fields.depends('invoice_date', 'company')
     def on_change_with_currency_date(self, name=None):
         Date = Pool().get('ir.date')
         if self.company:
             company_id = self.company.id
         else:
```

### Comparing `trytond_account_invoice-6.8.0/invoice.xml` & `trytond_account_invoice-6.8.1/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/bg.po` & `trytond_account_invoice-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/ca.po` & `trytond_account_invoice-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/cs.po` & `trytond_account_invoice-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/de.po` & `trytond_account_invoice-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/es.po` & `trytond_account_invoice-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/es_419.po` & `trytond_account_invoice-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/et.po` & `trytond_account_invoice-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/fa.po` & `trytond_account_invoice-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/fi.po` & `trytond_account_invoice-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/fr.po` & `trytond_account_invoice-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/hu.po` & `trytond_account_invoice-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/id.po` & `trytond_account_invoice-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/it.po` & `trytond_account_invoice-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/lo.po` & `trytond_account_invoice-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/lt.po` & `trytond_account_invoice-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/nl.po` & `trytond_account_invoice-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/pl.po` & `trytond_account_invoice-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/pt.po` & `trytond_account_invoice-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/ro.po` & `trytond_account_invoice-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/ru.po` & `trytond_account_invoice-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/sl.po` & `trytond_account_invoice-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/tr.po` & `trytond_account_invoice-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/uk.po` & `trytond_account_invoice-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/locale/zh_CN.po` & `trytond_account_invoice-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/message.xml` & `trytond_account_invoice-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/party.py` & `trytond_account_invoice-6.8.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/party.xml` & `trytond_account_invoice-6.8.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/payment_term.py` & `trytond_account_invoice-6.8.1/payment_term.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/payment_term.xml` & `trytond_account_invoice-6.8.1/payment_term.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/setup.py` & `trytond_account_invoice-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_cancelling_invoice_move.rst` & `trytond_account_invoice-6.8.1/tests/scenario_cancelling_invoice_move.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_credit_note.rst` & `trytond_account_invoice-6.8.1/tests/scenario_credit_note.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_alternate_currency.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_alternate_currency.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_alternate_currency_lower_rate.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_alternate_currency_lower_rate.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_alternate_currency_rate_change.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_alternate_currency_rate_change.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_alternative_payee.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_alternative_payee.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_customer_sequential.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_customer_sequential.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_group_line.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_group_line.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_in_future.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_in_future.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_manual_tax.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_manual_tax.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_overpayment.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_overpayment.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_reschedule_lines.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_reschedule_lines.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_supplier.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_supplier.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_supplier_post_paid.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_supplier_post_paid.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_tax_deductible.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_tax_deductible.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_invoice_with_credit.rst` & `trytond_account_invoice-6.8.1/tests/scenario_invoice_with_credit.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/scenario_renew_fiscalyear.rst` & `trytond_account_invoice-6.8.1/tests/scenario_renew_fiscalyear.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/test_module.py` & `trytond_account_invoice-6.8.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tests/tools.py` & `trytond_account_invoice-6.8.1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/tox.ini` & `trytond_account_invoice-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/PKG-INFO` & `trytond_account_invoice-6.8.1/trytond_account_invoice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-account-invoice
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module for invoicing
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_invoice-6.8.0/trytond_account_invoice.egg-info/SOURCES.txt` & `trytond_account_invoice-6.8.1/trytond_account_invoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/credit_start_form.xml` & `trytond_account_invoice-6.8.1/view/credit_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/invoice_form.xml` & `trytond_account_invoice-6.8.1/view/invoice_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/invoice_line_form.xml` & `trytond_account_invoice-6.8.1/view/invoice_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/invoice_line_tree.xml` & `trytond_account_invoice-6.8.1/view/invoice_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/invoice_line_tree_sequence.xml` & `trytond_account_invoice-6.8.1/view/invoice_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/invoice_sequence_form.xml` & `trytond_account_invoice-6.8.1/view/invoice_sequence_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/invoice_tax_form.xml` & `trytond_account_invoice-6.8.1/view/invoice_tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/invoice_tax_tree_sequence.xml` & `trytond_account_invoice-6.8.1/view/invoice_tax_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/invoice_tree.xml` & `trytond_account_invoice-6.8.1/view/invoice_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/party_form.xml` & `trytond_account_invoice-6.8.1/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/pay_ask_form.xml` & `trytond_account_invoice-6.8.1/view/pay_ask_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/pay_start_form.xml` & `trytond_account_invoice-6.8.1/view/pay_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/payment_method_form.xml` & `trytond_account_invoice-6.8.1/view/payment_method_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/payment_term_form.xml` & `trytond_account_invoice-6.8.1/view/payment_term_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/payment_term_line_form.xml` & `trytond_account_invoice-6.8.1/view/payment_term_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-6.8.0/view/payment_term_line_relativedelta_form.xml` & `trytond_account_invoice-6.8.1/view/payment_term_line_relativedelta_form.xml`

 * *Files identical despite different names*

