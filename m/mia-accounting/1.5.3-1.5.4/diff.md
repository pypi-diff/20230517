# Comparing `tmp/mia-accounting-1.5.3.tar.gz` & `tmp/mia-accounting-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia-accounting-1.5.3.tar", last modified: Sun Apr 30 07:07:32 2023, max compression
+gzip compressed data, was "mia-accounting-1.5.4.tar", last modified: Wed May 17 16:11:23 2023, max compression
```

## Comparing `mia-accounting-1.5.3.tar` & `mia-accounting-1.5.4.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.849173 mia-accounting-1.5.3/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.5.3/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.5.3/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-04-30 07:07:32.849173 mia-accounting-1.5.3/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     2525 2023-04-23 12:04:20.000000 mia-accounting-1.5.3/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.809174 mia-accounting-1.5.3/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.5.3/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.5.3/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.813174 mia-accounting-1.5.3/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.813174 mia-accounting-1.5.3/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.5.3/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.813174 mia-accounting-1.5.3/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.5.3/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-18 01:25:56.000000 mia-accounting-1.5.3/docs/source/accounting.account.rst
--rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-18 01:25:56.000000 mia-accounting-1.5.3/docs/source/accounting.base_account.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-18 01:25:56.000000 mia-accounting-1.5.3/docs/source/accounting.currency.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-18 01:25:56.000000 mia-accounting-1.5.3/docs/source/accounting.journal_entry.forms.rst
--rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-18 01:25:56.000000 mia-accounting-1.5.3/docs/source/accounting.journal_entry.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-18 01:25:56.000000 mia-accounting-1.5.3/docs/source/accounting.journal_entry.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-18 01:25:56.000000 mia-accounting-1.5.3/docs/source/accounting.option.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-18 01:25:56.000000 mia-accounting-1.5.3/docs/source/accounting.report.period.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-04-18 01:32:44.000000 mia-accounting-1.5.3/docs/source/accounting.report.reports.rst
--rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-18 01:25:56.000000 mia-accounting-1.5.3/docs/source/accounting.report.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2168 2023-04-18 01:32:44.000000 mia-accounting-1.5.3/docs/source/accounting.report.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1301 2023-04-18 01:32:44.000000 mia-accounting-1.5.3/docs/source/accounting.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2405 2023-04-18 01:32:44.000000 mia-accounting-1.5.3/docs/source/accounting.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     7777 2023-04-30 07:07:07.000000 mia-accounting-1.5.3/docs/source/changelog.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1051 2023-04-23 12:12:53.000000 mia-accounting-1.5.3/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.5.3/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.5.3/docs/source/history.rst
--rw-r--r--   0 imacat    (1000) users      (100)      521 2023-04-23 12:04:21.000000 mia-accounting-1.5.3/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     3462 2023-04-23 12:13:33.000000 mia-accounting-1.5.3/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.5.3/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1994 2023-04-23 12:12:53.000000 mia-accounting-1.5.3/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-30 07:07:32.849173 mia-accounting-1.5.3/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.797174 mia-accounting-1.5.3/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.817174 mia-accounting-1.5.3/src/accounting/
--rw-r--r--   0 imacat    (1000) users      (100)     3045 2023-04-30 07:05:40.000000 mia-accounting-1.5.3/src/accounting/__init__.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.817174 mia-accounting-1.5.3/src/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.5.3/src/accounting/account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-29 21:45:45.000000 mia-accounting-1.5.3/src/accounting/account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.5.3/src/accounting/account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.5.3/src/accounting/account/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.5.3/src/accounting/account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.5.3/src/accounting/account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.821174 mia-accounting-1.5.3/src/accounting/base_account/
--rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.5.3/src/accounting/base_account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.5.3/src/accounting/base_account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.5.3/src/accounting/base_account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.5.3/src/accounting/base_account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.5.3/src/accounting/base_account/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.5.3/src/accounting/commands.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.821174 mia-accounting-1.5.3/src/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.5.3/src/accounting/currency/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2206 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/currency/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.5.3/src/accounting/currency/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.5.3/src/accounting/currency/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.5.3/src/accounting/currency/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.5.3/src/accounting/currency/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.821174 mia-accounting-1.5.3/src/accounting/data/
--rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.5.3/src/accounting/data/base_accounts.csv
--rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.5.3/src/accounting/data/currencies.csv
--rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.5.3/src/accounting/forms.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.821174 mia-accounting-1.5.3/src/accounting/journal_entry/
--rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.5.3/src/accounting/journal_entry/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3302 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/journal_entry/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.821174 mia-accounting-1.5.3/src/accounting/journal_entry/forms/
--rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.5.3/src/accounting/journal_entry/forms/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    11003 2023-04-23 05:21:41.000000 mia-accounting-1.5.3/src/accounting/journal_entry/forms/currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    24568 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/journal_entry/forms/journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    19807 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/journal_entry/forms/line_item.py
--rw-r--r--   0 imacat    (1000) users      (100)     3291 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/journal_entry/forms/reorder.py
--rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.5.3/src/accounting/journal_entry/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.825173 mia-accounting-1.5.3/src/accounting/journal_entry/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.5.3/src/accounting/journal_entry/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1802 2023-04-17 23:37:17.000000 mia-accounting-1.5.3/src/accounting/journal_entry/utils/account_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    12981 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/journal_entry/utils/description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)    12676 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/journal_entry/utils/operators.py
--rw-r--r--   0 imacat    (1000) users      (100)     3722 2023-04-23 05:21:41.000000 mia-accounting-1.5.3/src/accounting/journal_entry/utils/original_line_items.py
--rw-r--r--   0 imacat    (1000) users      (100)     9351 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/journal_entry/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.5.3/src/accounting/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    32618 2023-04-30 07:03:58.000000 mia-accounting-1.5.3/src/accounting/models.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.825173 mia-accounting-1.5.3/src/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.5.3/src/accounting/option/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.5.3/src/accounting/option/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.5.3/src/accounting/option/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.825173 mia-accounting-1.5.3/src/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.5.3/src/accounting/report/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.5.3/src/accounting/report/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.825173 mia-accounting-1.5.3/src/accounting/report/period/
--rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.5.3/src/accounting/report/period/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3702 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/period/chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     5557 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/period/description.py
--rw-r--r--   0 imacat    (1000) users      (100)     1050 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/period/month_end.py
--rw-r--r--   0 imacat    (1000) users      (100)     4127 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/period/parser.py
--rw-r--r--   0 imacat    (1000) users      (100)     4522 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/period/period.py
--rw-r--r--   0 imacat    (1000) users      (100)     4785 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/period/shortcuts.py
--rw-r--r--   0 imacat    (1000) users      (100)     3915 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/period/specification.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.829173 mia-accounting-1.5.3/src/accounting/report/reports/
--rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.5.3/src/accounting/report/reports/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.5.3/src/accounting/report/reports/balance_sheet.py
--rw-r--r--   0 imacat    (1000) users      (100)    18807 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/reports/income_expenses.py
--rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.5.3/src/accounting/report/reports/income_statement.py
--rw-r--r--   0 imacat    (1000) users      (100)     8130 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/reports/journal.py
--rw-r--r--   0 imacat    (1000) users      (100)    16530 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/reports/ledger.py
--rw-r--r--   0 imacat    (1000) users      (100)     8472 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/reports/search.py
--rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.5.3/src/accounting/report/reports/trial_balance.py
--rw-r--r--   0 imacat    (1000) users      (100)     8099 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/reports/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     5210 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/reports/unapplied_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     8169 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/reports/unmatched.py
--rw-r--r--   0 imacat    (1000) users      (100)     5191 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/reports/unmatched_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.5.3/src/accounting/report/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.829173 mia-accounting-1.5.3/src/accounting/report/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.5.3/src/accounting/report/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/utils/base_page_params.py
--rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.5.3/src/accounting/report/utils/base_report.py
--rw-r--r--   0 imacat    (1000) users      (100)     3334 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/utils/csv_export.py
--rw-r--r--   0 imacat    (1000) users      (100)     7321 2023-04-29 22:38:16.000000 mia-accounting-1.5.3/src/accounting/report/utils/offset_matcher.py
--rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.5.3/src/accounting/report/utils/option_link.py
--rw-r--r--   0 imacat    (1000) users      (100)     7881 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/report/utils/report_chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     1371 2023-04-17 08:41:57.000000 mia-accounting-1.5.3/src/accounting/report/utils/report_type.py
--rw-r--r--   0 imacat    (1000) users      (100)     4385 2023-04-23 05:21:41.000000 mia-accounting-1.5.3/src/accounting/report/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     2221 2023-04-23 05:21:41.000000 mia-accounting-1.5.3/src/accounting/report/utils/unmatched.py
--rw-r--r--   0 imacat    (1000) users      (100)     5440 2023-04-18 00:59:05.000000 mia-accounting-1.5.3/src/accounting/report/utils/urls.py
--rw-r--r--   0 imacat    (1000) users      (100)    14167 2023-04-18 01:14:44.000000 mia-accounting-1.5.3/src/accounting/report/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.793174 mia-accounting-1.5.3/src/accounting/static/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.829173 mia-accounting-1.5.3/src/accounting/static/css/
--rw-r--r--   0 imacat    (1000) users      (100)    13431 2023-04-18 00:10:33.000000 mia-accounting-1.5.3/src/accounting/static/css/style.css
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.833173 mia-accounting-1.5.3/src/accounting/static/js/
--rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.5.3/src/accounting/static/js/account-form.js
--rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.5.3/src/accounting/static/js/account-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.5.3/src/accounting/static/js/currency-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    38865 2023-04-17 23:44:56.000000 mia-accounting-1.5.3/src/accounting/static/js/description-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.5.3/src/accounting/static/js/drag-and-drop-reorder.js
--rw-r--r--   0 imacat    (1000) users      (100)     9211 2023-04-17 23:32:14.000000 mia-accounting-1.5.3/src/accounting/static/js/journal-entry-account-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    33086 2023-04-17 23:52:58.000000 mia-accounting-1.5.3/src/accounting/static/js/journal-entry-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    19665 2023-04-30 07:03:59.000000 mia-accounting-1.5.3/src/accounting/static/js/journal-entry-line-item-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.5.3/src/accounting/static/js/journal-entry-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.5.3/src/accounting/static/js/material-fab-speed-dial.js
--rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.5.3/src/accounting/static/js/option-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    11670 2023-04-17 23:40:31.000000 mia-accounting-1.5.3/src/accounting/static/js/original-line-item-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.5.3/src/accounting/static/js/period-chooser.js
--rw-r--r--   0 imacat    (1000) users      (100)     2712 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/template_filters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1137 2023-04-23 01:43:59.000000 mia-accounting-1.5.3/src/accounting/template_globals.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.793174 mia-accounting-1.5.3/src/accounting/templates/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.833173 mia-accounting-1.5.3/src/accounting/templates/accounting/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.833173 mia-accounting-1.5.3/src/accounting/templates/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/account/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/account/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.833173 mia-accounting-1.5.3/src/accounting/templates/accounting/account/include/
--rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/account/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/account/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.833173 mia-accounting-1.5.3/src/accounting/templates/accounting/base-account/
--rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/base-account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/base-account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/base.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.833173 mia-accounting-1.5.3/src/accounting/templates/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/currency/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/currency/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/currency/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.833173 mia-accounting-1.5.3/src/accounting/templates/accounting/currency/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/currency/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/currency/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.833173 mia-accounting-1.5.3/src/accounting/templates/accounting/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-17 15:07:31.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/include/nav.html
--rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/include/pagination.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.833173 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.833173 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/disbursement/
--rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/disbursement/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.833173 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/disbursement/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.837173 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3406 2023-04-17 23:32:14.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)    14492 2023-04-17 23:42:37.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3242 2023-04-17 23:11:57.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
--rw-r--r--   0 imacat    (1000) users      (100)     4554 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
--rw-r--r--   0 imacat    (1000) users      (100)     6442 2023-04-17 23:54:15.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
--rw-r--r--   0 imacat    (1000) users      (100)     3791 2023-04-18 00:10:33.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3069 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.837173 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/receipt/
--rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/receipt/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/receipt/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/receipt/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.837173 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/receipt/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.837173 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/transfer/
--rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/transfer/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/transfer/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/transfer/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.837173 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/transfer/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.837173 mia-accounting-1.5.3/src/accounting/templates/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/option/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/option/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.837173 mia-accounting-1.5.3/src/accounting/templates/accounting/option/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
--rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/option/include/form-recurring-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.841173 mia-accounting-1.5.3/src/accounting/templates/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     5435 2023-04-18 00:39:27.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/balance-sheet.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.841173 mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
--rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/balance-sheet-section.html
--rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/period-chooser.html
--rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/search-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     5600 2023-04-18 00:10:33.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/toolbar-buttons.html
--rw-r--r--   0 imacat    (1000) users      (100)     4841 2023-04-18 00:34:44.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/income-expenses.html
--rw-r--r--   0 imacat    (1000) users      (100)     4618 2023-04-18 00:37:47.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/income-statement.html
--rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/journal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4946 2023-04-18 00:33:38.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/ledger.html
--rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/search.html
--rw-r--r--   0 imacat    (1000) users      (100)     3710 2023-04-18 00:36:16.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/trial-balance.html
--rw-r--r--   0 imacat    (1000) users      (100)     3037 2023-04-18 00:59:05.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/unapplied-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     3843 2023-04-18 00:59:06.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/unapplied.html
--rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-18 00:59:05.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/unmatched-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     6998 2023-04-18 00:59:05.000000 mia-accounting-1.5.3/src/accounting/templates/accounting/report/unmatched.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.841173 mia-accounting-1.5.3/src/accounting/translations/
--rw-r--r--   0 imacat    (1000) users      (100)    49437 2023-04-18 01:32:01.000000 mia-accounting-1.5.3/src/accounting/translations/accounting.pot
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.5.3/src/accounting/translations/babel.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.797174 mia-accounting-1.5.3/src/accounting/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.841173 mia-accounting-1.5.3/src/accounting/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.3/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.3/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.797174 mia-accounting-1.5.3/src/accounting/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.841173 mia-accounting-1.5.3/src/accounting/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.3/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.3/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.845173 mia-accounting-1.5.3/src/accounting/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.5.3/src/accounting/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1058 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/utils/cast.py
--rw-r--r--   0 imacat    (1000) users      (100)     3363 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/utils/current_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     1426 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/utils/flash_errors.py
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.5.3/src/accounting/utils/journal_entry_types.py
--rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.5.3/src/accounting/utils/next_uri.py
--rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/utils/offset_alias.py
--rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.5.3/src/accounting/utils/options.py
--rw-r--r--   0 imacat    (1000) users      (100)    11745 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/utils/pagination.py
--rw-r--r--   0 imacat    (1000) users      (100)     4262 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/utils/permission.py
--rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.5.3/src/accounting/utils/query.py
--rw-r--r--   0 imacat    (1000) users      (100)     1221 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/utils/random_id.py
--rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.5.3/src/accounting/utils/strip_text.py
--rw-r--r--   0 imacat    (1000) users      (100)     4985 2023-04-29 21:45:46.000000 mia-accounting-1.5.3/src/accounting/utils/user.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.845173 mia-accounting-1.5.3/src/mia_accounting.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-04-30 07:07:32.000000 mia-accounting-1.5.3/src/mia_accounting.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    11434 2023-04-30 07:07:32.000000 mia-accounting-1.5.3/src/mia_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-30 07:07:32.000000 mia-accounting-1.5.3/src/mia_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)      107 2023-04-30 07:07:32.000000 mia-accounting-1.5.3/src/mia_accounting.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-30 07:07:32.000000 mia-accounting-1.5.3/src/mia_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.845173 mia-accounting-1.5.3/tests/
--rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.5.3/tests/babel-utils-test-site.py
--rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.5.3/tests/babel-utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    32727 2023-04-29 21:45:47.000000 mia-accounting-1.5.3/tests/test_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.5.3/tests/test_base_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-29 21:45:47.000000 mia-accounting-1.5.3/tests/test_commands.py
--rw-r--r--   0 imacat    (1000) users      (100)    23815 2023-04-29 21:45:47.000000 mia-accounting-1.5.3/tests/test_currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    15998 2023-04-29 21:45:47.000000 mia-accounting-1.5.3/tests/test_description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)   103428 2023-04-29 21:45:47.000000 mia-accounting-1.5.3/tests/test_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    38887 2023-04-13 01:09:51.000000 mia-accounting-1.5.3/tests/test_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    15940 2023-04-29 21:45:47.000000 mia-accounting-1.5.3/tests/test_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    17864 2023-04-29 21:45:47.000000 mia-accounting-1.5.3/tests/test_report.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.849173 mia-accounting-1.5.3/tests/test_site/
--rw-r--r--   0 imacat    (1000) users      (100)     4508 2023-04-29 21:45:47.000000 mia-accounting-1.5.3/tests/test_site/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3958 2023-04-29 21:45:47.000000 mia-accounting-1.5.3/tests/test_site/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)    13199 2023-04-29 21:45:47.000000 mia-accounting-1.5.3/tests/test_site/lib.py
--rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.5.3/tests/test_site/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    13050 2023-04-29 21:45:47.000000 mia-accounting-1.5.3/tests/test_site/reset.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.849173 mia-accounting-1.5.3/tests/test_site/static/
--rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.5.3/tests/test_site/static/favicon.svg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.849173 mia-accounting-1.5.3/tests/test_site/templates/
--rw-r--r--   0 imacat    (1000) users      (100)     6435 2023-04-12 10:05:13.000000 mia-accounting-1.5.3/tests/test_site/templates/base.html
--rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.5.3/tests/test_site/templates/home.html
--rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.5.3/tests/test_site/templates/login.html
--rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.5.3/tests/test_site/templates/reset.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.849173 mia-accounting-1.5.3/tests/test_site/translations/
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.5.3/tests/test_site/translations/babel.cfg
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.5.3/tests/test_site/translations/messages.pot
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.801174 mia-accounting-1.5.3/tests/test_site/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.849173 mia-accounting-1.5.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.5.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.801174 mia-accounting-1.5.3/tests/test_site/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-30 07:07:32.849173 mia-accounting-1.5.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.5.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0 imacat    (1000) users      (100)    27794 2023-04-18 01:14:44.000000 mia-accounting-1.5.3/tests/test_unmatched_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.5.3/tests/test_utils.py
--rw-r--r--   0 imacat    (1000) users      (100)     5175 2023-04-29 21:45:47.000000 mia-accounting-1.5.3/tests/testlib.py
--rw-r--r--   0 imacat    (1000) users      (100)    16669 2023-04-29 21:45:47.000000 mia-accounting-1.5.3/tests/testlib_journal_entry.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:23.422509 mia-accounting-1.5.4/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.5.4/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.5.4/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-05-17 16:11:23.418509 mia-accounting-1.5.4/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     2525 2023-04-23 12:04:20.000000 mia-accounting-1.5.4/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.566549 mia-accounting-1.5.4/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.5.4/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.5.4/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.838531 mia-accounting-1.5.4/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.894530 mia-accounting-1.5.4/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.5.4/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.894530 mia-accounting-1.5.4/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.5.4/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.base_account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.currency.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.journal_entry.forms.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.journal_entry.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.journal_entry.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.option.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.report.period.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-04-18 01:32:44.000000 mia-accounting-1.5.4/docs/source/accounting.report.reports.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.report.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2168 2023-04-18 01:32:44.000000 mia-accounting-1.5.4/docs/source/accounting.report.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1301 2023-04-18 01:32:44.000000 mia-accounting-1.5.4/docs/source/accounting.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2405 2023-04-18 01:32:44.000000 mia-accounting-1.5.4/docs/source/accounting.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     8083 2023-05-17 16:05:22.000000 mia-accounting-1.5.4/docs/source/changelog.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1051 2023-04-23 12:12:53.000000 mia-accounting-1.5.4/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.5.4/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.5.4/docs/source/history.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      521 2023-04-23 12:04:21.000000 mia-accounting-1.5.4/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     3568 2023-05-06 15:58:29.000000 mia-accounting-1.5.4/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.5.4/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1994 2023-05-09 00:42:23.000000 mia-accounting-1.5.4/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-05-17 16:11:23.422509 mia-accounting-1.5.4/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.898530 mia-accounting-1.5.4/src/accounting/
+-rw-r--r--   0 imacat    (1000) users      (100)     3045 2023-05-17 14:58:29.000000 mia-accounting-1.5.4/src/accounting/__init__.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.902530 mia-accounting-1.5.4/src/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.5.4/src/accounting/account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-29 21:45:45.000000 mia-accounting-1.5.4/src/accounting/account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.5.4/src/accounting/account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.5.4/src/accounting/account/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.5.4/src/accounting/account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.5.4/src/accounting/account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.902530 mia-accounting-1.5.4/src/accounting/base_account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.5.4/src/accounting/base_account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.5.4/src/accounting/base_account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.5.4/src/accounting/base_account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.5.4/src/accounting/base_account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.5.4/src/accounting/base_account/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.5.4/src/accounting/commands.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.906530 mia-accounting-1.5.4/src/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.5.4/src/accounting/currency/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2206 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/currency/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.5.4/src/accounting/currency/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.5.4/src/accounting/currency/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.5.4/src/accounting/currency/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.5.4/src/accounting/currency/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.906530 mia-accounting-1.5.4/src/accounting/data/
+-rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.5.4/src/accounting/data/base_accounts.csv
+-rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.5.4/src/accounting/data/currencies.csv
+-rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.5.4/src/accounting/forms.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.910530 mia-accounting-1.5.4/src/accounting/journal_entry/
+-rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.5.4/src/accounting/journal_entry/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3302 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.914530 mia-accounting-1.5.4/src/accounting/journal_entry/forms/
+-rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.5.4/src/accounting/journal_entry/forms/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11003 2023-04-23 05:21:41.000000 mia-accounting-1.5.4/src/accounting/journal_entry/forms/currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24568 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/forms/journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    19807 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/forms/line_item.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3291 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/forms/reorder.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.5.4/src/accounting/journal_entry/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.914530 mia-accounting-1.5.4/src/accounting/journal_entry/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.5.4/src/accounting/journal_entry/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1802 2023-04-17 23:37:17.000000 mia-accounting-1.5.4/src/accounting/journal_entry/utils/account_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12981 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/utils/description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12676 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/utils/operators.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3722 2023-04-23 05:21:41.000000 mia-accounting-1.5.4/src/accounting/journal_entry/utils/original_line_items.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9351 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.5.4/src/accounting/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32618 2023-04-30 07:03:58.000000 mia-accounting-1.5.4/src/accounting/models.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.918530 mia-accounting-1.5.4/src/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.5.4/src/accounting/option/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.5.4/src/accounting/option/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.5.4/src/accounting/option/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.918530 mia-accounting-1.5.4/src/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.5.4/src/accounting/report/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.5.4/src/accounting/report/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.922530 mia-accounting-1.5.4/src/accounting/report/period/
+-rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.5.4/src/accounting/report/period/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3702 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5557 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/description.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1050 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/month_end.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4127 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/parser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4522 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/period.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4785 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/shortcuts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3915 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/specification.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.926530 mia-accounting-1.5.4/src/accounting/report/reports/
+-rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.5.4/src/accounting/report/reports/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.5.4/src/accounting/report/reports/balance_sheet.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18807 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/income_expenses.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.5.4/src/accounting/report/reports/income_statement.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8130 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/journal.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16530 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/ledger.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8472 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/search.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.5.4/src/accounting/report/reports/trial_balance.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8099 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5210 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/unapplied_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8169 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5191 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/unmatched_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.5.4/src/accounting/report/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.926530 mia-accounting-1.5.4/src/accounting/report/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.5.4/src/accounting/report/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/utils/base_page_params.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.5.4/src/accounting/report/utils/base_report.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3334 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/utils/csv_export.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7321 2023-04-29 22:38:16.000000 mia-accounting-1.5.4/src/accounting/report/utils/offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.5.4/src/accounting/report/utils/option_link.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7881 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/utils/report_chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1371 2023-04-17 08:41:57.000000 mia-accounting-1.5.4/src/accounting/report/utils/report_type.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4385 2023-04-23 05:21:41.000000 mia-accounting-1.5.4/src/accounting/report/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2221 2023-04-23 05:21:41.000000 mia-accounting-1.5.4/src/accounting/report/utils/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5440 2023-04-18 00:59:05.000000 mia-accounting-1.5.4/src/accounting/report/utils/urls.py
+-rw-r--r--   0 imacat    (1000) users      (100)    14167 2023-04-18 01:14:44.000000 mia-accounting-1.5.4/src/accounting/report/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/src/accounting/static/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.930530 mia-accounting-1.5.4/src/accounting/static/css/
+-rw-r--r--   0 imacat    (1000) users      (100)    13431 2023-04-18 00:10:33.000000 mia-accounting-1.5.4/src/accounting/static/css/style.css
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.930530 mia-accounting-1.5.4/src/accounting/static/js/
+-rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/account-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/account-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/currency-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    38865 2023-04-17 23:44:56.000000 mia-accounting-1.5.4/src/accounting/static/js/description-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/drag-and-drop-reorder.js
+-rw-r--r--   0 imacat    (1000) users      (100)     9211 2023-04-17 23:32:14.000000 mia-accounting-1.5.4/src/accounting/static/js/journal-entry-account-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    33086 2023-04-17 23:52:58.000000 mia-accounting-1.5.4/src/accounting/static/js/journal-entry-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    19665 2023-04-30 07:03:59.000000 mia-accounting-1.5.4/src/accounting/static/js/journal-entry-line-item-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/journal-entry-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/material-fab-speed-dial.js
+-rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/option-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    11670 2023-04-17 23:40:31.000000 mia-accounting-1.5.4/src/accounting/static/js/original-line-item-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/period-chooser.js
+-rw-r--r--   0 imacat    (1000) users      (100)     2712 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/template_filters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1137 2023-04-23 01:43:59.000000 mia-accounting-1.5.4/src/accounting/template_globals.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/src/accounting/templates/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.930530 mia-accounting-1.5.4/src/accounting/templates/accounting/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/account/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/account/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/account/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/account/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2734 2023-05-17 13:41:19.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/account/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/base-account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/base-account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2095 2023-05-17 13:41:20.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/base-account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/base.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2606 2023-05-17 13:41:19.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-17 15:07:31.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/include/nav.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/include/pagination.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/
+-rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.938529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3406 2023-04-17 23:32:14.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)    14521 2023-05-17 13:55:39.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3242 2023-04-17 23:11:57.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4554 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6442 2023-04-17 23:54:15.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4191 2023-05-17 13:55:40.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3791 2023-04-18 00:10:33.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3069 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.938529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/
+-rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.938529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.938529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/
+-rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.942529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.942529 mia-accounting-1.5.4/src/accounting/templates/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/option/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/option/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.942529 mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/form-recurring-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4305 2023-05-17 13:55:39.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.942529 mia-accounting-1.5.4/src/accounting/templates/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     5435 2023-04-18 00:39:27.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/balance-sheet.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.942529 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/balance-sheet-section.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/period-chooser.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1963 2023-05-17 13:41:20.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/search-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     5630 2023-05-17 13:41:20.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/toolbar-buttons.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4841 2023-04-18 00:34:44.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/income-expenses.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4618 2023-04-18 00:37:47.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/income-statement.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/journal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4946 2023-04-18 00:33:38.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/ledger.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/search.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3710 2023-04-18 00:36:16.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/trial-balance.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3037 2023-04-18 00:59:05.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/unapplied-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3843 2023-04-18 00:59:06.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/unapplied.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-18 00:59:05.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/unmatched-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6998 2023-04-18 00:59:05.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/unmatched.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.186526 mia-accounting-1.5.4/src/accounting/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)    49437 2023-04-18 01:32:01.000000 mia-accounting-1.5.4/src/accounting/translations/accounting.pot
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.5.4/src/accounting/translations/babel.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/src/accounting/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.286525 mia-accounting-1.5.4/src/accounting/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.4/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.4/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/src/accounting/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.542521 mia-accounting-1.5.4/src/accounting/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.4/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.4/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.754518 mia-accounting-1.5.4/src/accounting/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.5.4/src/accounting/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1036 2023-05-17 07:33:36.000000 mia-accounting-1.5.4/src/accounting/utils/cast.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3325 2023-05-04 01:35:20.000000 mia-accounting-1.5.4/src/accounting/utils/current_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1426 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/utils/flash_errors.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.5.4/src/accounting/utils/journal_entry_types.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3086 2023-05-17 08:11:10.000000 mia-accounting-1.5.4/src/accounting/utils/next_uri.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/utils/offset_alias.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.5.4/src/accounting/utils/options.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11745 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/utils/pagination.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4262 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/utils/permission.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.5.4/src/accounting/utils/query.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1221 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/utils/random_id.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.5.4/src/accounting/utils/strip_text.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4985 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/utils/user.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.754518 mia-accounting-1.5.4/src/mia_accounting.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-05-17 16:11:20.000000 mia-accounting-1.5.4/src/mia_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)    11434 2023-05-17 16:11:20.000000 mia-accounting-1.5.4/src/mia_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-05-17 16:11:20.000000 mia-accounting-1.5.4/src/mia_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)      107 2023-05-17 16:11:20.000000 mia-accounting-1.5.4/src/mia_accounting.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       11 2023-05-17 16:11:20.000000 mia-accounting-1.5.4/src/mia_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.762518 mia-accounting-1.5.4/tests/
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.5.4/tests/babel-utils-test-site.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.5.4/tests/babel-utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32727 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.5.4/tests/test_base_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)    23815 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15998 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)   103433 2023-05-17 16:04:33.000000 mia-accounting-1.5.4/tests/test_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    38887 2023-04-13 01:09:51.000000 mia-accounting-1.5.4/tests/test_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15940 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17864 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_report.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.762518 mia-accounting-1.5.4/tests/test_site/
+-rw-r--r--   0 imacat    (1000) users      (100)     4589 2023-05-17 11:57:24.000000 mia-accounting-1.5.4/tests/test_site/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3958 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_site/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13199 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_site/lib.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3367 2023-05-17 11:57:23.000000 mia-accounting-1.5.4/tests/test_site/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13050 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_site/reset.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.762518 mia-accounting-1.5.4/tests/test_site/static/
+-rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.5.4/tests/test_site/static/favicon.svg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.834517 mia-accounting-1.5.4/tests/test_site/templates/
+-rw-r--r--   0 imacat    (1000) users      (100)     6435 2023-05-06 15:53:46.000000 mia-accounting-1.5.4/tests/test_site/templates/base.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.5.4/tests/test_site/templates/home.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.5.4/tests/test_site/templates/login.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.5.4/tests/test_site/templates/reset.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.986515 mia-accounting-1.5.4/tests/test_site/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.5.4/tests/test_site/translations/babel.cfg
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.5.4/tests/test_site/translations/messages.pot
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/tests/test_site/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:23.162512 mia-accounting-1.5.4/tests/test_site/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.4/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.5.4/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/tests/test_site/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:23.378509 mia-accounting-1.5.4/tests/test_site/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.4/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.5.4/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0 imacat    (1000) users      (100)    27794 2023-04-18 01:14:44.000000 mia-accounting-1.5.4/tests/test_unmatched_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16216 2023-05-17 08:26:34.000000 mia-accounting-1.5.4/tests/test_utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5175 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/testlib.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16669 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/testlib_journal_entry.py
```

### Comparing `mia-accounting-1.5.3/LICENSE` & `mia-accounting-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/MANIFEST.in` & `mia-accounting-1.5.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/PKG-INFO` & `mia-accounting-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
```

### Comparing `mia-accounting-1.5.3/README.rst` & `mia-accounting-1.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/Makefile` & `mia-accounting-1.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/make.bat` & `mia-accounting-1.5.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/accounting.account.rst` & `mia-accounting-1.5.4/docs/source/accounting.account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/accounting.base_account.rst` & `mia-accounting-1.5.4/docs/source/accounting.base_account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/accounting.currency.rst` & `mia-accounting-1.5.4/docs/source/accounting.currency.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/accounting.journal_entry.forms.rst` & `mia-accounting-1.5.4/docs/source/accounting.journal_entry.forms.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/accounting.journal_entry.rst` & `mia-accounting-1.5.4/docs/source/accounting.journal_entry.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/accounting.journal_entry.utils.rst` & `mia-accounting-1.5.4/docs/source/accounting.journal_entry.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/accounting.option.rst` & `mia-accounting-1.5.4/docs/source/accounting.option.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/accounting.report.period.rst` & `mia-accounting-1.5.4/docs/source/accounting.report.period.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/accounting.report.reports.rst` & `mia-accounting-1.5.4/docs/source/accounting.report.reports.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/accounting.report.rst` & `mia-accounting-1.5.4/docs/source/accounting.report.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/accounting.report.utils.rst` & `mia-accounting-1.5.4/docs/source/accounting.report.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/accounting.rst` & `mia-accounting-1.5.4/docs/source/accounting.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/accounting.utils.rst` & `mia-accounting-1.5.4/docs/source/accounting.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/changelog.rst` & `mia-accounting-1.5.4/docs/source/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 Change Log
 ==========
 
 
+Version 1.5.4
+-------------
+
+Released 2023/5/18
+
+Security fixes.
+
+* Added safeguard to the next URI utilities, to prevent Cross-Site
+  Scripting (XSS) attacks.
+* Applied the safe next URI utilities to the test site.
+* Added the ``SameSite`` and ``Secure`` flags to the session cookie
+  of the test site.
+
+
 Version 1.5.3
 -------------
 
 Released 2023/4/30
 
 * Fixed the error of the net balance in the unmatched offset list.
 * Revised the original line item editor not to override the existing
```

### Comparing `mia-accounting-1.5.3/docs/source/conf.py` & `mia-accounting-1.5.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/examples.rst` & `mia-accounting-1.5.4/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/history.rst` & `mia-accounting-1.5.4/docs/source/history.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/index.rst` & `mia-accounting-1.5.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/docs/source/intro.rst` & `mia-accounting-1.5.4/docs/source/intro.rst`

 * *Files 6% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 The primary key of the user data model must be integer.  You also
 need at least one user.
 
 The following front-end JavaScript libraries must be loaded.  You may
 download it locally or use CDN_.
 
 * Bootstrap_ 5.2.3 or above
-* FontAwesome_ 6.2.1 or above
-* `Decimal.js`_ 6.4.3 or above
-* `Tempus-Dominus`_ 6.4.3 or above
+* FontAwesome_ 6.4.0 or above
+* `decimal.js`_ 10.4.3 or above, or `decimal.js-light`_ 2.5.1 or above.
+* `Tempus-Dominus`_ 6.7.7 or above
 
 
 Configuration
 -------------
 
 You need to pass the Flask *app* and an implementation of
 :py:class:`accounting.utils.user.UserUtilityInterface` to the
@@ -110,10 +110,11 @@
 .. _source distribution: https://pypi.org/project/mia-accounting/#files
 .. _PyPI project page: https://pypi.org/project/mia-accounting
 .. _release page: https://github.com/imacat/mia-accounting/releases
 .. _Git repository: https://github.com/imacat/mia-accounting
 .. _CDN: https://en.wikipedia.org/wiki/Content_delivery_network
 .. _Bootstrap: https://getbootstrap.com
 .. _FontAwesome: https://fontawesome.com
-.. _Decimal.js: https://mikemcl.github.io/decimal.js
+.. _decimal.js: https://mikemcl.github.io/decimal.js
+.. _decimal.js-light: https://mikemcl.github.io/decimal.js-light
 .. _Tempus-Dominus: https://getdatepicker.com
 .. _Bootstrap navigation bar: https://getbootstrap.com/docs/5.3/components/navbar/
```

### Comparing `mia-accounting-1.5.3/pyproject.toml` & `mia-accounting-1.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/__init__.py` & `mia-accounting-1.5.4/src/accounting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pathlib import Path
 
 from flask import Flask, Blueprint
 from flask_sqlalchemy import SQLAlchemy
 
 from accounting.utils.user import UserUtilityInterface
 
-VERSION: str = "1.5.3"
+VERSION: str = "1.5.4"
 """The package version."""
 db: SQLAlchemy = SQLAlchemy()
 """The database instance."""
 data_dir: Path = Path(__file__).parent / "data"
 """The data directory."""
```

### Comparing `mia-accounting-1.5.3/src/accounting/account/__init__.py` & `mia-accounting-1.5.4/src/accounting/account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/account/commands.py` & `mia-accounting-1.5.4/src/accounting/account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/account/converters.py` & `mia-accounting-1.5.4/src/accounting/account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/account/forms.py` & `mia-accounting-1.5.4/src/accounting/account/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/account/queries.py` & `mia-accounting-1.5.4/src/accounting/account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/account/views.py` & `mia-accounting-1.5.4/src/accounting/account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/base_account/__init__.py` & `mia-accounting-1.5.4/src/accounting/base_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/base_account/commands.py` & `mia-accounting-1.5.4/src/accounting/base_account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/base_account/converters.py` & `mia-accounting-1.5.4/src/accounting/base_account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/base_account/queries.py` & `mia-accounting-1.5.4/src/accounting/base_account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/base_account/views.py` & `mia-accounting-1.5.4/src/accounting/base_account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/commands.py` & `mia-accounting-1.5.4/src/accounting/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/currency/__init__.py` & `mia-accounting-1.5.4/src/accounting/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/currency/commands.py` & `mia-accounting-1.5.4/src/accounting/currency/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/currency/converters.py` & `mia-accounting-1.5.4/src/accounting/currency/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/currency/forms.py` & `mia-accounting-1.5.4/src/accounting/currency/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/currency/queries.py` & `mia-accounting-1.5.4/src/accounting/currency/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/currency/views.py` & `mia-accounting-1.5.4/src/accounting/currency/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/data/base_accounts.csv` & `mia-accounting-1.5.4/src/accounting/data/base_accounts.csv`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/forms.py` & `mia-accounting-1.5.4/src/accounting/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/__init__.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/converters.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/forms/__init__.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/forms/currency.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/forms/currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/forms/journal_entry.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/forms/journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/forms/line_item.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/forms/line_item.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/forms/reorder.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/forms/reorder.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/template_filters.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/utils/__init__.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/utils/account_option.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/utils/account_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/utils/description_editor.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/utils/description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/utils/operators.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/utils/operators.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/utils/original_line_items.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/utils/original_line_items.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/journal_entry/views.py` & `mia-accounting-1.5.4/src/accounting/journal_entry/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/locale.py` & `mia-accounting-1.5.4/src/accounting/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/models.py` & `mia-accounting-1.5.4/src/accounting/models.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/option/__init__.py` & `mia-accounting-1.5.4/src/accounting/option/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/option/forms.py` & `mia-accounting-1.5.4/src/accounting/option/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/option/views.py` & `mia-accounting-1.5.4/src/accounting/option/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/__init__.py` & `mia-accounting-1.5.4/src/accounting/report/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/converters.py` & `mia-accounting-1.5.4/src/accounting/report/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/period/__init__.py` & `mia-accounting-1.5.4/src/accounting/report/period/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/period/chooser.py` & `mia-accounting-1.5.4/src/accounting/report/period/chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/period/description.py` & `mia-accounting-1.5.4/src/accounting/report/period/description.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/period/month_end.py` & `mia-accounting-1.5.4/src/accounting/report/period/month_end.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/period/parser.py` & `mia-accounting-1.5.4/src/accounting/report/period/parser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/period/period.py` & `mia-accounting-1.5.4/src/accounting/report/period/period.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/period/shortcuts.py` & `mia-accounting-1.5.4/src/accounting/report/period/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/period/specification.py` & `mia-accounting-1.5.4/src/accounting/report/period/specification.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/reports/__init__.py` & `mia-accounting-1.5.4/src/accounting/report/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/reports/balance_sheet.py` & `mia-accounting-1.5.4/src/accounting/report/reports/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/reports/income_expenses.py` & `mia-accounting-1.5.4/src/accounting/report/reports/income_expenses.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/reports/income_statement.py` & `mia-accounting-1.5.4/src/accounting/report/reports/income_statement.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/reports/journal.py` & `mia-accounting-1.5.4/src/accounting/report/reports/journal.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/reports/ledger.py` & `mia-accounting-1.5.4/src/accounting/report/reports/ledger.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/reports/search.py` & `mia-accounting-1.5.4/src/accounting/report/reports/search.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/reports/trial_balance.py` & `mia-accounting-1.5.4/src/accounting/report/reports/trial_balance.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/reports/unapplied.py` & `mia-accounting-1.5.4/src/accounting/report/reports/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/reports/unapplied_accounts.py` & `mia-accounting-1.5.4/src/accounting/report/reports/unapplied_accounts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/reports/unmatched.py` & `mia-accounting-1.5.4/src/accounting/report/reports/unmatched.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/reports/unmatched_accounts.py` & `mia-accounting-1.5.4/src/accounting/report/reports/unmatched_accounts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/template_filters.py` & `mia-accounting-1.5.4/src/accounting/report/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/utils/__init__.py` & `mia-accounting-1.5.4/src/accounting/report/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/utils/base_page_params.py` & `mia-accounting-1.5.4/src/accounting/report/utils/base_page_params.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/utils/base_report.py` & `mia-accounting-1.5.4/src/accounting/report/utils/base_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/utils/csv_export.py` & `mia-accounting-1.5.4/src/accounting/report/utils/csv_export.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/utils/offset_matcher.py` & `mia-accounting-1.5.4/src/accounting/report/utils/offset_matcher.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/utils/option_link.py` & `mia-accounting-1.5.4/src/accounting/report/utils/option_link.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/utils/report_chooser.py` & `mia-accounting-1.5.4/src/accounting/report/utils/report_chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/utils/report_type.py` & `mia-accounting-1.5.4/src/accounting/report/utils/report_type.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/utils/unapplied.py` & `mia-accounting-1.5.4/src/accounting/report/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/utils/unmatched.py` & `mia-accounting-1.5.4/src/accounting/report/utils/unmatched.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/utils/urls.py` & `mia-accounting-1.5.4/src/accounting/report/utils/urls.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/report/views.py` & `mia-accounting-1.5.4/src/accounting/report/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/css/style.css` & `mia-accounting-1.5.4/src/accounting/static/css/style.css`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/js/account-form.js` & `mia-accounting-1.5.4/src/accounting/static/js/account-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/js/account-order.js` & `mia-accounting-1.5.4/src/accounting/static/js/account-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/js/currency-form.js` & `mia-accounting-1.5.4/src/accounting/static/js/currency-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/js/description-editor.js` & `mia-accounting-1.5.4/src/accounting/static/js/description-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/js/drag-and-drop-reorder.js` & `mia-accounting-1.5.4/src/accounting/static/js/drag-and-drop-reorder.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/js/journal-entry-account-selector.js` & `mia-accounting-1.5.4/src/accounting/static/js/journal-entry-account-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/js/journal-entry-form.js` & `mia-accounting-1.5.4/src/accounting/static/js/journal-entry-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/js/journal-entry-line-item-editor.js` & `mia-accounting-1.5.4/src/accounting/static/js/journal-entry-line-item-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/js/journal-entry-order.js` & `mia-accounting-1.5.4/src/accounting/static/js/journal-entry-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/js/material-fab-speed-dial.js` & `mia-accounting-1.5.4/src/accounting/static/js/material-fab-speed-dial.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/js/option-form.js` & `mia-accounting-1.5.4/src/accounting/static/js/option-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/js/original-line-item-selector.js` & `mia-accounting-1.5.4/src/accounting/static/js/original-line-item-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/static/js/period-chooser.js` & `mia-accounting-1.5.4/src/accounting/static/js/period-chooser.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/template_filters.py` & `mia-accounting-1.5.4/src/accounting/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/template_globals.py` & `mia-accounting-1.5.4/src/accounting/template_globals.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/account/create.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/account/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/account/detail.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/account/edit.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/account/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/account/include/form.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/account/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/account/list.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/account/list.html`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 <div class="mb-2 accounting-toolbar">
   {% if accounting_can_edit() %}
     <a class="btn btn-primary text-nowrap d-none d-md-block" role="button" href="{{ url_for("accounting.account.create")|accounting_append_next }}">
       <i class="fa-solid fa-plus"></i>
       {{ A_("New") }}
     </a>
   {% endif %}
-  <form class="btn btn-primary d-flex input-group" action="{{ url_for("accounting.account.list") }}" method="get" role="search" aria-labelledby="accounting-toolbar-search-label">
+  <form class="btn btn-primary d-flex input-group" name="accounting-search-form" action="{{ url_for("accounting.account.list") }}" method="get" role="search" aria-labelledby="accounting-toolbar-search-label">
     <input id="accounting-toolbar-search" class="form-control form-control-sm" type="search" name="q" value="{{ request.args.q }}" placeholder=" " required="required">
     <label id="accounting-toolbar-search-label" for="accounting-toolbar-search" class="input-group-text">
       <button type="submit">
         <i class="fa-solid fa-magnifying-glass"></i>
         <span class="d-none d-md-inline">{{ A_("Search") }}</span>
       </button>
     </label>
```

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/account/order.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/account/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/base-account/detail.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/base-account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/base-account/list.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/base-account/list.html`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% extends "accounting/base.html" %}
 
 {% block header %}{% block title %}{% if request.args.q %}{{ A_("Search Result for \"%(query)s\"", query=request.args.q) }}{% else %}{{ A_("Base Account Managements") }}{% endif %}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <div class="mb-2 accounting-toolbar">
-  <form class="btn btn-primary d-flex input-group" action="{{ url_for("accounting.base-account.list") }}" method="get" role="search" aria-labelledby="accounting-toolbar-search-label">
+  <form class="btn btn-primary d-flex input-group" name="accounting-search-form" action="{{ url_for("accounting.base-account.list") }}" method="get" role="search" aria-labelledby="accounting-toolbar-search-label">
     <input id="accounting-toolbar-search" class="form-control form-control-sm" type="search" name="q" value="{{ request.args.q }}" placeholder=" " required="required">
     <label id="accounting-toolbar-search-label" for="accounting-toolbar-search" class="input-group-text">
       <button type="submit">
         <i class="fa-solid fa-magnifying-glass"></i>
         <span class="d-none d-md-inline">{{ A_("Search") }}</span>
       </button>
     </label>
```

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/base.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/currency/create.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/currency/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/currency/detail.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/currency/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/currency/edit.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/currency/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/currency/include/form.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/currency/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/currency/list.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/currency/list.html`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 <div class="mb-2 accounting-toolbar">
   {% if accounting_can_edit() %}
     <a class="btn btn-primary text-nowrap d-none d-md-block" role="button" href="{{ url_for("accounting.currency.create")|accounting_append_next }}">
       <i class="fa-solid fa-plus"></i>
       {{ A_("New") }}
     </a>
   {% endif %}
-  <form class="btn btn-primary d-flex input-group" action="{{ url_for("accounting.currency.list") }}" method="get" role="search" aria-labelledby="accounting-toolbar-search-label">
+  <form class="btn btn-primary d-flex input-group" name="accounting-search-form" action="{{ url_for("accounting.currency.list") }}" method="get" role="search" aria-labelledby="accounting-toolbar-search-label">
     <input id="accounting-toolbar-search" class="form-control form-control-sm" type="search" name="q" value="{{ request.args.q }}" placeholder=" " required="required">
     <label id="accounting-toolbar-search-label" for="accounting-toolbar-search" class="input-group-text">
       <button type="submit">
         <i class="fa-solid fa-magnifying-glass"></i>
         <span class="d-none d-md-inline">{{ A_("Search") }}</span>
       </button>
     </label>
```

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/include/nav.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/include/nav.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/include/pagination.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/include/pagination.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/disbursement/create.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/disbursement/detail.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/disbursement/edit.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
 
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/2/28
 #}
-<form id="accounting-description-editor-{{ description_editor.debit_credit }}" class="accounting-description-editor" data-debit-credit="{{ description_editor.debit_credit }}">
+<form id="accounting-description-editor-{{ description_editor.debit_credit }}" class="accounting-description-editor" name="accounting-dummy-form" data-debit-credit="{{ description_editor.debit_credit }}">
   <div id="accounting-description-editor-{{ description_editor.debit_credit }}-modal" class="modal fade" tabindex="-1" aria-labelledby="accounting-description-editor-{{ description_editor.debit_credit }}-modal-label" aria-hidden="true">
     <div class="modal-dialog">
       <div class="modal-content">
         <div class="modal-header">
           <h1 class="modal-title fs-5" id="accounting-description-editor-{{ description_editor.debit_credit }}-modal-label">
             <label for="accounting-description-editor-{{ description_editor.debit_credit }}-description">{{ A_("Description") }}</label>
           </h1>
```

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/detail.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/form-currency.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/form-line-item.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form-line-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/form.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
 
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/2/25
 #}
-<form id="accounting-line-item-editor">
+<form id="accounting-line-item-editor" name="accounting-dummy-form">
   <div id="accounting-line-item-editor-modal" class="modal fade" tabindex="-1" aria-labelledby="accounting-line-item-editor-modal-label" aria-hidden="true">
     <div class="modal-dialog">
       <div class="modal-content">
         <div class="modal-header">
           <h1 class="modal-title fs-5" id="accounting-line-item-editor-modal-label">{{ A_("Line Item Content") }}</h1>
           <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="{{ A_("Close") }}"></button>
         </div>
```

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/order.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/receipt/create.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/receipt/detail.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/receipt/edit.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/receipt/include/form.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/transfer/create.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/transfer/detail.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/transfer/edit.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/journal-entry/transfer/include/form.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/option/detail.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/option/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/option/form.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/option/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/option/include/form-recurring-item.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/form-recurring-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
 
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/3/22
 #}
-<form id="accounting-recurring-item-editor-{{ expense_income }}">
+<form id="accounting-recurring-item-editor-{{ expense_income }}" name="accounting-dummy-form">
   <div id="accounting-recurring-item-editor-{{ expense_income }}-modal" class="modal fade" tabindex="-1" aria-labelledby="accounting-recurring-item-editor-{{ expense_income }}-modal-label" aria-hidden="true">
     <div class="modal-dialog">
       <div class="modal-content">
         <div class="modal-header">
           <h1 class="modal-title fs-5" id="accounting-recurring-item-editor-{{ expense_income }}-modal-label">{{ title }}</h1>
           <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="{{ A_("Close") }}"></button>
         </div>
```

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/balance-sheet.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/balance-sheet.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/balance-sheet-section.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/balance-sheet-section.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/ledger-row-desktop.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/ledger-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/ledger-row-mobile.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/ledger-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/period-chooser.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/period-chooser.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/search-modal.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/search-modal.html`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
 
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/3/8
 #}
-<form action="{{ url_for("accounting-report.search") }}" method="get" role="search" aria-labelledby="accounting-search-modal-label">
+<form action="{{ url_for("accounting-report.search") }}" name="accounting-search-form" method="get" role="search" aria-labelledby="accounting-search-modal-label">
   <div class="modal fade" id="accounting-search-modal" tabindex="-1" aria-labelledby="accounting-search-modal-label" aria-hidden="true">
     <div class="modal-dialog">
       <div class="modal-content">
         <div class="modal-header">
           <h1 class="modal-title fs-5" id="accounting-search-modal-label">{{ A_("Search") }}</h1>
           <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="{{ A_("Close") }}"></button>
         </div>
```

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/include/toolbar-buttons.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/toolbar-buttons.html`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 {% else %}
   <button class="btn btn-secondary" type="button" disabled="disabled">
     <i class="fa-solid fa-download"></i>
     <span class="d-none d-md-inline">{{ A_("Download") }}</span>
   </button>
 {% endif %}
 {% if use_search %}
-  <form class="btn btn-primary d-flex input-group" action="{{ url_for("accounting-report.search") }}" method="get" role="search" aria-labelledby="accounting-toolbar-search-label">
+  <form class="btn btn-primary d-flex input-group" name="accounting-search-form" action="{{ url_for("accounting-report.search") }}" method="get" role="search" aria-labelledby="accounting-toolbar-search-label">
     <input id="accounting-toolbar-search" class="form-control form-control-sm" type="search" name="q" value="{{ request.args.q }}" placeholder=" " required="required">
     <label id="accounting-toolbar-search-label" for="accounting-toolbar-search" class="input-group-text">
       <button type="submit">
         <i class="fa-solid fa-magnifying-glass"></i>
         <span class="d-none d-md-inline">{{ A_("Search") }}</span>
       </button>
     </label>
```

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/income-expenses.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/income-expenses.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/income-statement.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/income-statement.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/journal.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/journal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/ledger.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/ledger.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/search.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/search.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/trial-balance.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/trial-balance.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/unapplied-accounts.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/unapplied-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/unapplied.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/unapplied.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/unmatched-accounts.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/unmatched-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/templates/accounting/report/unmatched.html` & `mia-accounting-1.5.4/src/accounting/templates/accounting/report/unmatched.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/translations/accounting.pot` & `mia-accounting-1.5.4/src/accounting/translations/accounting.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo` & `mia-accounting-1.5.4/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po` & `mia-accounting-1.5.4/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo` & `mia-accounting-1.5.4/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po` & `mia-accounting-1.5.4/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/utils/__init__.py` & `mia-accounting-1.5.4/src/accounting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/utils/cast.py` & `mia-accounting-1.5.4/src/accounting/utils/cast.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-"""The utility to cast a SQLAlchemy column into the column type, to avoid
-warnings from the IDE.
+"""The utilities to cast values into desired types, to avoid IDE warnings.
 
 This module should not import any other module from the application.
 
 """
 from typing import Any
```

### Comparing `mia-accounting-1.5.3/src/accounting/utils/current_account.py` & `mia-accounting-1.5.4/src/accounting/utils/current_account.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 """The current assets and liabilities account.
 
 """
 from typing import Self
 
 import sqlalchemy as sa
 
-from accounting import db
 from accounting.locale import gettext
 from accounting.models import Account
 
 
 class CurrentAccount:
     """A current assets and liabilities account."""
     CURRENT_AL_CODE: str = "0000-000"
@@ -71,15 +70,15 @@
     def accounts(cls) -> list[Self]:
         """Returns the current assets and liabilities accounts.
 
         :return: The current assets and liabilities accounts.
         """
         accounts: list[cls] = [cls.current_assets_and_liabilities()]
         accounts.extend([CurrentAccount(x)
-                         for x in db.session.query(Account)
+                         for x in Account.query
                         .filter(cls.sql_condition())
                         .order_by(Account.base_code, Account.no)])
         return accounts
 
     @classmethod
     def sql_condition(cls) -> sa.BinaryExpression:
         """Returns the SQL condition for the current assets and liabilities
```

### Comparing `mia-accounting-1.5.3/src/accounting/utils/flash_errors.py` & `mia-accounting-1.5.4/src/accounting/utils/flash_errors.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/utils/journal_entry_types.py` & `mia-accounting-1.5.4/src/accounting/utils/journal_entry_types.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/utils/next_uri.py` & `mia-accounting-1.5.4/src/accounting/utils/next_uri.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,30 +37,40 @@
 
 def inherit_next(uri: str) -> str:
     """Inherits the current next URI to the query argument, if exists.
 
     :param uri: The URI.
     :return: The URI with the current next URI added at the query argument.
     """
-    next_uri: str | None = request.form.get("next") \
-        if request.method == "POST" else request.args.get("next")
-    if next_uri is None:
-        return uri
-    return __set_next(uri, next_uri)
+    next_uri: str | None = __get_next_uri()
+    return uri if next_uri is None else __set_next(uri, next_uri)
 
 
 def or_next(uri: str) -> str:
     """Returns the next URI, if exists, or the supplied URI.
 
     :param uri: The URI.
     :return: The next URI or the supplied URI.
     """
+    next_uri: str | None = __get_next_uri()
+    return uri if next_uri is None else next_uri
+
+
+def __get_next_uri() -> str | None:
+    """Returns the valid next URI.
+
+    :return: The valid next URI.
+    """
     next_uri: str | None = request.form.get("next") \
         if request.method == "POST" else request.args.get("next")
-    return uri if next_uri is None else next_uri
+    if next_uri is None or not next_uri.startswith("/"):
+        return None
+    if len(next_uri) > 512:
+        return next_uri[:512]
+    return next_uri
 
 
 def __set_next(uri: str, next_uri: str) -> str:
     """Sets the next URI to the query arguments.
 
     :param uri: The URI.
     :param next_uri: The next URI.
```

### Comparing `mia-accounting-1.5.3/src/accounting/utils/offset_alias.py` & `mia-accounting-1.5.4/src/accounting/utils/offset_alias.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/utils/options.py` & `mia-accounting-1.5.4/src/accounting/utils/options.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/utils/pagination.py` & `mia-accounting-1.5.4/src/accounting/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/utils/permission.py` & `mia-accounting-1.5.4/src/accounting/utils/permission.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/utils/query.py` & `mia-accounting-1.5.4/src/accounting/utils/query.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/utils/random_id.py` & `mia-accounting-1.5.4/src/accounting/utils/random_id.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/utils/strip_text.py` & `mia-accounting-1.5.4/src/accounting/utils/strip_text.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/accounting/utils/user.py` & `mia-accounting-1.5.4/src/accounting/utils/user.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/src/mia_accounting.egg-info/PKG-INFO` & `mia-accounting-1.5.4/src/mia_accounting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
```

### Comparing `mia-accounting-1.5.3/src/mia_accounting.egg-info/SOURCES.txt` & `mia-accounting-1.5.4/src/mia_accounting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/babel-utils-test-site.py` & `mia-accounting-1.5.4/tests/babel-utils-test-site.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/babel-utils.py` & `mia-accounting-1.5.4/tests/babel-utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_account.py` & `mia-accounting-1.5.4/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_base_account.py` & `mia-accounting-1.5.4/tests/test_base_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_commands.py` & `mia-accounting-1.5.4/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_currency.py` & `mia-accounting-1.5.4/tests/test_currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_description_editor.py` & `mia-accounting-1.5.4/tests/test_description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_journal_entry.py` & `mia-accounting-1.5.4/tests/test_journal_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -2149,15 +2149,15 @@
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{id_2}?next=%2F_next")
 
         with self.app.app_context():
             self.assertEqual(db.session.get(JournalEntry, id_1).no, 1)
             self.assertEqual(db.session.get(JournalEntry, id_2).no, 3)
             self.assertEqual(db.session.get(JournalEntry, id_3).no, 2)
-            self.assertEqual(db.session.get(JournalEntry, id_4).no, 1)
+            self.assertEqual(   db.session.get(JournalEntry, id_4).no, 1)
             self.assertEqual(db.session.get(JournalEntry, id_5).no, 2)
 
     def test_reorder(self) -> None:
         """Tests to reorder the journal entries in a same day.
 
         :return: None.
         """
@@ -2177,22 +2177,22 @@
 
         with self.app.app_context():
             date: dt.date = db.session.get(JournalEntry, id_1).date
 
         response = self.client.post(
             f"{PREFIX}/dates/{date.isoformat()}",
             data={"csrf_token": self.csrf_token,
-                  "next": "/next",
+                  "next": NEXT_URI,
                   f"{id_1}-no": "4",
                   f"{id_2}-no": "1",
                   f"{id_3}-no": "5",
                   f"{id_4}-no": "2",
                   f"{id_5}-no": "3"})
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], f"/next")
+        self.assertEqual(response.headers["Location"], NEXT_URI)
 
         with self.app.app_context():
             self.assertEqual(db.session.get(JournalEntry, id_1).no, 4)
             self.assertEqual(db.session.get(JournalEntry, id_2).no, 1)
             self.assertEqual(db.session.get(JournalEntry, id_3).no, 5)
             self.assertEqual(db.session.get(JournalEntry, id_4).no, 2)
             self.assertEqual(db.session.get(JournalEntry, id_5).no, 3)
@@ -2205,20 +2205,20 @@
             db.session.get(JournalEntry, id_4).no = 8
             db.session.get(JournalEntry, id_5).no = 9
             db.session.commit()
 
         response = self.client.post(
             f"{PREFIX}/dates/{date.isoformat()}",
             data={"csrf_token": self.csrf_token,
-                  "next": "/next",
+                  "next": NEXT_URI,
                   f"{id_2}-no": "3a",
                   f"{id_3}-no": "5",
                   f"{id_4}-no": "2"})
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], f"/next")
+        self.assertEqual(response.headers["Location"], NEXT_URI)
 
         with self.app.app_context():
             self.assertEqual(db.session.get(JournalEntry, id_1).no, 3)
             self.assertEqual(db.session.get(JournalEntry, id_2).no, 4)
             self.assertEqual(db.session.get(JournalEntry, id_3).no, 2)
             self.assertEqual(db.session.get(JournalEntry, id_4).no, 1)
             self.assertEqual(db.session.get(JournalEntry, id_5).no, 5)
```

### Comparing `mia-accounting-1.5.3/tests/test_offset.py` & `mia-accounting-1.5.4/tests/test_offset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_option.py` & `mia-accounting-1.5.4/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_report.py` & `mia-accounting-1.5.4/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_site/__init__.py` & `mia-accounting-1.5.4/tests/test_site/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     """
     import accounting
 
     app: Flask = Flask(__name__)
     db_uri: str = "sqlite:///" if is_testing else "sqlite:///local.sqlite"
     app.config.from_mapping({
         "SECRET_KEY": os.environ.get("SECRET_KEY", token_urlsafe(32)),
+        "SESSION_COOKIE_SAMESITE": "Lax",
+        "SESSION_COOKIE_SECURE": True,
         "SQLALCHEMY_DATABASE_URI": db_uri,
         "BABEL_DEFAULT_LOCALE": "en",
         "ALL_LINGUAS": "zh_Hant|正體中文,en|English,zh_Hans|简体中文",
     })
     if is_testing:
         app.config["TESTING"] = True
```

### Comparing `mia-accounting-1.5.3/tests/test_site/auth.py` & `mia-accounting-1.5.4/tests/test_site/auth.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_site/lib.py` & `mia-accounting-1.5.4/tests/test_site/lib.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_site/locale.py` & `mia-accounting-1.5.4/tests/test_site/locale.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The localization for the Mia! Accounting demonstration website.
 
 """
 from babel import Locale
 from flask import request, session, current_app, Blueprint, Response, \
-    redirect, url_for, Flask
+    redirect, Flask
 from flask_babel import Babel
 from werkzeug.datastructures import LanguageAccept
 
+from accounting.utils.next_uri import or_next
+
 bp: Blueprint = Blueprint("locale", __name__, url_prefix="/")
 
 
 def get_locale():
     """Returns the locale of the user
 
     :return: The locale of the user.
@@ -64,17 +66,15 @@
     """Sets the locale for the user.
 
     :return: The response.
     """
     all_linguas: dict[str, str] = get_all_linguas()
     if "locale" in request.form and request.form["locale"] in all_linguas:
         session["locale"] = request.form["locale"]
-    if "next" in request.form:
-        return redirect(request.form["next"])
-    return redirect(url_for("home.home"))
+    return redirect(or_next("/"))
 
 
 def get_all_linguas() -> dict[str, str]:
     """Returns all the available languages.
 
     :return: All the available languages, as a dictionary of the language code
         and their local names.
```

### Comparing `mia-accounting-1.5.3/tests/test_site/reset.py` & `mia-accounting-1.5.4/tests/test_site/reset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_site/static/favicon.svg` & `mia-accounting-1.5.4/tests/test_site/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_site/templates/base.html` & `mia-accounting-1.5.4/tests/test_site/templates/base.html`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" lang="{{ _("en") }}">
 <head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <meta name="author" content="{{ "imacat" }}" />
   <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" crossorigin="anonymous">
-  <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.2.1/css/all.min.css" crossorigin="anonymous">
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@eonasdan/tempus-dominus@6.4.3/dist/css/tempus-dominus.min.css" crossorigin="anonymous">
+  <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.4.0/css/all.min.css" crossorigin="anonymous">
+  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@eonasdan/tempus-dominus@6.7.7/dist/css/tempus-dominus.min.css" crossorigin="anonymous">
   {% block styles %}{% endblock %}
   <script src="{{ url_for("babel_catalog") }}"></script>
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-kenU1KFdBIe4zVF0s0G1M5b4hcpxyD9F7jL+jjXkk+Q2h455rYXK/7HAuoJl+0I4" crossorigin="anonymous"></script>
   <script src="https://cdn.jsdelivr.net/npm/decimal.js-light@2.5.1/decimal.min.js" integrity="sha384-QdsxGEq4Y0erX8WUIsZJDtfoSSyBF6dmNCnzRNYCa2AOM/xzNsyhHu0RbdFBAm+l" crossorigin="anonymous"></script>
-  <script src="https://cdn.jsdelivr.net/npm/@eonasdan/tempus-dominus@6.4.3/dist/js/tempus-dominus.min.js" integrity="sha384-2MkID2vkc9sxBCqs2us3mB8fV+c0o7uPtOvAPjaC8gKv9Bk21UHT0r2Q7Kv70+zO" crossorigin="anonymous"></script>
+  <script src="https://cdn.jsdelivr.net/npm/@eonasdan/tempus-dominus@6.7.7/dist/js/tempus-dominus.min.js" integrity="sha384-MxHp+/TqTjbku1jSTIe1e/4l6CZTLhACLDbWyxYaFRgD3AM4oh99AY8bxsGhIoRc" crossorigin="anonymous"></script>
   {% block scripts %}{% endblock %}
   <link rel="shortcut icon" href="{{ url_for("static", filename="favicon.svg") }}">
   <title>{% block title %}{% endblock %}</title>
 </head>
 <body>
 
 <nav class="navbar navbar-expand-lg bg-body-tertiary bg-dark navbar-dark">
```

### Comparing `mia-accounting-1.5.3/tests/test_site/templates/home.html` & `mia-accounting-1.5.4/tests/test_site/templates/home.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_site/templates/login.html` & `mia-accounting-1.5.4/tests/test_site/templates/login.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_site/templates/reset.html` & `mia-accounting-1.5.4/tests/test_site/templates/reset.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_site/translations/messages.pot` & `mia-accounting-1.5.4/tests/test_site/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo` & `mia-accounting-1.5.4/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po` & `mia-accounting-1.5.4/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo` & `mia-accounting-1.5.4/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po` & `mia-accounting-1.5.4/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_unmatched_offset.py` & `mia-accounting-1.5.4/tests/test_unmatched_offset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/test_utils.py` & `mia-accounting-1.5.4/tests/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -97,14 +97,68 @@
 
         response = client.get("/test-no-next?q=abc&page-no=4")
         self.assertEqual(response.status_code, 200)
         response = client.post("/test-no-next", data={"csrf_token": csrf_token,
                                                       "name": "viewer"})
         self.assertEqual(response.status_code, 200)
 
+    def test_invalid(self) -> None:
+        """Tests the next URI utilities without an invalid next URI.
+
+        :return: None.
+        """
+        def test_invalid_next_uri_view() -> str:
+            """The test view without the next URI."""
+            self.assertEqual(inherit_next(self.TARGET),
+                             request.args.get("inherit-expected"))
+            self.assertEqual(or_next(self.TARGET),
+                             request.args.get("or-expected"))
+            return ""
+
+        self.app.add_url_rule("/test-invalid-next",
+                              view_func=test_invalid_next_uri_view,
+                              methods=["GET", "POST"])
+        client: httpx.Client = httpx.Client(app=self.app, base_url=TEST_SERVER)
+        client.headers["Referer"] = TEST_SERVER
+        csrf_token: str = get_csrf_token(client)
+        next_uri: str
+        expected1: str
+        expected2: str
+        response: httpx.Response
+
+        # A foreign URI
+        next_uri = "https://example.com"
+        expected1 = self.TARGET
+        expected2 = self.TARGET
+        response = client.get(f"/test-invalid-next?next={quote_plus(next_uri)}"
+                              f"&inherit-expected={quote_plus(expected1)}"
+                              f"&or-expected={quote_plus(expected2)}")
+        self.assertEqual(response.status_code, 200)
+        response = client.post("/test-invalid-next"
+                               f"?inherit-expected={quote_plus(expected1)}"
+                               f"&or-expected={quote_plus(expected2)}",
+                               data={"csrf_token": csrf_token,
+                                     "next": next_uri})
+        self.assertEqual(response.status_code, 200)
+
+        # An extremely-long URI to trigger the error
+        next_uri = "/" + "x" * 1024
+        expected2 = next_uri[:512]
+        expected1 = f"{self.TARGET}?next={quote_plus(expected2)}"
+        response = client.get(f"/test-invalid-next?next={quote_plus(next_uri)}"
+                              f"&inherit-expected={quote_plus(expected1)}"
+                              f"&or-expected={quote_plus(expected2)}")
+        self.assertEqual(response.status_code, 200)
+        response = client.post("/test-invalid-next"
+                               f"?inherit-expected={quote_plus(expected1)}"
+                               f"&or-expected={quote_plus(expected2)}",
+                               data={"csrf_token": csrf_token,
+                                     "next": next_uri})
+        self.assertEqual(response.status_code, 200)
+
 
 class QueryKeywordParserTestCase(unittest.TestCase):
     """The test case for the query keyword parser."""
 
     def test_default(self) -> None:
         """Tests the query keyword parser.
```

### Comparing `mia-accounting-1.5.3/tests/testlib.py` & `mia-accounting-1.5.4/tests/testlib.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.3/tests/testlib_journal_entry.py` & `mia-accounting-1.5.4/tests/testlib_journal_entry.py`

 * *Files identical despite different names*

