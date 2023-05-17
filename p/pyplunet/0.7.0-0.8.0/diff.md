# Comparing `tmp/pyplunet-0.7.0.tar.gz` & `tmp/pyplunet-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplunet-0.7.0.tar", last modified: Mon May  8 14:42:46 2023, max compression
+gzip compressed data, was "pyplunet-0.8.0.tar", last modified: Wed May 17 21:44:53 2023, max compression
```

## Comparing `pyplunet-0.7.0.tar` & `pyplunet-0.8.0.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-08 14:42:46.555818 pyplunet-0.7.0/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1067 2022-06-16 21:31:29.000000 pyplunet-0.7.0/LICENCE
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)        0 2022-06-16 21:00:13.000000 pyplunet-0.7.0/MANIFEST.in
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6741 2023-05-08 14:42:46.555678 pyplunet-0.7.0/PKG-INFO
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6208 2023-05-08 14:38:47.000000 pyplunet-0.7.0/README.md
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1170 2023-05-08 14:42:30.000000 pyplunet-0.7.0/pyproject.toml
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       38 2023-05-08 14:42:46.555860 pyplunet-0.7.0/setup.cfg
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       38 2022-06-16 21:32:43.000000 pyplunet-0.7.0/setup.py
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-08 14:42:46.545428 pyplunet-0.7.0/src/
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-08 14:42:46.547505 pyplunet-0.7.0/src/pyplunet/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)      157 2023-05-08 14:42:30.000000 pyplunet-0.7.0/src/pyplunet/__init__.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     5649 2023-05-08 14:02:53.000000 pyplunet-0.7.0/src/pyplunet/client.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     7929 2023-02-12 18:25:15.000000 pyplunet-0.7.0/src/pyplunet/enums.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    70877 2023-01-24 12:52:24.000000 pyplunet-0.7.0/src/pyplunet/exceptions.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    45076 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/models.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1853 2023-05-08 13:35:08.000000 pyplunet-0.7.0/src/pyplunet/retrying_client.py
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-08 14:42:46.551514 pyplunet-0.7.0/src/pyplunet/services/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1530 2023-05-08 13:35:08.000000 pyplunet-0.7.0/src/pyplunet/services/__init__.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     5396 2023-05-08 14:02:53.000000 pyplunet-0.7.0/src/pyplunet/services/data_admin30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    32955 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_credit_note30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     9635 2023-05-08 14:02:53.000000 pyplunet-0.7.0/src/pyplunet/services/data_custom_fields30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    39564 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_customer30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    20418 2023-05-08 14:02:53.000000 pyplunet-0.7.0/src/pyplunet/services/data_customer_address30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    22388 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_customer_contact30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     4408 2023-05-08 14:02:53.000000 pyplunet-0.7.0/src/pyplunet/services/data_document30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    75643 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_item30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    65363 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_job30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    11826 2023-05-08 14:02:53.000000 pyplunet-0.7.0/src/pyplunet/services/data_job_round30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    49374 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_order30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    44579 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_outgoing_invoice30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    26937 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_payable30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    34509 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_quote30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    47453 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_request30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    44462 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_resource30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    17537 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_resource_address30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    23275 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_resource_contact30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     2054 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/data_user30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1348 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/report_customer30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1238 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/report_job30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    10611 2023-05-08 14:02:54.000000 pyplunet-0.7.0/src/pyplunet/services/request_doc_text30.py
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-08 14:42:46.545358 pyplunet-0.7.0/src/pyplunet/venv/
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-08 14:42:46.551643 pyplunet-0.7.0/src/pyplunet/venv/bin/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1176 2023-02-11 15:54:46.000000 pyplunet-0.7.0/src/pyplunet/venv/bin/activate_this.py
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-08 14:42:46.548136 pyplunet-0.7.0/src/pyplunet.egg-info/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6741 2023-05-08 14:42:46.000000 pyplunet-0.7.0/src/pyplunet.egg-info/PKG-INFO
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     2125 2023-05-08 14:42:46.000000 pyplunet-0.7.0/src/pyplunet.egg-info/SOURCES.txt
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)        1 2023-05-08 14:42:46.000000 pyplunet-0.7.0/src/pyplunet.egg-info/dependency_links.txt
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)      100 2023-05-08 14:42:46.000000 pyplunet-0.7.0/src/pyplunet.egg-info/requires.txt
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       14 2023-05-08 14:42:46.000000 pyplunet-0.7.0/src/pyplunet.egg-info/top_level.txt
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-08 14:42:46.545476 pyplunet-0.7.0/src/venv/
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-08 14:42:46.551915 pyplunet-0.7.0/src/venv/bin/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1200 2022-11-22 08:52:14.000000 pyplunet-0.7.0/src/venv/bin/activate_this.py
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-08 14:42:46.555456 pyplunet-0.7.0/tests/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     5923 2023-05-08 14:14:27.000000 pyplunet-0.7.0/tests/test_DataAdmin30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    32511 2023-05-08 14:14:04.000000 pyplunet-0.7.0/tests/test_DataCreditNote30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6388 2023-05-08 14:14:09.000000 pyplunet-0.7.0/tests/test_DataCustomFields30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    38127 2023-05-08 14:14:06.000000 pyplunet-0.7.0/tests/test_DataCustomer30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    21662 2023-05-08 14:14:07.000000 pyplunet-0.7.0/tests/test_DataCustomerAddress30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    23055 2023-05-08 14:14:07.000000 pyplunet-0.7.0/tests/test_DataCustomerContact30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     3475 2023-05-08 14:14:09.000000 pyplunet-0.7.0/tests/test_DataDocument30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    47839 2023-05-08 14:14:06.000000 pyplunet-0.7.0/tests/test_DataItem30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    42177 2023-05-08 14:14:04.000000 pyplunet-0.7.0/tests/test_DataJob30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    10662 2023-05-08 14:14:05.000000 pyplunet-0.7.0/tests/test_DataJobRound30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    45330 2023-05-08 14:14:05.000000 pyplunet-0.7.0/tests/test_DataOrder30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    45908 2023-05-08 14:14:04.000000 pyplunet-0.7.0/tests/test_DataOutgoingInvoice30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    28255 2023-05-08 14:14:03.000000 pyplunet-0.7.0/tests/test_DataPayable30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    32151 2023-05-08 14:14:05.000000 pyplunet-0.7.0/tests/test_DataQuote30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    42688 2023-05-08 14:14:06.000000 pyplunet-0.7.0/tests/test_DataRequest30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    40943 2023-05-08 14:14:06.000000 pyplunet-0.7.0/tests/test_DataResource30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    18933 2023-05-08 14:14:08.000000 pyplunet-0.7.0/tests/test_DataResourceAddress30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    25135 2023-05-08 14:14:07.000000 pyplunet-0.7.0/tests/test_DataResourceContact30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     2958 2023-05-08 14:14:09.000000 pyplunet-0.7.0/tests/test_DataUser30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     3128 2023-05-08 14:06:14.000000 pyplunet-0.7.0/tests/test_PlunetAPI.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1766 2023-05-08 14:14:07.000000 pyplunet-0.7.0/tests/test_ReportCustomer30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1691 2023-05-08 14:14:05.000000 pyplunet-0.7.0/tests/test_ReportJob30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    10341 2023-05-08 14:14:09.000000 pyplunet-0.7.0/tests/test_RequestDocText30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     2484 2023-05-08 13:07:23.000000 pyplunet-0.7.0/tests/test_client_factory.py
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.841118 pyplunet-0.8.0/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1067 2022-06-16 21:31:29.000000 pyplunet-0.8.0/LICENCE
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)        0 2022-06-16 21:00:13.000000 pyplunet-0.8.0/MANIFEST.in
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6643 2023-05-17 21:44:53.840984 pyplunet-0.8.0/PKG-INFO
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6132 2023-05-17 21:41:39.000000 pyplunet-0.8.0/README.md
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1141 2023-05-17 21:44:32.000000 pyplunet-0.8.0/pyproject.toml
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       38 2023-05-17 21:44:53.841226 pyplunet-0.8.0/setup.cfg
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       38 2022-06-16 21:32:43.000000 pyplunet-0.8.0/setup.py
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.823533 pyplunet-0.8.0/src/
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.826056 pyplunet-0.8.0/src/pyplunet/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       84 2023-05-17 21:44:32.000000 pyplunet-0.8.0/src/pyplunet/__init__.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     5649 2023-05-08 14:02:53.000000 pyplunet-0.8.0/src/pyplunet/client.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     8664 2023-05-17 21:23:00.000000 pyplunet-0.8.0/src/pyplunet/enums.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    70877 2023-01-24 12:52:24.000000 pyplunet-0.8.0/src/pyplunet/exceptions.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    45076 2023-05-08 14:02:54.000000 pyplunet-0.8.0/src/pyplunet/models.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1853 2023-05-08 13:35:08.000000 pyplunet-0.8.0/src/pyplunet/retrying_client.py
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.829860 pyplunet-0.8.0/src/pyplunet/services/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1530 2023-05-08 13:35:08.000000 pyplunet-0.8.0/src/pyplunet/services/__init__.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     5312 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_admin30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    32871 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_credit_note30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     9551 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_custom_fields30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    39480 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_customer30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    20334 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_customer_address30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    22304 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_customer_contact30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     4324 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_document30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    75559 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_item30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    65279 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_job30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    11742 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_job_round30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    49290 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_order30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    44495 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_outgoing_invoice30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    26853 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_payable30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    34425 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_quote30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    47369 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_request30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    44378 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_resource30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    17453 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_resource_address30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    23191 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_resource_contact30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1970 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_user30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1264 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/report_customer30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1154 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/report_job30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    10527 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/request_doc_text30.py
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.823460 pyplunet-0.8.0/src/pyplunet/venv/
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.829995 pyplunet-0.8.0/src/pyplunet/venv/bin/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1176 2023-02-11 15:54:46.000000 pyplunet-0.8.0/src/pyplunet/venv/bin/activate_this.py
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.826774 pyplunet-0.8.0/src/pyplunet.egg-info/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6643 2023-05-17 21:44:53.000000 pyplunet-0.8.0/src/pyplunet.egg-info/PKG-INFO
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     2145 2023-05-17 21:44:53.000000 pyplunet-0.8.0/src/pyplunet.egg-info/SOURCES.txt
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)        1 2023-05-17 21:44:53.000000 pyplunet-0.8.0/src/pyplunet.egg-info/dependency_links.txt
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       74 2023-05-17 21:44:53.000000 pyplunet-0.8.0/src/pyplunet.egg-info/requires.txt
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       14 2023-05-17 21:44:53.000000 pyplunet-0.8.0/src/pyplunet.egg-info/top_level.txt
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.823583 pyplunet-0.8.0/src/venv/
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.831238 pyplunet-0.8.0/src/venv/bin/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1200 2022-11-22 08:52:14.000000 pyplunet-0.8.0/src/venv/bin/activate_this.py
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.840799 pyplunet-0.8.0/tests/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     5667 2023-05-17 21:41:39.000000 pyplunet-0.8.0/tests/test_DataAdmin30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    32511 2023-05-08 14:14:04.000000 pyplunet-0.8.0/tests/test_DataCreditNote30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6388 2023-05-08 14:14:09.000000 pyplunet-0.8.0/tests/test_DataCustomFields30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    38127 2023-05-08 14:14:06.000000 pyplunet-0.8.0/tests/test_DataCustomer30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    21662 2023-05-08 14:14:07.000000 pyplunet-0.8.0/tests/test_DataCustomerAddress30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    23055 2023-05-08 14:14:07.000000 pyplunet-0.8.0/tests/test_DataCustomerContact30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     3475 2023-05-08 14:14:09.000000 pyplunet-0.8.0/tests/test_DataDocument30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    47839 2023-05-08 14:14:06.000000 pyplunet-0.8.0/tests/test_DataItem30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    42177 2023-05-08 14:14:04.000000 pyplunet-0.8.0/tests/test_DataJob30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    10662 2023-05-08 14:14:05.000000 pyplunet-0.8.0/tests/test_DataJobRound30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    45330 2023-05-08 14:14:05.000000 pyplunet-0.8.0/tests/test_DataOrder30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    45908 2023-05-08 14:14:04.000000 pyplunet-0.8.0/tests/test_DataOutgoingInvoice30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    28255 2023-05-08 14:14:03.000000 pyplunet-0.8.0/tests/test_DataPayable30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    32151 2023-05-08 14:14:05.000000 pyplunet-0.8.0/tests/test_DataQuote30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    42688 2023-05-08 14:14:06.000000 pyplunet-0.8.0/tests/test_DataRequest30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    40943 2023-05-08 14:14:06.000000 pyplunet-0.8.0/tests/test_DataResource30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    18933 2023-05-08 14:14:08.000000 pyplunet-0.8.0/tests/test_DataResourceAddress30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    25135 2023-05-08 14:14:07.000000 pyplunet-0.8.0/tests/test_DataResourceContact30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     2958 2023-05-08 14:14:09.000000 pyplunet-0.8.0/tests/test_DataUser30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     3128 2023-05-08 14:06:14.000000 pyplunet-0.8.0/tests/test_PlunetAPI.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1766 2023-05-08 14:14:07.000000 pyplunet-0.8.0/tests/test_ReportCustomer30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1691 2023-05-08 14:14:05.000000 pyplunet-0.8.0/tests/test_ReportJob30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    10341 2023-05-08 14:14:09.000000 pyplunet-0.8.0/tests/test_RequestDocText30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1282 2023-05-17 21:41:52.000000 pyplunet-0.8.0/tests/test_client_factory.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)      438 2023-05-17 21:18:03.000000 pyplunet-0.8.0/tests/test_enums.py
```

### Comparing `pyplunet-0.7.0/LICENCE` & `pyplunet-0.8.0/LICENCE`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/PKG-INFO` & `pyplunet-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: pyplunet
-Version: 0.7.0
-Summary: Client for the Plunet 3.0 SOAP API.
-Author-email: Henrik Kühnemann <hello@yellownape.se>
-Project-URL: Homepage, https://github.com/kuhnemann/pyplunet
-Keywords: plunet,api,translation,localization,tms
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: retry
-License-File: LICENCE
-
 <div id="top"></div>
 
 
 <!-- PROJECT SHIELDS -->
 
 
 [![Forks][forks-shield]][forks-url]
@@ -53,17 +37,17 @@
 
 - Implements all services and methods as per Plunet 9.2 (the latest version of ApiDocs available)
 - Fully typed for validation and code completion support
 - Fully documented methods with complete content of the Plunet JavaDocs.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-### New in 0.7.0
-- Retrying client that uses tenacity to retry on ConnectionError from zeep/requests
-- Improved typing for enums - all are still not covered but getting there
+### New in 0.8.0
+- Decided to remove the retrying client 
+- Improved flexibility for enums, which now accept both integers and strings that are possible to cast as ints
 
 ### Built With
 
 * [zeep](https://docs.python-zeep.org/en/master/)
 * [pydantic](https://docs.pydantic.dev/)
 * [plunetapi](https://github.com/kuhnemann/plunetapi/)
 
@@ -81,19 +65,14 @@
 
 Install via pip
 
    ```sh
    pip install pyplunet
    ```
 
-To include tenacity:
-   ```sh
-   pip install pyplunet[retry] 
-   ```
-
 Or clone the repo
 
    ```sh
    git clone https://github.com/kuhnemann/pyplunet.git
    ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
@@ -251,8 +230,8 @@
 
 [license-url]: https://github.com/kuhnemann/pyplunet/blob/main/LICENCE
 
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 
 [linkedin-url]: https://linkedin.com/in/henrik-kuhnemann
 
-[product-screenshot]: images/screenshot.png
+[product-screenshot]: images/screenshot.png
```

#### html2text {}

```diff
@@ -1,37 +1,29 @@
-Metadata-Version: 2.1 Name: pyplunet Version: 0.7.0 Summary: Client for the
-Plunet 3.0 SOAP API. Author-email: Henrik KÃ¼hnemann
-yellownape.se> Project-URL: Homepage, https://github.com/kuhnemann/pyplunet
-Keywords: plunet,api,translation,localization,tms Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Requires-Python: >=3.9 Description-Content-
-Type: text/markdown Provides-Extra: dev Provides-Extra: retry License-File:
-LICENCE
  [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url] [![MIT License][license-shield]]
 [license-url] [![LinkedIn][linkedin-shield]][linkedin-url]
                               **** PyPlunet ****
       Modern Python client for interacting with the Plunet SOAP 3.0 API.
  ## About The Project Modern Python client for interacting with the Plunet SOAP
 API, without having to deal with any of the soapiness. Ready to use out of the
 box, you can jump directly into the business logic. Pip install, import and
 start working. It really is as easy as that! - Implements all services and
 methods as per Plunet 9.2 (the latest version of ApiDocs available) - Fully
 typed for validation and code completion support - Fully documented methods
 with complete content of the Plunet JavaDocs.
                                                                   (back_to_top)
-### New in 0.7.0 - Retrying client that uses tenacity to retry on
-ConnectionError from zeep/requests - Improved typing for enums - all are still
-not covered but getting there ### Built With * [zeep](https://docs.python-
-zeep.org/en/master/) * [pydantic](https://docs.pydantic.dev/) * [plunetapi]
-(https://github.com/kuhnemann/plunetapi/)
+### New in 0.8.0 - Decided to remove the retrying client - Improved flexibility
+for enums, which now accept both integers and strings that are possible to cast
+as ints ### Built With * [zeep](https://docs.python-zeep.org/en/master/) *
+[pydantic](https://docs.pydantic.dev/) * [plunetapi](https://github.com/
+kuhnemann/plunetapi/)
                                                                   (back_to_top)
  ## Getting Started ### Installation Install via pip ```sh pip install pyplunet
-``` To include tenacity: ```sh pip install pyplunet[retry] ``` Or clone the
-repo ```sh git clone https://github.com/kuhnemann/pyplunet.git ```
+``` Or clone the repo ```sh git clone https://github.com/kuhnemann/pyplunet.git
+```
                                                                   (back_to_top)
  ## Usage Install using pip like so: ```sh pip install pyplunet ``` Initialize
 the client with the base URL of your Plunet instance, authenticate and start
 doing whatever you aim to do. ```sh from pyplunet import PlunetClient
 plunet_client = PlunetClient(base_url="YOUR_URL") plunet_client.login
 (username=username, password=password) order_result =
 plunet_client.order.get_order_object(order_id=1234) ``` Complex types and enums
```

### Comparing `pyplunet-0.7.0/README.md` & `pyplunet-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pyplunet
+Version: 0.8.0
+Summary: Client for the Plunet 3.0 SOAP API.
+Author-email: Henrik Kühnemann <hello@yellownape.se>
+Project-URL: Homepage, https://github.com/kuhnemann/pyplunet
+Keywords: plunet,api,translation,localization,tms
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENCE
+
 <div id="top"></div>
 
 
 <!-- PROJECT SHIELDS -->
 
 
 [![Forks][forks-shield]][forks-url]
@@ -37,17 +52,17 @@
 
 - Implements all services and methods as per Plunet 9.2 (the latest version of ApiDocs available)
 - Fully typed for validation and code completion support
 - Fully documented methods with complete content of the Plunet JavaDocs.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-### New in 0.7.0
-- Retrying client that uses tenacity to retry on ConnectionError from zeep/requests
-- Improved typing for enums - all are still not covered but getting there
+### New in 0.8.0
+- Decided to remove the retrying client 
+- Improved flexibility for enums, which now accept both integers and strings that are possible to cast as ints
 
 ### Built With
 
 * [zeep](https://docs.python-zeep.org/en/master/)
 * [pydantic](https://docs.pydantic.dev/)
 * [plunetapi](https://github.com/kuhnemann/plunetapi/)
 
@@ -65,19 +80,14 @@
 
 Install via pip
 
    ```sh
    pip install pyplunet
    ```
 
-To include tenacity:
-   ```sh
-   pip install pyplunet[retry] 
-   ```
-
 Or clone the repo
 
    ```sh
    git clone https://github.com/kuhnemann/pyplunet.git
    ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
@@ -235,8 +245,8 @@
 
 [license-url]: https://github.com/kuhnemann/pyplunet/blob/main/LICENCE
 
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 
 [linkedin-url]: https://linkedin.com/in/henrik-kuhnemann
 
-[product-screenshot]: images/screenshot.png
+[product-screenshot]: images/screenshot.png
```

#### html2text {}

```diff
@@ -1,29 +1,36 @@
+Metadata-Version: 2.1 Name: pyplunet Version: 0.8.0 Summary: Client for the
+Plunet 3.0 SOAP API. Author-email: Henrik KÃ¼hnemann
+yellownape.se> Project-URL: Homepage, https://github.com/kuhnemann/pyplunet
+Keywords: plunet,api,translation,localization,tms Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Requires-Python: >=3.9 Description-Content-
+Type: text/markdown Provides-Extra: dev License-File: LICENCE
  [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url] [![MIT License][license-shield]]
 [license-url] [![LinkedIn][linkedin-shield]][linkedin-url]
                               **** PyPlunet ****
       Modern Python client for interacting with the Plunet SOAP 3.0 API.
  ## About The Project Modern Python client for interacting with the Plunet SOAP
 API, without having to deal with any of the soapiness. Ready to use out of the
 box, you can jump directly into the business logic. Pip install, import and
 start working. It really is as easy as that! - Implements all services and
 methods as per Plunet 9.2 (the latest version of ApiDocs available) - Fully
 typed for validation and code completion support - Fully documented methods
 with complete content of the Plunet JavaDocs.
                                                                   (back_to_top)
-### New in 0.7.0 - Retrying client that uses tenacity to retry on
-ConnectionError from zeep/requests - Improved typing for enums - all are still
-not covered but getting there ### Built With * [zeep](https://docs.python-
-zeep.org/en/master/) * [pydantic](https://docs.pydantic.dev/) * [plunetapi]
-(https://github.com/kuhnemann/plunetapi/)
+### New in 0.8.0 - Decided to remove the retrying client - Improved flexibility
+for enums, which now accept both integers and strings that are possible to cast
+as ints ### Built With * [zeep](https://docs.python-zeep.org/en/master/) *
+[pydantic](https://docs.pydantic.dev/) * [plunetapi](https://github.com/
+kuhnemann/plunetapi/)
                                                                   (back_to_top)
  ## Getting Started ### Installation Install via pip ```sh pip install pyplunet
-``` To include tenacity: ```sh pip install pyplunet[retry] ``` Or clone the
-repo ```sh git clone https://github.com/kuhnemann/pyplunet.git ```
+``` Or clone the repo ```sh git clone https://github.com/kuhnemann/pyplunet.git
+```
                                                                   (back_to_top)
  ## Usage Install using pip like so: ```sh pip install pyplunet ``` Initialize
 the client with the base URL of your Plunet instance, authenticate and start
 doing whatever you aim to do. ```sh from pyplunet import PlunetClient
 plunet_client = PlunetClient(base_url="YOUR_URL") plunet_client.login
 (username=username, password=password) order_result =
 plunet_client.order.get_order_object(order_id=1234) ``` Complex types and enums
```

### Comparing `pyplunet-0.7.0/pyproject.toml` & `pyplunet-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyplunet"
-version = "0.7.0"
+version = "0.8.0"
 description = "Client for the Plunet 3.0 SOAP API."
 readme = "README.md"
 authors = [{ name = "Henrik Kühnemann", email = "hello@yellownape.se" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -20,22 +20,21 @@
 dependencies = [
     "plunetapi>=0.3", "pydantic>=1.10"
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
-retry = ["tenactity>=8.2.2"]
 
 [project.urls]
 Homepage = "https://github.com/kuhnemann/pyplunet"
 
 
 [tool.bumpver]
-current_version = "0.7.0"
+current_version = "0.8.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyplunet-0.7.0/src/pyplunet/client.py` & `pyplunet-0.8.0/src/pyplunet/client.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/src/pyplunet/enums.py` & `pyplunet-0.8.0/src/pyplunet/enums.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 from enum import Enum
 
+class StrIntEnum(Enum):
 
-class SearchSelection_Resource(Enum):
+    @classmethod
+    def _missing_(cls, value):
+        try:
+            int_value = int(value)
+            for member in cls:
+                if member.name == value or member.value == int_value:
+                    return member
+        except ValueError:
+            pass
+        raise ValueError(f"{value} ({type(value)}) is not a valid {cls.__name__}. Valid values: {', '.join([str(x) for x in cls])}")
+
+
+class SearchSelection_Resource(StrIntEnum):
     AGENCY = 9
     RESOURCE = 1
 
 
-class FolderTypes(Enum):
+class FolderTypes(StrIntEnum):
     CUSTOMER = 19
     INVOICE = 13
     ORDER_FINAL = 12
     ORDER_ITEM_CAT = 8
     ORDER_ITEM_REFERENCE = 17
     ORDER_ITEM_SOURCE = 16
     ORDER_JOB_IN = 22
@@ -30,93 +43,93 @@
     QUOTE_REFERENCE = 3
     QUOTE_SOURCE = 4
     REQUEST_REFERENCE = 1
     REQUEST_SOURCE = 2
     RESOURCE = 18
 
 
-class InvoiceType(Enum):
+class InvoiceType(StrIntEnum):
     CREDIT_NOTES = 2
     PAYABLES = 3
     RECEIVABLES = 1
 
 
-class WorkingStatus(Enum):
+class WorkingStatus(StrIntEnum):
     EXTERNAL = 2
     INTERNAL = 1
 
 
-class QuoteStatusType(Enum):
+class QuoteStatusType(StrIntEnum):
     ACCEPTED = 7
     CANCELED = 5
     CHANGE_INTO_ORDER = 4
     CHECK_CLEARANCE = 11
     EXPIRED = 6
     IN_PREPARATION = 9
     NEW = 8
     PENDING = 1
     REJECTED = 3
     REVISED = 2
 
 
-class Format(Enum):
+class Format(StrIntEnum):
     ABBREVIATED_VERSION = 1
     OUTPUT_AS_IN_ORDER = 6
     QUANTITY_NOT_WEIGHTED = 4
     STANDARD = 0
     STANDARD_WITH_PRICE_MEMO = 5
     TM_DISCONT = 3
     WEIGHTED_QUANTITY = 2
 
 
-class WorkflowType(Enum):
+class WorkflowType(StrIntEnum):
     ORDER = 1
     QUOTE_ORDER = 2
     STANDARD = 0
 
 
-class AddressType(Enum):
+class AddressType(StrIntEnum):
     DELIVERY = 1
     INVOICE = 2
     OTHER = 3
 
 
-class JobRequestRankingMethod(Enum):
+class JobRequestRankingMethod(StrIntEnum):
     JOB_FEEDBACK = 3
     JOBS_FOR_CUSTOMER = 2
     PRICE = 4
     RANKING_RESOURCE_ASSESSMENT = 1
 
 
-class FormOfAddressType(Enum):
+class FormOfAddressType(StrIntEnum):
     COMPANY = 3
     MADAM = 2
     SIR = 1
 
 
-class JobRoundAssignmentMethod(Enum):
+class JobRoundAssignmentMethod(StrIntEnum):
     FIRST_COME_FIRST_SERVE = 2
     MANUAL = 1
     TOP_RANKED = 4
 
 
-class TimeFrameRelation_Quote(Enum):
+class TimeFrameRelation_Quote(StrIntEnum):
     EVENT_END_DATE = 9
     EVENT_START_DATE = 8
     INSTRUCTED_DATE = 10
     ITEM_CREATION_DATE = 2
     ITEM_DELIVERY_DATE = 4
     QUOTE_BINDING_DEADLINE_DATE = 6
     QUOTE_CREATION_DATE = 1
     QUOTE_DELIVERY_DATE = 3
     REJECTION_DATE = 7
     REQUEST_DATE = 5
 
 
-class DocumentStatus(Enum):
+class DocumentStatus(StrIntEnum):
     DOCUMENTS_APPROVED = 7
     DOCUMENTS_AVAILABLE = 1
     DOCUMENTS_DOWNLOADED = 2
     DOCUMENTS_IN_REVIEW = 3
     DOCUMENTS_RE_DELIVERED = 6
     NO_DOCUMENTS_AVAILABLE = 0
     POSTPROCESSING_IN_PROGRESS = 5
@@ -124,41 +137,41 @@
 
 
 class APIVersion(Enum):
     Version_25 = "Version_25"
     Version_30 = "Version_30"
 
 
-class CurrencyType(Enum):
+class CurrencyType(StrIntEnum):
     HOMECURRENCY = 2
     PROJECTCURRENCY = 1
 
 
-class CompanyCodeType(Enum):
+class CompanyCodeType(StrIntEnum):
     INVOICE = 1
     RIGHTS = 2
 
 
-class CustomerType(Enum):
+class CustomerType(StrIntEnum):
     DIRECT = 0
     DIRECT_INDIRECT = 1
     INDIRECT = 2
 
 
-class JobRoundStatus(Enum):
+class JobRoundStatus(StrIntEnum):
     ASSIGNMENT_ERROR = 2
     CANCELED = 5
     IN_PREPARATION = 0
     JOB_ASSIGNED = 3
     NO_ASSIGNMENT = 4
     REACTION_TIME_ELAPSED = 6
     REQUESTED = 1
 
 
-class CatType(Enum):
+class CatType(StrIntEnum):
     ACROSS = 5
     CATALYST = 14
     DEJAVU = 12
     FALCON = 17
     FUSION = 11
     HELIUM = 15
     IDIOM = 9
@@ -169,21 +182,21 @@
     PRACTICOUNT = 6
     TRADOS = 1
     TRANSIT = 3
     WORDFAST = 13
     XTM = 10
 
 
-class SearchSelection_TeamMember(Enum):
+class SearchSelection_TeamMember(StrIntEnum):
     PROJECT_MANAGER = 4
     RESOURCE = 1
     SUPERVISOR = 8
 
 
-class ItemStatus(Enum):
+class ItemStatus(StrIntEnum):
     ACCEPTED = 12
     APPROVED = 3
     CANCELED = 5
     DELIVERABLE = 7
     DELIVERED = 2
     IN_PREPERATION = 8
     IN_PROGRESS = 1
@@ -192,107 +205,107 @@
     PAID = 9
     PENDING = 11
     REJECTED = 13
     SUM = 14
     WITHOUT_INVOICE = 10
 
 
-class ArchivStatus(Enum):
+class ArchivStatus(StrIntEnum):
     ACTIVE = 1
     ARCHIVED = 3
     COMPLETED = 6
     COMPLETED_ARCHIVABLE = 2
     IN_PREPARATION = 5
     QUOTE_MOVED_TO_ORDER = 4
 
 
-class JobRoundAssignmentLimitType(Enum):
+class JobRoundAssignmentLimitType(StrIntEnum):
     ALL = 0
     LIMIT_X = 1
     MANUAL_SELECTED = 2
 
 
-class SearchSelection_Customer(Enum):
+class SearchSelection_Customer(StrIntEnum):
     ACCOUNT_MANAGER = 7
     CUSTOMER = 1
     INDIRECT_CUSTOMER = 3
 
 
-class TimeFrameRelation_Request(Enum):
+class TimeFrameRelation_Request(StrIntEnum):
     REQUEST_DATE = 1
 
 
-class PayableStatus(Enum):
+class PayableStatus(StrIntEnum):
     CANCELED = 3
     CREATED_BY_EXTERNAL_USER = 4
     IN_PREPARATION = 5
     INVOICE_CHECKED = 6
     OUTSTANDING = 1
     PAID = 2
 
 
-class RequestStatusType(Enum):
+class RequestStatusType(StrIntEnum):
     CANCELED = 5
     CHANGED_INTO_ORDER = 7
     CHANGED_INTO_QUOTE = 6
     IN_PREPARATION = 1
     NEW_AUTO = 8
     PENDING = 2
     REJECTED = 9
 
 
-class ResourceStatus(Enum):
+class ResourceStatus(StrIntEnum):
     ACTIVE = 1
     BLOCKED = 3
     DELETION_REQUESTED = 10
     DISQUALIFIED = 9
     NEW = 4
     NEW_AUTO = 6
     NOT_ACTIVE_OR_OLD = 2
     PREMIUM = 5
     PROBATION = 7
     QUALIFIED = 8
 
 
-class ProjectType(Enum):
+class ProjectType(StrIntEnum):
     ORDER = 3
     QUOTE = 1
 
 
-class PropertyUsageArea(Enum):
+class PropertyUsageArea(StrIntEnum):
     CUSTOMER = 1
     ORDER = 6
     ORDER_ITEM = 10
     ORDER_JOB = 12
     QUOTE = 5
     QUOTE_ITEM = 9
     QUOTE_JOB = 11
     REQUEST = 4
     RESOURCE = 2
 
 
-class ResourceType(Enum):
+class ResourceType(StrIntEnum):
     PROJECT_MANAGER = 2
     RESOURCES = 0
     SUPERVISOR = 3
     TEAM_MEMBER = 1
 
 
-class CustomerStatus(Enum):
+class CustomerStatus(StrIntEnum):
     ACTIVE = 1
     AQUISITION_ADDRESS = 6
     BLOCKED = 5
     CONTACTED = 3
     DELETION_REQUESTED = 8
     NEW = 4
     NEW_AUTO = 7
     NOT_ACTIVE = 2
 
 
-class JobStatus(Enum):
+class JobStatus(StrIntEnum):
     APPROVED = 3
     ASSIGNED_WAITING = 7
     CANCELED = 4
     DELIVERED = 2
     IN_PREPERATION = 0
     IN_PROGRESS = 1
     INVOICE_ACCEPTED = 5
@@ -301,39 +314,39 @@
     OVERDUE = 13
     PAYED = 6
     REQUESTED = 8
     TRANSFERRED_TO_ORDER = 12
     WITHOUT_INVOICE = 11
 
 
-class CallbackType(Enum):
+class CallbackType(StrIntEnum):
     NOTIFY = 2
     OBSERVER = 1
 
 
-class WorkflowStatus(Enum):
+class WorkflowStatus(StrIntEnum):
     CANCELED = 2
     INPREPARATION = 0
     RELEASED = 1
     RELEASED_FOR_SELECTION = 3
 
 
-class SearchScope(Enum):
+class SearchScope(StrIntEnum):
     DATE_OF_ORDER = 1
     END_dATE_EVENT = 8
     INSTALLMENT_DATE = 6
     ITEM_CREATION_DATE = 2
     ITEM_DELIVERED_ON = 5
     ITEM_DUE_DATE = 4
     ORDER_CLOSING_DATE = 9
     ORDER_DUE_DATE = 3
     START_DATE_EVENT = 7
 
 
-class TaxType(Enum):
+class TaxType(StrIntEnum):
     INFO = 3
     INFO_SUM = 6
     PRICE_BLOCK = 12
     SUM = 4
     TAX_1 = 0
     TAX_1_2 = 5
     TAX_1_2_3 = 8
@@ -346,72 +359,72 @@
     TAX_2_4_5 = 16
     TAX_3 = 7
     TAX_4 = 9
     TAX_5 = 13
     WITHOUT_TAX = 2
 
 
-class TimeFrameRelation_Invoice(Enum):
+class TimeFrameRelation_Invoice(StrIntEnum):
     INVOICE_DATE = 1
     PAYABLE_UNTIL = 3
     PAYED = 4
     VALUTA = 2
 
 
-class ExportedType(Enum):
+class ExportedType(StrIntEnum):
     BOTH = 3
     EXPORTED = 1
     NOT_EXPORTED = 2
 
 
-class JobActionLink(Enum):
+class JobActionLink(StrIntEnum):
     ACCEPT_JOB = 1
     DECLINE_JOB = 2
     DOWNLOADLINK_DOCUMENTS_JOB = 4
     JUMP_INTO_JOB = 3
 
 
-class TextModuleType(Enum):
+class TextModuleType(StrIntEnum):
     DATE_FIELD = 3
     HYPER_LINK = 7
     LIST_BOX = 2
     MEMO_FIELD = 4
     MEMO_HISTORY_FIELD = 5
     NUMBER_FIELD = 6
     TEXT_FIELD = 1
 
 
-class InvoiceStatusType(Enum):
+class InvoiceStatusType(StrIntEnum):
     CANCELED = 3
     CANCELLATION_VOUCHER = 7
     IN_PREPARATION = 5
     OUTSTANDING = 1
     PAID = 2
     REMINDER_CREATED = 4
     UNCOLLECTABLE = 6
     UNDEFINED = 0
 
 
-class EventType(Enum):
+class EventType(StrIntEnum):
     DELIVERY_DATE_CHANGED = 5
     ENTRY_DELETED = 3
     NEW_ENTRY_CREATED = 2
     START_DATE_CHANGED = 4
     STATUS_CHANGED = 1
     UNDEFINED = 0
 
 
-class ContactPersonStatus(Enum):
+class ContactPersonStatus(StrIntEnum):
     ACTIVE = 1
     CONTACTED = 3
     DELETION_REQUESTED = 4
     NOT_ACTIVE = 2
 
 
-class TextModuleUsageArea(Enum):
+class TextModuleUsageArea(StrIntEnum):
     CUSTOMER = 1
     ORDER = 6
     ORDER_CUSTOMER_LOGIN = 19
     ORDER_JOB = 11
     PAYMENT = 8
     QUOTE = 5
     QUOTE_CUSTOMER_LOGIN = 18
@@ -420,43 +433,44 @@
     RECEIVABLES_CREDIT_NOTE = 9
     REQUEST = 4
     REQUEST_CUSTOMER_LOGIN = 17
     RESOURCE = 2
     VENDOR = 3
 
 
-class ContactType(Enum):
+class ContactType(StrIntEnum):
     CUSTOMER = 1
     MISCELLANEOUS = 3
     RESOURCE = 2
 
 
-class CreditNoteStatus(Enum):
+class CreditNoteStatus(StrIntEnum):
     CANCELLATION_VOUCHER = 5
     CANCELLED = 4
     CLEARED = 3
     IN_PREPARATION = 1
     OPEN = 2
     PAID = 6
 
 
-class ProjectManagementType(Enum):
+class ProjectManagementType(StrIntEnum):
     MEMBER_OF_PROJECT_TEAM = 1
     PROJECT_MANAGEMENT = 0
     PROJECT_MANAGER = 2
     SUPERVISOR = 3
 
 
-class PropertyType(Enum):
+class PropertyType(StrIntEnum):
     MULTI_SELECT = 2
     SINGLE_SELECT = 1
 
 
-class OrderActionLink(Enum):
+class OrderActionLink(StrIntEnum):
     JUMP_INTO_ORDER = 1
     JUMP_INTO_ORDER_ASSET = 2
 
 
-class ProjectClassType(Enum):
+class ProjectClassType(StrIntEnum):
     ALL = 0
     INTERPRETING = 2
     TRANSLATION = 1
+
```

### Comparing `pyplunet-0.7.0/src/pyplunet/exceptions.py` & `pyplunet-0.8.0/src/pyplunet/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/src/pyplunet/models.py` & `pyplunet-0.8.0/src/pyplunet/models.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/src/pyplunet/retrying_client.py` & `pyplunet-0.8.0/src/pyplunet/retrying_client.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/src/pyplunet/services/__init__.py` & `pyplunet-0.8.0/src/pyplunet/services/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_admin30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_admin30.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,18 @@
     ServiceListResult,
     StringArrayResult,
     StringResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataAdmin30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
     def get_domestic_currency(
         self,
     ) -> StringResult:
         """
         Returns the default currency.
@@ -60,46 +59,48 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=None,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_list_of_registered_callbacks(
-        self,
-    ) -> CallbackListResult:
+    def get_available_countries(self, language_code: str) -> CountryListResult:
         """
-        Returns a list of all registered callbacks (observer & notifies) to the current user
+        Method returns an instance of CountryListResult,
+        which contains an array of available countries in the system,
+        returned in the language specified by the language code.
 
 
-        :return: CallbackListResult
+        :param language_code: str
+        :return: CountryListResult
         """
 
-        proxy = self.__client.plunet_server.DataAdmin30.getListOfRegisteredCallbacks
-        response_model = CallbackListResult
+        proxy = self.__client.plunet_server.DataAdmin30.getAvailableCountries
+        response_model = CountryListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=None,
+            argument=language_code,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_company_code_list(
+    def get_system_currencies(
         self,
-    ) -> CompanyCodeListResult:
+    ) -> CurrencyList:
         """
-        Returns a list of all possible company-codes.
+        Returns a list of all currencies configured within the administration
+        area
 
 
-        :return: CompanyCodeListResult
+        :return: CurrencyList
         """
 
-        proxy = self.__client.plunet_server.DataAdmin30.getCompanyCodeList
-        response_model = CompanyCodeListResult
+        proxy = self.__client.plunet_server.DataAdmin30.getSystemCurrencies
+        response_model = CurrencyList
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=None,
             response_model=response_model,
             unpack_dict=False,
         )
@@ -122,69 +123,67 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=language_code,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_available_countries(self, language_code: str) -> CountryListResult:
+    def get_available_languages(self, language_code: str) -> LanguageListResult:
         """
-        Method returns an instance of CountryListResult,
-        which contains an array of available countries in the system,
+        Method returns an instance of LanguageListResult,
+        which contains an array of available languages in the system,
         returned in the language specified by the language code.
 
 
         :param language_code: str
-        :return: CountryListResult
+        :return: LanguageListResult
         """
 
-        proxy = self.__client.plunet_server.DataAdmin30.getAvailableCountries
-        response_model = CountryListResult
+        proxy = self.__client.plunet_server.DataAdmin30.getAvailableLanguages
+        response_model = LanguageListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=language_code,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_system_currencies(
+    def get_company_code_list(
         self,
-    ) -> CurrencyList:
+    ) -> CompanyCodeListResult:
         """
-        Returns a list of all currencies configured within the administration
-        area
+        Returns a list of all possible company-codes.
 
 
-        :return: CurrencyList
+        :return: CompanyCodeListResult
         """
 
-        proxy = self.__client.plunet_server.DataAdmin30.getSystemCurrencies
-        response_model = CurrencyList
+        proxy = self.__client.plunet_server.DataAdmin30.getCompanyCodeList
+        response_model = CompanyCodeListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=None,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_available_languages(self, language_code: str) -> LanguageListResult:
+    def get_list_of_registered_callbacks(
+        self,
+    ) -> CallbackListResult:
         """
-        Method returns an instance of LanguageListResult,
-        which contains an array of available languages in the system,
-        returned in the language specified by the language code.
+        Returns a list of all registered callbacks (observer & notifies) to the current user
 
 
-        :param language_code: str
-        :return: LanguageListResult
+        :return: CallbackListResult
         """
 
-        proxy = self.__client.plunet_server.DataAdmin30.getAvailableLanguages
-        response_model = LanguageListResult
+        proxy = self.__client.plunet_server.DataAdmin30.getListOfRegisteredCallbacks
+        response_model = CallbackListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=language_code,
+            argument=None,
             response_model=response_model,
             unpack_dict=False,
         )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_credit_note30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_credit_note30.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,62 +18,20 @@
     SearchFilter_CreditNote,
     StringResult,
     TaxListResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataCreditNote30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
-    def get_subject(self, credit_note_id: int) -> StringResult:
-        """
-        Returns an instance of StringResult, which contains the subject.
-
-
-        :param credit_note_id: int
-        :return: StringResult
-        """
-
-        proxy = self.__client.plunet_server.DataCreditNote30.getSubject
-        response_model = StringResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=credit_note_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def set_subject(self, subject: str, credit_note_id: int) -> Result:
-        """
-        Defines the subject.
-
-
-        :param subject: str
-        :param credit_note_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataCreditNote30.setSubject
-        response_model = Result
-
-        arg = {"subject": subject, "creditNoteID": credit_note_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
     def search(
         self, search_filter: Union[SearchFilter_CreditNote, dict]
     ) -> IntegerArrayResult:
         """
         Search implementation to filter for any existing credit note based on
         the search filter.
 
@@ -93,110 +51,51 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=search_filter,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_receivable_account(self, account_id: int, credit_note_id: int) -> Result:
-        """
-        Sets the receivable account.
-
-
-        :param account_id: int
-        :param credit_note_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataCreditNote30.setReceivableAccount
-        response_model = Result
-
-        arg = {"accountID": account_id, "creditNoteID": credit_note_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def get_revenue_account(self, credit_note_id: int) -> StringResult:
-        """
-        Returns the revenue account.
-
-
-        :param credit_note_id: int
-        :return: StringResult
-        """
-
-        proxy = self.__client.plunet_server.DataCreditNote30.getRevenueAccount
-        response_model = StringResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=credit_note_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def get_receivable_account(self, credit_note_id: int) -> StringResult:
+    def get_currency_code(self, credit_note_id: int) -> StringResult:
         """
-        Returns the receivable account.
+        Returns an instance of StringResult, which contains the currency code
+        of the specified credit note (the amount is standard currency).
 
 
         :param credit_note_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getReceivableAccount
+        proxy = self.__client.plunet_server.DataCreditNote30.getCurrencyCode
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_revenue_account(self, account_id: int, credit_note_id: int) -> Result:
-        """
-        Sets the revenue account.
-
-
-        :param account_id: int
-        :param credit_note_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataCreditNote30.setRevenueAccount
-        response_model = Result
-
-        arg = {"accountID": account_id, "creditNoteID": credit_note_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def get_tax_by_currency_type(
+    def get_outstanding_by_currency_type(
         self, credit_note_id: int, currency_type: Union[CurrencyType, int]
     ) -> DoubleResult:
         """
-        Returns an instance of DoubleResult, which contains the summed up taxes in the specified (project or home) currency.
+        Returns an instance of DoubleResult, which contains the outstanding
+        amount in the specified (project or home) currency.
         Default currency is the project currency.
 
 
         :param credit_note_id: int
         :param currency_type: CurrencyType
         :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getTaxByCurrencyType
+        proxy = (
+            self.__client.plunet_server.DataCreditNote30.getOutstandingByCurrencyType
+        )
         response_model = DoubleResult
 
         if type(currency_type) == CurrencyType:
             currency_type = currency_type.value
         elif type(currency_type) == int:
             currency_type = currency_type
         else:
@@ -254,29 +153,68 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def delete_credit_note_item(self, credit_note_item_id: int) -> Result:
+    def get_gross_by_currency_type(
+        self, credit_note_id: int, currency_type: Union[CurrencyType, int]
+    ) -> DoubleResult:
         """
-        Deletes an credit note item.
+        Returns an instance of DoubleResult, which contains the credit note amount in the specified (project or home) currency.
+        Default currency is the project currency.
 
 
-        :param credit_note_item_id: int
-        :return: Result
+        :param credit_note_id: int
+        :param currency_type: CurrencyType
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.deleteCreditNoteItem
-        response_model = Result
+        proxy = self.__client.plunet_server.DataCreditNote30.getGrossByCurrencyType
+        response_model = DoubleResult
+
+        if type(currency_type) == CurrencyType:
+            currency_type = currency_type.value
+        elif type(currency_type) == int:
+            currency_type = currency_type
+        else:
+            currency_type = int(currency_type)
+
+        arg = {"creditNoteID": credit_note_id, "currencyType": currency_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=credit_note_item_id,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def insert_credit_note_item(
+        self, credit_note_item_in: Union[CreditNoteItemIN, dict]
+    ) -> IntegerResult:
+        """
+        Inserts a new credit note item.
+
+
+        :param credit_note_item_in: CreditNoteItemIN
+        :return: IntegerResult
+        """
+
+        proxy = self.__client.plunet_server.DataCreditNote30.insertCreditNoteItem
+        response_model = IntegerResult
+
+        if type(credit_note_item_in) != CreditNoteItemIN:
+            credit_note_item_in = CreditNoteItemIN(**credit_note_item_in).dict()
+        else:
+            credit_note_item_in = credit_note_item_in.dict()
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=credit_note_item_in,
             response_model=response_model,
             unpack_dict=False,
         )
 
     def get_credit_note_item_list(self, credit_note_id: int) -> CreditNoteListResult:
         """
         Retunrs a list of all credit note items.
@@ -292,38 +230,44 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def insert_credit_note_item(
-        self, credit_note_item_in: Union[CreditNoteItemIN, dict]
-    ) -> IntegerResult:
+    def get_tax_by_currency_type(
+        self, credit_note_id: int, currency_type: Union[CurrencyType, int]
+    ) -> DoubleResult:
         """
-        Inserts a new credit note item.
+        Returns an instance of DoubleResult, which contains the summed up taxes in the specified (project or home) currency.
+        Default currency is the project currency.
 
 
-        :param credit_note_item_in: CreditNoteItemIN
-        :return: IntegerResult
+        :param credit_note_id: int
+        :param currency_type: CurrencyType
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.insertCreditNoteItem
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataCreditNote30.getTaxByCurrencyType
+        response_model = DoubleResult
 
-        if type(credit_note_item_in) != CreditNoteItemIN:
-            credit_note_item_in = CreditNoteItemIN(**credit_note_item_in).dict()
+        if type(currency_type) == CurrencyType:
+            currency_type = currency_type.value
+        elif type(currency_type) == int:
+            currency_type = currency_type
         else:
-            credit_note_item_in = credit_note_item_in.dict()
+            currency_type = int(currency_type)
+
+        arg = {"creditNoteID": credit_note_id, "currencyType": currency_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=credit_note_item_in,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
     def update_credit_note_item(
         self,
         credit_note_item_id: int,
         credit_note_item_in: Union[CreditNoteItemIN, dict],
     ) -> Result:
@@ -384,468 +328,534 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_gross_by_currency_type(
-        self, credit_note_id: int, currency_type: Union[CurrencyType, int]
-    ) -> DoubleResult:
+    def delete_credit_note_item(self, credit_note_item_id: int) -> Result:
         """
-        Returns an instance of DoubleResult, which contains the credit note amount in the specified (project or home) currency.
-        Default currency is the project currency.
+        Deletes an credit note item.
 
 
-        :param credit_note_id: int
-        :param currency_type: CurrencyType
-        :return: DoubleResult
+        :param credit_note_item_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getGrossByCurrencyType
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataCreditNote30.deleteCreditNoteItem
+        response_model = Result
 
-        if type(currency_type) == CurrencyType:
-            currency_type = currency_type.value
-        elif type(currency_type) == int:
-            currency_type = currency_type
-        else:
-            currency_type = int(currency_type)
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=credit_note_item_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
 
-        arg = {"creditNoteID": credit_note_id, "currencyType": currency_type}
+    def set_address_id(self, credit_note_id: int, address_id: int) -> Result:
+        """
+        Sets the addressID which has to be related to the credit note related customer.
+        Address information can be obtained over
+        DataCustomerAddress30
+
+
+        :param credit_note_id: int
+        :param address_id: int
+        :return: Result
+        """
+
+        proxy = self.__client.plunet_server.DataCreditNote30.setAddressID
+        response_model = Result
+
+        arg = {"creditNoteID": credit_note_id, "addressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_outstanding_by_currency_type(
-        self, credit_note_id: int, currency_type: Union[CurrencyType, int]
-    ) -> DoubleResult:
+    def set_customer_id(self, customer_id: int, credit_note_id: int) -> Result:
         """
-        Returns an instance of DoubleResult, which contains the outstanding
-        amount in the specified (project or home) currency.
-        Default currency is the project currency.
+        Sets the customer ID for the specified credit note.
 
 
+        :param customer_id: int
         :param credit_note_id: int
-        :param currency_type: CurrencyType
-        :return: DoubleResult
+        :return: Result
         """
 
-        proxy = (
-            self.__client.plunet_server.DataCreditNote30.getOutstandingByCurrencyType
-        )
-        response_model = DoubleResult
-
-        if type(currency_type) == CurrencyType:
-            currency_type = currency_type.value
-        elif type(currency_type) == int:
-            currency_type = currency_type
-        else:
-            currency_type = int(currency_type)
+        proxy = self.__client.plunet_server.DataCreditNote30.setCustomerID
+        response_model = Result
 
-        arg = {"creditNoteID": credit_note_id, "currencyType": currency_type}
+        arg = {"customerID": customer_id, "creditNoteID": credit_note_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_currency_code(self, credit_note_id: int) -> StringResult:
+    def get_invoice_id(self, credit_note_id: int) -> IntegerResult:
         """
-        Returns an instance of StringResult, which contains the currency code
-        of the specified credit note (the amount is standard currency).
+        Returns the credit note related invoice ID.
 
 
         :param credit_note_id: int
-        :return: StringResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getCurrencyCode
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCreditNote30.getInvoiceID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_customer_id(self, customer_id: int, credit_note_id: int) -> Result:
+    def update_price_line(self, price_line_in: Union[PriceLineIN, dict]) -> Result:
         """
-        Sets the customer ID for the specified credit note.
+        Updates a existing PriceLine.
 
 
-        :param customer_id: int
-        :param credit_note_id: int
+        :param price_line_in: PriceLineIN
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.setCustomerID
+        proxy = self.__client.plunet_server.DataCreditNote30.updatePriceLine
         response_model = Result
 
-        arg = {"customerID": customer_id, "creditNoteID": credit_note_id}
+        if type(price_line_in) != PriceLineIN:
+            price_line_in = PriceLineIN(**price_line_in).dict()
+        else:
+            price_line_in = price_line_in.dict()
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=price_line_in,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def insert_price_line(
+        self, credit_note_item_id: int, price_line_in: Union[PriceLineIN, dict]
+    ) -> IntegerResult:
+        """
+        Inserts a new PriceLineIN to the specified credit note
+        item.
+
+
+        :param credit_note_item_id: int
+        :param price_line_in: PriceLineIN
+        :return: IntegerResult
+        """
+
+        proxy = self.__client.plunet_server.DataCreditNote30.insertPriceLine
+        response_model = IntegerResult
+
+        if type(price_line_in) != PriceLineIN:
+            price_line_in = PriceLineIN(**price_line_in).dict()
+        else:
+            price_line_in = price_line_in.dict()
+
+        arg = {"creditNoteItemID": credit_note_item_id, "priceLineIN": price_line_in}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_address_id(self, credit_note_id: int, address_id: int) -> Result:
+    def delete_price_line(self, price_line_id: int) -> Result:
         """
-        Sets the addressID which has to be related to the credit note related customer.
-        Address information can be obtained over
-        DataCustomerAddress30
+        Deletes an existing PriceLine.
 
 
-        :param credit_note_id: int
-        :param address_id: int
+        :param price_line_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.setAddressID
+        proxy = self.__client.plunet_server.DataCreditNote30.deletePriceLine
         response_model = Result
 
-        arg = {"creditNoteID": credit_note_id, "addressID": address_id}
-
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=price_line_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_status(self, credit_note_id: int) -> IntegerResult:
+    def get_net(self, credit_note_id: int) -> DoubleResult:
         """
-        Returns an instance of IntegerResult, which contains the
-        CreditNoteStatus.
+        Returns an instance of DoubleResult, which contains the net amount (in project currency).
 
 
         :param credit_note_id: int
-        :return: IntegerResult
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getStatus
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataCreditNote30.getNet
+        response_model = DoubleResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_status(self, status: int, credit_note_id: int) -> Result:
+    def get_gross(self, credit_note_id: int) -> DoubleResult:
         """
-        Defines the CreditNoteStatus.
+        Returns an instance of DoubleResult, which contains the credit note amount (in project currency).
 
 
-        :param status: int
         :param credit_note_id: int
-        :return: Result
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.setStatus
-        response_model = Result
+        proxy = self.__client.plunet_server.DataCreditNote30.getGross
+        response_model = DoubleResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=credit_note_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_outstanding(self, credit_note_id: int) -> DoubleResult:
+        """
+        Returns an instance of DoubleResult, which contains the outstanding
+        amount (in project currency).
 
-        arg = {"Status": status, "creditNoteID": credit_note_id}
+
+        :param credit_note_id: int
+        :return: DoubleResult
+        """
+
+        proxy = self.__client.plunet_server.DataCreditNote30.getOutstanding
+        response_model = DoubleResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=credit_note_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_brief_description(self, credit_note_id: int) -> StringResult:
+    def get_tax(self, credit_note_id: int) -> DoubleResult:
         """
-        Returns the brief description.
+        Returns an instance of DoubleResult, which contains all taxes as summed up values (in project currency).
 
 
         :param credit_note_id: int
-        :return: StringResult
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getBriefDescription
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCreditNote30.getTax
+        response_model = DoubleResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_brief_description(self, description: str, credit_note_id: int) -> Result:
+    def get_tax_types(self, credit_note_id: int) -> TaxListResult:
         """
-        Sets the brief description.
+        Returns a list of all tax types which are used within the transfered credit note.
+        Possible currency codes can be configured over Admin|Settings|Comany Code
 
 
-        :param description: str
         :param credit_note_id: int
-        :return: Result
+        :return: TaxListResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.setBriefDescription
-        response_model = Result
+        proxy = self.__client.plunet_server.DataCreditNote30.getTaxTypes
+        response_model = TaxListResult
 
-        arg = {"description": description, "creditNoteID": credit_note_id}
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=credit_note_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_credit_date(self, credit_note_id: int) -> DateResult:
+        """
+        Returns an instance of DateResult, which contains the credit note date.
+
+
+        :param credit_note_id: int
+        :return: DateResult
+        """
+
+        proxy = self.__client.plunet_server.DataCreditNote30.getCreditDate
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=credit_note_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_contact_person_id(self, credit_note_id: int) -> IntegerResult:
+    def get_credit_note_nr(self, credit_note_id: int) -> StringResult:
         """
-        Returns the id to the credit note related contact person
-        (resource).
+        Returns an instance of StringResult, which contains the credit note
+        number.
 
-        Contact Person details can be obtained over
-        DataCustomerContact30
+
+        :param credit_note_id: int
+        :return: StringResult
+        """
+
+        proxy = self.__client.plunet_server.DataCreditNote30.getCreditNoteNr
+        response_model = StringResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=credit_note_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_company_code(self, credit_note_id: int) -> IntegerResult:
+        """
+        Returns the type dependent company code, related to the specified
+        credit note.
 
 
         :param credit_note_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getContactPersonID
+        proxy = self.__client.plunet_server.DataCreditNote30.getCompanyCode
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_contact_person_id(
-        self, credit_note_id: int, contact_person_id: int
-    ) -> Result:
+    def set_is_exported(self, credit_note_id: int, is_exported: bool) -> Result:
         """
-        Sets the customer depended contact person for the specified credit note.
-        Contact Person details can be obtained over
-        DataCustomerContact30
+        Defines if the credit note is already exported.
 
 
         :param credit_note_id: int
-        :param contact_person_id: int
+        :param is_exported: bool
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.setContactPersonID
+        proxy = self.__client.plunet_server.DataCreditNote30.setIsExported
         response_model = Result
 
-        arg = {"creditNoteID": credit_note_id, "contactPersonID": contact_person_id}
+        arg = {"creditNoteID": credit_note_id, "isExported": is_exported}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def update_price_line(self, price_line_in: Union[PriceLineIN, dict]) -> Result:
+    def set_credit_date(self, credit_date: datetime, credit_note_id: int) -> Result:
         """
-        Updates a existing PriceLine.
+        Defines the credit date.
 
 
-        :param price_line_in: PriceLineIN
+        :param credit_date: datetime
+        :param credit_note_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.updatePriceLine
+        proxy = self.__client.plunet_server.DataCreditNote30.setCreditDate
         response_model = Result
 
-        if type(price_line_in) != PriceLineIN:
-            price_line_in = PriceLineIN(**price_line_in).dict()
-        else:
-            price_line_in = price_line_in.dict()
+        arg = {"creditDate": credit_date, "creditNoteID": credit_note_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=price_line_in,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def insert_price_line(
-        self, credit_note_item_id: int, price_line_in: Union[PriceLineIN, dict]
-    ) -> IntegerResult:
+    def get_adress_id(self, credit_note_id: int) -> IntegerResult:
         """
-        Inserts a new PriceLineIN to the specified credit note
-        item.
+        Return the ID of the customer address entry this credit note is mapped to.
+        Address information can be obtained over
+        DataCustomerAddress30
 
 
-        :param credit_note_item_id: int
-        :param price_line_in: PriceLineIN
+        :param credit_note_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.insertPriceLine
+        proxy = self.__client.plunet_server.DataCreditNote30.getAdressID
         response_model = IntegerResult
 
-        if type(price_line_in) != PriceLineIN:
-            price_line_in = PriceLineIN(**price_line_in).dict()
-        else:
-            price_line_in = price_line_in.dict()
-
-        arg = {"creditNoteItemID": credit_note_item_id, "priceLineIN": price_line_in}
-
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=credit_note_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def delete_price_line(self, price_line_id: int) -> Result:
+    def get_price_line(self, price_line_id: int) -> PriceLineResult:
         """
-        Deletes an existing PriceLine.
+        Returns an existing PriceLine.
 
 
         :param price_line_id: int
-        :return: Result
+        :return: PriceLineResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.deletePriceLine
-        response_model = Result
+        proxy = self.__client.plunet_server.DataCreditNote30.getPriceLine
+        response_model = PriceLineResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=price_line_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_po_number(self, credit_note_id: int, po_number: str) -> Result:
+    def set_paid_date(self, credit_note_id: int, paid_date: datetime) -> Result:
         """
-        Defines the po number of the related credit note.
+        Defines the date the credit note is payed.
 
 
         :param credit_note_id: int
-        :param po_number: str
+        :param paid_date: datetime
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.setPONumber
+        proxy = self.__client.plunet_server.DataCreditNote30.setPaidDate
         response_model = Result
 
-        arg = {"creditNoteID": credit_note_id, "poNumber": po_number}
+        arg = {"creditNoteID": credit_note_id, "paidDate": paid_date}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_outstanding(self, credit_note_id: int) -> DoubleResult:
+    def get_credit_note_id(
+        self, display_name: str, company_code_id: int
+    ) -> IntegerResult:
         """
-        Returns an instance of DoubleResult, which contains the outstanding
-        amount (in project currency).
+        Get the creditNoteId based on the display name and company code of the credit note.
 
 
-        :param credit_note_id: int
-        :return: DoubleResult
+        :param display_name: str
+        :param company_code_id: int
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getOutstanding
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataCreditNote30.getCreditNoteId
+        response_model = IntegerResult
+
+        arg = {"displayName": display_name, "companyCodeId": company_code_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=credit_note_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_gross(self, credit_note_id: int) -> DoubleResult:
+    def get_is_exported(self, credit_note_id: int) -> BooleanResult:
         """
-        Returns an instance of DoubleResult, which contains the credit note amount (in project currency).
+        Returns if the credit note is already exported.
 
 
         :param credit_note_id: int
-        :return: DoubleResult
+        :return: BooleanResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getGross
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataCreditNote30.getIsExported
+        response_model = BooleanResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_net(self, credit_note_id: int) -> DoubleResult:
+    def get_paid_date(self, credit_note_id: int) -> DateResult:
         """
-        Returns an instance of DoubleResult, which contains the net amount (in project currency).
+        Retuns the date the credit note is payed.
 
 
         :param credit_note_id: int
-        :return: DoubleResult
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getNet
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataCreditNote30.getPaidDate
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_tax(self, credit_note_id: int) -> DoubleResult:
+    def get_po_number(self, credit_note_id: int) -> StringResult:
         """
-        Returns an instance of DoubleResult, which contains all taxes as summed up values (in project currency).
+        Returns the PO-number
 
 
         :param credit_note_id: int
-        :return: DoubleResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getTax
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataCreditNote30.getPONumber
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_invoice_id(self, credit_note_id: int) -> IntegerResult:
+    def set_status(self, status: int, credit_note_id: int) -> Result:
         """
-        Returns the credit note related invoice ID.
+        Defines the CreditNoteStatus.
 
 
+        :param status: int
         :param credit_note_id: int
-        :return: IntegerResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getInvoiceID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataCreditNote30.setStatus
+        response_model = Result
+
+        arg = {"Status": status, "creditNoteID": credit_note_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=credit_note_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
     def get_customer_id(self, credit_note_id: int) -> IntegerResult:
         """
         Returns an instance of IntegerResult, which contains the
         customer ID.
 
@@ -860,272 +870,261 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_adress_id(self, credit_note_id: int) -> IntegerResult:
+    def get_status(self, credit_note_id: int) -> IntegerResult:
         """
-        Return the ID of the customer address entry this credit note is mapped to.
-        Address information can be obtained over
-        DataCustomerAddress30
+        Returns an instance of IntegerResult, which contains the
+        CreditNoteStatus.
 
 
         :param credit_note_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getAdressID
+        proxy = self.__client.plunet_server.DataCreditNote30.getStatus
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_is_exported(self, credit_note_id: int) -> BooleanResult:
+    def get_subject(self, credit_note_id: int) -> StringResult:
         """
-        Returns if the credit note is already exported.
+        Returns an instance of StringResult, which contains the subject.
 
 
         :param credit_note_id: int
-        :return: BooleanResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getIsExported
-        response_model = BooleanResult
+        proxy = self.__client.plunet_server.DataCreditNote30.getSubject
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_is_exported(self, credit_note_id: int, is_exported: bool) -> Result:
+    def set_subject(self, subject: str, credit_note_id: int) -> Result:
         """
-        Defines if the credit note is already exported.
+        Defines the subject.
 
 
+        :param subject: str
         :param credit_note_id: int
-        :param is_exported: bool
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.setIsExported
+        proxy = self.__client.plunet_server.DataCreditNote30.setSubject
         response_model = Result
 
-        arg = {"creditNoteID": credit_note_id, "isExported": is_exported}
+        arg = {"subject": subject, "creditNoteID": credit_note_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_paid_date(self, credit_note_id: int) -> DateResult:
+    def set_po_number(self, credit_note_id: int, po_number: str) -> Result:
         """
-        Retuns the date the credit note is payed.
+        Defines the po number of the related credit note.
 
 
         :param credit_note_id: int
-        :return: DateResult
+        :param po_number: str
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getPaidDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataCreditNote30.setPONumber
+        response_model = Result
+
+        arg = {"creditNoteID": credit_note_id, "poNumber": po_number}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=credit_note_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_po_number(self, credit_note_id: int) -> StringResult:
+    def get_brief_description(self, credit_note_id: int) -> StringResult:
         """
-        Returns the PO-number
+        Returns the brief description.
 
 
         :param credit_note_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getPONumber
+        proxy = self.__client.plunet_server.DataCreditNote30.getBriefDescription
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_credit_note_id(
-        self, display_name: str, company_code_id: int
-    ) -> IntegerResult:
+    def set_brief_description(self, description: str, credit_note_id: int) -> Result:
         """
-        Get the creditNoteId based on the display name and company code of the credit note.
+        Sets the brief description.
 
 
-        :param display_name: str
-        :param company_code_id: int
-        :return: IntegerResult
+        :param description: str
+        :param credit_note_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getCreditNoteId
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataCreditNote30.setBriefDescription
+        response_model = Result
 
-        arg = {"displayName": display_name, "companyCodeId": company_code_id}
+        arg = {"description": description, "creditNoteID": credit_note_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_credit_date(self, credit_note_id: int) -> DateResult:
+    def get_revenue_account(self, credit_note_id: int) -> StringResult:
         """
-        Returns an instance of DateResult, which contains the credit note date.
+        Returns the revenue account.
 
 
         :param credit_note_id: int
-        :return: DateResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getCreditDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataCreditNote30.getRevenueAccount
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_paid_date(self, credit_note_id: int, paid_date: datetime) -> Result:
+    def get_receivable_account(self, credit_note_id: int) -> StringResult:
         """
-        Defines the date the credit note is payed.
+        Returns the receivable account.
 
 
         :param credit_note_id: int
-        :param paid_date: datetime
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.setPaidDate
-        response_model = Result
-
-        arg = {"creditNoteID": credit_note_id, "paidDate": paid_date}
+        proxy = self.__client.plunet_server.DataCreditNote30.getReceivableAccount
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=credit_note_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_price_line(self, price_line_id: int) -> PriceLineResult:
+    def set_receivable_account(self, account_id: int, credit_note_id: int) -> Result:
         """
-        Returns an existing PriceLine.
+        Sets the receivable account.
 
 
-        :param price_line_id: int
-        :return: PriceLineResult
+        :param account_id: int
+        :param credit_note_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getPriceLine
-        response_model = PriceLineResult
+        proxy = self.__client.plunet_server.DataCreditNote30.setReceivableAccount
+        response_model = Result
+
+        arg = {"accountID": account_id, "creditNoteID": credit_note_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=price_line_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_credit_date(self, credit_date: datetime, credit_note_id: int) -> Result:
+    def set_revenue_account(self, account_id: int, credit_note_id: int) -> Result:
         """
-        Defines the credit date.
+        Sets the revenue account.
 
 
-        :param credit_date: datetime
+        :param account_id: int
         :param credit_note_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.setCreditDate
+        proxy = self.__client.plunet_server.DataCreditNote30.setRevenueAccount
         response_model = Result
 
-        arg = {"creditDate": credit_date, "creditNoteID": credit_note_id}
+        arg = {"accountID": account_id, "creditNoteID": credit_note_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_company_code(self, credit_note_id: int) -> IntegerResult:
+    def get_contact_person_id(self, credit_note_id: int) -> IntegerResult:
         """
-        Returns the type dependent company code, related to the specified
-        credit note.
+        Returns the id to the credit note related contact person
+        (resource).
+
+        Contact Person details can be obtained over
+        DataCustomerContact30
 
 
         :param credit_note_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getCompanyCode
+        proxy = self.__client.plunet_server.DataCreditNote30.getContactPersonID
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=credit_note_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_tax_types(self, credit_note_id: int) -> TaxListResult:
+    def set_contact_person_id(
+        self, credit_note_id: int, contact_person_id: int
+    ) -> Result:
         """
-        Returns a list of all tax types which are used within the transfered credit note.
-        Possible currency codes can be configured over Admin|Settings|Comany Code
+        Sets the customer depended contact person for the specified credit note.
+        Contact Person details can be obtained over
+        DataCustomerContact30
 
 
         :param credit_note_id: int
-        :return: TaxListResult
-        """
-
-        proxy = self.__client.plunet_server.DataCreditNote30.getTaxTypes
-        response_model = TaxListResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=credit_note_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def get_credit_note_nr(self, credit_note_id: int) -> StringResult:
+        :param contact_person_id: int
+        :return: Result
         """
-        Returns an instance of StringResult, which contains the credit note
-        number.
-
 
-        :param credit_note_id: int
-        :return: StringResult
-        """
+        proxy = self.__client.plunet_server.DataCreditNote30.setContactPersonID
+        response_model = Result
 
-        proxy = self.__client.plunet_server.DataCreditNote30.getCreditNoteNr
-        response_model = StringResult
+        arg = {"creditNoteID": credit_note_id, "contactPersonID": contact_person_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=credit_note_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_custom_fields30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_custom_fields30.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,18 @@
     StringResult,
     TextmoduleIN,
     TextmoduleResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataCustomFields30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
     def get_property(
         self,
         property_name_english: str,
         property_usage_area: Union[PropertyUsageArea, int],
         main_id: int,
@@ -62,105 +61,14 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_property_value_list(
-        self,
-        property_name_english: str,
-        property_usage_area: Union[PropertyUsageArea, int],
-        property_value_list: Union[IntegerList, dict],
-        main_id: int,
-    ) -> Result:
-        """
-        Changes the current selected property value for the specific object
-        (mainID) to the specified property value ID.
-        Possible property values for the property can be obtained over
-        getProperty(String, String, int, int).
-        Properties can be configured over admin/properties.
-        The PropertyNameEnglish can be obtained there.
-        The type of the MainID is related to the used PropertyUsageArea.
-        e.g. Should the property be related to an order, the propertyusageArea
-        must be set to PropertyUsageArea.ORDER
-        Note:
-        Properties can also be modified over general plunet api calls. Please
-        check PropertyUsageArea for more details, which call can affect
-        which kind of properties.
-
-
-        :param property_name_english: str
-        :param property_usage_area: PropertyUsageArea
-        :param property_value_list: IntegerList
-        :param main_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataCustomFields30.setPropertyValueList
-        response_model = Result
-
-        if type(property_value_list) != IntegerList:
-            property_value_list = IntegerList(**property_value_list).dict()
-        else:
-            property_value_list = property_value_list.dict()
-
-        if type(property_usage_area) == PropertyUsageArea:
-            property_usage_area = property_usage_area.value
-        elif type(property_usage_area) == int:
-            property_usage_area = property_usage_area
-        else:
-            property_usage_area = int(property_usage_area)
-
-        arg = {
-            "PropertyNameEnglish": property_name_english,
-            "PropertyUsageArea": property_usage_area,
-            "PropertyValueList": property_value_list,
-            "MainID": main_id,
-        }
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def get_property_value_text(
-        self, property_name_english: str, property_value_id: int, language_code: str
-    ) -> StringResult:
-        """
-        Returns the value text dependent on the language-code and propertyValueID.
-        Language-Codes can be configured over admin/languages
-        Properties can be configured over admin/properties.
-        The PropertyNameEnglish can be obtained there.
-
-
-        :param property_name_english: str
-        :param property_value_id: int
-        :param language_code: str
-        :return: StringResult
-        """
-
-        proxy = self.__client.plunet_server.DataCustomFields30.getPropertyValueText
-        response_model = StringResult
-
-        arg = {
-            "PropertyNameEnglish": property_name_english,
-            "PropertyValueID": property_value_id,
-            "languageCode": language_code,
-        }
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
     def get_textmodule(
         self,
         flag: str,
         text_module_usage_area: Union[TextModuleUsageArea, int],
         id: int,
         language_code: str,
     ) -> TextmoduleResult:
@@ -273,9 +181,100 @@
             "MainID": main_id,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def get_property_value_text(
+        self, property_name_english: str, property_value_id: int, language_code: str
+    ) -> StringResult:
+        """
+        Returns the value text dependent on the language-code and propertyValueID.
+        Language-Codes can be configured over admin/languages
+        Properties can be configured over admin/properties.
+        The PropertyNameEnglish can be obtained there.
+
+
+        :param property_name_english: str
+        :param property_value_id: int
+        :param language_code: str
+        :return: StringResult
+        """
+
+        proxy = self.__client.plunet_server.DataCustomFields30.getPropertyValueText
+        response_model = StringResult
+
+        arg = {
+            "PropertyNameEnglish": property_name_english,
+            "PropertyValueID": property_value_id,
+            "languageCode": language_code,
+        }
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def set_property_value_list(
+        self,
+        property_name_english: str,
+        property_usage_area: Union[PropertyUsageArea, int],
+        property_value_list: Union[IntegerList, dict],
+        main_id: int,
+    ) -> Result:
+        """
+        Changes the current selected property value for the specific object
+        (mainID) to the specified property value ID.
+        Possible property values for the property can be obtained over
+        getProperty(String, String, int, int).
+        Properties can be configured over admin/properties.
+        The PropertyNameEnglish can be obtained there.
+        The type of the MainID is related to the used PropertyUsageArea.
+        e.g. Should the property be related to an order, the propertyusageArea
+        must be set to PropertyUsageArea.ORDER
+        Note:
+        Properties can also be modified over general plunet api calls. Please
+        check PropertyUsageArea for more details, which call can affect
+        which kind of properties.
+
+
+        :param property_name_english: str
+        :param property_usage_area: PropertyUsageArea
+        :param property_value_list: IntegerList
+        :param main_id: int
+        :return: Result
+        """
+
+        proxy = self.__client.plunet_server.DataCustomFields30.setPropertyValueList
+        response_model = Result
+
+        if type(property_value_list) != IntegerList:
+            property_value_list = IntegerList(**property_value_list).dict()
+        else:
+            property_value_list = property_value_list.dict()
+
+        if type(property_usage_area) == PropertyUsageArea:
+            property_usage_area = property_usage_area.value
+        elif type(property_usage_area) == int:
+            property_usage_area = property_usage_area
+        else:
+            property_usage_area = int(property_usage_area)
+
+        arg = {
+            "PropertyNameEnglish": property_name_english,
+            "PropertyUsageArea": property_usage_area,
+            "PropertyValueList": property_value_list,
+            "MainID": main_id,
+        }
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
             unpack_dict=True,
         )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_customer30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_customer30.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,18 @@
     SearchFilter_Customer,
     StringResult,
     WorkflowListResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataCustomer30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
     def update(
         self, customer_in: Union[CustomerIN, dict], enable_null_or_empty_values: bool
     ) -> Result:
         """
         Updates an Customer per Object.
@@ -148,1230 +147,1230 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_project_manager_id(self, customer_id: int) -> IntegerResult:
+    def get_full_name(self, customer_id: int) -> StringResult:
         """
-        Returns the resourceID of the project-manager of the
-        the specified customer.
-
-        Returns resourceID = 0 when no project-manager is specified.
+        Returns an instance of StringResult, which contains the full name of the
+        currently selected customer.
 
 
         :param customer_id: int
-        :return: IntegerResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getProjectManagerID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataCustomer30.getFullName
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_created_by_resource_id(self, customer_id: int) -> IntegerResult:
+    def set_dossier(self, customer_id: int, dossier: str) -> Result:
         """
-        Returns the ResourceID which has created the Customer.
+        Sets the dossier field.
 
 
         :param customer_id: int
-        :return: IntegerResult
+        :param dossier: str
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getCreatedByResourceID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataCustomer30.setDossier
+        response_model = Result
+
+        arg = {"customerID": customer_id, "dossier": dossier}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_payment_information(
-        self, customer_id: int, payment_info: Union[PaymentInfo, dict]
-    ) -> Result:
+    def get_dossier(self, customer_id: int) -> StringResult:
         """
-        Allows to transfer a PaymentInfo object so change
-        multiple payment related values.
-        External-resources are not allowed to change account information
+        Returns the value of the dossier field.
 
 
         :param customer_id: int
-        :param payment_info: PaymentInfo
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setPaymentInformation
-        response_model = Result
+        proxy = self.__client.plunet_server.DataCustomer30.getDossier
+        response_model = StringResult
 
-        if type(payment_info) != PaymentInfo:
-            payment_info = PaymentInfo(**payment_info).dict()
-        else:
-            payment_info = payment_info.dict()
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=customer_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_account(self, account_id: int) -> AccountResult:
+        """
+        Allows the access to account details dependent on the transfered
+        accountID.
 
-        arg = {"customerID": customer_id, "paymentInfo": payment_info}
+
+        :param account_id: int
+        :return: AccountResult
+        """
+
+        proxy = self.__client.plunet_server.DataCustomer30.getAccount
+        response_model = AccountResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=account_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_account_manager_id(self, customer_id: int) -> IntegerResult:
+    def seek_by_external_id(self, external_id: str) -> IntegerResult:
         """
-        Returns the resourceID of the account-manager of the
-        the specified customer.
-
-        Returns resourceID = 0 when no account-manager is specified.
+        Method returns an instance of IntegerResult, which contains the ID of
+        the customer dataset, which was identified via the external id.
 
 
-        :param customer_id: int
+        :param external_id: str
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getAccountManagerID
+        proxy = self.__client.plunet_server.DataCustomer30.seekByExternalID
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_id,
+            argument=external_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_account_manager_id(self, customer_id: int, resource_id: int) -> Result:
+    def set_status(self, status: int, customer_id: int) -> Result:
         """
-        Sets a resource as the account manager for the specified customer.
+        Method to set the CustomerStatus. Returns an instance of Result.
 
 
+        :param status: int
         :param customer_id: int
-        :param resource_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setAccountManagerID
+        proxy = self.__client.plunet_server.DataCustomer30.setStatus
         response_model = Result
 
-        arg = {"customerID": customer_id, "resourceID": resource_id}
+        arg = {"Status": status, "customerID": customer_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_project_manager_id(self, customer_id: int, resource_id: int) -> Result:
+    def get_status(self, customer_id: int) -> IntegerResult:
         """
-        Sets a resource as the project manager for the specified customer.
+        Returns an instance of IntegerResult, which contains the status id as
+        integer.
 
 
         :param customer_id: int
-        :param resource_id: int
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setProjectManagerID
-        response_model = Result
-
-        arg = {"customerID": customer_id, "resourceID": resource_id}
+        proxy = self.__client.plunet_server.DataCustomer30.getStatus
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=customer_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_available_workflows(self, customer_id: int) -> WorkflowListResult:
+    def get_skype_id(self, customer_id: int) -> StringResult:
         """
-        Returns a list of all available workflows for the customer.
+        Returns an instance of StringResult, which contains the SkypeID of the
+        currently selected customer.
 
 
         :param customer_id: int
-        :return: WorkflowListResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getAvailableWorkflows
-        response_model = WorkflowListResult
+        proxy = self.__client.plunet_server.DataCustomer30.getSkypeID
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_payment_information(self, customer_id: int) -> PaymentInfoResult:
+    def set_academic_title(self, academic_title: str, customer_id: int) -> Result:
         """
-        Returns an PaymentInfo included within the result, which
-        contains information like IBAN, bank-code or credit account.
+        Method to set the academic title. Returns an instance of Result.
 
 
+        :param academic_title: str
         :param customer_id: int
-        :return: PaymentInfoResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getPaymentInformation
-        response_model = PaymentInfoResult
+        proxy = self.__client.plunet_server.DataCustomer30.setAcademicTitle
+        response_model = Result
+
+        arg = {"AcademicTitle": academic_title, "customerID": customer_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_available_payment_method_list(
-        self,
-    ) -> IntegerArrayResult:
+    def get_academic_title(self, customer_id: int) -> StringResult:
         """
-        Returns a list of all available payment methods.
+        Returns an instance of StringResult, which contains the academic title
+        of the currently selected customer.
 
 
-        :return: IntegerArrayResult
+        :param customer_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getAvailablePaymentMethodList
-        response_model = IntegerArrayResult
+        proxy = self.__client.plunet_server.DataCustomer30.getAcademicTitle
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=None,
+            argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_source_of_contact(self, customer_id: int, text: str) -> Result:
+    def set_opening(self, opening: str, customer_id: int) -> Result:
         """
-        Sets the value of the 'source of contact' test field.
-        Located in contacts -> customers -> marketing
+        Method to set the opening. Returns an instance of Result.
 
 
+        :param opening: str
         :param customer_id: int
-        :param text: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setSourceOfContact
+        proxy = self.__client.plunet_server.DataCustomer30.setOpening
         response_model = Result
 
-        arg = {"customerID": customer_id, "text": text}
+        arg = {"Opening": opening, "customerID": customer_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_date_of_initial_contact(self, customer_id: int) -> DateResult:
+    def set_name1(self, name: str, customer_id: int) -> Result:
         """
-        Returns the Date set as initial contact.
+        Method to set the name1 / last name. Returns an instance of Result.
 
 
+        :param name: str
         :param customer_id: int
-        :return: DateResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getDateOfInitialContact
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataCustomer30.setName1
+        response_model = Result
+
+        arg = {"Name": name, "customerID": customer_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_payment_method_description(
-        self, payment_method_id: int, system_language_code: str
-    ) -> StringResult:
+    def set_phone(self, phone_number: str, customer_id: int) -> Result:
         """
-        Returns the description of the transfered payment method in the
-        specified language.
+        Method to set phone number. Returns an instance of Result.
 
 
-        :param payment_method_id: int
-        :param system_language_code: str
-        :return: StringResult
+        :param phone_number: str
+        :param customer_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getPaymentMethodDescription
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomer30.setPhone
+        response_model = Result
 
-        arg = {
-            "paymentMethodID": payment_method_id,
-            "systemLanguageCode": system_language_code,
-        }
+        arg = {"PhoneNumber": phone_number, "customerID": customer_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_source_of_contact(self, customer_id: int) -> StringResult:
+    def set_mobile_phone(self, phone_number: str, customer_id: int) -> Result:
         """
-        Returns the value of the 'source of contact' test field.
-        Located in contacts -> customers -> marketing
+        Method to set mobile number. Returns an instance of Result.
 
 
+        :param phone_number: str
         :param customer_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getSourceOfContact
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomer30.setMobilePhone
+        response_model = Result
+
+        arg = {"PhoneNumber": phone_number, "customerID": customer_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def deregister_callback_observer(self, customer_id: int) -> Result:
+    def get_name1(self, customer_id: int) -> StringResult:
         """
-        Deletes an observer.
-        Warning: observer can only deleted by the user who has created them
+        Returns an instance of StringResult, which contains the name1 / last name
+        of the currently selected customer.
 
 
         :param customer_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.deregisterCallback_Observer
-        response_model = Result
+        proxy = self.__client.plunet_server.DataCustomer30.getName1
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def register_callback_notify(
-        self,
-        server_authentication_string: str,
-        server_address: str,
-        event_type: Union[EventType, int],
-    ) -> Result:
+    def set_external_id(self, external_id: str, customer_id: int) -> Result:
         """
-        Register to get notified when the specified event (EventType)
-        occurs for any customer
-
-        If the EventType occurs PBM will call the callback web service,
-        which is hosted within your environment. Please check
-        CallbackCustomer30 for the exact specification for this service.
-
-
-        Warning: each user can only create one notifier per event
-
-
-        The  must match one of the following formats:
-
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
-
-        In the first two cases, the address will be autocompleted by appending
-        the corresponding directory "CallbackCustomer30?wsdl".
-
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+        Method to set the external ID. Returns an instance of Result.
 
 
-        :param server_authentication_string: str
-        :param server_address: str
-        :param event_type: EventType
+        :param external_id: str
+        :param customer_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.registerCallback_Notify
+        proxy = self.__client.plunet_server.DataCustomer30.setExternalID
         response_model = Result
 
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
-        else:
-            event_type = int(event_type)
-
-        arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "EventType": event_type,
-        }
+        arg = {"ExternalID": external_id, "customerID": customer_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_date_of_initial_contact(
-        self, customer_id: int, date_initial_contact: datetime
-    ) -> Result:
+    def set_fax(self, fax: str, customer_id: int) -> Result:
         """
-        Sets the provided Date as initial contact.
+        Method to set the fax address. Returns an instance of Result.
 
 
+        :param fax: str
         :param customer_id: int
-        :param date_initial_contact: datetime
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setDateOfInitialContact
+        proxy = self.__client.plunet_server.DataCustomer30.setFax
         response_model = Result
 
-        arg = {"customerID": customer_id, "dateInitialContact": date_initial_contact}
+        arg = {"Fax": fax, "customerID": customer_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_available_account_id_list(
-        self,
-    ) -> IntegerArrayResult:
+    def insert2(self, customer_in: Union[CustomerIN, dict]) -> IntegerResult:
         """
-        Returns a list of all available accountIDÂ´s.
+        Method to create a new customer due to transfered object.
 
 
-        :return: IntegerArrayResult
+        :param customer_in: CustomerIN
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getAvailableAccountIDList
-        response_model = IntegerArrayResult
+        proxy = self.__client.plunet_server.DataCustomer30.insert2
+        response_model = IntegerResult
+
+        if type(customer_in) != CustomerIN:
+            customer_in = CustomerIN(**customer_in).dict()
+        else:
+            customer_in = customer_in.dict()
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=None,
+            argument=customer_in,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
+    def get_mobile_phone(self, customer_id: int) -> StringResult:
         """
-        Deletes an registered notify request.
-        Warning: notify requests can only be deleted by the user who has created them
+        Returns an instance of StringResult, which contains the mobile phone
+        number of the currently selected customer.
 
 
-        :param event_type: EventType
-        :return: Result
+        :param customer_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.deregisterCallback_Notify
-        response_model = Result
-
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
-        else:
-            event_type = int(event_type)
+        proxy = self.__client.plunet_server.DataCustomer30.getMobilePhone
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=event_type,
+            argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def register_callback_observer(
-        self, server_authentication_string: str, server_address: str, customer_id: int
-    ) -> Result:
+    def get_fax(self, customer_id: int) -> StringResult:
         """
-        Register to observe a specific object for any supported
-        EventType.
-
-        As soon as any supported event occurs, PBM will call the callback web
-        service, which is hosted within your environment. Please check
-        CallbackCustomer30 for the exact specification for this service.
-
-
-        (each user can only create one observer per id)
+        Returns an instance of StringResult, which contains the fax address of
+        the currently selected customer.
 
 
-        The  must match one of the following formats:
+        :param customer_id: int
+        :return: StringResult
+        """
 
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
+        proxy = self.__client.plunet_server.DataCustomer30.getFax
+        response_model = StringResult
 
-        In the first two cases, the address will be autocompleted by appending
-        the corresponding directory "CallbackCustomer30?wsdl".
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=customer_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
 
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+    def set_email(self, e_mail: str, customer_id: int) -> Result:
+        """
+        Method to set the e-mail address. Returns an instance of Result.
 
 
-        :param server_authentication_string: str
-        :param server_address: str
+        :param e_mail: str
         :param customer_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.registerCallback_Observer
+        proxy = self.__client.plunet_server.DataCustomer30.setEmail
         response_model = Result
 
-        arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "CustomerID": customer_id,
-        }
+        arg = {"EMail": e_mail, "customerID": customer_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_full_name(self, customer_id: int) -> StringResult:
+    def get_phone(self, customer_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the full name of the
-        currently selected customer.
+        Returns an instance of StringResult, which contains the phone number of
+        the currently selected customer.
 
 
         :param customer_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getFullName
+        proxy = self.__client.plunet_server.DataCustomer30.getPhone
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_status(self, customer_id: int) -> IntegerResult:
+    def set_form_of_address(self, form_of_address: int, customer_id: int) -> Result:
         """
-        Returns an instance of IntegerResult, which contains the status id as
-        integer.
+        Method to set the form of address. Returns an instance of Result.
 
 
+        :param form_of_address: int
         :param customer_id: int
-        :return: IntegerResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getStatus
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataCustomer30.setFormOfAddress
+        response_model = Result
+
+        arg = {"FormOfAddress": form_of_address, "customerID": customer_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_status(self, status: int, customer_id: int) -> Result:
+    def get_email(self, customer_id: int) -> StringResult:
         """
-        Method to set the CustomerStatus. Returns an instance of Result.
+        Returns an instance of StringResult, which contains the e-mail address
+        of the currently selected customer.
 
 
-        :param status: int
         :param customer_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setStatus
-        response_model = Result
-
-        arg = {"Status": status, "customerID": customer_id}
+        proxy = self.__client.plunet_server.DataCustomer30.getEmail
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=customer_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_all_customer_objects2(
-        self, status_list: Union[IntegerList, dict]
-    ) -> CustomerListResult:
+    def set_name2(self, name: str, customer_id: int) -> Result:
         """
-        Returns an instance of CustomerListResult, which contains a list of
-        customers, which are filtered by a list of CustomerStatus.
+        Method to set the name2 / first name. Returns an instance of Result.
 
 
-        :param status_list: IntegerList
-        :return: CustomerListResult
+        :param name: str
+        :param customer_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getAllCustomerObjects2
-        response_model = CustomerListResult
+        proxy = self.__client.plunet_server.DataCustomer30.setName2
+        response_model = Result
 
-        if type(status_list) != IntegerList:
-            status_list = IntegerList(**status_list).dict()
-        else:
-            status_list = status_list.dict()
+        arg = {"Name": name, "customerID": customer_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=status_list,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_customer_object(self, customer_id: int) -> CustomerResult:
+    def get_name2(self, customer_id: int) -> StringResult:
         """
-        Returns an instance of CustomerResult, which contains an instance of customer.
+        Returns an instance of StringResult, which contains the name2 / first
+        name of the currently selected customer.
 
 
         :param customer_id: int
-        :return: CustomerResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getCustomerObject
-        response_model = CustomerResult
+        proxy = self.__client.plunet_server.DataCustomer30.getName2
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_all_customer_objects(self, status: int) -> CustomerListResult:
+    def get_external_id(self, customer_id: int) -> StringResult:
         """
-        Returns an instance of CustomerListResult, which contains a list of
-        customers, which are filtered by the CustomerStatus.
+        Returns an instance of StringResult, which contains the external id of
+        the currently selected customer.
 
 
-        :param status: int
-        :return: CustomerListResult
+        :param customer_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getAllCustomerObjects
-        response_model = CustomerListResult
+        proxy = self.__client.plunet_server.DataCustomer30.getExternalID
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=status,
+            argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_account(self, account_id: int) -> AccountResult:
+    def get_form_of_address(self, customer_id: int) -> IntegerResult:
         """
-        Allows the access to account details dependent on the transfered
-        accountID.
+        Returns an instance of IntegerResult, which contains the id of the form of address.
 
 
-        :param account_id: int
-        :return: AccountResult
+        :param customer_id: int
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getAccount
-        response_model = AccountResult
+        proxy = self.__client.plunet_server.DataCustomer30.getFormOfAddress
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=account_id,
+            argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_dossier(self, customer_id: int, dossier: str) -> Result:
+    def set_website(self, website: str, customer_id: int) -> Result:
         """
-        Sets the dossier field.
+        Method to set the website. Returns an instance of Result.
 
 
+        :param website: str
         :param customer_id: int
-        :param dossier: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setDossier
+        proxy = self.__client.plunet_server.DataCustomer30.setWebsite
         response_model = Result
 
-        arg = {"customerID": customer_id, "dossier": dossier}
+        arg = {"Website": website, "customerID": customer_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_dossier(self, customer_id: int) -> StringResult:
+    def get_website(self, customer_id: int) -> StringResult:
         """
-        Returns the value of the dossier field.
+        Returns an instance of StringResult, which contains the website of the
+        currently selected customer.
 
 
         :param customer_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getDossier
+        proxy = self.__client.plunet_server.DataCustomer30.getWebsite
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_fax(self, customer_id: int) -> StringResult:
+    def set_skype_id(self, skype_id: str, customer_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains the fax address of
-        the currently selected customer.
+        Method to set the SkypeID. Returns an instance of Result.
 
 
+        :param skype_id: str
         :param customer_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getFax
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomer30.setSkypeID
+        response_model = Result
+
+        arg = {"SkypeID": skype_id, "customerID": customer_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_name1(self, customer_id: int) -> StringResult:
+    def get_opening(self, customer_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the name1 / last name
-        of the currently selected customer.
+        Returns an instance of StringResult, which contains the opening of the
+        currently selected customer.
 
 
         :param customer_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getName1
+        proxy = self.__client.plunet_server.DataCustomer30.getOpening
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_form_of_address(self, form_of_address: int, customer_id: int) -> Result:
+    def get_customer_object(self, customer_id: int) -> CustomerResult:
         """
-        Method to set the form of address. Returns an instance of Result.
+        Returns an instance of CustomerResult, which contains an instance of customer.
 
 
-        :param form_of_address: int
         :param customer_id: int
-        :return: Result
+        :return: CustomerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setFormOfAddress
-        response_model = Result
-
-        arg = {"FormOfAddress": form_of_address, "customerID": customer_id}
+        proxy = self.__client.plunet_server.DataCustomer30.getCustomerObject
+        response_model = CustomerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=customer_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_form_of_address(self, customer_id: int) -> IntegerResult:
+    def get_all_customer_objects(self, status: int) -> CustomerListResult:
         """
-        Returns an instance of IntegerResult, which contains the id of the form of address.
+        Returns an instance of CustomerListResult, which contains a list of
+        customers, which are filtered by the CustomerStatus.
 
 
-        :param customer_id: int
-        :return: IntegerResult
+        :param status: int
+        :return: CustomerListResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getFormOfAddress
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataCustomer30.getAllCustomerObjects
+        response_model = CustomerListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_id,
+            argument=status,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_website(self, website: str, customer_id: int) -> Result:
+    def get_all_customer_objects2(
+        self, status_list: Union[IntegerList, dict]
+    ) -> CustomerListResult:
         """
-        Method to set the website. Returns an instance of Result.
+        Returns an instance of CustomerListResult, which contains a list of
+        customers, which are filtered by a list of CustomerStatus.
 
 
-        :param website: str
-        :param customer_id: int
-        :return: Result
+        :param status_list: IntegerList
+        :return: CustomerListResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setWebsite
-        response_model = Result
+        proxy = self.__client.plunet_server.DataCustomer30.getAllCustomerObjects2
+        response_model = CustomerListResult
 
-        arg = {"Website": website, "customerID": customer_id}
+        if type(status_list) != IntegerList:
+            status_list = IntegerList(**status_list).dict()
+        else:
+            status_list = status_list.dict()
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=status_list,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_fax(self, fax: str, customer_id: int) -> Result:
+    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
         """
-        Method to set the fax address. Returns an instance of Result.
+        Deletes an registered notify request.
+        Warning: notify requests can only be deleted by the user who has created them
 
 
-        :param fax: str
-        :param customer_id: int
+        :param event_type: EventType
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setFax
+        proxy = self.__client.plunet_server.DataCustomer30.deregisterCallback_Notify
         response_model = Result
 
-        arg = {"Fax": fax, "customerID": customer_id}
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
+        else:
+            event_type = int(event_type)
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=event_type,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_skype_id(self, skype_id: str, customer_id: int) -> Result:
+    def set_date_of_initial_contact(
+        self, customer_id: int, date_initial_contact: datetime
+    ) -> Result:
         """
-        Method to set the SkypeID. Returns an instance of Result.
+        Sets the provided Date as initial contact.
 
 
-        :param skype_id: str
         :param customer_id: int
+        :param date_initial_contact: datetime
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setSkypeID
+        proxy = self.__client.plunet_server.DataCustomer30.setDateOfInitialContact
         response_model = Result
 
-        arg = {"SkypeID": skype_id, "customerID": customer_id}
+        arg = {"customerID": customer_id, "dateInitialContact": date_initial_contact}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_skype_id(self, customer_id: int) -> StringResult:
+    def get_payment_information(self, customer_id: int) -> PaymentInfoResult:
         """
-        Returns an instance of StringResult, which contains the SkypeID of the
-        currently selected customer.
+        Returns an PaymentInfo included within the result, which
+        contains information like IBAN, bank-code or credit account.
 
 
         :param customer_id: int
-        :return: StringResult
+        :return: PaymentInfoResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getSkypeID
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomer30.getPaymentInformation
+        response_model = PaymentInfoResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_academic_title(self, customer_id: int) -> StringResult:
+    def get_payment_method_description(
+        self, payment_method_id: int, system_language_code: str
+    ) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the academic title
-        of the currently selected customer.
+        Returns the description of the transfered payment method in the
+        specified language.
 
 
-        :param customer_id: int
+        :param payment_method_id: int
+        :param system_language_code: str
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getAcademicTitle
+        proxy = self.__client.plunet_server.DataCustomer30.getPaymentMethodDescription
         response_model = StringResult
 
+        arg = {
+            "paymentMethodID": payment_method_id,
+            "systemLanguageCode": system_language_code,
+        }
+
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def insert2(self, customer_in: Union[CustomerIN, dict]) -> IntegerResult:
+    def get_available_workflows(self, customer_id: int) -> WorkflowListResult:
         """
-        Method to create a new customer due to transfered object.
+        Returns a list of all available workflows for the customer.
 
 
-        :param customer_in: CustomerIN
-        :return: IntegerResult
+        :param customer_id: int
+        :return: WorkflowListResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.insert2
-        response_model = IntegerResult
-
-        if type(customer_in) != CustomerIN:
-            customer_in = CustomerIN(**customer_in).dict()
-        else:
-            customer_in = customer_in.dict()
+        proxy = self.__client.plunet_server.DataCustomer30.getAvailableWorkflows
+        response_model = WorkflowListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_in,
+            argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_phone(self, customer_id: int) -> StringResult:
+    def get_available_account_id_list(
+        self,
+    ) -> IntegerArrayResult:
         """
-        Returns an instance of StringResult, which contains the phone number of
-        the currently selected customer.
+        Returns a list of all available accountIDÂ´s.
 
 
-        :param customer_id: int
-        :return: StringResult
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getPhone
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomer30.getAvailableAccountIDList
+        response_model = IntegerArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_id,
+            argument=None,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_name1(self, name: str, customer_id: int) -> Result:
+    def register_callback_notify(
+        self,
+        server_authentication_string: str,
+        server_address: str,
+        event_type: Union[EventType, int],
+    ) -> Result:
         """
-        Method to set the name1 / last name. Returns an instance of Result.
+        Register to get notified when the specified event (EventType)
+        occurs for any customer
 
+        If the EventType occurs PBM will call the callback web service,
+        which is hosted within your environment. Please check
+        CallbackCustomer30 for the exact specification for this service.
 
-        :param name: str
-        :param customer_id: int
+
+        Warning: each user can only create one notifier per event
+
+
+        The  must match one of the following formats:
+
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
+
+        In the first two cases, the address will be autocompleted by appending
+        the corresponding directory "CallbackCustomer30?wsdl".
+
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
+
+
+        :param server_authentication_string: str
+        :param server_address: str
+        :param event_type: EventType
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setName1
+        proxy = self.__client.plunet_server.DataCustomer30.registerCallback_Notify
         response_model = Result
 
-        arg = {"Name": name, "customerID": customer_id}
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
+        else:
+            event_type = int(event_type)
+
+        arg = {
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "EventType": event_type,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_mobile_phone(self, customer_id: int) -> StringResult:
+    def get_date_of_initial_contact(self, customer_id: int) -> DateResult:
         """
-        Returns an instance of StringResult, which contains the mobile phone
-        number of the currently selected customer.
+        Returns the Date set as initial contact.
 
 
         :param customer_id: int
-        :return: StringResult
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getMobilePhone
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomer30.getDateOfInitialContact
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_website(self, customer_id: int) -> StringResult:
+    def get_available_payment_method_list(
+        self,
+    ) -> IntegerArrayResult:
         """
-        Returns an instance of StringResult, which contains the website of the
-        currently selected customer.
+        Returns a list of all available payment methods.
+
+
+        :return: IntegerArrayResult
+        """
+
+        proxy = self.__client.plunet_server.DataCustomer30.getAvailablePaymentMethodList
+        response_model = IntegerArrayResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=None,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_project_manager_id(self, customer_id: int) -> IntegerResult:
+        """
+        Returns the resourceID of the project-manager of the
+        the specified customer.
+
+        Returns resourceID = 0 when no project-manager is specified.
 
 
         :param customer_id: int
-        :return: StringResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getWebsite
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomer30.getProjectManagerID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_external_id(self, external_id: str, customer_id: int) -> Result:
+    def get_account_manager_id(self, customer_id: int) -> IntegerResult:
         """
-        Method to set the external ID. Returns an instance of Result.
+        Returns the resourceID of the account-manager of the
+        the specified customer.
+
+        Returns resourceID = 0 when no account-manager is specified.
 
 
-        :param external_id: str
         :param customer_id: int
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setExternalID
-        response_model = Result
-
-        arg = {"ExternalID": external_id, "customerID": customer_id}
+        proxy = self.__client.plunet_server.DataCustomer30.getAccountManagerID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=customer_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_name2(self, name: str, customer_id: int) -> Result:
+    def set_account_manager_id(self, customer_id: int, resource_id: int) -> Result:
         """
-        Method to set the name2 / first name. Returns an instance of Result.
+        Sets a resource as the account manager for the specified customer.
 
 
-        :param name: str
         :param customer_id: int
+        :param resource_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setName2
+        proxy = self.__client.plunet_server.DataCustomer30.setAccountManagerID
         response_model = Result
 
-        arg = {"Name": name, "customerID": customer_id}
+        arg = {"customerID": customer_id, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_email(self, e_mail: str, customer_id: int) -> Result:
+    def set_project_manager_id(self, customer_id: int, resource_id: int) -> Result:
         """
-        Method to set the e-mail address. Returns an instance of Result.
+        Sets a resource as the project manager for the specified customer.
 
 
-        :param e_mail: str
         :param customer_id: int
+        :param resource_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setEmail
+        proxy = self.__client.plunet_server.DataCustomer30.setProjectManagerID
         response_model = Result
 
-        arg = {"EMail": e_mail, "customerID": customer_id}
+        arg = {"customerID": customer_id, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_opening(self, customer_id: int) -> StringResult:
+    def get_created_by_resource_id(self, customer_id: int) -> IntegerResult:
         """
-        Returns an instance of StringResult, which contains the opening of the
-        currently selected customer.
+        Returns the ResourceID which has created the Customer.
 
 
         :param customer_id: int
-        :return: StringResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getOpening
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomer30.getCreatedByResourceID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_academic_title(self, academic_title: str, customer_id: int) -> Result:
+    def set_source_of_contact(self, customer_id: int, text: str) -> Result:
         """
-        Method to set the academic title. Returns an instance of Result.
+        Sets the value of the 'source of contact' test field.
+        Located in contacts -> customers -> marketing
 
 
-        :param academic_title: str
         :param customer_id: int
+        :param text: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setAcademicTitle
+        proxy = self.__client.plunet_server.DataCustomer30.setSourceOfContact
         response_model = Result
 
-        arg = {"AcademicTitle": academic_title, "customerID": customer_id}
+        arg = {"customerID": customer_id, "text": text}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_opening(self, opening: str, customer_id: int) -> Result:
+    def register_callback_observer(
+        self, server_authentication_string: str, server_address: str, customer_id: int
+    ) -> Result:
         """
-        Method to set the opening. Returns an instance of Result.
+        Register to observe a specific object for any supported
+        EventType.
 
+        As soon as any supported event occurs, PBM will call the callback web
+        service, which is hosted within your environment. Please check
+        CallbackCustomer30 for the exact specification for this service.
 
-        :param opening: str
-        :param customer_id: int
-        :return: Result
-        """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setOpening
-        response_model = Result
+        (each user can only create one observer per id)
 
-        arg = {"Opening": opening, "customerID": customer_id}
 
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
+        The  must match one of the following formats:
 
-    def set_phone(self, phone_number: str, customer_id: int) -> Result:
-        """
-        Method to set phone number. Returns an instance of Result.
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
 
+        In the first two cases, the address will be autocompleted by appending
+        the corresponding directory "CallbackCustomer30?wsdl".
 
-        :param phone_number: str
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
+
+
+        :param server_authentication_string: str
+        :param server_address: str
         :param customer_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setPhone
+        proxy = self.__client.plunet_server.DataCustomer30.registerCallback_Observer
         response_model = Result
 
-        arg = {"PhoneNumber": phone_number, "customerID": customer_id}
+        arg = {
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "CustomerID": customer_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_email(self, customer_id: int) -> StringResult:
-        """
-        Returns an instance of StringResult, which contains the e-mail address
-        of the currently selected customer.
-
-
-        :param customer_id: int
-        :return: StringResult
-        """
-
-        proxy = self.__client.plunet_server.DataCustomer30.getEmail
-        response_model = StringResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=customer_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def get_external_id(self, customer_id: int) -> StringResult:
+    def deregister_callback_observer(self, customer_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains the external id of
-        the currently selected customer.
+        Deletes an observer.
+        Warning: observer can only deleted by the user who has created them
 
 
         :param customer_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getExternalID
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomer30.deregisterCallback_Observer
+        response_model = Result
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_mobile_phone(self, phone_number: str, customer_id: int) -> Result:
+    def set_payment_information(
+        self, customer_id: int, payment_info: Union[PaymentInfo, dict]
+    ) -> Result:
         """
-        Method to set mobile number. Returns an instance of Result.
+        Allows to transfer a PaymentInfo object so change
+        multiple payment related values.
+        External-resources are not allowed to change account information
 
 
-        :param phone_number: str
         :param customer_id: int
+        :param payment_info: PaymentInfo
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.setMobilePhone
+        proxy = self.__client.plunet_server.DataCustomer30.setPaymentInformation
         response_model = Result
 
-        arg = {"PhoneNumber": phone_number, "customerID": customer_id}
+        if type(payment_info) != PaymentInfo:
+            payment_info = PaymentInfo(**payment_info).dict()
+        else:
+            payment_info = payment_info.dict()
+
+        arg = {"customerID": customer_id, "paymentInfo": payment_info}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_name2(self, customer_id: int) -> StringResult:
+    def get_source_of_contact(self, customer_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the name2 / first
-        name of the currently selected customer.
+        Returns the value of the 'source of contact' test field.
+        Located in contacts -> customers -> marketing
 
 
         :param customer_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomer30.getName2
+        proxy = self.__client.plunet_server.DataCustomer30.getSourceOfContact
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
-
-    def seek_by_external_id(self, external_id: str) -> IntegerResult:
-        """
-        Method returns an instance of IntegerResult, which contains the ID of
-        the customer dataset, which was identified via the external id.
-
-
-        :param external_id: str
-        :return: IntegerResult
-        """
-
-        proxy = self.__client.plunet_server.DataCustomer30.seekByExternalID
-        response_model = IntegerResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=external_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_customer_address30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_customer_address30.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 from typing import TYPE_CHECKING, List, Union
 
 from ..enums import AddressType
 from ..models import AddressIN, IntegerArrayResult, IntegerResult, Result, StringResult
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataCustomerAddress30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
     def update(
         self, address_in: Union[AddressIN, dict], enable_null_or_empty_values: bool
     ) -> Result:
         """
         updates an customer address per Object.
@@ -147,32 +146,34 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_address_type(self, address_id: int) -> IntegerResult:
+    def set_description(self, description: str, address_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains the AddressType of
-        the currently selected customer.
+        Method to set the address description. Returns an instance of Result.
 
 
+        :param description: str
         :param address_id: int
-        :return: IntegerResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.getAddressType
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataCustomerAddress30.setDescription
+        response_model = Result
+
+        arg = {"Description": description, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=address_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
     def get_description(self, address_id: int) -> StringResult:
         """
         Returns an instance of StringResult, which contains the address description.
 
 
@@ -186,146 +187,129 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=address_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_description(self, description: str, address_id: int) -> Result:
+    def get_zip(self, address_id: int) -> StringResult:
         """
-        Method to set the address description. Returns an instance of Result.
+        Returns an instance of StringResult, which contains the zip code
+        depending on the transfered AddressID.
 
 
-        :param description: str
         :param address_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.setDescription
-        response_model = Result
-
-        arg = {"Description": description, "AddressID": address_id}
+        proxy = self.__client.plunet_server.DataCustomerAddress30.getZip
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=address_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_sales_taxation_type(self, address_id: int, language: str) -> StringResult:
+    def get_city(self, address_id: int) -> StringResult:
         """
-        Returns the defined sales tax id./b>
-        This is not a standard feature and requires an active module
+        Returns an instance of StringResult, which contains the city
+        depending on the transfered AddressID.
 
 
         :param address_id: int
-        :param language: str
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.getSalesTaxationType
+        proxy = self.__client.plunet_server.DataCustomerAddress30.getCity
         response_model = StringResult
 
-        arg = {"AddressID": address_id, "language": language}
-
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=address_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_address_type(
-        self, address_type: Union[AddressType, int], address_id: int
-    ) -> Result:
+    def set_country(self, country: str, address_id: int) -> Result:
         """
-        Method to set the AddressType. Returns an instance of Result.
+        Method to set the country. Returns an instance of Result.
 
 
-        :param address_type: AddressType
+        :param country: str
         :param address_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.setAddressType
+        proxy = self.__client.plunet_server.DataCustomerAddress30.setCountry
         response_model = Result
 
-        if type(address_type) == AddressType:
-            address_type = address_type.value
-        elif type(address_type) == int:
-            address_type = address_type
-        else:
-            address_type = int(address_type)
-
-        arg = {"AddressType": address_type, "addressID": address_id}
+        arg = {"Country": country, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_taxation_type(self, address_id: int, language: str) -> StringResult:
+    def get_all_addresses(self, customer_id: int) -> IntegerArrayResult:
         """
-        Returns the defined taxation type for the specified address
-        This is not a standard feature and requires an active module
+        Returns an instance of IntegerArrayResult, which contains a list of all
+        available addressIDs for this customer.
 
 
-        :param address_id: int
-        :param language: str
-        :return: StringResult
+        :param customer_id: int
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.getTaxationType
-        response_model = StringResult
-
-        arg = {"AddressID": address_id, "language": language}
+        proxy = self.__client.plunet_server.DataCustomerAddress30.getAllAddresses
+        response_model = IntegerArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=customer_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_street2(self, street2: str, address_id: int) -> Result:
+    def set_office(self, external_id: str, address_id: int) -> Result:
         """
-        Method to set street 2. Returns an instance of Result.
+        Method to set the office name. Returns an instance of Result.
 
 
-        :param street2: str
+        :param external_id: str
         :param address_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.setStreet2
+        proxy = self.__client.plunet_server.DataCustomerAddress30.setOffice
         response_model = Result
 
-        arg = {"Street2": street2, "AddressID": address_id}
+        arg = {"ExternalID": external_id, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_street2(self, address_id: int) -> StringResult:
+    def get_street(self, address_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains street 2
+        Returns an instance of StringResult, which contains street
         depending on the transfered AddressID.
 
 
         :param address_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.getStreet2
+        proxy = self.__client.plunet_server.DataCustomerAddress30.getStreet
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=address_id,
             response_model=response_model,
             unpack_dict=False,
@@ -349,214 +333,270 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_city(self, address_id: int) -> StringResult:
+    def get_address_id(
+        self,
+    ) -> IntegerResult:
         """
-        Returns an instance of StringResult, which contains the city
+        Deprecated.
+
+
+        :return: IntegerResult
+        """
+
+        proxy = self.__client.plunet_server.DataCustomerAddress30.getAddressID
+        response_model = IntegerResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=None,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_office(self, address_id: int) -> StringResult:
+        """
+        Returns an instance of StringResult, which contains the office name
         depending on the transfered AddressID.
 
 
         :param address_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.getCity
+        proxy = self.__client.plunet_server.DataCustomerAddress30.getOffice
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=address_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_country(self, country: str, address_id: int) -> Result:
+    def set_street(self, street: str, address_id: int) -> Result:
         """
-        Method to set the country. Returns an instance of Result.
+        Method to set street. Returns an instance of Result.
 
 
-        :param country: str
+        :param street: str
         :param address_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.setCountry
+        proxy = self.__client.plunet_server.DataCustomerAddress30.setStreet
         response_model = Result
 
-        arg = {"Country": country, "AddressID": address_id}
+        arg = {"Street": street, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_all_addresses(self, customer_id: int) -> IntegerArrayResult:
+    def set_street2(self, street2: str, address_id: int) -> Result:
         """
-        Returns an instance of IntegerArrayResult, which contains a list of all
-        available addressIDs for this customer.
+        Method to set street 2. Returns an instance of Result.
 
 
-        :param customer_id: int
-        :return: IntegerArrayResult
+        :param street2: str
+        :param address_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.getAllAddresses
-        response_model = IntegerArrayResult
+        proxy = self.__client.plunet_server.DataCustomerAddress30.setStreet2
+        response_model = Result
+
+        arg = {"Street2": street2, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_address_id(
-        self,
-    ) -> IntegerResult:
+    def get_street2(self, address_id: int) -> StringResult:
         """
-        Deprecated.
+        Returns an instance of StringResult, which contains street 2
+        depending on the transfered AddressID.
 
 
-        :return: IntegerResult
+        :param address_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.getAddressID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataCustomerAddress30.getStreet2
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=None,
+            argument=address_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_office(self, external_id: str, address_id: int) -> Result:
+    def set_zip(self, zip: str, address_id: int) -> Result:
         """
-        Method to set the office name. Returns an instance of Result.
+        Method to set zip code. Returns an instance of Result.
 
 
-        :param external_id: str
+        :param zip: str
         :param address_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.setOffice
+        proxy = self.__client.plunet_server.DataCustomerAddress30.setZip
         response_model = Result
 
-        arg = {"ExternalID": external_id, "AddressID": address_id}
+        arg = {"Zip": zip, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_street(self, address_id: int) -> StringResult:
+    def get_address_type(self, address_id: int) -> IntegerResult:
         """
-        Returns an instance of StringResult, which contains street
-        depending on the transfered AddressID.
+        Returns an instance of StringResult, which contains the AddressType of
+        the currently selected customer.
 
 
         :param address_id: int
-        :return: StringResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.getStreet
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomerAddress30.getAddressType
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=address_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_street(self, street: str, address_id: int) -> Result:
+    def set_address_type(
+        self, address_type: Union[AddressType, int], address_id: int
+    ) -> Result:
         """
-        Method to set street. Returns an instance of Result.
+        Method to set the AddressType. Returns an instance of Result.
 
 
-        :param street: str
+        :param address_type: AddressType
         :param address_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.setStreet
+        proxy = self.__client.plunet_server.DataCustomerAddress30.setAddressType
         response_model = Result
 
-        arg = {"Street": street, "AddressID": address_id}
+        if type(address_type) == AddressType:
+            address_type = address_type.value
+        elif type(address_type) == int:
+            address_type = address_type
+        else:
+            address_type = int(address_type)
+
+        arg = {"AddressType": address_type, "addressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_zip(self, address_id: int) -> StringResult:
+    def get_taxation_type(self, address_id: int, language: str) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the zip code
-        depending on the transfered AddressID.
+        Returns the defined taxation type for the specified address
+        This is not a standard feature and requires an active module
 
 
         :param address_id: int
+        :param language: str
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.getZip
+        proxy = self.__client.plunet_server.DataCustomerAddress30.getTaxationType
         response_model = StringResult
 
+        arg = {"AddressID": address_id, "language": language}
+
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=address_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_office(self, address_id: int) -> StringResult:
+    def set_cost_center(self, cost_center: str, address_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains the office name
-        depending on the transfered AddressID.
+        Method to set the cost center. Returns an instance of Result.
+
+
+        :param cost_center: str
+        :param address_id: int
+        :return: Result
+        """
+
+        proxy = self.__client.plunet_server.DataCustomerAddress30.setCostCenter
+        response_model = Result
+
+        arg = {"CostCenter": cost_center, "AddressID": address_id}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def get_cost_center(self, address_id: int) -> StringResult:
+        """
+        Returns an instance of StringResult, which contains the cost center
+        of the specified customer contact.
 
 
         :param address_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.getOffice
+        proxy = self.__client.plunet_server.DataCustomerAddress30.getCostCenter
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=address_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_zip(self, zip: str, address_id: int) -> Result:
+    def set_name1(self, name: str, address_id: int) -> Result:
         """
-        Method to set zip code. Returns an instance of Result.
+        Method to set the name1 / last name. Returns an instance of Result.
 
 
-        :param zip: str
+        :param name: str
         :param address_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.setZip
+        proxy = self.__client.plunet_server.DataCustomerAddress30.setName1
         response_model = Result
 
-        arg = {"Zip": zip, "AddressID": address_id}
+        arg = {"Name": name, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
@@ -606,58 +646,14 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_name1(self, name: str, address_id: int) -> Result:
-        """
-        Method to set the name1 / last name. Returns an instance of Result.
-
-
-        :param name: str
-        :param address_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataCustomerAddress30.setName1
-        response_model = Result
-
-        arg = {"Name": name, "AddressID": address_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def set_cost_center(self, cost_center: str, address_id: int) -> Result:
-        """
-        Method to set the cost center. Returns an instance of Result.
-
-
-        :param cost_center: str
-        :param address_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataCustomerAddress30.setCostCenter
-        response_model = Result
-
-        arg = {"CostCenter": cost_center, "AddressID": address_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
     def set_name2(self, name: str, address_id: int) -> Result:
         """
         Method to set the name2 / first name. Returns an instance of Result.
 
 
         :param name: str
         :param address_id: int
@@ -692,26 +688,29 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=address_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_cost_center(self, address_id: int) -> StringResult:
+    def get_sales_taxation_type(self, address_id: int, language: str) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the cost center
-        of the specified customer contact.
+        Returns the defined sales tax id./b>
+        This is not a standard feature and requires an active module
 
 
         :param address_id: int
+        :param language: str
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerAddress30.getCostCenter
+        proxy = self.__client.plunet_server.DataCustomerAddress30.getSalesTaxationType
         response_model = StringResult
 
+        arg = {"AddressID": address_id, "language": language}
+
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=address_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_customer_contact30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_customer_contact30.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,18 @@
     IntegerResult,
     Result,
     StringResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataCustomerContact30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
     def update(
         self,
         customer_contact_in: Union[CustomerContactIN, dict],
         enable_null_or_empty_values: bool,
     ) -> Result:
@@ -77,34 +76,60 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=partner_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_contact_object(self, contact_id: int) -> CustomerContactResult:
+    def get_address_id(self, contact_id: int) -> IntegerResult:
         """
-        Returns an instance of CustomerContactResult, which contains a specific customer contact
-        object.
+        Returns an instance of IntegerResult, which contains the address id of the customer
+        contact.
+
+        Use the DataResourceAddress25 service, to manage addresses for this customer contact.
 
 
         :param contact_id: int
-        :return: CustomerContactResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getContactObject
-        response_model = CustomerContactResult
+        proxy = self.__client.plunet_server.DataCustomerContact30.getAddressID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
+    def set_address_id(self, address_id: int, contact_id: int) -> Result:
+        """
+        Method to set the default address for this customer contact.
+
+        Use the DataResourceAddress25 service, to manage addresses for this customer contact.
+
+
+        :param address_id: int
+        :param contact_id: int
+        :return: Result
+        """
+
+        proxy = self.__client.plunet_server.DataCustomerContact30.setAddressID
+        response_model = Result
+
+        arg = {"AddressID": address_id, "ContactID": contact_id}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
     def set_supervisor1(self, login_name: str, contact_id: int) -> Result:
         """
         Method to set the supervisor 1
 
 
         :param login_name: str
         :param contact_id: int
@@ -119,29 +144,30 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_supervisor1(self, contact_id: int) -> StringResult:
+    def get_all_contacts(self, customer_id: int) -> IntegerArrayResult:
         """
-        Returns an instance of StringResult, which contains the loginname of the supervisor 1.
+        Returns an instance of IntegerArrayResult, which contains a list of all available customer
+        contact ids.
 
 
-        :param contact_id: int
-        :return: StringResult
+        :param customer_id: int
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getSupervisor1
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomerContact30.getAllContacts
+        response_model = IntegerArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=contact_id,
+            argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
     def set_supervisor2(self, login_name: str, contact_id: int) -> Result:
         """
         Method to set the supervisor 2.
@@ -160,53 +186,33 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_supervisor2(self, contact_id: int) -> StringResult:
+    def get_supervisor1(self, contact_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the loginname of the supervisor 2.
+        Returns an instance of StringResult, which contains the loginname of the supervisor 1.
 
 
         :param contact_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getSupervisor2
+        proxy = self.__client.plunet_server.DataCustomerContact30.getSupervisor1
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_all_contacts(self, customer_id: int) -> IntegerArrayResult:
-        """
-        Returns an instance of IntegerArrayResult, which contains a list of all available customer
-        contact ids.
-
-
-        :param customer_id: int
-        :return: IntegerArrayResult
-        """
-
-        proxy = self.__client.plunet_server.DataCustomerContact30.getAllContacts
-        response_model = IntegerArrayResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=customer_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
     def set_customer_id(self, customer_id: int, contact_id: int) -> Result:
         """
         Method to set the CustomerID.
 
         Returns an instance of Result.
 
 
@@ -223,274 +229,283 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_address_id(self, address_id: int, contact_id: int) -> Result:
+    def get_supervisor2(self, contact_id: int) -> StringResult:
         """
-        Method to set the default address for this customer contact.
-
-        Use the DataResourceAddress25 service, to manage addresses for this customer contact.
+        Returns an instance of StringResult, which contains the loginname of the supervisor 2.
 
 
-        :param address_id: int
         :param contact_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.setAddressID
-        response_model = Result
-
-        arg = {"AddressID": address_id, "ContactID": contact_id}
+        proxy = self.__client.plunet_server.DataCustomerContact30.getSupervisor2
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=contact_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_status(self, contact_id: int) -> IntegerResult:
+    def get_contact_object(self, contact_id: int) -> CustomerContactResult:
         """
-        Returns an instance of IntegerResult, which contains the ContactPersonStatus as
-        integer.
+        Returns an instance of CustomerContactResult, which contains a specific customer contact
+        object.
 
 
         :param contact_id: int
-        :return: IntegerResult
+        :return: CustomerContactResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getStatus
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataCustomerContact30.getContactObject
+        response_model = CustomerContactResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_status(self, status: int, contact_id: int) -> Result:
+    def seek_by_external_id(self, external_id: str) -> IntegerArrayResult:
         """
-        Method to set the status of the customer contact.
+        Returns an instance of IntegerArrayResult, which contains a list of customer contactIDs.
+
+
+        :param external_id: str
+        :return: IntegerArrayResult
+        """
+
+        proxy = self.__client.plunet_server.DataCustomerContact30.seekByExternalID
+        response_model = IntegerArrayResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=external_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def set_cost_center(self, cost_center: str, contact_id: int) -> Result:
+        """
+        Method to set the cost center.
 
         Returns an instance of Result.
 
 
-        :param status: int
+        :param cost_center: str
         :param contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.setStatus
+        proxy = self.__client.plunet_server.DataCustomerContact30.setCostCenter
         response_model = Result
 
-        arg = {"Status": status, "ContactID": contact_id}
+        arg = {"CostCenter": cost_center, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_all_contact_objects(self, customer_id: int) -> CustomerContactListResult:
+    def get_cost_center(self, contact_id: int) -> StringResult:
         """
-        Returns an instance of CustomerContactListResult, which contains a list of all available
-        customer contact objects.
+        Returns an instance of StringResult, which contains the cost center of the currently selected
+        customer contact.
 
 
-        :param customer_id: int
-        :return: CustomerContactListResult
+        :param contact_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getAllContactObjects
-        response_model = CustomerContactListResult
+        proxy = self.__client.plunet_server.DataCustomerContact30.getCostCenter
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_id,
+            argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_address_id(self, contact_id: int) -> IntegerResult:
+    def get_user_id(self, contact_id: int) -> IntegerResult:
         """
-        Returns an instance of IntegerResult, which contains the address id of the customer
+        Returns an instance of IntegerResult, which contains the user id of the selected customer
         contact.
 
-        Use the DataResourceAddress25 service, to manage addresses for this customer contact.
-
 
         :param contact_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getAddressID
+        proxy = self.__client.plunet_server.DataCustomerContact30.getUserId
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_fax(self, contact_id: int) -> StringResult:
+    def set_status(self, status: int, contact_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains the fax address of the currently selected
-        customer contact.
+        Method to set the status of the customer contact.
+
+        Returns an instance of Result.
 
 
+        :param status: int
         :param contact_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getFax
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomerContact30.setStatus
+        response_model = Result
+
+        arg = {"Status": status, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=contact_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_name1(self, contact_id: int) -> StringResult:
+    def get_customer_id(self, contact_id: int) -> IntegerResult:
         """
-        Returns an instance of StringResult, which contains the name1 / last name of the currently
-        selected customer contact.
+        Returns an instance of IntegerResult, which contains CustomerID of the currently selected
+        customer contact.
 
 
         :param contact_id: int
-        :return: StringResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getName1
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomerContact30.getCustomerID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_fax(self, fax: str, contact_id: int) -> Result:
+    def get_status(self, contact_id: int) -> IntegerResult:
         """
-        Method to set the fax address.
-
-        Returns an instance of Result.
+        Returns an instance of IntegerResult, which contains the ContactPersonStatus as
+        integer.
 
 
-        :param fax: str
         :param contact_id: int
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.setFax
-        response_model = Result
-
-        arg = {"Fax": fax, "ContactID": contact_id}
+        proxy = self.__client.plunet_server.DataCustomerContact30.getStatus
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=contact_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def insert2(
-        self, customer_contact_in: Union[CustomerContactIN, dict]
-    ) -> IntegerResult:
+    def set_name1(self, name: str, contact_id: int) -> Result:
         """
-        Method to create a new, empty customer contact dataset by Object.
+        Method to set the name1 / last name.
 
-        The method will return an instance of IntegerResult, which contains the identifier of the new
-        generated customer contact. Further api calls via this port will maninpulate this customer
-        contact (except methods with an customer contact id as parameter ), until another customer
-        contact is fetched or the session is invalidated.
+        Returns an instance of Result.
 
 
-        :param customer_contact_in: CustomerContactIN
-        :return: IntegerResult
+        :param name: str
+        :param contact_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.insert2
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataCustomerContact30.setName1
+        response_model = Result
 
-        if type(customer_contact_in) != CustomerContactIN:
-            customer_contact_in = CustomerContactIN(**customer_contact_in).dict()
-        else:
-            customer_contact_in = customer_contact_in.dict()
+        arg = {"Name": name, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=customer_contact_in,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_phone(self, contact_id: int) -> StringResult:
+    def set_phone(self, phone_number: str, contact_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains the phone number of the currently selected
-        customer contact.
+        Method to set phone number.
+
+        Returns an instance of Result.
 
 
+        :param phone_number: str
         :param contact_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getPhone
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataCustomerContact30.setPhone
+        response_model = Result
+
+        arg = {"PhoneNumber": phone_number, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=contact_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_name1(self, name: str, contact_id: int) -> Result:
+    def set_mobile_phone(self, phone_number: str, contact_id: int) -> Result:
         """
-        Method to set the name1 / last name.
+        Method to set mobile number.
 
         Returns an instance of Result.
 
 
-        :param name: str
+        :param phone_number: str
         :param contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.setName1
+        proxy = self.__client.plunet_server.DataCustomerContact30.setMobilePhone
         response_model = Result
 
-        arg = {"Name": name, "ContactID": contact_id}
+        arg = {"PhoneNumber": phone_number, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_mobile_phone(self, contact_id: int) -> StringResult:
+    def get_name1(self, contact_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the mobile phone number of the currently
+        Returns an instance of StringResult, which contains the name1 / last name of the currently
         selected customer contact.
 
 
         :param contact_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getMobilePhone
+        proxy = self.__client.plunet_server.DataCustomerContact30.getName1
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
@@ -516,186 +531,189 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_cost_center(self, cost_center: str, contact_id: int) -> Result:
+    def set_fax(self, fax: str, contact_id: int) -> Result:
         """
-        Method to set the cost center.
+        Method to set the fax address.
 
         Returns an instance of Result.
 
 
-        :param cost_center: str
+        :param fax: str
         :param contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.setCostCenter
+        proxy = self.__client.plunet_server.DataCustomerContact30.setFax
         response_model = Result
 
-        arg = {"CostCenter": cost_center, "ContactID": contact_id}
+        arg = {"Fax": fax, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_user_id(self, contact_id: int) -> IntegerResult:
+    def insert2(
+        self, customer_contact_in: Union[CustomerContactIN, dict]
+    ) -> IntegerResult:
         """
-        Returns an instance of IntegerResult, which contains the user id of the selected customer
-        contact.
+        Method to create a new, empty customer contact dataset by Object.
 
+        The method will return an instance of IntegerResult, which contains the identifier of the new
+        generated customer contact. Further api calls via this port will maninpulate this customer
+        contact (except methods with an customer contact id as parameter ), until another customer
+        contact is fetched or the session is invalidated.
 
-        :param contact_id: int
+
+        :param customer_contact_in: CustomerContactIN
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getUserId
+        proxy = self.__client.plunet_server.DataCustomerContact30.insert2
         response_model = IntegerResult
 
+        if type(customer_contact_in) != CustomerContactIN:
+            customer_contact_in = CustomerContactIN(**customer_contact_in).dict()
+        else:
+            customer_contact_in = customer_contact_in.dict()
+
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=contact_id,
+            argument=customer_contact_in,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_name2(self, name: str, contact_id: int) -> Result:
+    def get_mobile_phone(self, contact_id: int) -> StringResult:
         """
-        Method to set the name2 / first name.
-
-        Returns an instance of Result.
+        Returns an instance of StringResult, which contains the mobile phone number of the currently
+        selected customer contact.
 
 
-        :param name: str
         :param contact_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.setName2
-        response_model = Result
-
-        arg = {"Name": name, "ContactID": contact_id}
+        proxy = self.__client.plunet_server.DataCustomerContact30.getMobilePhone
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=contact_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_email(self, e_mail: str, contact_id: int) -> Result:
+    def get_fax(self, contact_id: int) -> StringResult:
         """
-        Method to set the e-mail address.
-
-        Returns an instance of Result.
+        Returns an instance of StringResult, which contains the fax address of the currently selected
+        customer contact.
 
 
-        :param e_mail: str
         :param contact_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.setEmail
-        response_model = Result
-
-        arg = {"EMail": e_mail, "ContactID": contact_id}
+        proxy = self.__client.plunet_server.DataCustomerContact30.getFax
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=contact_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_phone(self, phone_number: str, contact_id: int) -> Result:
+    def set_email(self, e_mail: str, contact_id: int) -> Result:
         """
-        Method to set phone number.
+        Method to set the e-mail address.
 
         Returns an instance of Result.
 
 
-        :param phone_number: str
+        :param e_mail: str
         :param contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.setPhone
+        proxy = self.__client.plunet_server.DataCustomerContact30.setEmail
         response_model = Result
 
-        arg = {"PhoneNumber": phone_number, "ContactID": contact_id}
+        arg = {"EMail": e_mail, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_email(self, contact_id: int) -> StringResult:
+    def get_phone(self, contact_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the e-mail address of the currently
-        selected customer contact.
+        Returns an instance of StringResult, which contains the phone number of the currently selected
+        customer contact.
 
 
         :param contact_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getEmail
+        proxy = self.__client.plunet_server.DataCustomerContact30.getPhone
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_external_id(self, contact_id: int) -> StringResult:
+    def get_email(self, contact_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the external id of the currently selected
-        customer contact.
+        Returns an instance of StringResult, which contains the e-mail address of the currently
+        selected customer contact.
 
 
         :param contact_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getExternalID
+        proxy = self.__client.plunet_server.DataCustomerContact30.getEmail
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_mobile_phone(self, phone_number: str, contact_id: int) -> Result:
+    def set_name2(self, name: str, contact_id: int) -> Result:
         """
-        Method to set mobile number.
+        Method to set the name2 / first name.
 
         Returns an instance of Result.
 
 
-        :param phone_number: str
+        :param name: str
         :param contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.setMobilePhone
+        proxy = self.__client.plunet_server.DataCustomerContact30.setName2
         response_model = Result
 
-        arg = {"PhoneNumber": phone_number, "ContactID": contact_id}
+        arg = {"Name": name, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
@@ -716,65 +734,46 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def seek_by_external_id(self, external_id: str) -> IntegerArrayResult:
-        """
-        Returns an instance of IntegerArrayResult, which contains a list of customer contactIDs.
-
-
-        :param external_id: str
-        :return: IntegerArrayResult
-        """
-
-        proxy = self.__client.plunet_server.DataCustomerContact30.seekByExternalID
-        response_model = IntegerArrayResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=external_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def get_cost_center(self, contact_id: int) -> StringResult:
+    def get_external_id(self, contact_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the cost center of the currently selected
+        Returns an instance of StringResult, which contains the external id of the currently selected
         customer contact.
 
 
         :param contact_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getCostCenter
+        proxy = self.__client.plunet_server.DataCustomerContact30.getExternalID
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_customer_id(self, contact_id: int) -> IntegerResult:
+    def get_all_contact_objects(self, customer_id: int) -> CustomerContactListResult:
         """
-        Returns an instance of IntegerResult, which contains CustomerID of the currently selected
-        customer contact.
+        Returns an instance of CustomerContactListResult, which contains a list of all available
+        customer contact objects.
 
 
-        :param contact_id: int
-        :return: IntegerResult
+        :param customer_id: int
+        :return: CustomerContactListResult
         """
 
-        proxy = self.__client.plunet_server.DataCustomerContact30.getCustomerID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataCustomerContact30.getAllContactObjects
+        response_model = CustomerContactListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=contact_id,
+            argument=customer_id,
             response_model=response_model,
             unpack_dict=False,
         )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_document30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_document30.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,51 +4,55 @@
 from typing import TYPE_CHECKING, List, Union
 
 from ..enums import FolderTypes
 from ..models import FileResult, Result, StringArrayResult
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataDocument30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
-    def download_document(
-        self, main_id: int, folder_type: Union[FolderTypes, int], file_path_name: str
-    ) -> FileResult:
+    def get_file_list(
+        self, main_id: int, folder_type: Union[FolderTypes, int]
+    ) -> StringArrayResult:
         """
-        Returns a FileResult containing the specified file as byte-stream.
+        Returns a StringArrayResult containing all files with all sub folders after the,
+        on the main and folder-type depending directory.
 
-        The FilePathName can be obtained over getFileList(String, int, int)
+        Example: MainID = 500 (OrderID) and FolderTypes.ORDER_REFERENCE
+
+
+        Returns:
+
+
+        de-de/examplefile_1.txt
+        de-de/examplefile_2.txt
+        testfiles5.csv
+        en/testfiles6.pdf
 
 
         :param main_id: int
         :param folder_type: FolderTypes
-        :param file_path_name: str
-        :return: FileResult
+        :return: StringArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataDocument30.download_Document
-        response_model = FileResult
+        proxy = self.__client.plunet_server.DataDocument30.getFileList
+        response_model = StringArrayResult
 
         if type(folder_type) == FolderTypes:
             folder_type = folder_type.value
         elif type(folder_type) == int:
             folder_type = folder_type
         else:
             folder_type = int(folder_type)
 
-        arg = {
-            "MainID": main_id,
-            "FolderType": folder_type,
-            "FilePathName": file_path_name,
-        }
+        arg = {"MainID": main_id, "FolderType": folder_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
@@ -111,49 +115,44 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_file_list(
-        self, main_id: int, folder_type: Union[FolderTypes, int]
-    ) -> StringArrayResult:
+    def download_document(
+        self, main_id: int, folder_type: Union[FolderTypes, int], file_path_name: str
+    ) -> FileResult:
         """
-        Returns a StringArrayResult containing all files with all sub folders after the,
-        on the main and folder-type depending directory.
-
-        Example: MainID = 500 (OrderID) and FolderTypes.ORDER_REFERENCE
-
-
-        Returns:
-
+        Returns a FileResult containing the specified file as byte-stream.
 
-        de-de/examplefile_1.txt
-        de-de/examplefile_2.txt
-        testfiles5.csv
-        en/testfiles6.pdf
+        The FilePathName can be obtained over getFileList(String, int, int)
 
 
         :param main_id: int
         :param folder_type: FolderTypes
-        :return: StringArrayResult
+        :param file_path_name: str
+        :return: FileResult
         """
 
-        proxy = self.__client.plunet_server.DataDocument30.getFileList
-        response_model = StringArrayResult
+        proxy = self.__client.plunet_server.DataDocument30.download_Document
+        response_model = FileResult
 
         if type(folder_type) == FolderTypes:
             folder_type = folder_type.value
         elif type(folder_type) == int:
             folder_type = folder_type
         else:
             folder_type = int(folder_type)
 
-        arg = {"MainID": main_id, "FolderType": folder_type}
+        arg = {
+            "MainID": main_id,
+            "FolderType": folder_type,
+            "FilePathName": file_path_name,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_item30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_item30.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,163 +23,127 @@
     Result,
     StringArrayResult,
     StringResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataItem30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
-    def get_items_by_status2(
-        self, project_id: int, project_type: Union[ProjectType, int], status: int
-    ) -> ItemListResult:
+    def update(
+        self, item_in: Union[ItemIN, dict], enable_null_or_empty_values: bool
+    ) -> Result:
         """
-        Method returns an instance of ItemListResult, which contains a list of item objects for a
-        certain project.
-
-        Items are filtered by the item status.
+        Updates the item by the transfered item object Use EnableNullOrEmptyValues to decide if Null
+        or empty strings are saved into Plunet or ignored.
 
 
-        :param project_id: int
-        :param project_type: ProjectType
-        :param status: int
-        :return: ItemListResult
+        :param item_in: ItemIN
+        :param enable_null_or_empty_values: bool
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getItemsByStatus2
-        response_model = ItemListResult
+        proxy = self.__client.plunet_server.DataItem30.update
+        response_model = Result
 
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
+        if type(item_in) != ItemIN:
+            item_in = ItemIN(**item_in).dict()
         else:
-            project_type = int(project_type)
+            item_in = item_in.dict()
 
-        arg = {"projectID": project_id, "projectType": project_type, "status": status}
+        arg = {
+            "ItemIN": item_in,
+            "enableNullOrEmptyValues": enable_null_or_empty_values,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def add_language_combination(
-        self,
-        source_language: str,
-        target_language: str,
-        project_type: Union[ProjectType, int],
-        project_id: int,
-        item_id: int,
-    ) -> IntegerResult:
+    def delete(self, item_id: int, project_type: Union[ProjectType, int]) -> Result:
         """
-        Deprecated. Please use {link addLanguageCombination2(String, String, String, int, int)
-        instead the itemID is not required for this method.
+        Deletes the specified item.
 
 
-        :param source_language: str
-        :param target_language: str
-        :param project_type: ProjectType
-        :param project_id: int
         :param item_id: int
-        :return: IntegerResult
+        :param project_type: ProjectType
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.addLanguageCombination
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataItem30.delete
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "sourceLanguage": source_language,
-            "targetLanguage": target_language,
-            "projectType": project_type,
-            "projectID": project_id,
-            "itemID": item_id,
-        }
+        arg = {"itemID": item_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_items_by_status3(
-        self,
-        project_type: Union[ProjectType, int],
-        status: int,
-        document_status: Union[DocumentStatus, int],
-    ) -> ItemListResult:
+    def insert(
+        self, project_id: int, project_type: Union[ProjectType, int]
+    ) -> IntegerResult:
         """
-        Method returns an instance of ItemListResult, which contains a list of item objects.
-
-        Items are filtered by the item status and the document status.
+        Inserts a new item into the the specified project
 
 
+        :param project_id: int
         :param project_type: ProjectType
-        :param status: int
-        :param document_status: DocumentStatus
-        :return: ItemListResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getItemsByStatus3
-        response_model = ItemListResult
+        proxy = self.__client.plunet_server.DataItem30.insert
+        response_model = IntegerResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        if type(document_status) == DocumentStatus:
-            document_status = document_status.value
-        elif type(document_status) == int:
-            document_status = document_status
-        else:
-            document_status = int(document_status)
-
-        arg = {
-            "projectType": project_type,
-            "status": status,
-            "documentStatus": document_status,
-        }
+        arg = {"projectID": project_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_source_language(
+    def get_comment(
         self, project_type: Union[ProjectType, int], item_id: int
     ) -> StringResult:
         """
-        Method returns an instance of StringResult, the source language depending on the itemID
+        Method returns an instance of StringResult, which contains the comment depending on the
+        itemID.
 
 
         :param project_type: ProjectType
         :param item_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getSourceLanguage
+        proxy = self.__client.plunet_server.DataItem30.getComment
         response_model = StringResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
@@ -190,387 +154,353 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def seek_language_combination(
-        self,
-        source_language: str,
-        target_language: str,
-        project_type: Union[ProjectType, int],
-        project_id: int,
-        item_id: int,
-    ) -> IntegerResult:
+    def set_comment(
+        self, comment: str, project_type: Union[ProjectType, int], item_id: int
+    ) -> Result:
         """
-        Method returns an instance of IntegerResult, which contains the ID of a specific language
-        combination for the specified project.
+        Method sets the comment depending on the itemID.
 
 
-        :param source_language: str
-        :param target_language: str
+        :param comment: str
         :param project_type: ProjectType
-        :param project_id: int
         :param item_id: int
-        :return: IntegerResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.seekLanguageCombination
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataItem30.setComment
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "sourceLanguage": source_language,
-            "targetLanguage": target_language,
-            "projectType": project_type,
-            "projectID": project_id,
-            "itemID": item_id,
-        }
+        arg = {"comment": comment, "projectType": project_type, "itemID": item_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_jobs_with_status(
-        self, status: int, project_type: Union[ProjectType, int], item_id: int
-    ) -> IntegerArrayResult:
-        """
-        Method returns an instance of IntegerArrayResult, which contains a list of IDs of job, which
-        were linked to the currently selected item and have a specific status.
-
-
-        :param status: int
-        :param project_type: ProjectType
-        :param item_id: int
-        :return: IntegerArrayResult
+    def set_cat_report(
+        self,
+        path_or_url: str,
+        overwrite_existing_price_lines: bool,
+        cat_type: Union[CatType, int],
+        project_type: Union[ProjectType, int],
+        copy_results_to_item: bool,
+        item_id: int,
+    ) -> Result:
         """
+        Deprecated. Please use
+        setCatReport2(String, byte[], String, int, boolean, int, int, boolean, int)
+        instead. Please note that this call is now deactivated by default. For Reactivation
+        please contact Support@plunet.com.
 
-        proxy = self.__client.plunet_server.DataItem30.getJobsWithStatus
-        response_model = IntegerArrayResult
-
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
-        else:
-            project_type = int(project_type)
-
-        arg = {"Status": status, "projectType": project_type, "itemID": item_id}
 
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
+        Uploads a report file into the report folder of the specified item.
 
-    def get_all_item_objects(
-        self, project_id: int, project_type: Union[ProjectType, int]
-    ) -> ItemListResult:
-        """
-        Method returns an instance of ItemListResult, which contains a list of item objects.
+        Also allows to copy the results of the report into the item (optionally overwriting
+        existing price lines)
 
 
-        :param project_id: int
+        :param path_or_url: str
+        :param overwrite_existing_price_lines: bool
+        :param cat_type: CatType
         :param project_type: ProjectType
-        :return: ItemListResult
+        :param copy_results_to_item: bool
+        :param item_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getAllItemObjects
-        response_model = ItemListResult
+        proxy = self.__client.plunet_server.DataItem30.setCatReport
+        response_model = Result
+
+        if type(cat_type) == CatType:
+            cat_type = cat_type.value
+        elif type(cat_type) == int:
+            cat_type = cat_type
+        else:
+            cat_type = int(cat_type)
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectID": project_id, "projectType": project_type}
+        arg = {
+            "pathOrUrl": path_or_url,
+            "overwriteExistingPriceLines": overwrite_existing_price_lines,
+            "catType": cat_type,
+            "projectType": project_type,
+            "copyResultsToItem": copy_results_to_item,
+            "itemID": item_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_target_language(
-        self, project_type: Union[ProjectType, int], item_id: int
-    ) -> StringResult:
+    def get_all_items(
+        self, project_type: Union[ProjectType, int], project_id: int
+    ) -> IntegerArrayResult:
         """
-        Method returns an instance of StringResult, which contains the target language depending on
-        the itemID
+        Method returns an instance of IntegerArrayResult, which contains a list of all item
+        ids for the specified project.
 
 
         :param project_type: ProjectType
-        :param item_id: int
-        :return: StringResult
+        :param project_id: int
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getTargetLanguage
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataItem30.getAllItems
+        response_model = IntegerArrayResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "itemID": item_id}
+        arg = {"projectType": project_type, "projectID": project_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_language_combination_id(
+    def set_cat_report2(
         self,
-        language_combination_id: int,
+        file_byte_stream: bytes,
+        file_path_name: str,
+        filesize: int,
+        overwrite_existing_price_lines: bool,
+        cat_type: Union[CatType, int],
         project_type: Union[ProjectType, int],
+        copy_results_to_item: bool,
         item_id: int,
     ) -> Result:
         """
-        Method sets the language combination ID for the specified item.
+        Uploads a report file into the report folder of the specified item.
+
+        Also allows to copy the results of the report into the item (optionally overwriting existing
+        price lines)
 
 
-        :param language_combination_id: int
+        :param file_byte_stream: bytes
+        :param file_path_name: str
+        :param filesize: int
+        :param overwrite_existing_price_lines: bool
+        :param cat_type: CatType
         :param project_type: ProjectType
+        :param copy_results_to_item: bool
         :param item_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.setLanguageCombinationID
+        proxy = self.__client.plunet_server.DataItem30.setCatReport2
         response_model = Result
 
+        if type(cat_type) == CatType:
+            cat_type = cat_type.value
+        elif type(cat_type) == int:
+            cat_type = cat_type
+        else:
+            cat_type = int(cat_type)
+
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
         arg = {
-            "languageCombinationID": language_combination_id,
+            "FileByteStream": file_byte_stream,
+            "FilePathName": file_path_name,
+            "Filesize": filesize,
+            "overwriteExistingPriceLines": overwrite_existing_price_lines,
+            "catType": cat_type,
             "projectType": project_type,
+            "copyResultsToItem": copy_results_to_item,
             "itemID": item_id,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_items_by_status1(
-        self, project_type: Union[ProjectType, int], status: int
-    ) -> ItemListResult:
+    def set_total_price(
+        self, project_type: Union[ProjectType, int], total_price: float, item_id: int
+    ) -> Result:
         """
-        Method returns an instance of ItemListResult, which contains a list of item objects. Items are
-        filtered by the item status.
+        Method sets total price for an item (project currency).
 
 
         :param project_type: ProjectType
-        :param status: int
-        :return: ItemListResult
+        :param total_price: float
+        :param item_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getItemsByStatus1
-        response_model = ItemListResult
+        proxy = self.__client.plunet_server.DataItem30.setTotalPrice
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "status": status}
+        arg = {
+            "projectType": project_type,
+            "totalPrice": total_price,
+            "itemID": item_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_items_by_status4(
-        self,
-        project_id: int,
-        project_type: Union[ProjectType, int],
-        status: int,
-        document_status: Union[DocumentStatus, int],
-    ) -> ItemListResult:
+    def get_item_object(
+        self, project_type: Union[ProjectType, int], item_id: int
+    ) -> ItemResult:
         """
-        Method returns an instance of ItemListResult, which contains a list of item objects for a
-        certain project.
-
-        Items are filtered by the item status and the document status.
+        Method returns an instance of ItemResult.
 
 
-        :param project_id: int
         :param project_type: ProjectType
-        :param status: int
-        :param document_status: DocumentStatus
-        :return: ItemListResult
+        :param item_id: int
+        :return: ItemResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getItemsByStatus4
-        response_model = ItemListResult
+        proxy = self.__client.plunet_server.DataItem30.getItemObject
+        response_model = ItemResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        if type(document_status) == DocumentStatus:
-            document_status = document_status.value
-        elif type(document_status) == int:
-            document_status = document_status
-        else:
-            document_status = int(document_status)
-
-        arg = {
-            "projectID": project_id,
-            "projectType": project_type,
-            "status": status,
-            "documentStatus": document_status,
-        }
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def update(
-        self, item_in: Union[ItemIN, dict], enable_null_or_empty_values: bool
-    ) -> Result:
-        """
-        Updates the item by the transfered item object Use EnableNullOrEmptyValues to decide if Null
-        or empty strings are saved into Plunet or ignored.
-
-
-        :param item_in: ItemIN
-        :param enable_null_or_empty_values: bool
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataItem30.update
-        response_model = Result
-
-        if type(item_in) != ItemIN:
-            item_in = ItemIN(**item_in).dict()
-        else:
-            item_in = item_in.dict()
-
-        arg = {
-            "ItemIN": item_in,
-            "enableNullOrEmptyValues": enable_null_or_empty_values,
-        }
+        arg = {"projectType": project_type, "itemID": item_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def delete(self, item_id: int, project_type: Union[ProjectType, int]) -> Result:
+    def get_total_price(
+        self, project_type: Union[ProjectType, int], item_id: int
+    ) -> DoubleResult:
         """
-        Deletes the specified item.
+        Method returns total price for an item (project currency).
 
 
-        :param item_id: int
         :param project_type: ProjectType
-        :return: Result
+        :param item_id: int
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.delete
-        response_model = Result
+        proxy = self.__client.plunet_server.DataItem30.getTotalPrice
+        response_model = DoubleResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"itemID": item_id, "projectType": project_type}
+        arg = {"projectType": project_type, "itemID": item_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def insert(
-        self, project_id: int, project_type: Union[ProjectType, int]
+    def get_invoice_id(
+        self, project_type: Union[ProjectType, int], item_id: int
     ) -> IntegerResult:
         """
-        Inserts a new item into the the specified project
+        Method returns an instance of IntegerResult, which contains the ID of the invoice for the
+        currently selected item.
+
+        This method is only available for an order items.
 
 
-        :param project_id: int
         :param project_type: ProjectType
+        :param item_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.insert
+        proxy = self.__client.plunet_server.DataItem30.getInvoiceID
         response_model = IntegerResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectID": project_id, "projectType": project_type}
+        arg = {"projectType": project_type, "itemID": item_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_comment(
+    def get_jobs(
         self, project_type: Union[ProjectType, int], item_id: int
-    ) -> StringResult:
+    ) -> IntegerArrayResult:
         """
-        Method returns an instance of StringResult, which contains the comment depending on the
+        Method returns an instance of IntegerArrayResult, which contains all job IDs depending on the
         itemID.
 
 
         :param project_type: ProjectType
         :param item_id: int
-        :return: StringResult
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getComment
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataItem30.getJobs
+        response_model = IntegerArrayResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
@@ -580,675 +510,599 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_comment(
-        self, comment: str, project_type: Union[ProjectType, int], item_id: int
-    ) -> Result:
+    def set_delivery_date(self, delivery_date: datetime, item_id: int) -> Result:
         """
-        Method sets the comment depending on the itemID.
+        Method sets the delivery date for the specified item (order items only!).
 
 
-        :param comment: str
-        :param project_type: ProjectType
+        :param delivery_date: datetime
         :param item_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.setComment
+        proxy = self.__client.plunet_server.DataItem30.setDeliveryDate
         response_model = Result
 
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
-        else:
-            project_type = int(project_type)
-
-        arg = {"comment": comment, "projectType": project_type, "itemID": item_id}
+        arg = {"deliveryDate": delivery_date, "itemID": item_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def deregister_callback_observer(
-        self, item_id: int, project_type: Union[ProjectType, int]
-    ) -> Result:
+    def get_delivery_date(self, item_id: int) -> DateResult:
         """
-        Deletes an observer.
-
-        Observer can only deleted by the user who has created them.
+        Method returns an instance of DateResult, which contains the delivery date of the item
+        (order items only!).
 
 
         :param item_id: int
-        :param project_type: ProjectType
-        :return: Result
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.deregisterCallback_Observer
-        response_model = Result
-
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
-        else:
-            project_type = int(project_type)
-
-        arg = {"ItemID": item_id, "ProjectType": project_type}
+        proxy = self.__client.plunet_server.DataItem30.getDeliveryDate
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=item_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def register_callback_notify(
+    def update_price_line(
         self,
-        server_authentication_string: str,
-        server_address: str,
-        event_type: Union[EventType, int],
-    ) -> Result:
+        item_id: int,
+        project_type: Union[ProjectType, int],
+        price_line_in: Union[PriceLineIN, dict],
+    ) -> PriceLineResult:
         """
-        Register to get notified when the specified EventType occurs for any item.
-
-        If the EventType occurs PBM will call the callback web service, which is hosted within
-        your environment. The notifier will only be notified if the event is triggered by a different
-        user.
-
-
-        Please check CallbackItem30 for the exact specification for this service.
-
-
-        Info:Each user can only create one notifier per event
-
-
-        The  must match one of the following formats:
-
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
-
-
-        In the first two cases, the address will be autocompleted by appending the corresponding
-        directory "CallbackItem30?wsdl".
-
-
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+        Updates a existing PriceLine.
 
 
-        :param server_authentication_string: str
-        :param server_address: str
-        :param event_type: EventType
-        :return: Result
+        :param item_id: int
+        :param project_type: ProjectType
+        :param price_line_in: PriceLineIN
+        :return: PriceLineResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.registerCallback_Notify
-        response_model = Result
+        proxy = self.__client.plunet_server.DataItem30.updatePriceLine
+        response_model = PriceLineResult
 
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
+        if type(price_line_in) != PriceLineIN:
+            price_line_in = PriceLineIN(**price_line_in).dict()
         else:
-            event_type = int(event_type)
+            price_line_in = price_line_in.dict()
+
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
+        else:
+            project_type = int(project_type)
 
         arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "EventType": event_type,
+            "itemID": item_id,
+            "projectType": project_type,
+            "priceLineIN": price_line_in,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
+    def get_services_list(self, language_code: str) -> StringArrayResult:
         """
-        Deletes an registered notify request.
-
-        Info:Notify requests can only be deleted by the user who has created them
+        Deprecated. Please use DataAdmin30.getAvailableServices(String, String) instead.
+        Returns a list of all available services.
 
 
-        :param event_type: EventType
-        :return: Result
+        :param language_code: str
+        :return: StringArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.deregisterCallback_Notify
-        response_model = Result
-
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
-        else:
-            event_type = int(event_type)
+        proxy = self.__client.plunet_server.DataItem30.getServices_List
+        response_model = StringArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=event_type,
+            argument=language_code,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def register_callback_observer(
-        self,
-        server_authentication_string: str,
-        server_address: str,
-        item_id: int,
-        project_type: Union[ProjectType, int],
-    ) -> Result:
+    def get_item_reference(
+        self, project_type: Union[ProjectType, int], item_id: int
+    ) -> StringResult:
         """
-        Register to observe a specific object for any supported EventType.
-
-        As soon as any supported EventType occurs, PBM will call the callback web service, which
-        is hosted within your environment. The observer will only be notified if the event is triggered
-        by a different user.
-
-
-        Please check CallbackItem30 for the exact specification for this service.
-
-
-        Info:Each user can only create one observer per id
+        Method returns item reference StringResult.
 
 
-        The  must match one of the following formats:
+        :param project_type: ProjectType
+        :param item_id: int
+        :return: StringResult
+        """
 
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
+        proxy = self.__client.plunet_server.DataItem30.getItemReference
+        response_model = StringResult
 
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
+        else:
+            project_type = int(project_type)
 
-        In the first two cases, the address will be autocompleted by appending the corresponding
-        directory "CallbackItem30?wsdl".
+        arg = {"projectType": project_type, "itemID": item_id}
 
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
 
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+    def get_pricelist(
+        self, item_id: int, project_type: Union[ProjectType, int]
+    ) -> PricelistResult:
+        """
+        Returns the current selected Pricelist for the specified item
 
 
-        :param server_authentication_string: str
-        :param server_address: str
         :param item_id: int
         :param project_type: ProjectType
-        :return: Result
+        :return: PricelistResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.registerCallback_Observer
-        response_model = Result
+        proxy = self.__client.plunet_server.DataItem30.getPricelist
+        response_model = PricelistResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "ItemID": item_id,
-            "ProjectType": project_type,
-        }
+        arg = {"itemID": item_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def add_language_combination2(
+    def get_by_language(
         self,
-        source_language: str,
-        target_language: str,
         project_type: Union[ProjectType, int],
         project_id: int,
+        source_language: str,
+        target_language: str,
     ) -> IntegerResult:
         """
-        Method adds a new language combination to the currently selected projected.
-
-        This will be done without calling the update method. Returns an instance of IntegerResult, which
-        contains the identifier of the new language combination.
+        Returns the itemID for the Project with the specified source/target language.
 
 
-        :param source_language: str
-        :param target_language: str
         :param project_type: ProjectType
         :param project_id: int
+        :param source_language: str
+        :param target_language: str
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.addLanguageCombination2
+        proxy = self.__client.plunet_server.DataItem30.get_ByLanguage
         response_model = IntegerResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
         arg = {
-            "sourceLanguage": source_language,
-            "targetLanguage": target_language,
             "projectType": project_type,
             "projectID": project_id,
+            "sourceLanguage": source_language,
+            "targetLanguage": target_language,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def copy_jobs_from_workflow(
-        self, workflow_id: int, project_type: Union[ProjectType, int], item_id: int
+    def set_item_reference(
+        self, project_type: Union[ProjectType, int], item_id: int, reference: str
     ) -> Result:
         """
-        Adds all jobs from the workflow jobs to the position.
+        Sets item reference.
 
 
-        :param workflow_id: int
         :param project_type: ProjectType
         :param item_id: int
+        :param reference: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.copyJobsFromWorkflow
+        proxy = self.__client.plunet_server.DataItem30.setItemReference
         response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "workflowID": workflow_id,
-            "projectType": project_type,
-            "itemID": item_id,
-        }
+        arg = {"projectType": project_type, "itemID": item_id, "reference": reference}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_price_line_list(
-        self, item_id: int, project_type: Union[ProjectType, int]
-    ) -> PriceLineListResult:
+    def get_price_unit(self, price_unit_id: int, language_code: str) -> PriceUnitResult:
         """
-        Returns a list of all item related PriceLine
+        Returns a PriceUnitResult object.
+
+        Possible PriceUnitÂ´s can be obtained over getPriceUnit_List(java.lang.String, java.lang.String, java.lang.String)
 
 
-        :param item_id: int
-        :param project_type: ProjectType
-        :return: PriceLineListResult
+        :param price_unit_id: int
+        :param language_code: str
+        :return: PriceUnitResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getPriceLine_List
-        response_model = PriceLineListResult
-
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
-        else:
-            project_type = int(project_type)
+        proxy = self.__client.plunet_server.DataItem30.getPriceUnit
+        response_model = PriceUnitResult
 
-        arg = {"itemID": item_id, "projectType": project_type}
+        arg = {"PriceUnitID": price_unit_id, "languageCode": language_code}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_language_independent_item_object(
+    def insert_price_line(
         self,
+        item_id: int,
         project_type: Union[ProjectType, int],
-        project_id: int,
-        currency_type: Union[CurrencyType, int],
-    ) -> ItemResult:
+        price_line_in: Union[PriceLineIN, dict],
+        create_as_first_item: bool,
+    ) -> PriceLineResult:
         """
-        Method returns an instance of ItemResult.
-
-        The total price will be displayed in the specified CurrencyType (default: project
-        currency).
+        Inserts a new PriceLine to the specified item
 
 
+        :param item_id: int
         :param project_type: ProjectType
-        :param project_id: int
-        :param currency_type: CurrencyType
-        :return: ItemResult
+        :param price_line_in: PriceLineIN
+        :param create_as_first_item: bool
+        :return: PriceLineResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getLanguageIndependentItemObject
-        response_model = ItemResult
+        proxy = self.__client.plunet_server.DataItem30.insertPriceLine
+        response_model = PriceLineResult
+
+        if type(price_line_in) != PriceLineIN:
+            price_line_in = PriceLineIN(**price_line_in).dict()
+        else:
+            price_line_in = price_line_in.dict()
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        if type(currency_type) == CurrencyType:
-            currency_type = currency_type.value
-        elif type(currency_type) == int:
-            currency_type = currency_type
-        else:
-            currency_type = int(currency_type)
-
         arg = {
+            "itemID": item_id,
             "projectType": project_type,
-            "projectID": project_id,
-            "currencyType": currency_type,
+            "priceLineIN": price_line_in,
+            "createAsFirstItem": create_as_first_item,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_price_unit_list(
-        self, language_code: str, service: str
-    ) -> PriceUnitListResult:
+    def set_pricelist(
+        self, item_id: int, project_type: Union[ProjectType, int], price_list_id: int
+    ) -> Result:
         """
-        Returns a list of priceUnit related to the specified service.
-
-        Possible services can be obtained over DataAdmin30.getAvailableServices(String, String)
+        SetÂ´s the selected Pricelist for the specified item
 
 
-        :param language_code: str
-        :param service: str
-        :return: PriceUnitListResult
+        :param item_id: int
+        :param project_type: ProjectType
+        :param price_list_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getPriceUnit_List
-        response_model = PriceUnitListResult
+        proxy = self.__client.plunet_server.DataItem30.setPricelist
+        response_model = Result
 
-        arg = {"languageCode": language_code, "service": service}
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
+        else:
+            project_type = int(project_type)
+
+        arg = {
+            "itemID": item_id,
+            "projectType": project_type,
+            "priceListID": price_list_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def insert_language_independent_item(
-        self, item_in: Union[ItemIN, dict]
+    def get_best_pricelist(
+        self, project_type: Union[ProjectType, int], item_id: int
     ) -> IntegerResult:
         """
-        Inserts a new language indipendend item into the the specified project.
-
-        There can only be one language independent item per project
+        Method returns the ID of the best fitting customer pricelist IntegerResult.
 
 
-        :param item_in: ItemIN
+        :param project_type: ProjectType
+        :param item_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.insertLanguageIndependentItem
+        proxy = self.__client.plunet_server.DataItem30.getBestPricelist
         response_model = IntegerResult
 
-        if type(item_in) != ItemIN:
-            item_in = ItemIN(**item_in).dict()
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
         else:
-            item_in = item_in.dict()
+            project_type = int(project_type)
+
+        arg = {"projectType": project_type, "itemID": item_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=item_in,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_items_by_status3_by_currency_type(
-        self,
-        project_type: Union[ProjectType, int],
-        status: int,
-        document_status: Union[DocumentStatus, int],
-        currency_type: Union[CurrencyType, int],
-    ) -> ItemListResult:
+    def delete_price_line(
+        self, item_id: int, project_type: Union[ProjectType, int], price_line_id: int
+    ) -> Result:
         """
-        Method returns an instance of ItemListResult, which contains a list of item objects.
-
-        Items are filtered by the item status and the document status. The total price of the items can
-        be returned in the project or home currency.
+        Deletes an existing PriceLine
 
 
+        :param item_id: int
         :param project_type: ProjectType
-        :param status: int
-        :param document_status: DocumentStatus
-        :param currency_type: CurrencyType
-        :return: ItemListResult
+        :param price_line_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getItemsByStatus3ByCurrencyType
-        response_model = ItemListResult
+        proxy = self.__client.plunet_server.DataItem30.deletePriceLine
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        if type(document_status) == DocumentStatus:
-            document_status = document_status.value
-        elif type(document_status) == int:
-            document_status = document_status
-        else:
-            document_status = int(document_status)
-
-        if type(currency_type) == CurrencyType:
-            currency_type = currency_type.value
-        elif type(currency_type) == int:
-            currency_type = currency_type
-        else:
-            currency_type = int(currency_type)
-
         arg = {
+            "itemID": item_id,
             "projectType": project_type,
-            "status": status,
-            "documentStatus": document_status,
-            "currencyType": currency_type,
+            "priceLineID": price_line_id,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_total_price_by_currency_type(
-        self,
-        project_type: Union[ProjectType, int],
-        item_id: int,
-        currency_type: Union[CurrencyType, int],
-    ) -> DoubleResult:
+    def set_status(
+        self, status: int, project_type: Union[ProjectType, int], item_id: int
+    ) -> Result:
         """
-        Method returns total price for an item.
-
-        By default, the price is returned in project currency.
+        Method to set the ItemStatus for the specified item.
 
 
+        :param status: int
         :param project_type: ProjectType
         :param item_id: int
-        :param currency_type: CurrencyType
-        :return: DoubleResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getTotalPriceByCurrencyType
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataItem30.setStatus
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        if type(currency_type) == CurrencyType:
-            currency_type = currency_type.value
-        elif type(currency_type) == int:
-            currency_type = currency_type
+        arg = {"status": status, "projectType": project_type, "itemID": item_id}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def get_order_id(
+        self, project_type: Union[ProjectType, int], item_id: int
+    ) -> IntegerResult:
+        """
+        This method is only available for a quote items.
+
+        The method returns an instance of IntegerResult, which contains the order ID, to which this item
+        (quote) is linked with the order creation.
+
+
+        :param project_type: ProjectType
+        :param item_id: int
+        :return: IntegerResult
+        """
+
+        proxy = self.__client.plunet_server.DataItem30.getOrderID
+        response_model = IntegerResult
+
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
         else:
-            currency_type = int(currency_type)
+            project_type = int(project_type)
 
-        arg = {
-            "projectType": project_type,
-            "itemID": item_id,
-            "currencyType": currency_type,
-        }
+        arg = {"projectType": project_type, "itemID": item_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_items_by_status4_by_currency_type(
+    def get_all_item_objects_by_currency(
         self,
         project_id: int,
         project_type: Union[ProjectType, int],
-        status: int,
-        document_status: Union[DocumentStatus, int],
-        current_type: Union[CurrencyType, int],
+        currency_type: Union[CurrencyType, int],
     ) -> ItemListResult:
         """
-        Method returns an instance of ItemListResult, which contains a list of item objects for a
-        certain project.
+        Method returns an instance of ItemListResult, which contains a list of item objects.
 
-        Items are filtered by the item status and the document status. The total price of the items can
-        be returned in the project or home currency.
+        The total prices will be displayed in the specified CurrencyType (default: project
+        currency).
 
 
         :param project_id: int
         :param project_type: ProjectType
-        :param status: int
-        :param document_status: DocumentStatus
-        :param current_type: CurrencyType
+        :param currency_type: CurrencyType
         :return: ItemListResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getItemsByStatus4ByCurrencyType
+        proxy = self.__client.plunet_server.DataItem30.getAllItemObjectsByCurrency
         response_model = ItemListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        if type(document_status) == DocumentStatus:
-            document_status = document_status.value
-        elif type(document_status) == int:
-            document_status = document_status
-        else:
-            document_status = int(document_status)
-
-        if type(current_type) == CurrencyType:
-            current_type = current_type.value
-        elif type(current_type) == int:
-            current_type = current_type
+        if type(currency_type) == CurrencyType:
+            currency_type = currency_type.value
+        elif type(currency_type) == int:
+            currency_type = currency_type
         else:
-            current_type = int(current_type)
+            currency_type = int(currency_type)
 
         arg = {
             "projectID": project_id,
             "projectType": project_type,
-            "status": status,
-            "documentStatus": document_status,
-            "currentType": current_type,
+            "currencyType": currency_type,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_default_contact_person(
-        self, project_type: Union[ProjectType, int], item_id: int
-    ) -> IntegerResult:
+    def get_pricelist_list(
+        self, item_id: int, project_type: Union[ProjectType, int]
+    ) -> PricelistListResult:
         """
-        Returns the resourceID of the default contact person set for the item.
+        Returns all avaliable Pricelist for this item.
+
+        Note: This is dependent on the related project and the selected customer
 
 
-        :param project_type: ProjectType
         :param item_id: int
-        :return: IntegerResult
+        :param project_type: ProjectType
+        :return: PricelistListResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getDefaultContactPerson
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataItem30.getPricelist_List
+        response_model = PricelistListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "itemID": item_id}
+        arg = {"itemID": item_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_all_item_objects_by_currency(
+    def get_language_independent_item_object(
         self,
-        project_id: int,
         project_type: Union[ProjectType, int],
+        project_id: int,
         currency_type: Union[CurrencyType, int],
-    ) -> ItemListResult:
+    ) -> ItemResult:
         """
-        Method returns an instance of ItemListResult, which contains a list of item objects.
+        Method returns an instance of ItemResult.
 
-        The total prices will be displayed in the specified CurrencyType (default: project
+        The total price will be displayed in the specified CurrencyType (default: project
         currency).
 
 
-        :param project_id: int
         :param project_type: ProjectType
+        :param project_id: int
         :param currency_type: CurrencyType
-        :return: ItemListResult
+        :return: ItemResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getAllItemObjectsByCurrency
-        response_model = ItemListResult
+        proxy = self.__client.plunet_server.DataItem30.getLanguageIndependentItemObject
+        response_model = ItemResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
@@ -1257,16 +1111,16 @@
             currency_type = currency_type.value
         elif type(currency_type) == int:
             currency_type = currency_type
         else:
             currency_type = int(currency_type)
 
         arg = {
-            "projectID": project_id,
             "projectType": project_type,
+            "projectID": project_id,
             "currencyType": currency_type,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
@@ -1348,86 +1202,63 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_pricelist_list(
-        self, item_id: int, project_type: Union[ProjectType, int]
-    ) -> PricelistListResult:
-        """
-        Returns all avaliable Pricelist for this item.
-
-        Note: This is dependent on the related project and the selected customer
-
-
-        :param item_id: int
-        :param project_type: ProjectType
-        :return: PricelistListResult
-        """
-
-        proxy = self.__client.plunet_server.DataItem30.getPricelist_List
-        response_model = PricelistListResult
-
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
-        else:
-            project_type = int(project_type)
-
-        arg = {"itemID": item_id, "projectType": project_type}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def get_price_line_list_by_currency(
+    def get_items_by_status3_by_currency_type(
         self,
-        item_id: int,
         project_type: Union[ProjectType, int],
+        status: int,
+        document_status: Union[DocumentStatus, int],
         currency_type: Union[CurrencyType, int],
-    ) -> PriceLineListResult:
+    ) -> ItemListResult:
         """
-        Returns a list of all item related PriceLine
+        Method returns an instance of ItemListResult, which contains a list of item objects.
 
-        The PriceLine will be returned in the specified CurrencyType (default: project
-        currency).
+        Items are filtered by the item status and the document status. The total price of the items can
+        be returned in the project or home currency.
 
 
-        :param item_id: int
         :param project_type: ProjectType
+        :param status: int
+        :param document_status: DocumentStatus
         :param currency_type: CurrencyType
-        :return: PriceLineListResult
+        :return: ItemListResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getPriceLine_ListByCurrency
-        response_model = PriceLineListResult
+        proxy = self.__client.plunet_server.DataItem30.getItemsByStatus3ByCurrencyType
+        response_model = ItemListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
+        if type(document_status) == DocumentStatus:
+            document_status = document_status.value
+        elif type(document_status) == int:
+            document_status = document_status
+        else:
+            document_status = int(document_status)
+
         if type(currency_type) == CurrencyType:
             currency_type = currency_type.value
         elif type(currency_type) == int:
             currency_type = currency_type
         else:
             currency_type = int(currency_type)
 
         arg = {
-            "itemID": item_id,
             "projectType": project_type,
+            "status": status,
+            "documentStatus": document_status,
             "currencyType": currency_type,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
@@ -1466,28 +1297,27 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_status(
+    def get_default_contact_person(
         self, project_type: Union[ProjectType, int], item_id: int
     ) -> IntegerResult:
         """
-        Method returns an instance of IntegerResult, which contains the ItemStatus depending
-        on the itemID.
+        Returns the resourceID of the default contact person set for the item.
 
 
         :param project_type: ProjectType
         :param item_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getStatus
+        proxy = self.__client.plunet_server.DataItem30.getDefaultContactPerson
         response_model = IntegerResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
@@ -1498,239 +1328,355 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_status(
-        self, status: int, project_type: Union[ProjectType, int], item_id: int
-    ) -> Result:
+    def get_price_line_list_by_currency(
+        self,
+        item_id: int,
+        project_type: Union[ProjectType, int],
+        currency_type: Union[CurrencyType, int],
+    ) -> PriceLineListResult:
         """
-        Method to set the ItemStatus for the specified item.
+        Returns a list of all item related PriceLine
+
+        The PriceLine will be returned in the specified CurrencyType (default: project
+        currency).
 
 
-        :param status: int
-        :param project_type: ProjectType
         :param item_id: int
-        :return: Result
+        :param project_type: ProjectType
+        :param currency_type: CurrencyType
+        :return: PriceLineListResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.setStatus
-        response_model = Result
+        proxy = self.__client.plunet_server.DataItem30.getPriceLine_ListByCurrency
+        response_model = PriceLineListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"status": status, "projectType": project_type, "itemID": item_id}
+        if type(currency_type) == CurrencyType:
+            currency_type = currency_type.value
+        elif type(currency_type) == int:
+            currency_type = currency_type
+        else:
+            currency_type = int(currency_type)
+
+        arg = {
+            "itemID": item_id,
+            "projectType": project_type,
+            "currencyType": currency_type,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_brief_description(
-        self, project_type: Union[ProjectType, int], item_id: int
-    ) -> StringResult:
+    def insert_language_independent_item(
+        self, item_in: Union[ItemIN, dict]
+    ) -> IntegerResult:
         """
-        Method returns an instance of StringResult, which contains the the brief description
-        depending on the itemID.
+        Inserts a new language indipendend item into the the specified project.
+
+        There can only be one language independent item per project
+
+
+        :param item_in: ItemIN
+        :return: IntegerResult
+        """
+
+        proxy = self.__client.plunet_server.DataItem30.insertLanguageIndependentItem
+        response_model = IntegerResult
+
+        if type(item_in) != ItemIN:
+            item_in = ItemIN(**item_in).dict()
+        else:
+            item_in = item_in.dict()
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=item_in,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_price_line_list(
+        self, item_id: int, project_type: Union[ProjectType, int]
+    ) -> PriceLineListResult:
+        """
+        Returns a list of all item related PriceLine
 
 
-        :param project_type: ProjectType
         :param item_id: int
-        :return: StringResult
+        :param project_type: ProjectType
+        :return: PriceLineListResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getBriefDescription
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataItem30.getPriceLine_List
+        response_model = PriceLineListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "itemID": item_id}
+        arg = {"itemID": item_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_document_status(
+    def get_price_unit_list(
+        self, language_code: str, service: str
+    ) -> PriceUnitListResult:
+        """
+        Returns a list of priceUnit related to the specified service.
+
+        Possible services can be obtained over DataAdmin30.getAvailableServices(String, String)
+
+
+        :param language_code: str
+        :param service: str
+        :return: PriceUnitListResult
+        """
+
+        proxy = self.__client.plunet_server.DataItem30.getPriceUnit_List
+        response_model = PriceUnitListResult
+
+        arg = {"languageCode": language_code, "service": service}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def get_total_price_by_currency_type(
         self,
-        document_status: Union[DocumentStatus, int],
         project_type: Union[ProjectType, int],
         item_id: int,
-    ) -> Result:
+        currency_type: Union[CurrencyType, int],
+    ) -> DoubleResult:
         """
-        Method to set the DocumentStatus for the specified item.
+        Method returns total price for an item.
+
+        By default, the price is returned in project currency.
 
 
-        :param document_status: DocumentStatus
         :param project_type: ProjectType
         :param item_id: int
-        :return: Result
+        :param currency_type: CurrencyType
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.setDocumentStatus
-        response_model = Result
-
-        if type(document_status) == DocumentStatus:
-            document_status = document_status.value
-        elif type(document_status) == int:
-            document_status = document_status
-        else:
-            document_status = int(document_status)
+        proxy = self.__client.plunet_server.DataItem30.getTotalPriceByCurrencyType
+        response_model = DoubleResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
+        if type(currency_type) == CurrencyType:
+            currency_type = currency_type.value
+        elif type(currency_type) == int:
+            currency_type = currency_type
+        else:
+            currency_type = int(currency_type)
+
         arg = {
-            "documentStatus": document_status,
             "projectType": project_type,
             "itemID": item_id,
+            "currencyType": currency_type,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_delivery_deadline(
-        self, deadline: datetime, project_type: Union[ProjectType, int], item_id: int
-    ) -> Result:
+    def add_language_combination2(
+        self,
+        source_language: str,
+        target_language: str,
+        project_type: Union[ProjectType, int],
+        project_id: int,
+    ) -> IntegerResult:
         """
-        Method sets the delivery deadline for the specified item.
+        Method adds a new language combination to the currently selected projected.
 
+        This will be done without calling the update method. Returns an instance of IntegerResult, which
+        contains the identifier of the new language combination.
 
-        :param deadline: datetime
+
+        :param source_language: str
+        :param target_language: str
         :param project_type: ProjectType
-        :param item_id: int
-        :return: Result
+        :param project_id: int
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.setDeliveryDeadline
-        response_model = Result
+        proxy = self.__client.plunet_server.DataItem30.addLanguageCombination2
+        response_model = IntegerResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"deadline": deadline, "projectType": project_type, "itemID": item_id}
+        arg = {
+            "sourceLanguage": source_language,
+            "targetLanguage": target_language,
+            "projectType": project_type,
+            "projectID": project_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_brief_description(
-        self, description: str, project_type: Union[ProjectType, int], item_id: int
-    ) -> Result:
+    def get_items_by_status4_by_currency_type(
+        self,
+        project_id: int,
+        project_type: Union[ProjectType, int],
+        status: int,
+        document_status: Union[DocumentStatus, int],
+        current_type: Union[CurrencyType, int],
+    ) -> ItemListResult:
         """
-        Method sets the brief description for the currently selected item.
+        Method returns an instance of ItemListResult, which contains a list of item objects for a
+        certain project.
 
+        Items are filtered by the item status and the document status. The total price of the items can
+        be returned in the project or home currency.
 
-        :param description: str
+
+        :param project_id: int
         :param project_type: ProjectType
-        :param item_id: int
-        :return: Result
+        :param status: int
+        :param document_status: DocumentStatus
+        :param current_type: CurrencyType
+        :return: ItemListResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.setBriefDescription
-        response_model = Result
+        proxy = self.__client.plunet_server.DataItem30.getItemsByStatus4ByCurrencyType
+        response_model = ItemListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
+        if type(document_status) == DocumentStatus:
+            document_status = document_status.value
+        elif type(document_status) == int:
+            document_status = document_status
+        else:
+            document_status = int(document_status)
+
+        if type(current_type) == CurrencyType:
+            current_type = current_type.value
+        elif type(current_type) == int:
+            current_type = current_type
+        else:
+            current_type = int(current_type)
+
         arg = {
-            "description": description,
+            "projectID": project_id,
             "projectType": project_type,
-            "itemID": item_id,
+            "status": status,
+            "documentStatus": document_status,
+            "currentType": current_type,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_document_status(
-        self, project_type: Union[ProjectType, int], item_id: int
-    ) -> IntegerResult:
+    def copy_jobs_from_workflow(
+        self, workflow_id: int, project_type: Union[ProjectType, int], item_id: int
+    ) -> Result:
         """
-        Method returns an instance of IntegerResult, which contains the DocumentStatus
-        depending on the itemID.
+        Adds all jobs from the workflow jobs to the position.
 
 
+        :param workflow_id: int
         :param project_type: ProjectType
         :param item_id: int
-        :return: IntegerResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getDocumentStatus
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataItem30.copyJobsFromWorkflow
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "itemID": item_id}
+        arg = {
+            "workflowID": workflow_id,
+            "projectType": project_type,
+            "itemID": item_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_delivery_deadline(
+    def get_status(
         self, project_type: Union[ProjectType, int], item_id: int
-    ) -> DateResult:
+    ) -> IntegerResult:
         """
-        Method returns an instance of DateResult, which contains the delivery deadline
-        depending on the itemID.
+        Method returns an instance of IntegerResult, which contains the ItemStatus depending
+        on the itemID.
 
 
         :param project_type: ProjectType
         :param item_id: int
-        :return: DateResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getDeliveryDeadline
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataItem30.getStatus
+        response_model = IntegerResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
@@ -1740,471 +1686,523 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_best_pricelist(
-        self, project_type: Union[ProjectType, int], item_id: int
-    ) -> IntegerResult:
+    def insert2(self, item_in: Union[ItemIN, dict]) -> IntegerResult:
         """
-        Method returns the ID of the best fitting customer pricelist IntegerResult.
+        Inserts a new item into the the specified project.
 
 
-        :param project_type: ProjectType
-        :param item_id: int
+        :param item_in: ItemIN
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getBestPricelist
+        proxy = self.__client.plunet_server.DataItem30.insert2
         response_model = IntegerResult
 
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
+        if type(item_in) != ItemIN:
+            item_in = ItemIN(**item_in).dict()
         else:
-            project_type = int(project_type)
+            item_in = item_in.dict()
 
-        arg = {"projectType": project_type, "itemID": item_id}
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=item_in,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
+        """
+        Deletes an registered notify request.
+
+        Info:Notify requests can only be deleted by the user who has created them
+
+
+        :param event_type: EventType
+        :return: Result
+        """
+
+        proxy = self.__client.plunet_server.DataItem30.deregisterCallback_Notify
+        response_model = Result
+
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
+        else:
+            event_type = int(event_type)
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=event_type,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_item_reference(
-        self, project_type: Union[ProjectType, int], item_id: int, reference: str
+    def register_callback_notify(
+        self,
+        server_authentication_string: str,
+        server_address: str,
+        event_type: Union[EventType, int],
     ) -> Result:
         """
-        Sets item reference.
+        Register to get notified when the specified EventType occurs for any item.
 
+        If the EventType occurs PBM will call the callback web service, which is hosted within
+        your environment. The notifier will only be notified if the event is triggered by a different
+        user.
 
-        :param project_type: ProjectType
-        :param item_id: int
-        :param reference: str
+
+        Please check CallbackItem30 for the exact specification for this service.
+
+
+        Info:Each user can only create one notifier per event
+
+
+        The  must match one of the following formats:
+
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
+
+
+        In the first two cases, the address will be autocompleted by appending the corresponding
+        directory "CallbackItem30?wsdl".
+
+
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
+
+
+        :param server_authentication_string: str
+        :param server_address: str
+        :param event_type: EventType
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.setItemReference
+        proxy = self.__client.plunet_server.DataItem30.registerCallback_Notify
         response_model = Result
 
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
         else:
-            project_type = int(project_type)
+            event_type = int(event_type)
 
-        arg = {"projectType": project_type, "itemID": item_id, "reference": reference}
+        arg = {
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "EventType": event_type,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def update_price_line(
+    def register_callback_observer(
         self,
+        server_authentication_string: str,
+        server_address: str,
         item_id: int,
         project_type: Union[ProjectType, int],
-        price_line_in: Union[PriceLineIN, dict],
-    ) -> PriceLineResult:
+    ) -> Result:
         """
-        Updates a existing PriceLine.
+        Register to observe a specific object for any supported EventType.
+
+        As soon as any supported EventType occurs, PBM will call the callback web service, which
+        is hosted within your environment. The observer will only be notified if the event is triggered
+        by a different user.
+
+
+        Please check CallbackItem30 for the exact specification for this service.
+
+
+        Info:Each user can only create one observer per id
+
+
+        The  must match one of the following formats:
+
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
+
+
+        In the first two cases, the address will be autocompleted by appending the corresponding
+        directory "CallbackItem30?wsdl".
+
+
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
 
 
+        :param server_authentication_string: str
+        :param server_address: str
         :param item_id: int
         :param project_type: ProjectType
-        :param price_line_in: PriceLineIN
-        :return: PriceLineResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.updatePriceLine
-        response_model = PriceLineResult
-
-        if type(price_line_in) != PriceLineIN:
-            price_line_in = PriceLineIN(**price_line_in).dict()
-        else:
-            price_line_in = price_line_in.dict()
+        proxy = self.__client.plunet_server.DataItem30.registerCallback_Observer
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
         arg = {
-            "itemID": item_id,
-            "projectType": project_type,
-            "priceLineIN": price_line_in,
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "ItemID": item_id,
+            "ProjectType": project_type,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_pricelist(
+    def deregister_callback_observer(
         self, item_id: int, project_type: Union[ProjectType, int]
-    ) -> PricelistResult:
+    ) -> Result:
         """
-        Returns the current selected Pricelist for the specified item
+        Deletes an observer.
+
+        Observer can only deleted by the user who has created them.
 
 
         :param item_id: int
         :param project_type: ProjectType
-        :return: PricelistResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getPricelist
-        response_model = PricelistResult
+        proxy = self.__client.plunet_server.DataItem30.deregisterCallback_Observer
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"itemID": item_id, "projectType": project_type}
+        arg = {"ItemID": item_id, "ProjectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_pricelist(
-        self, item_id: int, project_type: Union[ProjectType, int], price_list_id: int
-    ) -> Result:
+    def get_items_by_status2(
+        self, project_id: int, project_type: Union[ProjectType, int], status: int
+    ) -> ItemListResult:
         """
-        SetÂ´s the selected Pricelist for the specified item
+        Method returns an instance of ItemListResult, which contains a list of item objects for a
+        certain project.
 
+        Items are filtered by the item status.
 
-        :param item_id: int
+
+        :param project_id: int
         :param project_type: ProjectType
-        :param price_list_id: int
-        :return: Result
+        :param status: int
+        :return: ItemListResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.setPricelist
-        response_model = Result
+        proxy = self.__client.plunet_server.DataItem30.getItemsByStatus2
+        response_model = ItemListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "itemID": item_id,
-            "projectType": project_type,
-            "priceListID": price_list_id,
-        }
+        arg = {"projectID": project_id, "projectType": project_type, "status": status}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_item_reference(
-        self, project_type: Union[ProjectType, int], item_id: int
-    ) -> StringResult:
+    def get_items_by_status3(
+        self,
+        project_type: Union[ProjectType, int],
+        status: int,
+        document_status: Union[DocumentStatus, int],
+    ) -> ItemListResult:
         """
-        Method returns item reference StringResult.
+        Method returns an instance of ItemListResult, which contains a list of item objects.
+
+        Items are filtered by the item status and the document status.
 
 
         :param project_type: ProjectType
-        :param item_id: int
-        :return: StringResult
+        :param status: int
+        :param document_status: DocumentStatus
+        :return: ItemListResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getItemReference
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataItem30.getItemsByStatus3
+        response_model = ItemListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "itemID": item_id}
+        if type(document_status) == DocumentStatus:
+            document_status = document_status.value
+        elif type(document_status) == int:
+            document_status = document_status
+        else:
+            document_status = int(document_status)
+
+        arg = {
+            "projectType": project_type,
+            "status": status,
+            "documentStatus": document_status,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_services_list(self, language_code: str) -> StringArrayResult:
-        """
-        Deprecated. Please use DataAdmin30.getAvailableServices(String, String) instead.
-        Returns a list of all available services.
-
-
-        :param language_code: str
-        :return: StringArrayResult
+    def get_brief_description(
+        self, project_type: Union[ProjectType, int], item_id: int
+    ) -> StringResult:
         """
+        Method returns an instance of StringResult, which contains the the brief description
+        depending on the itemID.
 
-        proxy = self.__client.plunet_server.DataItem30.getServices_List
-        response_model = StringArrayResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=language_code,
-            response_model=response_model,
-            unpack_dict=False,
-        )
 
-    def get_price_unit(self, price_unit_id: int, language_code: str) -> PriceUnitResult:
+        :param project_type: ProjectType
+        :param item_id: int
+        :return: StringResult
         """
-        Returns a PriceUnitResult object.
-
-        Possible PriceUnitÂ´s can be obtained over getPriceUnit_List(java.lang.String, java.lang.String, java.lang.String)
-
 
-        :param price_unit_id: int
-        :param language_code: str
-        :return: PriceUnitResult
-        """
+        proxy = self.__client.plunet_server.DataItem30.getBriefDescription
+        response_model = StringResult
 
-        proxy = self.__client.plunet_server.DataItem30.getPriceUnit
-        response_model = PriceUnitResult
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
+        else:
+            project_type = int(project_type)
 
-        arg = {"PriceUnitID": price_unit_id, "languageCode": language_code}
+        arg = {"projectType": project_type, "itemID": item_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_by_language(
-        self,
-        project_type: Union[ProjectType, int],
-        project_id: int,
-        source_language: str,
-        target_language: str,
-    ) -> IntegerResult:
+    def get_target_language(
+        self, project_type: Union[ProjectType, int], item_id: int
+    ) -> StringResult:
         """
-        Returns the itemID for the Project with the specified source/target language.
+        Method returns an instance of StringResult, which contains the target language depending on
+        the itemID
 
 
         :param project_type: ProjectType
-        :param project_id: int
-        :param source_language: str
-        :param target_language: str
-        :return: IntegerResult
+        :param item_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.get_ByLanguage
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataItem30.getTargetLanguage
+        response_model = StringResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "projectType": project_type,
-            "projectID": project_id,
-            "sourceLanguage": source_language,
-            "targetLanguage": target_language,
-        }
+        arg = {"projectType": project_type, "itemID": item_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def insert_price_line(
-        self,
-        item_id: int,
-        project_type: Union[ProjectType, int],
-        price_line_in: Union[PriceLineIN, dict],
-        create_as_first_item: bool,
-    ) -> PriceLineResult:
+    def get_all_item_objects(
+        self, project_id: int, project_type: Union[ProjectType, int]
+    ) -> ItemListResult:
         """
-        Inserts a new PriceLine to the specified item
+        Method returns an instance of ItemListResult, which contains a list of item objects.
 
 
-        :param item_id: int
+        :param project_id: int
         :param project_type: ProjectType
-        :param price_line_in: PriceLineIN
-        :param create_as_first_item: bool
-        :return: PriceLineResult
+        :return: ItemListResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.insertPriceLine
-        response_model = PriceLineResult
-
-        if type(price_line_in) != PriceLineIN:
-            price_line_in = PriceLineIN(**price_line_in).dict()
-        else:
-            price_line_in = price_line_in.dict()
+        proxy = self.__client.plunet_server.DataItem30.getAllItemObjects
+        response_model = ItemListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "itemID": item_id,
-            "projectType": project_type,
-            "priceLineIN": price_line_in,
-            "createAsFirstItem": create_as_first_item,
-        }
+        arg = {"projectID": project_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def delete_price_line(
-        self, item_id: int, project_type: Union[ProjectType, int], price_line_id: int
-    ) -> Result:
+    def get_jobs_with_status(
+        self, status: int, project_type: Union[ProjectType, int], item_id: int
+    ) -> IntegerArrayResult:
         """
-        Deletes an existing PriceLine
+        Method returns an instance of IntegerArrayResult, which contains a list of IDs of job, which
+        were linked to the currently selected item and have a specific status.
 
 
-        :param item_id: int
+        :param status: int
         :param project_type: ProjectType
-        :param price_line_id: int
-        :return: Result
+        :param item_id: int
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.deletePriceLine
-        response_model = Result
+        proxy = self.__client.plunet_server.DataItem30.getJobsWithStatus
+        response_model = IntegerArrayResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "itemID": item_id,
-            "projectType": project_type,
-            "priceLineID": price_line_id,
-        }
+        arg = {"Status": status, "projectType": project_type, "itemID": item_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_delivery_date(self, delivery_date: datetime, item_id: int) -> Result:
+    def set_brief_description(
+        self, description: str, project_type: Union[ProjectType, int], item_id: int
+    ) -> Result:
         """
-        Method sets the delivery date for the specified item (order items only!).
+        Method sets the brief description for the currently selected item.
 
 
-        :param delivery_date: datetime
+        :param description: str
+        :param project_type: ProjectType
         :param item_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.setDeliveryDate
+        proxy = self.__client.plunet_server.DataItem30.setBriefDescription
         response_model = Result
 
-        arg = {"deliveryDate": delivery_date, "itemID": item_id}
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
+        else:
+            project_type = int(project_type)
+
+        arg = {
+            "description": description,
+            "projectType": project_type,
+            "itemID": item_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_delivery_date(self, item_id: int) -> DateResult:
+    def get_delivery_deadline(
+        self, project_type: Union[ProjectType, int], item_id: int
+    ) -> DateResult:
         """
-        Method returns an instance of DateResult, which contains the delivery date of the item
-        (order items only!).
+        Method returns an instance of DateResult, which contains the delivery deadline
+        depending on the itemID.
 
 
+        :param project_type: ProjectType
         :param item_id: int
         :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getDeliveryDate
+        proxy = self.__client.plunet_server.DataItem30.getDeliveryDeadline
         response_model = DateResult
 
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=item_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def insert2(self, item_in: Union[ItemIN, dict]) -> IntegerResult:
-        """
-        Inserts a new item into the the specified project.
-
-
-        :param item_in: ItemIN
-        :return: IntegerResult
-        """
-
-        proxy = self.__client.plunet_server.DataItem30.insert2
-        response_model = IntegerResult
-
-        if type(item_in) != ItemIN:
-            item_in = ItemIN(**item_in).dict()
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
         else:
-            item_in = item_in.dict()
+            project_type = int(project_type)
+
+        arg = {"projectType": project_type, "itemID": item_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=item_in,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_order_id(
+    def get_source_language(
         self, project_type: Union[ProjectType, int], item_id: int
-    ) -> IntegerResult:
+    ) -> StringResult:
         """
-        This method is only available for a quote items.
-
-        The method returns an instance of IntegerResult, which contains the order ID, to which this item
-        (quote) is linked with the order creation.
+        Method returns an instance of StringResult, the source language depending on the itemID
 
 
         :param project_type: ProjectType
         :param item_id: int
-        :return: IntegerResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getOrderID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataItem30.getSourceLanguage
+        response_model = StringResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
@@ -2214,330 +2212,331 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_cat_report2(
-        self,
-        file_byte_stream: bytes,
-        file_path_name: str,
-        filesize: int,
-        overwrite_existing_price_lines: bool,
-        cat_type: Union[CatType, int],
-        project_type: Union[ProjectType, int],
-        copy_results_to_item: bool,
-        item_id: int,
+    def set_delivery_deadline(
+        self, deadline: datetime, project_type: Union[ProjectType, int], item_id: int
     ) -> Result:
         """
-        Uploads a report file into the report folder of the specified item.
-
-        Also allows to copy the results of the report into the item (optionally overwriting existing
-        price lines)
+        Method sets the delivery deadline for the specified item.
 
 
-        :param file_byte_stream: bytes
-        :param file_path_name: str
-        :param filesize: int
-        :param overwrite_existing_price_lines: bool
-        :param cat_type: CatType
+        :param deadline: datetime
         :param project_type: ProjectType
-        :param copy_results_to_item: bool
         :param item_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.setCatReport2
+        proxy = self.__client.plunet_server.DataItem30.setDeliveryDeadline
         response_model = Result
 
-        if type(cat_type) == CatType:
-            cat_type = cat_type.value
-        elif type(cat_type) == int:
-            cat_type = cat_type
-        else:
-            cat_type = int(cat_type)
-
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "FileByteStream": file_byte_stream,
-            "FilePathName": file_path_name,
-            "Filesize": filesize,
-            "overwriteExistingPriceLines": overwrite_existing_price_lines,
-            "catType": cat_type,
-            "projectType": project_type,
-            "copyResultsToItem": copy_results_to_item,
-            "itemID": item_id,
-        }
+        arg = {"deadline": deadline, "projectType": project_type, "itemID": item_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_invoice_id(
-        self, project_type: Union[ProjectType, int], item_id: int
-    ) -> IntegerResult:
+    def get_items_by_status1(
+        self, project_type: Union[ProjectType, int], status: int
+    ) -> ItemListResult:
         """
-        Method returns an instance of IntegerResult, which contains the ID of the invoice for the
-        currently selected item.
-
-        This method is only available for an order items.
+        Method returns an instance of ItemListResult, which contains a list of item objects. Items are
+        filtered by the item status.
 
 
         :param project_type: ProjectType
-        :param item_id: int
-        :return: IntegerResult
+        :param status: int
+        :return: ItemListResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getInvoiceID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataItem30.getItemsByStatus1
+        response_model = ItemListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "itemID": item_id}
+        arg = {"projectType": project_type, "status": status}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_total_price(
-        self, project_type: Union[ProjectType, int], total_price: float, item_id: int
+    def set_language_combination_id(
+        self,
+        language_combination_id: int,
+        project_type: Union[ProjectType, int],
+        item_id: int,
     ) -> Result:
         """
-        Method sets total price for an item (project currency).
+        Method sets the language combination ID for the specified item.
 
 
+        :param language_combination_id: int
         :param project_type: ProjectType
-        :param total_price: float
         :param item_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.setTotalPrice
+        proxy = self.__client.plunet_server.DataItem30.setLanguageCombinationID
         response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
         arg = {
+            "languageCombinationID": language_combination_id,
             "projectType": project_type,
-            "totalPrice": total_price,
             "itemID": item_id,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_cat_report(
-        self,
-        path_or_url: str,
-        overwrite_existing_price_lines: bool,
-        cat_type: Union[CatType, int],
-        project_type: Union[ProjectType, int],
-        copy_results_to_item: bool,
-        item_id: int,
-    ) -> Result:
+    def get_document_status(
+        self, project_type: Union[ProjectType, int], item_id: int
+    ) -> IntegerResult:
         """
-        Deprecated. Please use
-        setCatReport2(String, byte[], String, int, boolean, int, int, boolean, int)
-        instead. Please note that this call is now deactivated by default. For Reactivation
-        please contact Support@plunet.com.
-
-
-        Uploads a report file into the report folder of the specified item.
-
-        Also allows to copy the results of the report into the item (optionally overwriting
-        existing price lines)
+        Method returns an instance of IntegerResult, which contains the DocumentStatus
+        depending on the itemID.
 
 
-        :param path_or_url: str
-        :param overwrite_existing_price_lines: bool
-        :param cat_type: CatType
         :param project_type: ProjectType
-        :param copy_results_to_item: bool
         :param item_id: int
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.setCatReport
-        response_model = Result
-
-        if type(cat_type) == CatType:
-            cat_type = cat_type.value
-        elif type(cat_type) == int:
-            cat_type = cat_type
-        else:
-            cat_type = int(cat_type)
+        proxy = self.__client.plunet_server.DataItem30.getDocumentStatus
+        response_model = IntegerResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "pathOrUrl": path_or_url,
-            "overwriteExistingPriceLines": overwrite_existing_price_lines,
-            "catType": cat_type,
-            "projectType": project_type,
-            "copyResultsToItem": copy_results_to_item,
-            "itemID": item_id,
-        }
+        arg = {"projectType": project_type, "itemID": item_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_item_object(
-        self, project_type: Union[ProjectType, int], item_id: int
-    ) -> ItemResult:
+    def get_items_by_status4(
+        self,
+        project_id: int,
+        project_type: Union[ProjectType, int],
+        status: int,
+        document_status: Union[DocumentStatus, int],
+    ) -> ItemListResult:
         """
-        Method returns an instance of ItemResult.
+        Method returns an instance of ItemListResult, which contains a list of item objects for a
+        certain project.
+
+        Items are filtered by the item status and the document status.
 
 
+        :param project_id: int
         :param project_type: ProjectType
-        :param item_id: int
-        :return: ItemResult
+        :param status: int
+        :param document_status: DocumentStatus
+        :return: ItemListResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getItemObject
-        response_model = ItemResult
+        proxy = self.__client.plunet_server.DataItem30.getItemsByStatus4
+        response_model = ItemListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "itemID": item_id}
+        if type(document_status) == DocumentStatus:
+            document_status = document_status.value
+        elif type(document_status) == int:
+            document_status = document_status
+        else:
+            document_status = int(document_status)
+
+        arg = {
+            "projectID": project_id,
+            "projectType": project_type,
+            "status": status,
+            "documentStatus": document_status,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_jobs(
-        self, project_type: Union[ProjectType, int], item_id: int
-    ) -> IntegerArrayResult:
+    def seek_language_combination(
+        self,
+        source_language: str,
+        target_language: str,
+        project_type: Union[ProjectType, int],
+        project_id: int,
+        item_id: int,
+    ) -> IntegerResult:
         """
-        Method returns an instance of IntegerArrayResult, which contains all job IDs depending on the
-        itemID.
+        Method returns an instance of IntegerResult, which contains the ID of a specific language
+        combination for the specified project.
 
 
+        :param source_language: str
+        :param target_language: str
         :param project_type: ProjectType
+        :param project_id: int
         :param item_id: int
-        :return: IntegerArrayResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getJobs
-        response_model = IntegerArrayResult
+        proxy = self.__client.plunet_server.DataItem30.seekLanguageCombination
+        response_model = IntegerResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "itemID": item_id}
+        arg = {
+            "sourceLanguage": source_language,
+            "targetLanguage": target_language,
+            "projectType": project_type,
+            "projectID": project_id,
+            "itemID": item_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_total_price(
-        self, project_type: Union[ProjectType, int], item_id: int
-    ) -> DoubleResult:
+    def add_language_combination(
+        self,
+        source_language: str,
+        target_language: str,
+        project_type: Union[ProjectType, int],
+        project_id: int,
+        item_id: int,
+    ) -> IntegerResult:
         """
-        Method returns total price for an item (project currency).
+        Deprecated. Please use {link addLanguageCombination2(String, String, String, int, int)
+        instead the itemID is not required for this method.
 
 
+        :param source_language: str
+        :param target_language: str
         :param project_type: ProjectType
+        :param project_id: int
         :param item_id: int
-        :return: DoubleResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getTotalPrice
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataItem30.addLanguageCombination
+        response_model = IntegerResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "itemID": item_id}
+        arg = {
+            "sourceLanguage": source_language,
+            "targetLanguage": target_language,
+            "projectType": project_type,
+            "projectID": project_id,
+            "itemID": item_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_all_items(
-        self, project_type: Union[ProjectType, int], project_id: int
-    ) -> IntegerArrayResult:
+    def set_document_status(
+        self,
+        document_status: Union[DocumentStatus, int],
+        project_type: Union[ProjectType, int],
+        item_id: int,
+    ) -> Result:
         """
-        Method returns an instance of IntegerArrayResult, which contains a list of all item
-        ids for the specified project.
+        Method to set the DocumentStatus for the specified item.
 
 
+        :param document_status: DocumentStatus
         :param project_type: ProjectType
-        :param project_id: int
-        :return: IntegerArrayResult
+        :param item_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataItem30.getAllItems
-        response_model = IntegerArrayResult
+        proxy = self.__client.plunet_server.DataItem30.setDocumentStatus
+        response_model = Result
+
+        if type(document_status) == DocumentStatus:
+            document_status = document_status.value
+        elif type(document_status) == int:
+            document_status = document_status
+        else:
+            document_status = int(document_status)
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "projectID": project_id}
+        arg = {
+            "documentStatus": document_status,
+            "projectType": project_type,
+            "itemID": item_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_job30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_job30.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,84 +25,20 @@
     Result,
     StringArrayResult,
     StringResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataJob30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
-    def get_creation_date(
-        self, project_type: Union[ProjectType, int], job_id: int
-    ) -> DateResult:
-        """
-        Returns an instance of IntegerResult containing the creation date of the job
-
-
-        :param project_type: ProjectType
-        :param job_id: int
-        :return: DateResult
-        """
-
-        proxy = self.__client.plunet_server.DataJob30.getCreationDate
-        response_model = DateResult
-
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
-        else:
-            project_type = int(project_type)
-
-        arg = {"projectType": project_type, "jobID": job_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def set_item_id(
-        self, project_type: Union[ProjectType, int], item_id: int, job_id: int
-    ) -> Result:
-        """
-        Method to set the item id for the specified job.
-
-
-        :param project_type: ProjectType
-        :param item_id: int
-        :param job_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataJob30.setItemID
-        response_model = Result
-
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
-        else:
-            project_type = int(project_type)
-
-        arg = {"projectType": project_type, "itemID": item_id, "jobID": job_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
     def update(
         self, job_in: Union[JobIN, dict], enable_null_or_empty_values: bool
     ) -> Result:
         """
         Updates a job depending on the transfered job object.
         Use the parameter "enabled" to decide if Null or empty Strings are saved
         into Plunet or ignored.
@@ -260,40 +196,38 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_resource_id(
-        self, project_type: Union[ProjectType, int], resource_id: int, job_id: int
+    def set_description(
+        self, project_type: Union[ProjectType, int], job_id: int, description: str
     ) -> Result:
         """
-        Deprecated. This method is no longer supported. Please use the new Endpoint DataJobRound30 for resource assignment.
-        For further information, please refer to the release notes.
-        Method to set the resource id for the specified Job.
+        Method to set the description of the job.
 
 
         :param project_type: ProjectType
-        :param resource_id: int
         :param job_id: int
+        :param description: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.setResourceID
+        proxy = self.__client.plunet_server.DataJob30.setDescription
         response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "resourceID": resource_id, "jobID": job_id}
+        arg = {"projectType": project_type, "jobID": job_id, "description": description}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
@@ -325,248 +259,310 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_description(
-        self, project_type: Union[ProjectType, int], job_id: int, description: str
+    def set_resource_id(
+        self, project_type: Union[ProjectType, int], resource_id: int, job_id: int
     ) -> Result:
         """
-        Method to set the description of the job.
+        Deprecated. This method is no longer supported. Please use the new Endpoint DataJobRound30 for resource assignment.
+        For further information, please refer to the release notes.
+        Method to set the resource id for the specified Job.
 
 
         :param project_type: ProjectType
+        :param resource_id: int
         :param job_id: int
-        :param description: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.setDescription
+        proxy = self.__client.plunet_server.DataJob30.setResourceID
         response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "jobID": job_id, "description": description}
+        arg = {"projectType": project_type, "resourceID": resource_id, "jobID": job_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def deregister_callback_observer(
-        self, job_id: int, project_type: Union[ProjectType, int]
+    def set_cat_report(
+        self,
+        path_or_url: str,
+        overwrite_existing_price_lines: bool,
+        cat_type: Union[CatType, int],
+        project_type: Union[ProjectType, int],
+        analyze_and_copy_result_to_job: bool,
+        job_id: int,
     ) -> Result:
         """
-        Deletes an observer.
-        Observer can only deleted by the user who has created them.
+        Deprecated. Please use setCatReport2(String, byte[], String, int, int, int, boolean, int) instead.
+        Please note that this call is now deactivated by default. For Reactivation please contact Support@plunet.com.
 
+        Uploads a report file into the report folder of the specified job.
+        Specify by value to copy the results of the report into the job and
+        if they should overwrite already existing price lines.
 
-        :param job_id: int
+
+        :param path_or_url: str
+        :param overwrite_existing_price_lines: bool
+        :param cat_type: CatType
         :param project_type: ProjectType
+        :param analyze_and_copy_result_to_job: bool
+        :param job_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.deregisterCallback_Observer
+        proxy = self.__client.plunet_server.DataJob30.setCatReport
         response_model = Result
 
+        if type(cat_type) == CatType:
+            cat_type = cat_type.value
+        elif type(cat_type) == int:
+            cat_type = cat_type
+        else:
+            cat_type = int(cat_type)
+
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"JobID": job_id, "ProjectType": project_type}
+        arg = {
+            "pathOrUrl": path_or_url,
+            "overwriteExistingPriceLines": overwrite_existing_price_lines,
+            "catType": cat_type,
+            "projectType": project_type,
+            "analyzeAndCopyResultToJob": analyze_and_copy_result_to_job,
+            "jobID": job_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def register_callback_notify(
+    def set_cat_report2(
         self,
-        server_authentication_string: str,
-        server_address: str,
-        event_type: Union[EventType, int],
+        file_byte_stream: bytes,
+        file_path_name: str,
+        filesize: int,
+        cat_type: Union[CatType, int],
+        project_type: Union[ProjectType, int],
+        analyze_and_copy_result_to_job: bool,
+        job_id: int,
     ) -> Result:
         """
-        Register to get notified when the specified EventType occurs
-        for any job.
-
-        If the EventType occurs PBM will call the callback web service,
-        which is hosted within your environment.
-
-
-        Please check CallbackCustomer30 for the exact specification for
-        this service.
-
-
-        Info:Each user can only create one notifier per event
-
-
-        The  must match one of the following formats:
-
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
-
-        In the first two cases, the address will be autocompleted by appending
-        the corresponding directory "CallbackJob30?wsdl".
-
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+        Uploads a report file into the report folder of the specified job.
+        Specify by value to copy the results of the report into the job and
+        if they should overwrite already existing price lines.
 
 
-        :param server_authentication_string: str
-        :param server_address: str
-        :param event_type: EventType
+        :param file_byte_stream: bytes
+        :param file_path_name: str
+        :param filesize: int
+        :param cat_type: CatType
+        :param project_type: ProjectType
+        :param analyze_and_copy_result_to_job: bool
+        :param job_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.registerCallback_Notify
+        proxy = self.__client.plunet_server.DataJob30.setCatReport2
         response_model = Result
 
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
+        if type(cat_type) == CatType:
+            cat_type = cat_type.value
+        elif type(cat_type) == int:
+            cat_type = cat_type
         else:
-            event_type = int(event_type)
+            cat_type = int(cat_type)
+
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
+        else:
+            project_type = int(project_type)
 
         arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "EventType": event_type,
+            "FileByteStream": file_byte_stream,
+            "FilePathName": file_path_name,
+            "Filesize": filesize,
+            "catType": cat_type,
+            "projectType": project_type,
+            "analyzeAndCopyResultToJob": analyze_and_copy_result_to_job,
+            "jobID": job_id,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
+    def set_item_id(
+        self, project_type: Union[ProjectType, int], item_id: int, job_id: int
+    ) -> Result:
         """
-        Deletes an registered notify request.
-        Info:Notify requests can only be deleted by the user who has created them
+        Method to set the item id for the specified job.
 
 
-        :param event_type: EventType
+        :param project_type: ProjectType
+        :param item_id: int
+        :param job_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.deregisterCallback_Notify
+        proxy = self.__client.plunet_server.DataJob30.setItemID
         response_model = Result
 
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
         else:
-            event_type = int(event_type)
+            project_type = int(project_type)
+
+        arg = {"projectType": project_type, "itemID": item_id, "jobID": job_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=event_type,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def register_callback_observer(
-        self,
-        server_authentication_string: str,
-        server_address: str,
-        job_id: int,
-        project_type: Union[ProjectType, int],
-    ) -> Result:
+    def get_delivery_date(
+        self, project_type: Union[ProjectType, int], job_id: int
+    ) -> DateResult:
         """
-        Register to observe a specific object for any supported
-        EventType.
-
-        As soon as any supported EventType occurs, PBM will call the
-        callback web service, which is hosted within your environment.
-
-
-        Please check CallbackCustomer30 for the exact specification for
-        this service.
+        Returns an instance of DateResult representing the delivery
+        date of the job using the default time zone.
 
 
-        Info:Each user can only create one observer per id
+        :param project_type: ProjectType
+        :param job_id: int
+        :return: DateResult
+        """
 
+        proxy = self.__client.plunet_server.DataJob30.getDeliveryDate
+        response_model = DateResult
 
-        The  must match one of the following formats:
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
+        else:
+            project_type = int(project_type)
 
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
+        arg = {"projectType": project_type, "jobID": job_id}
 
-        In the first two cases, the address will be autocompleted by appending
-        the corresponding directory "CallbackJob30?wsdl".
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
 
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+    def update_price_line(
+        self,
+        job_id: int,
+        project_type: Union[ProjectType, int],
+        price_line_in: Union[PriceLineIN, dict],
+    ) -> PriceLineResult:
+        """
+        Updates a existing PriceLine.
 
 
-        :param server_authentication_string: str
-        :param server_address: str
         :param job_id: int
         :param project_type: ProjectType
-        :return: Result
+        :param price_line_in: PriceLineIN
+        :return: PriceLineResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.registerCallback_Observer
-        response_model = Result
+        proxy = self.__client.plunet_server.DataJob30.updatePriceLine
+        response_model = PriceLineResult
+
+        if type(price_line_in) != PriceLineIN:
+            price_line_in = PriceLineIN(**price_line_in).dict()
+        else:
+            price_line_in = price_line_in.dict()
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
         arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "JobID": job_id,
-            "ProjectType": project_type,
+            "jobID": job_id,
+            "projectType": project_type,
+            "priceLineIN": price_line_in,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_price_line_list(
+    def get_services_list(self, language_code: str) -> StringArrayResult:
+        """
+        Deprecated. Please use DataAdmin30.getAvailableServices(String, String) instead.
+        Returns a list of all avaliable services.
+
+
+        :param language_code: str
+        :return: StringArrayResult
+        """
+
+        proxy = self.__client.plunet_server.DataJob30.getServices_List
+        response_model = StringArrayResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=language_code,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_pricelist(
         self, job_id: int, project_type: Union[ProjectType, int]
-    ) -> PriceLineListResult:
+    ) -> PricelistResult:
         """
-        Returns a list of all job related PriceLine
+        Returns the current selected Pricelist for the specified job
 
 
         :param job_id: int
         :param project_type: ProjectType
-        :return: PriceLineListResult
+        :return: PricelistResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getPriceLine_List
-        response_model = PriceLineListResult
+        proxy = self.__client.plunet_server.DataJob30.getPricelist
+        response_model = PricelistResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
@@ -576,718 +572,665 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_price_unit_list(
-        self, language_code: str, service: str
-    ) -> PriceUnitListResult:
+    def get_price_unit(self, price_unit_id: int, language_code: str) -> PriceUnitResult:
         """
-        Returns a list of priceUnit related to the specified service.
-        Possible services can be obtained over DataAdmin30.getAvailableServices(String, String)
+        Returns a PriceUnitResult object.
+        Possible PriceUnitÂ´s can be obtained over DataItem30.getPriceUnit_List(java.lang.String, java.lang.String, java.lang.String)
 
 
+        :param price_unit_id: int
         :param language_code: str
-        :param service: str
-        :return: PriceUnitListResult
+        :return: PriceUnitResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getPriceUnit_List
-        response_model = PriceUnitListResult
+        proxy = self.__client.plunet_server.DataJob30.getPriceUnit
+        response_model = PriceUnitResult
 
-        arg = {"languageCode": language_code, "service": service}
+        arg = {"PriceUnitID": price_unit_id, "languageCode": language_code}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_pricelist_entry_list(
-        self, pricelist_id: int, source_language: str, target_language: str
-    ) -> PricelistEntryList:
+    def insert_price_line(
+        self,
+        job_id: int,
+        project_type: Union[ProjectType, int],
+        price_line_in: Union[PriceLineIN, dict],
+        create_as_first_item: bool,
+    ) -> PriceLineResult:
         """
-        Provides all price entries which are related to the Pricelist
-        regarding the transfered source and target language.
+        Inserts a new PriceLine to the specified job
+        Warning: Job-Price lines do not support the price-line memo value.
+        This value will be ignored by this specific implementation.
 
 
-        :param pricelist_id: int
-        :param source_language: str
-        :param target_language: str
-        :return: PricelistEntryList
+        :param job_id: int
+        :param project_type: ProjectType
+        :param price_line_in: PriceLineIN
+        :param create_as_first_item: bool
+        :return: PriceLineResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getPricelistEntry_List
-        response_model = PricelistEntryList
+        proxy = self.__client.plunet_server.DataJob30.insertPriceLine
+        response_model = PriceLineResult
+
+        if type(price_line_in) != PriceLineIN:
+            price_line_in = PriceLineIN(**price_line_in).dict()
+        else:
+            price_line_in = price_line_in.dict()
+
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
+        else:
+            project_type = int(project_type)
 
         arg = {
-            "PricelistID": pricelist_id,
-            "SourceLanguage": source_language,
-            "TargetLanguage": target_language,
+            "jobID": job_id,
+            "projectType": project_type,
+            "priceLineIN": price_line_in,
+            "createAsFirstItem": create_as_first_item,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_pricelist_list(
-        self, job_id: int, project_type: Union[ProjectType, int]
-    ) -> PricelistListResult:
+    def set_pricelist(
+        self, job_id: int, project_type: Union[ProjectType, int], price_list_id: int
+    ) -> Result:
         """
-        Returns all avaliable Pricelist for this job.
-        Note: This is dependent on the related project and the selected customer
+        SetÂ´s the selected Pricelist for the specified job
 
 
         :param job_id: int
         :param project_type: ProjectType
-        :return: PricelistListResult
+        :param price_list_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getPricelist_List
-        response_model = PricelistListResult
+        proxy = self.__client.plunet_server.DataJob30.setPricelist
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"jobID": job_id, "projectType": project_type}
+        arg = {
+            "jobID": job_id,
+            "projectType": project_type,
+            "priceListID": price_list_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_contact_person_id(
-        self, project_type: Union[ProjectType, int], job_id: int
-    ) -> IntegerResult:
+    def delete_price_line(
+        self, job_id: int, project_type: Union[ProjectType, int], price_line_id: int
+    ) -> Result:
         """
-        Returns an instance of IntegerResult containing the resource ID
-        of the jobs contact person.
-        Refers to the field Job -> "Contact person for job" in the Plunet BM.
+        Deletes an existing PriceLine
 
 
-        :param project_type: ProjectType
         :param job_id: int
-        :return: IntegerResult
+        :param project_type: ProjectType
+        :param price_line_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getContactPersonID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataJob30.deletePriceLine
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "jobID": job_id}
+        arg = {
+            "jobID": job_id,
+            "projectType": project_type,
+            "priceLineID": price_line_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_job_type_long_name(
-        self, project_type: Union[ProjectType, int], job_id: int
+    def get_action_link(
+        self,
+        project_type: Union[ProjectType, int],
+        job_id: int,
+        user_id: int,
+        action_link_type: int,
     ) -> StringResult:
         """
-        Returns an instance of StringResult containing the full name (English)
-        of the job type for the specified job. â e.g. Translation.
+        Method to obtain any kind of job related action link.
 
 
         :param project_type: ProjectType
         :param job_id: int
+        :param user_id: int
+        :param action_link_type: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getJobType_LongName
+        proxy = self.__client.plunet_server.DataJob30.getActionLink
         response_model = StringResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "jobID": job_id}
+        arg = {
+            "projectType": project_type,
+            "jobID": job_id,
+            "userID": user_id,
+            "actionLinkType": action_link_type,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def add_job_tracking_time(
-        self,
-        job_id: int,
-        project_type: Union[ProjectType, int],
-        job_tracking_time_in: Union[JobTrackingTimeIN, dict],
-    ) -> Result:
+    def insert3(self, job_in: Union[JobIN, dict], job_type_short: str) -> IntegerResult:
         """
-        Add a JobTrackingTimeIN to the specified job.
-        Please note that the tracking time will not be added if one of the following conditions is violated:
-
-        The overall completed percentage of a job must not exceed 100%.
-        A Tracking time can only be added if the resource has access to the job.
-        The current (API) user must own the proper rights to set the tracking times (see Admin -> Rights -> Resources -> [API user] -> Time sheet).
+        Inserts a new Job.
 
 
-        :param job_id: int
-        :param project_type: ProjectType
-        :param job_tracking_time_in: JobTrackingTimeIN
-        :return: Result
+        :param job_in: JobIN
+        :param job_type_short: str
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.addJobTrackingTime
-        response_model = Result
-
-        if type(job_tracking_time_in) != JobTrackingTimeIN:
-            job_tracking_time_in = JobTrackingTimeIN(**job_tracking_time_in).dict()
-        else:
-            job_tracking_time_in = job_tracking_time_in.dict()
+        proxy = self.__client.plunet_server.DataJob30.insert3
+        response_model = IntegerResult
 
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
+        if type(job_in) != JobIN:
+            job_in = JobIN(**job_in).dict()
         else:
-            project_type = int(project_type)
+            job_in = job_in.dict()
 
-        arg = {
-            "jobID": job_id,
-            "projectType": project_type,
-            "JobTrackingTimeIN": job_tracking_time_in,
-        }
+        arg = {"JobIN": job_in, "JobTypeShort": job_type_short}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_contact_person_id(
-        self, project_type: Union[ProjectType, int], job_id: int, resource_id: int
-    ) -> Result:
+    def get_job_for_view(
+        self, job_id: int, project_type: Union[ProjectType, int]
+    ) -> JobResult:
         """
-        Method to set the resourceID of the contact-person for the specified job.
-        Refers to the field Job -> "Contact person for job" in the Plunet BM.
+        This method returns a single instance of job.
+        This method only returns a set of information about a job, e.g. to display
+        this information in your application.
 
 
-        :param project_type: ProjectType
         :param job_id: int
-        :param resource_id: int
-        :return: Result
+        :param project_type: ProjectType
+        :return: JobResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.setContactPersonID
-        response_model = Result
+        proxy = self.__client.plunet_server.DataJob30.getJob_ForView
+        response_model = JobResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "jobID": job_id, "resourceID": resource_id}
+        arg = {"jobID": job_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_job_list_for_view(
-        self, job_i_ds: str, project_type: Union[ProjectType, int]
-    ) -> JobListResult:
+    def set_price_liste_id(
+        self, project_type: Union[ProjectType, int], price_list_id: int, job_id: int
+    ) -> Result:
         """
-        Method returns an instance of JobListResult, containing a list of Job objects.
-        This method only returns a set of information about a set of jobs, e.g. to
-        display this information in your application.
+        Deprecated. This call is deprecated and may be removed in future api versions.
+        Please use setPricelist(String, int, int, int) instead.
 
 
-        :param job_i_ds: str
         :param project_type: ProjectType
-        :return: JobListResult
+        :param price_list_id: int
+        :param job_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getJobList_ForView
-        response_model = JobListResult
+        proxy = self.__client.plunet_server.DataJob30.setPriceListeID
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"jobIDs": job_i_ds, "projectType": project_type}
+        arg = {
+            "projectType": project_type,
+            "priceListID": price_list_id,
+            "jobID": job_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_resource_contact_person_id(
-        self, project_type: Union[ProjectType, int], job_id: int
-    ) -> IntegerResult:
+    def set_start_date(
+        self, project_type: Union[ProjectType, int], start_date: datetime, job_id: int
+    ) -> Result:
         """
-        Returns an instance of IntegerResult containing the resource ID
-        of the contact person.
-        Refers to the field Job -> "Contact persons" in the Plunet BM.
+        Method to set the start-date for the specified job.
 
 
         :param project_type: ProjectType
+        :param start_date: datetime
         :param job_id: int
-        :return: IntegerResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getResourceContactPersonID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataJob30.setStartDate
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "jobID": job_id}
+        arg = {"projectType": project_type, "startDate": start_date, "jobID": job_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_item_independent_jobs(
-        self, project_type: Union[ProjectType, int], project_id: int
-    ) -> JobListResult:
+    def get_due_date(
+        self, project_type: Union[ProjectType, int], job_id: int
+    ) -> DateResult:
         """
-        Returns an instance of JobListResult, which contains a list of all language
-        independent jobs .
+        Returns an instance of DateResult representing the due date of the job.
 
 
         :param project_type: ProjectType
-        :param project_id: int
-        :return: JobListResult
+        :param job_id: int
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getItemIndependentJobs
-        response_model = JobListResult
+        proxy = self.__client.plunet_server.DataJob30.getDueDate
+        response_model = DateResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "projectId": project_id}
+        arg = {"projectType": project_type, "jobID": job_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_job_tracking_times_list(
-        self, job_id: int, project_type: Union[ProjectType, int]
-    ) -> JobTrackingTimeResult:
+    def get_job_metrics(
+        self, job_id: int, project_type: Union[ProjectType, int], language_code: str
+    ) -> JobMetricResult:
         """
-        Returns a list of all job tracking times.
+        Retrieves the job's total price and amounts.
 
 
         :param job_id: int
         :param project_type: ProjectType
-        :return: JobTrackingTimeResult
+        :param language_code: str
+        :return: JobMetricResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getJobTrackingTimesList
-        response_model = JobTrackingTimeResult
+        proxy = self.__client.plunet_server.DataJob30.getJobMetrics
+        response_model = JobMetricResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"jobID": job_id, "projectType": project_type}
+        arg = {
+            "jobID": job_id,
+            "projectType": project_type,
+            "languageCode": language_code,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_job_list_of_item_for_view(
-        self, item_id: int, project_type: Union[ProjectType, int]
-    ) -> JobListResult:
+    def assign_job(
+        self, project_type: Union[ProjectType, int], job_id: int, resource_id: int
+    ) -> Result:
         """
-        Method returns an instance of JobListResult, containing a list of Job objects.
-        All available job for a specific itemID will be returned.
-        This method only returns a set of information about a set of jobs, e.g.
-        to display this information in your application.
+        Deprecated. This method is no longer supported. Please use the new Endpoint DataJobRound30 for resource assignment.
+        For further information, please refer to the release notes.
+        Assigns a job to a resource.
 
 
-        :param item_id: int
         :param project_type: ProjectType
-        :return: JobListResult
+        :param job_id: int
+        :param resource_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getJobListOfItem_ForView
-        response_model = JobListResult
+        proxy = self.__client.plunet_server.DataJob30.assignJob
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"itemID": item_id, "projectType": project_type}
+        arg = {"projectType": project_type, "jobID": job_id, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_job_type_short_name(
-        self, project_type: Union[ProjectType, int], job_id: int
-    ) -> StringResult:
+    def delete_job(self, job_id: int, project_type: Union[ProjectType, int]) -> Result:
         """
-        Returns an instance of StringResult containing the abbreviated name (English)
-        of the job type for the specified job. â e.g. TRA.
+        Deletes a job.
 
 
-        :param project_type: ProjectType
         :param job_id: int
-        :return: StringResult
+        :param project_type: ProjectType
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getJobType_ShortName
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataJob30.deleteJob
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "jobID": job_id}
+        arg = {"jobID": job_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_resource_contact_person_id(
-        self, project_type: Union[ProjectType, int], job_id: int, contact_id: int
+    def run_automatic_job(
+        self, job_id: int, project_type: Union[ProjectType, int]
     ) -> Result:
         """
-        Method to set the resourceID of the contact-person.
+        Start or restart an automatic job.
 
-        Refers to the field Job -> "Contact persons" in the Plunet BM.
+        Please note that a job can only be started in its initial job status (as
+        defined in the admin settings). This does not apply for restarting jobs.
 
 
-        :param project_type: ProjectType
         :param job_id: int
-        :param contact_id: int
+        :param project_type: ProjectType
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.setResourceContactPersonID
+        proxy = self.__client.plunet_server.DataJob30.runAutomaticJob
         response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "jobID": job_id, "contactID": contact_id}
+        arg = {"jobID": job_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def add_job_tracking_times_list(
-        self,
-        job_id: int,
-        project_type: Union[ProjectType, int],
-        job_tracking_time_list_in: Union[JobTrackingTimeListIN, dict],
+    def set_delivery_note(
+        self, project_type: Union[ProjectType, int], job_id: int, note: str
     ) -> Result:
         """
-        Add a JobTrackingTimeListIN to the specified job.
-        Please note that the tracking times will not be added if one of the following conditions is violated:
-
-        The overall completed percentage of a job must not exceed 100%.
-        A tracking time can only be added if the resource has access to the job.
-        The current (API) user must own the proper rights to set the tracking times (see Admin -> Rights -> Resources -> [API user] -> Time sheet).
-
-
-        If one of the conditions is violated for at least one tracking time, none of the tracking times will be added.
+        Method to set the delivery note for the specified job
 
 
-        :param job_id: int
         :param project_type: ProjectType
-        :param job_tracking_time_list_in: JobTrackingTimeListIN
+        :param job_id: int
+        :param note: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.addJobTrackingTimesList
+        proxy = self.__client.plunet_server.DataJob30.setDeliveryNote
         response_model = Result
 
-        if type(job_tracking_time_list_in) != JobTrackingTimeListIN:
-            job_tracking_time_list_in = JobTrackingTimeListIN(
-                **job_tracking_time_list_in
-            ).dict()
-        else:
-            job_tracking_time_list_in = job_tracking_time_list_in.dict()
-
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "jobID": job_id,
-            "projectType": project_type,
-            "JobTrackingTimeListIN": job_tracking_time_list_in,
-        }
+        arg = {"projectType": project_type, "jobID": job_id, "note": note}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_price_line_list_by_currency_type(
-        self,
-        job_id: int,
-        project_type: Union[ProjectType, int],
-        currency_type: Union[CurrencyType, int],
-    ) -> PriceLineListResult:
+    def get_job_number(
+        self, project_type: Union[ProjectType, int], job_id: int
+    ) -> StringResult:
         """
-        Returns a list of all job related PriceLine
-        The PriceLine will be returned in the specified CurrencyType (default: project currency).
+        Returns the job number, e.g. '001' for the job 'TRA-001'
 
 
-        :param job_id: int
         :param project_type: ProjectType
-        :param currency_type: CurrencyType
-        :return: PriceLineListResult
+        :param job_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getPriceLine_ListByCurrencyType
-        response_model = PriceLineListResult
+        proxy = self.__client.plunet_server.DataJob30.getJobNumber
+        response_model = StringResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        if type(currency_type) == CurrencyType:
-            currency_type = currency_type.value
-        elif type(currency_type) == int:
-            currency_type = currency_type
-        else:
-            currency_type = int(currency_type)
-
-        arg = {
-            "jobID": job_id,
-            "projectType": project_type,
-            "currencyType": currency_type,
-        }
+        arg = {"projectType": project_type, "jobID": job_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_download_url_source_data(
-        self, target_file_name: str, project_type: Union[ProjectType, int], job_id: int
+    def get_delivery_note(
+        self, project_type: Union[ProjectType, int], job_id: int
     ) -> StringResult:
         """
-        Returns an instance of StringResult containing an url
-        This can be used for downloading the source files as zip archive from
-        the specified job. The url is only available for the current api session.
-        Info:
-        For content based file up/download please use DataDocument30
+        Method to access the delivery note for the specified job
 
 
-        :param target_file_name: str
         :param project_type: ProjectType
         :param job_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getDownloadUrl_SourceData
+        proxy = self.__client.plunet_server.DataJob30.getDeliveryNote
         response_model = StringResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "targetFileName": target_file_name,
-            "projectType": project_type,
-            "jobID": job_id,
-        }
+        arg = {"projectType": project_type, "jobID": job_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def update_price_line(
-        self,
-        job_id: int,
-        project_type: Union[ProjectType, int],
-        price_line_in: Union[PriceLineIN, dict],
-    ) -> PriceLineResult:
+    def set_due_date(
+        self, project_type: Union[ProjectType, int], due_date: datetime, job_id: int
+    ) -> Result:
         """
-        Updates a existing PriceLine.
+        Method to set the due-date for the specified job.
 
 
-        :param job_id: int
         :param project_type: ProjectType
-        :param price_line_in: PriceLineIN
-        :return: PriceLineResult
+        :param due_date: datetime
+        :param job_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.updatePriceLine
-        response_model = PriceLineResult
-
-        if type(price_line_in) != PriceLineIN:
-            price_line_in = PriceLineIN(**price_line_in).dict()
-        else:
-            price_line_in = price_line_in.dict()
+        proxy = self.__client.plunet_server.DataJob30.setDueDate
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "jobID": job_id,
-            "projectType": project_type,
-            "priceLineIN": price_line_in,
-        }
+        arg = {"projectType": project_type, "dueDate": due_date, "jobID": job_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_action_link(
-        self,
-        project_type: Union[ProjectType, int],
-        job_id: int,
-        user_id: int,
-        action_link_type: int,
-    ) -> StringResult:
+    def set_job_status(
+        self, project_type: Union[ProjectType, int], job_id: int, status: int
+    ) -> Result:
         """
-        Method to obtain any kind of job related action link.
+        Method to set the status for the specified job.
 
 
         :param project_type: ProjectType
         :param job_id: int
-        :param user_id: int
-        :param action_link_type: int
-        :return: StringResult
+        :param status: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getActionLink
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataJob30.setJobStatus
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "projectType": project_type,
-            "jobID": job_id,
-            "userID": user_id,
-            "actionLinkType": action_link_type,
-        }
+        arg = {"projectType": project_type, "jobID": job_id, "status": status}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_pricelist(
+    def get_payable_id(
         self, job_id: int, project_type: Union[ProjectType, int]
-    ) -> PricelistResult:
+    ) -> IntegerResult:
         """
-        Returns the current selected Pricelist for the specified job
+        Returns the referenced payable ID
 
 
         :param job_id: int
         :param project_type: ProjectType
-        :return: PricelistResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getPricelist
-        response_model = PricelistResult
+        proxy = self.__client.plunet_server.DataJob30.getPayableID
+        response_model = IntegerResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
@@ -1297,192 +1240,219 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_pricelist(
-        self, job_id: int, project_type: Union[ProjectType, int], price_list_id: int
-    ) -> Result:
+    def get_resource_id(
+        self, project_type: Union[ProjectType, int], job_id: int
+    ) -> IntegerResult:
         """
-        SetÂ´s the selected Pricelist for the specified job
+        Returns an instance of IntegerResult, which contains the resource id
+        of the specified job.
 
 
-        :param job_id: int
         :param project_type: ProjectType
-        :param price_list_id: int
-        :return: Result
+        :param job_id: int
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.setPricelist
-        response_model = Result
+        proxy = self.__client.plunet_server.DataJob30.getResourceID
+        response_model = IntegerResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "jobID": job_id,
-            "projectType": project_type,
-            "priceListID": price_list_id,
-        }
+        arg = {"projectType": project_type, "jobID": job_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_services_list(self, language_code: str) -> StringArrayResult:
+    def get_pricelist_list(
+        self, job_id: int, project_type: Union[ProjectType, int]
+    ) -> PricelistListResult:
         """
-        Deprecated. Please use DataAdmin30.getAvailableServices(String, String) instead.
-        Returns a list of all avaliable services.
+        Returns all avaliable Pricelist for this job.
+        Note: This is dependent on the related project and the selected customer
 
 
-        :param language_code: str
-        :return: StringArrayResult
+        :param job_id: int
+        :param project_type: ProjectType
+        :return: PricelistListResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getServices_List
-        response_model = StringArrayResult
+        proxy = self.__client.plunet_server.DataJob30.getPricelist_List
+        response_model = PricelistListResult
+
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
+        else:
+            project_type = int(project_type)
+
+        arg = {"jobID": job_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=language_code,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_price_unit(self, price_unit_id: int, language_code: str) -> PriceUnitResult:
+    def get_pricelist_entry_list(
+        self, pricelist_id: int, source_language: str, target_language: str
+    ) -> PricelistEntryList:
         """
-        Returns a PriceUnitResult object.
-        Possible PriceUnitÂ´s can be obtained over DataItem30.getPriceUnit_List(java.lang.String, java.lang.String, java.lang.String)
+        Provides all price entries which are related to the Pricelist
+        regarding the transfered source and target language.
 
 
-        :param price_unit_id: int
-        :param language_code: str
-        :return: PriceUnitResult
+        :param pricelist_id: int
+        :param source_language: str
+        :param target_language: str
+        :return: PricelistEntryList
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getPriceUnit
-        response_model = PriceUnitResult
+        proxy = self.__client.plunet_server.DataJob30.getPricelistEntry_List
+        response_model = PricelistEntryList
 
-        arg = {"PriceUnitID": price_unit_id, "languageCode": language_code}
+        arg = {
+            "PricelistID": pricelist_id,
+            "SourceLanguage": source_language,
+            "TargetLanguage": target_language,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def insert_price_line(
-        self,
-        job_id: int,
-        project_type: Union[ProjectType, int],
-        price_line_in: Union[PriceLineIN, dict],
-        create_as_first_item: bool,
-    ) -> PriceLineResult:
+    def get_price_line_list(
+        self, job_id: int, project_type: Union[ProjectType, int]
+    ) -> PriceLineListResult:
         """
-        Inserts a new PriceLine to the specified job
-        Warning: Job-Price lines do not support the price-line memo value.
-        This value will be ignored by this specific implementation.
+        Returns a list of all job related PriceLine
 
 
         :param job_id: int
         :param project_type: ProjectType
-        :param price_line_in: PriceLineIN
-        :param create_as_first_item: bool
-        :return: PriceLineResult
+        :return: PriceLineListResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.insertPriceLine
-        response_model = PriceLineResult
-
-        if type(price_line_in) != PriceLineIN:
-            price_line_in = PriceLineIN(**price_line_in).dict()
-        else:
-            price_line_in = price_line_in.dict()
+        proxy = self.__client.plunet_server.DataJob30.getPriceLine_List
+        response_model = PriceLineListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "jobID": job_id,
-            "projectType": project_type,
-            "priceLineIN": price_line_in,
-            "createAsFirstItem": create_as_first_item,
-        }
+        arg = {"jobID": job_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def delete_price_line(
-        self, job_id: int, project_type: Union[ProjectType, int], price_line_id: int
-    ) -> Result:
+    def get_price_unit_list(
+        self, language_code: str, service: str
+    ) -> PriceUnitListResult:
         """
-        Deletes an existing PriceLine
+        Returns a list of priceUnit related to the specified service.
+        Possible services can be obtained over DataAdmin30.getAvailableServices(String, String)
 
 
-        :param job_id: int
+        :param language_code: str
+        :param service: str
+        :return: PriceUnitListResult
+        """
+
+        proxy = self.__client.plunet_server.DataJob30.getPriceUnit_List
+        response_model = PriceUnitListResult
+
+        arg = {"languageCode": language_code, "service": service}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def insert2(
+        self,
+        project_id: int,
+        project_type: Union[ProjectType, int],
+        job_type_abbrevation: str,
+        item_id: int,
+    ) -> IntegerResult:
+        """
+        Inserts a Job.
+
+
+        :param project_id: int
         :param project_type: ProjectType
-        :param price_line_id: int
-        :return: Result
+        :param job_type_abbrevation: str
+        :param item_id: int
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.deletePriceLine
-        response_model = Result
+        proxy = self.__client.plunet_server.DataJob30.insert2
+        response_model = IntegerResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
         arg = {
-            "jobID": job_id,
+            "projectID": project_id,
             "projectType": project_type,
-            "priceLineID": price_line_id,
+            "jobTypeAbbrevation": job_type_abbrevation,
+            "itemID": item_id,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_delivery_date(
+    def get_creation_date(
         self, project_type: Union[ProjectType, int], job_id: int
     ) -> DateResult:
         """
-        Returns an instance of DateResult representing the delivery
-        date of the job using the default time zone.
+        Returns an instance of IntegerResult containing the creation date of the job
 
 
         :param project_type: ProjectType
         :param job_id: int
         :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getDeliveryDate
+        proxy = self.__client.plunet_server.DataJob30.getCreationDate
         response_model = DateResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
@@ -1493,251 +1463,314 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_delivery_note(
-        self, project_type: Union[ProjectType, int], job_id: int, note: str
-    ) -> Result:
+    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
         """
-        Method to set the delivery note for the specified job
+        Deletes an registered notify request.
+        Info:Notify requests can only be deleted by the user who has created them
 
 
-        :param project_type: ProjectType
-        :param job_id: int
-        :param note: str
+        :param event_type: EventType
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.setDeliveryNote
+        proxy = self.__client.plunet_server.DataJob30.deregisterCallback_Notify
         response_model = Result
 
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
         else:
-            project_type = int(project_type)
-
-        arg = {"projectType": project_type, "jobID": job_id, "note": note}
+            event_type = int(event_type)
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=event_type,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_payable_id(
-        self, job_id: int, project_type: Union[ProjectType, int]
-    ) -> IntegerResult:
+    def register_callback_notify(
+        self,
+        server_authentication_string: str,
+        server_address: str,
+        event_type: Union[EventType, int],
+    ) -> Result:
         """
-        Returns the referenced payable ID
+        Register to get notified when the specified EventType occurs
+        for any job.
 
+        If the EventType occurs PBM will call the callback web service,
+        which is hosted within your environment.
 
-        :param job_id: int
-        :param project_type: ProjectType
-        :return: IntegerResult
+
+        Please check CallbackCustomer30 for the exact specification for
+        this service.
+
+
+        Info:Each user can only create one notifier per event
+
+
+        The  must match one of the following formats:
+
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
+
+        In the first two cases, the address will be autocompleted by appending
+        the corresponding directory "CallbackJob30?wsdl".
+
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
+
+
+        :param server_authentication_string: str
+        :param server_address: str
+        :param event_type: EventType
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getPayableID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataJob30.registerCallback_Notify
+        response_model = Result
 
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
         else:
-            project_type = int(project_type)
+            event_type = int(event_type)
 
-        arg = {"jobID": job_id, "projectType": project_type}
+        arg = {
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "EventType": event_type,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_job_number(
-        self, project_type: Union[ProjectType, int], job_id: int
-    ) -> StringResult:
+    def register_callback_observer(
+        self,
+        server_authentication_string: str,
+        server_address: str,
+        job_id: int,
+        project_type: Union[ProjectType, int],
+    ) -> Result:
         """
-        Returns the job number, e.g. '001' for the job 'TRA-001'
+        Register to observe a specific object for any supported
+        EventType.
+
+        As soon as any supported EventType occurs, PBM will call the
+        callback web service, which is hosted within your environment.
 
 
-        :param project_type: ProjectType
+        Please check CallbackCustomer30 for the exact specification for
+        this service.
+
+
+        Info:Each user can only create one observer per id
+
+
+        The  must match one of the following formats:
+
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
+
+        In the first two cases, the address will be autocompleted by appending
+        the corresponding directory "CallbackJob30?wsdl".
+
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
+
+
+        :param server_authentication_string: str
+        :param server_address: str
         :param job_id: int
-        :return: StringResult
+        :param project_type: ProjectType
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getJobNumber
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataJob30.registerCallback_Observer
+        response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "jobID": job_id}
+        arg = {
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "JobID": job_id,
+            "ProjectType": project_type,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def run_automatic_job(
+    def deregister_callback_observer(
         self, job_id: int, project_type: Union[ProjectType, int]
     ) -> Result:
         """
-        Start or restart an automatic job.
-
-        Please note that a job can only be started in its initial job status (as
-        defined in the admin settings). This does not apply for restarting jobs.
+        Deletes an observer.
+        Observer can only deleted by the user who has created them.
 
 
         :param job_id: int
         :param project_type: ProjectType
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.runAutomaticJob
+        proxy = self.__client.plunet_server.DataJob30.deregisterCallback_Observer
         response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"jobID": job_id, "projectType": project_type}
+        arg = {"JobID": job_id, "ProjectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def insert3(self, job_in: Union[JobIN, dict], job_type_short: str) -> IntegerResult:
+    def get_contact_person_id(
+        self, project_type: Union[ProjectType, int], job_id: int
+    ) -> IntegerResult:
         """
-        Inserts a new Job.
+        Returns an instance of IntegerResult containing the resource ID
+        of the jobs contact person.
+        Refers to the field Job -> "Contact person for job" in the Plunet BM.
 
 
-        :param job_in: JobIN
-        :param job_type_short: str
+        :param project_type: ProjectType
+        :param job_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.insert3
+        proxy = self.__client.plunet_server.DataJob30.getContactPersonID
         response_model = IntegerResult
 
-        if type(job_in) != JobIN:
-            job_in = JobIN(**job_in).dict()
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
         else:
-            job_in = job_in.dict()
+            project_type = int(project_type)
 
-        arg = {"JobIN": job_in, "JobTypeShort": job_type_short}
+        arg = {"projectType": project_type, "jobID": job_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def delete_job(self, job_id: int, project_type: Union[ProjectType, int]) -> Result:
+    def get_job_type_short_name(
+        self, project_type: Union[ProjectType, int], job_id: int
+    ) -> StringResult:
         """
-        Deletes a job.
+        Returns an instance of StringResult containing the abbreviated name (English)
+        of the job type for the specified job. â e.g. TRA.
 
 
-        :param job_id: int
         :param project_type: ProjectType
-        :return: Result
+        :param job_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.deleteJob
-        response_model = Result
+        proxy = self.__client.plunet_server.DataJob30.getJobType_ShortName
+        response_model = StringResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"jobID": job_id, "projectType": project_type}
+        arg = {"projectType": project_type, "jobID": job_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_price_liste_id(
-        self, project_type: Union[ProjectType, int], price_list_id: int, job_id: int
-    ) -> Result:
+    def get_item_independent_jobs(
+        self, project_type: Union[ProjectType, int], project_id: int
+    ) -> JobListResult:
         """
-        Deprecated. This call is deprecated and may be removed in future api versions.
-        Please use setPricelist(String, int, int, int) instead.
+        Returns an instance of JobListResult, which contains a list of all language
+        independent jobs .
 
 
         :param project_type: ProjectType
-        :param price_list_id: int
-        :param job_id: int
-        :return: Result
+        :param project_id: int
+        :return: JobListResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.setPriceListeID
-        response_model = Result
+        proxy = self.__client.plunet_server.DataJob30.getItemIndependentJobs
+        response_model = JobListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "projectType": project_type,
-            "priceListID": price_list_id,
-            "jobID": job_id,
-        }
+        arg = {"projectType": project_type, "projectId": project_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def assign_job(
+    def set_contact_person_id(
         self, project_type: Union[ProjectType, int], job_id: int, resource_id: int
     ) -> Result:
         """
-        Deprecated. This method is no longer supported. Please use the new Endpoint DataJobRound30 for resource assignment.
-        For further information, please refer to the release notes.
-        Assigns a job to a resource.
+        Method to set the resourceID of the contact-person for the specified job.
+        Refers to the field Job -> "Contact person for job" in the Plunet BM.
 
 
         :param project_type: ProjectType
         :param job_id: int
         :param resource_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.assignJob
+        proxy = self.__client.plunet_server.DataJob30.setContactPersonID
         response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
@@ -1748,156 +1781,144 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_start_date(
-        self, project_type: Union[ProjectType, int], start_date: datetime, job_id: int
-    ) -> Result:
+    def get_resource_contact_person_id(
+        self, project_type: Union[ProjectType, int], job_id: int
+    ) -> IntegerResult:
         """
-        Method to set the start-date for the specified job.
+        Returns an instance of IntegerResult containing the resource ID
+        of the contact person.
+        Refers to the field Job -> "Contact persons" in the Plunet BM.
 
 
         :param project_type: ProjectType
-        :param start_date: datetime
         :param job_id: int
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.setStartDate
-        response_model = Result
+        proxy = self.__client.plunet_server.DataJob30.getResourceContactPersonID
+        response_model = IntegerResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "startDate": start_date, "jobID": job_id}
+        arg = {"projectType": project_type, "jobID": job_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_due_date(
-        self, project_type: Union[ProjectType, int], due_date: datetime, job_id: int
+    def add_job_tracking_time(
+        self,
+        job_id: int,
+        project_type: Union[ProjectType, int],
+        job_tracking_time_in: Union[JobTrackingTimeIN, dict],
     ) -> Result:
         """
-        Method to set the due-date for the specified job.
+        Add a JobTrackingTimeIN to the specified job.
+        Please note that the tracking time will not be added if one of the following conditions is violated:
+
+        The overall completed percentage of a job must not exceed 100%.
+        A Tracking time can only be added if the resource has access to the job.
+        The current (API) user must own the proper rights to set the tracking times (see Admin -> Rights -> Resources -> [API user] -> Time sheet).
 
 
-        :param project_type: ProjectType
-        :param due_date: datetime
         :param job_id: int
+        :param project_type: ProjectType
+        :param job_tracking_time_in: JobTrackingTimeIN
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.setDueDate
+        proxy = self.__client.plunet_server.DataJob30.addJobTrackingTime
         response_model = Result
 
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
+        if type(job_tracking_time_in) != JobTrackingTimeIN:
+            job_tracking_time_in = JobTrackingTimeIN(**job_tracking_time_in).dict()
         else:
-            project_type = int(project_type)
-
-        arg = {"projectType": project_type, "dueDate": due_date, "jobID": job_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def get_job_for_view(
-        self, job_id: int, project_type: Union[ProjectType, int]
-    ) -> JobResult:
-        """
-        This method returns a single instance of job.
-        This method only returns a set of information about a job, e.g. to display
-        this information in your application.
-
-
-        :param job_id: int
-        :param project_type: ProjectType
-        :return: JobResult
-        """
-
-        proxy = self.__client.plunet_server.DataJob30.getJob_ForView
-        response_model = JobResult
+            job_tracking_time_in = job_tracking_time_in.dict()
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"jobID": job_id, "projectType": project_type}
+        arg = {
+            "jobID": job_id,
+            "projectType": project_type,
+            "JobTrackingTimeIN": job_tracking_time_in,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_job_status(
-        self, project_type: Union[ProjectType, int], job_id: int, status: int
+    def set_resource_contact_person_id(
+        self, project_type: Union[ProjectType, int], job_id: int, contact_id: int
     ) -> Result:
         """
-        Method to set the status for the specified job.
+        Method to set the resourceID of the contact-person.
+
+        Refers to the field Job -> "Contact persons" in the Plunet BM.
 
 
         :param project_type: ProjectType
         :param job_id: int
-        :param status: int
+        :param contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.setJobStatus
+        proxy = self.__client.plunet_server.DataJob30.setResourceContactPersonID
         response_model = Result
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "jobID": job_id, "status": status}
+        arg = {"projectType": project_type, "jobID": job_id, "contactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_delivery_note(
+    def get_job_type_long_name(
         self, project_type: Union[ProjectType, int], job_id: int
     ) -> StringResult:
         """
-        Method to access the delivery note for the specified job
+        Returns an instance of StringResult containing the full name (English)
+        of the job type for the specified job. â e.g. Translation.
 
 
         :param project_type: ProjectType
         :param job_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getDeliveryNote
+        proxy = self.__client.plunet_server.DataJob30.getJobType_LongName
         response_model = StringResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
@@ -1908,267 +1929,245 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_due_date(
-        self, project_type: Union[ProjectType, int], job_id: int
-    ) -> DateResult:
+    def add_job_tracking_times_list(
+        self,
+        job_id: int,
+        project_type: Union[ProjectType, int],
+        job_tracking_time_list_in: Union[JobTrackingTimeListIN, dict],
+    ) -> Result:
         """
-        Returns an instance of DateResult representing the due date of the job.
+        Add a JobTrackingTimeListIN to the specified job.
+        Please note that the tracking times will not be added if one of the following conditions is violated:
+
+        The overall completed percentage of a job must not exceed 100%.
+        A tracking time can only be added if the resource has access to the job.
+        The current (API) user must own the proper rights to set the tracking times (see Admin -> Rights -> Resources -> [API user] -> Time sheet).
+
+
+        If one of the conditions is violated for at least one tracking time, none of the tracking times will be added.
 
 
-        :param project_type: ProjectType
         :param job_id: int
-        :return: DateResult
+        :param project_type: ProjectType
+        :param job_tracking_time_list_in: JobTrackingTimeListIN
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getDueDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataJob30.addJobTrackingTimesList
+        response_model = Result
+
+        if type(job_tracking_time_list_in) != JobTrackingTimeListIN:
+            job_tracking_time_list_in = JobTrackingTimeListIN(
+                **job_tracking_time_list_in
+            ).dict()
+        else:
+            job_tracking_time_list_in = job_tracking_time_list_in.dict()
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "jobID": job_id}
+        arg = {
+            "jobID": job_id,
+            "projectType": project_type,
+            "JobTrackingTimeListIN": job_tracking_time_list_in,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_job_metrics(
-        self, job_id: int, project_type: Union[ProjectType, int], language_code: str
-    ) -> JobMetricResult:
+    def get_job_list_of_item_for_view(
+        self, item_id: int, project_type: Union[ProjectType, int]
+    ) -> JobListResult:
         """
-        Retrieves the job's total price and amounts.
+        Method returns an instance of JobListResult, containing a list of Job objects.
+        All available job for a specific itemID will be returned.
+        This method only returns a set of information about a set of jobs, e.g.
+        to display this information in your application.
 
 
-        :param job_id: int
+        :param item_id: int
         :param project_type: ProjectType
-        :param language_code: str
-        :return: JobMetricResult
+        :return: JobListResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getJobMetrics
-        response_model = JobMetricResult
+        proxy = self.__client.plunet_server.DataJob30.getJobListOfItem_ForView
+        response_model = JobListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "jobID": job_id,
-            "projectType": project_type,
-            "languageCode": language_code,
-        }
+        arg = {"itemID": item_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def insert2(
-        self,
-        project_id: int,
-        project_type: Union[ProjectType, int],
-        job_type_abbrevation: str,
-        item_id: int,
-    ) -> IntegerResult:
+    def get_job_tracking_times_list(
+        self, job_id: int, project_type: Union[ProjectType, int]
+    ) -> JobTrackingTimeResult:
         """
-        Inserts a Job.
+        Returns a list of all job tracking times.
 
 
-        :param project_id: int
+        :param job_id: int
         :param project_type: ProjectType
-        :param job_type_abbrevation: str
-        :param item_id: int
-        :return: IntegerResult
+        :return: JobTrackingTimeResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.insert2
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataJob30.getJobTrackingTimesList
+        response_model = JobTrackingTimeResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "projectID": project_id,
-            "projectType": project_type,
-            "jobTypeAbbrevation": job_type_abbrevation,
-            "itemID": item_id,
-        }
+        arg = {"jobID": job_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_resource_id(
-        self, project_type: Union[ProjectType, int], job_id: int
-    ) -> IntegerResult:
+    def get_price_line_list_by_currency_type(
+        self,
+        job_id: int,
+        project_type: Union[ProjectType, int],
+        currency_type: Union[CurrencyType, int],
+    ) -> PriceLineListResult:
         """
-        Returns an instance of IntegerResult, which contains the resource id
-        of the specified job.
+        Returns a list of all job related PriceLine
+        The PriceLine will be returned in the specified CurrencyType (default: project currency).
 
 
-        :param project_type: ProjectType
         :param job_id: int
-        :return: IntegerResult
+        :param project_type: ProjectType
+        :param currency_type: CurrencyType
+        :return: PriceLineListResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.getResourceID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataJob30.getPriceLine_ListByCurrencyType
+        response_model = PriceLineListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {"projectType": project_type, "jobID": job_id}
+        if type(currency_type) == CurrencyType:
+            currency_type = currency_type.value
+        elif type(currency_type) == int:
+            currency_type = currency_type
+        else:
+            currency_type = int(currency_type)
+
+        arg = {
+            "jobID": job_id,
+            "projectType": project_type,
+            "currencyType": currency_type,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_cat_report2(
-        self,
-        file_byte_stream: bytes,
-        file_path_name: str,
-        filesize: int,
-        cat_type: Union[CatType, int],
-        project_type: Union[ProjectType, int],
-        analyze_and_copy_result_to_job: bool,
-        job_id: int,
-    ) -> Result:
+    def get_download_url_source_data(
+        self, target_file_name: str, project_type: Union[ProjectType, int], job_id: int
+    ) -> StringResult:
         """
-        Uploads a report file into the report folder of the specified job.
-        Specify by value to copy the results of the report into the job and
-        if they should overwrite already existing price lines.
+        Returns an instance of StringResult containing an url
+        This can be used for downloading the source files as zip archive from
+        the specified job. The url is only available for the current api session.
+        Info:
+        For content based file up/download please use DataDocument30
 
 
-        :param file_byte_stream: bytes
-        :param file_path_name: str
-        :param filesize: int
-        :param cat_type: CatType
+        :param target_file_name: str
         :param project_type: ProjectType
-        :param analyze_and_copy_result_to_job: bool
         :param job_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.setCatReport2
-        response_model = Result
-
-        if type(cat_type) == CatType:
-            cat_type = cat_type.value
-        elif type(cat_type) == int:
-            cat_type = cat_type
-        else:
-            cat_type = int(cat_type)
+        proxy = self.__client.plunet_server.DataJob30.getDownloadUrl_SourceData
+        response_model = StringResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
         arg = {
-            "FileByteStream": file_byte_stream,
-            "FilePathName": file_path_name,
-            "Filesize": filesize,
-            "catType": cat_type,
+            "targetFileName": target_file_name,
             "projectType": project_type,
-            "analyzeAndCopyResultToJob": analyze_and_copy_result_to_job,
             "jobID": job_id,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_cat_report(
-        self,
-        path_or_url: str,
-        overwrite_existing_price_lines: bool,
-        cat_type: Union[CatType, int],
-        project_type: Union[ProjectType, int],
-        analyze_and_copy_result_to_job: bool,
-        job_id: int,
-    ) -> Result:
+    def get_job_list_for_view(
+        self, job_i_ds: str, project_type: Union[ProjectType, int]
+    ) -> JobListResult:
         """
-        Deprecated. Please use setCatReport2(String, byte[], String, int, int, int, boolean, int) instead.
-        Please note that this call is now deactivated by default. For Reactivation please contact Support@plunet.com.
-
-        Uploads a report file into the report folder of the specified job.
-        Specify by value to copy the results of the report into the job and
-        if they should overwrite already existing price lines.
+        Method returns an instance of JobListResult, containing a list of Job objects.
+        This method only returns a set of information about a set of jobs, e.g. to
+        display this information in your application.
 
 
-        :param path_or_url: str
-        :param overwrite_existing_price_lines: bool
-        :param cat_type: CatType
+        :param job_i_ds: str
         :param project_type: ProjectType
-        :param analyze_and_copy_result_to_job: bool
-        :param job_id: int
-        :return: Result
+        :return: JobListResult
         """
 
-        proxy = self.__client.plunet_server.DataJob30.setCatReport
-        response_model = Result
-
-        if type(cat_type) == CatType:
-            cat_type = cat_type.value
-        elif type(cat_type) == int:
-            cat_type = cat_type
-        else:
-            cat_type = int(cat_type)
+        proxy = self.__client.plunet_server.DataJob30.getJobList_ForView
+        response_model = JobListResult
 
         if type(project_type) == ProjectType:
             project_type = project_type.value
         elif type(project_type) == int:
             project_type = project_type
         else:
             project_type = int(project_type)
 
-        arg = {
-            "pathOrUrl": path_or_url,
-            "overwriteExistingPriceLines": overwrite_existing_price_lines,
-            "catType": cat_type,
-            "projectType": project_type,
-            "analyzeAndCopyResultToJob": analyze_and_copy_result_to_job,
-            "jobID": job_id,
-        }
+        arg = {"jobIDs": job_i_ds, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_job_round30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_job_round30.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,18 @@
     JobRoundSearchCriteriaIN,
     JobRoundSearchcriteriaResult,
     Result,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataJobRound30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
     def delete(self, round_id: int) -> Result:
         """
         Deletes a round.
 
         Note: You cannot remove all rounds from a job! One round always has to exist.
@@ -42,157 +41,203 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=round_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_ranking_methods(self, round_id: int) -> JobRoundRankingMethodListResult:
+    def assign_resource(
+        self, resource_id: int, resource_contact_id: int, round_id: int
+    ) -> Result:
         """
-        Returns the ranking methods set for a round.
+        Assigns the job to a resource.
+
+        The resource is assigned to the job. If a valid resourceContactId is submitted, the contact
+        person will be set instead. Please ensure the contactPersonId corresponds to the resourceId
+        submitted.
 
 
+        :param resource_id: int
+        :param resource_contact_id: int
         :param round_id: int
-        :return: JobRoundRankingMethodListResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJobRound30.getRankingMethods
-        response_model = JobRoundRankingMethodListResult
+        proxy = self.__client.plunet_server.DataJobRound30.assignResource
+        response_model = Result
+
+        arg = {
+            "resourceID": resource_id,
+            "resourceContactID": resource_contact_id,
+            "roundID": round_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=round_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_resources_for_round(self, round_id: int) -> IntegerArrayResult:
+    def add_round(
+        self,
+        job_id: int,
+        project_type: Union[ProjectType, int],
+        job_round_in: Union[JobRoundIN, dict],
+    ) -> IntegerResult:
         """
-        Returns the IDs of all resources matching the round criteria.
+        Adds a new round to the job.
 
+        Note: Inserting a job will already create a round for this job. You can only add additional
+        rounds if you either have the Vendor Search Manager PRO module enabled or no more active rounds
+        in the job.
 
-        :param round_id: int
-        :return: IntegerArrayResult
+
+        :param job_id: int
+        :param project_type: ProjectType
+        :param job_round_in: JobRoundIN
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataJobRound30.getResourcesForRound
-        response_model = IntegerArrayResult
+        proxy = self.__client.plunet_server.DataJobRound30.addRound
+        response_model = IntegerResult
+
+        if type(job_round_in) != JobRoundIN:
+            job_round_in = JobRoundIN(**job_round_in).dict()
+        else:
+            job_round_in = job_round_in.dict()
+
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
+        else:
+            project_type = int(project_type)
+
+        arg = {"jobID": job_id, "projectType": project_type, "jobRoundIN": job_round_in}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=round_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_resource_for_review(
-        self, resource_id: int, resource_contact_id: int, round_id: int
-    ) -> Result:
+    def get_all_round_i_ds(
+        self, job_id: int, project_type: Union[ProjectType, int]
+    ) -> IntegerArrayResult:
         """
-        Sets the resource of a job.
-
-        The resource is not confirmed yet, but awaits confirmation.
+        Returns all roundIDs corresponding to the job.
 
 
-        :param resource_id: int
-        :param resource_contact_id: int
-        :param round_id: int
-        :return: Result
+        :param job_id: int
+        :param project_type: ProjectType
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataJobRound30.setResourceForReview
-        response_model = Result
+        proxy = self.__client.plunet_server.DataJobRound30.getAllRoundIDs
+        response_model = IntegerArrayResult
 
-        arg = {
-            "resourceID": resource_id,
-            "resourceContactID": resource_contact_id,
-            "roundID": round_id,
-        }
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
+        else:
+            project_type = int(project_type)
+
+        arg = {"jobID": job_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def assign_resource_in_review(self, round_id: int) -> Result:
+    def update_round(self, round_in: Union[JobRoundIN, dict]) -> Result:
         """
-        Assigns the job to a preselected resource.
-
-        The resource in review is assigned to the job.
+        Updates a round.
 
 
-        :param round_id: int
+        :param round_in: JobRoundIN
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJobRound30.assignResource_InReview
+        proxy = self.__client.plunet_server.DataJobRound30.updateRound
         response_model = Result
 
+        if type(round_in) != JobRoundIN:
+            round_in = JobRoundIN(**round_in).dict()
+        else:
+            round_in = round_in.dict()
+
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=round_id,
+            argument=round_in,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_search_criteria(self, round_id: int) -> JobRoundSearchcriteriaResult:
+    def get_round_object(self, round_id: int) -> JobRoundResult:
         """
-        Returns the search criteria of a round.
+        Returns a job round object.
 
 
         :param round_id: int
-        :return: JobRoundSearchcriteriaResult
+        :return: JobRoundResult
         """
 
-        proxy = self.__client.plunet_server.DataJobRound30.getSearchCriteria
-        response_model = JobRoundSearchcriteriaResult
+        proxy = self.__client.plunet_server.DataJobRound30.getRoundObject
+        response_model = JobRoundResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=round_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_search_criteria(
-        self,
-        job_round_search_criteria_in: Union[JobRoundSearchCriteriaIN, dict],
-        round_id: int,
-    ) -> Result:
+    def assign_resource_in_review(self, round_id: int) -> Result:
         """
-        Sets the search criteria of a round.
+        Assigns the job to a preselected resource.
+
+        The resource in review is assigned to the job.
 
 
-        :param job_round_search_criteria_in: JobRoundSearchCriteriaIN
         :param round_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJobRound30.setSearchCriteria
+        proxy = self.__client.plunet_server.DataJobRound30.assignResource_InReview
         response_model = Result
 
-        if type(job_round_search_criteria_in) != JobRoundSearchCriteriaIN:
-            job_round_search_criteria_in = JobRoundSearchCriteriaIN(
-                **job_round_search_criteria_in
-            ).dict()
-        else:
-            job_round_search_criteria_in = job_round_search_criteria_in.dict()
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=round_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
 
-        arg = {
-            "JobRoundSearchCriteriaIN": job_round_search_criteria_in,
-            "roundID": round_id,
-        }
+    def get_ranking_methods(self, round_id: int) -> JobRoundRankingMethodListResult:
+        """
+        Returns the ranking methods set for a round.
+
+
+        :param round_id: int
+        :return: JobRoundRankingMethodListResult
+        """
+
+        proxy = self.__client.plunet_server.DataJobRound30.getRankingMethods
+        response_model = JobRoundRankingMethodListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=round_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
     def set_ranking_methods(
         self,
         job_round_ranking_method_list: Union[JobRoundRankingMethodList, dict],
         round_id: int,
     ) -> Result:
@@ -256,157 +301,111 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_round_object(self, round_id: int) -> JobRoundResult:
-        """
-        Returns a job round object.
-
-
-        :param round_id: int
-        :return: JobRoundResult
-        """
-
-        proxy = self.__client.plunet_server.DataJobRound30.getRoundObject
-        response_model = JobRoundResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=round_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def assign_resource(
-        self, resource_id: int, resource_contact_id: int, round_id: int
+    def set_search_criteria(
+        self,
+        job_round_search_criteria_in: Union[JobRoundSearchCriteriaIN, dict],
+        round_id: int,
     ) -> Result:
         """
-        Assigns the job to a resource.
-
-        The resource is assigned to the job. If a valid resourceContactId is submitted, the contact
-        person will be set instead. Please ensure the contactPersonId corresponds to the resourceId
-        submitted.
+        Sets the search criteria of a round.
 
 
-        :param resource_id: int
-        :param resource_contact_id: int
+        :param job_round_search_criteria_in: JobRoundSearchCriteriaIN
         :param round_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataJobRound30.assignResource
+        proxy = self.__client.plunet_server.DataJobRound30.setSearchCriteria
         response_model = Result
 
+        if type(job_round_search_criteria_in) != JobRoundSearchCriteriaIN:
+            job_round_search_criteria_in = JobRoundSearchCriteriaIN(
+                **job_round_search_criteria_in
+            ).dict()
+        else:
+            job_round_search_criteria_in = job_round_search_criteria_in.dict()
+
         arg = {
-            "resourceID": resource_id,
-            "resourceContactID": resource_contact_id,
+            "JobRoundSearchCriteriaIN": job_round_search_criteria_in,
             "roundID": round_id,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def update_round(self, round_in: Union[JobRoundIN, dict]) -> Result:
+    def get_resources_for_round(self, round_id: int) -> IntegerArrayResult:
         """
-        Updates a round.
+        Returns the IDs of all resources matching the round criteria.
 
 
-        :param round_in: JobRoundIN
-        :return: Result
+        :param round_id: int
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataJobRound30.updateRound
-        response_model = Result
-
-        if type(round_in) != JobRoundIN:
-            round_in = JobRoundIN(**round_in).dict()
-        else:
-            round_in = round_in.dict()
+        proxy = self.__client.plunet_server.DataJobRound30.getResourcesForRound
+        response_model = IntegerArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=round_in,
+            argument=round_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def add_round(
-        self,
-        job_id: int,
-        project_type: Union[ProjectType, int],
-        job_round_in: Union[JobRoundIN, dict],
-    ) -> IntegerResult:
+    def get_search_criteria(self, round_id: int) -> JobRoundSearchcriteriaResult:
         """
-        Adds a new round to the job.
-
-        Note: Inserting a job will already create a round for this job. You can only add additional
-        rounds if you either have the Vendor Search Manager PRO module enabled or no more active rounds
-        in the job.
+        Returns the search criteria of a round.
 
 
-        :param job_id: int
-        :param project_type: ProjectType
-        :param job_round_in: JobRoundIN
-        :return: IntegerResult
+        :param round_id: int
+        :return: JobRoundSearchcriteriaResult
         """
 
-        proxy = self.__client.plunet_server.DataJobRound30.addRound
-        response_model = IntegerResult
-
-        if type(job_round_in) != JobRoundIN:
-            job_round_in = JobRoundIN(**job_round_in).dict()
-        else:
-            job_round_in = job_round_in.dict()
-
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
-        else:
-            project_type = int(project_type)
-
-        arg = {"jobID": job_id, "projectType": project_type, "jobRoundIN": job_round_in}
+        proxy = self.__client.plunet_server.DataJobRound30.getSearchCriteria
+        response_model = JobRoundSearchcriteriaResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=round_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_all_round_i_ds(
-        self, job_id: int, project_type: Union[ProjectType, int]
-    ) -> IntegerArrayResult:
+    def set_resource_for_review(
+        self, resource_id: int, resource_contact_id: int, round_id: int
+    ) -> Result:
         """
-        Returns all roundIDs corresponding to the job.
+        Sets the resource of a job.
 
+        The resource is not confirmed yet, but awaits confirmation.
 
-        :param job_id: int
-        :param project_type: ProjectType
-        :return: IntegerArrayResult
-        """
 
-        proxy = self.__client.plunet_server.DataJobRound30.getAllRoundIDs
-        response_model = IntegerArrayResult
+        :param resource_id: int
+        :param resource_contact_id: int
+        :param round_id: int
+        :return: Result
+        """
 
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
-        else:
-            project_type = int(project_type)
+        proxy = self.__client.plunet_server.DataJobRound30.setResourceForReview
+        response_model = Result
 
-        arg = {"jobID": job_id, "projectType": project_type}
+        arg = {
+            "resourceID": resource_id,
+            "resourceContactID": resource_contact_id,
+            "roundID": round_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_order30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_order30.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,213 +20,328 @@
     StringArrayResult,
     StringResult,
     TemplateListResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataOrder30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
-    def add_language_combination(
-        self, source_language: str, target_language: str, order_id: int
-    ) -> IntegerResult:
+    def set_currency_and_rate(
+        self, order_id: int, currency_iso_code: str, rate: float
+    ) -> Result:
         """
-        Adds a language combination to the specified order.
-        All language descriptions were expected in English language or as ISO-Code.
-        Returns an instance of Result.
+        Method to change the currency and rate for the current project.
+        The rate refers to the default currency / domestic currency,
+        which is configured in the admin section of the Plunet BusinessManager.
+        Changing the currency / rate will cause a recalculation of item prices.
 
 
-        :param source_language: str
-        :param target_language: str
         :param order_id: int
-        :return: IntegerResult
+        :param currency_iso_code: str
+        :param rate: float
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.addLanguageCombination
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataOrder30.setCurrencyAndRate
+        response_model = Result
 
-        arg = {
-            "sourceLanguage": source_language,
-            "targetLanguage": target_language,
-            "orderID": order_id,
-        }
+        arg = {"orderID": order_id, "currencyIsoCode": currency_iso_code, "rate": rate}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_rate(self, order_id: int) -> DoubleResult:
+    def create_order_confirmation(
+        self, template: str, format_id: int, order_id: int
+    ) -> StringResult:
         """
-        Returns an instance of DoubleResult, which contains the rate.
+        Method creates the order confirmation as rtf-file and returns an instance of StringResult,
+        which contains the network path where the file is located.
+
+
+        :param template: str
+        :param format_id: int
+        :param order_id: int
+        :return: StringResult
+        """
+
+        proxy = self.__client.plunet_server.DataOrder30.createOrderConfirmation
+        response_model = StringResult
+
+        arg = {"template": template, "formatId": format_id, "orderID": order_id}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def set_en15038_requested(self, is_en15038: bool, order_id: int) -> Result:
+        """
+        Method to mark a project, that the clients wants the project to correspond to the EN 10538 standard.
 
 
+        :param is_en15038: bool
         :param order_id: int
-        :return: DoubleResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getRate
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataOrder30.setEN15038Requested
+        response_model = Result
+
+        arg = {"isEN15038": is_en15038, "orderID": order_id}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def get_order_no_for_view(self, order_id: int) -> StringResult:
+        """
+        Returns an instance of StringResult, which contains the formatted order number.
+
+
+        :param order_id: int
+        :return: StringResult
+        """
+
+        proxy = self.__client.plunet_server.DataOrder30.getOrderNo_for_View
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_request_id(self, order_id: int) -> IntegerResult:
+    def get_language_combination(self, order_id: int) -> StringArrayResult:
         """
-        Returns an instance of IntegerResult, which contains the requestId.
+        Returns an instance of StringArrayResult which contains a list.
 
 
         :param order_id: int
-        :return: IntegerResult
+        :return: StringArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getRequestId
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataOrder30.getLanguageCombination
+        response_model = StringArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_project_name(self, name: str, order_id: int) -> Result:
+    def get_documents_within_source_folder(self, order_id: int) -> StringArrayResult:
         """
-        Sets the project name for the currently selected project. Returns an instance of Result.
+        Deprecated. Please use DataDocument30.getFileList(String, int, int) with Folder Type = 6 instead
+        for compatibility reasons with DataDocument30.
+
+        Returns an instance of StringArrayResult, which contains a list
+        of network paths to source files.
+        Info: For content based file up/download please use DataDocument30
 
 
-        :param name: str
         :param order_id: int
-        :return: Result
+        :return: StringArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setProjectName
-        response_model = Result
-
-        arg = {"name": name, "orderID": order_id}
+        proxy = self.__client.plunet_server.DataOrder30.getDocuments_Within_SourceFolder
+        response_model = StringArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=order_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_subject(self, order_id: int) -> StringResult:
+    def get_delivery_comment(self, order_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the subject.
+        Method returns an instance of StringResult, which contains the delivery comment.
 
 
         :param order_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getSubject
+        proxy = self.__client.plunet_server.DataOrder30.getDeliveryComment
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_subject(self, subject: str, order_id: int) -> Result:
+    def get_projectmanager_id(self, order_id: int) -> IntegerResult:
         """
-        Sets the subject for the currently selected project.
+        Returns an instance of IntegerResult, which contains the resource id.
 
 
-        :param subject: str
         :param order_id: int
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setSubject
-        response_model = Result
+        proxy = self.__client.plunet_server.DataOrder30.getProjectmanagerID
+        response_model = IntegerResult
 
-        arg = {"subject": subject, "orderID": order_id}
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=order_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_order_object_list(
+        self, order_id_list: Union[IntegerList, dict]
+    ) -> OrderListResult:
+        """
+        Method returns an instance of OrderListResult, which contains a list of order objects.
+
+
+        :param order_id_list: IntegerList
+        :return: OrderListResult
+        """
+
+        proxy = self.__client.plunet_server.DataOrder30.getOrderObjectList
+        response_model = OrderListResult
+
+        if type(order_id_list) != IntegerList:
+            order_id_list = IntegerList(**order_id_list).dict()
+        else:
+            order_id_list = order_id_list.dict()
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=order_id_list,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_project_name(self, order_id: int) -> StringResult:
+    def get_en15038_requested(self, order_id: int) -> BooleanResult:
         """
-        Returns an instance of String Result, which contains the project name.
+        Method returns an instance of BooleanResult, which contains the information,
+        whether the client requests the EN15038 standard.
 
 
         :param order_id: int
-        :return: StringResult
+        :return: BooleanResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getProjectName
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataOrder30.getEN15038Requested
+        response_model = BooleanResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_request_id(self, order_id: int, request_id: int) -> Result:
+    def get_order_confirmations(self, order_id: int) -> StringArrayResult:
         """
-        Method to set the project related request ID.
+        Returns an instance of StringArrayResult, which contains a list of relative
+        network paths to all existing order confirmation documents.
+        Info: For content based file up/download please use DataDocument30
 
 
         :param order_id: int
-        :param request_id: int
-        :return: Result
+        :return: StringArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setRequestID
-        response_model = Result
+        proxy = self.__client.plunet_server.DataOrder30.getOrderConfirmations
+        response_model = StringArrayResult
 
-        arg = {"orderID": order_id, "requestID": request_id}
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=order_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_documents_within_final_folder(self, order_id: int) -> StringArrayResult:
+        """
+        Deprecated. Please use DataDocument30.getFileList(String, int, int) with Folder Type = 12 instead
+        for compatibility reasons with DataDocument30.
+
+        Returns an instance of StringArrayResult, which contains a list of network
+        paths to all documents located in the final folder.
+        Info: For content based file up/download please use DataDocument30
+
+
+        :param order_id: int
+        :return: StringArrayResult
+        """
+
+        proxy = self.__client.plunet_server.DataOrder30.getDocuments_Within_FinalFolder
+        response_model = StringArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=order_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_creation_date(self, order_id: int) -> DateResult:
+    def get_order_closing_date(self, order_id: int) -> DateResult:
         """
-        Returns an instance of DateResult, which contains the creation date.
+        Method returns an instance of DateResult, which contains the order closing date.
 
 
         :param order_id: int
         :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getCreationDate
+        proxy = self.__client.plunet_server.DataOrder30.getOrderClosingDate
         response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
+    def set_projectmanager_id(self, resource_id: int, order_id: int) -> Result:
+        """
+        Sets the resourceID of the project manager for defined order.
+
+
+        :param resource_id: int
+        :param order_id: int
+        :return: Result
+        """
+
+        proxy = self.__client.plunet_server.DataOrder30.setProjectmanagerID
+        response_model = Result
+
+        arg = {"resourceID": resource_id, "orderID": order_id}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
     def set_property(
         self, order_id: int, property_name_english: str, property_value_english: str
     ) -> Result:
         """
         Deprecated.
 
 
@@ -439,879 +554,720 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_reference_number(self, order_id: int, reference: str) -> Result:
+    def set_customer_id(self, customer_id: int, order_id: int) -> Result:
         """
-        Method set reference number for order by orderID.
+        Sets the customerID for the currently selected project.
 
 
+        :param customer_id: int
         :param order_id: int
-        :param reference: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setReferenceNumber
+        proxy = self.__client.plunet_server.DataOrder30.setCustomerID
         response_model = Result
 
-        arg = {"orderID": order_id, "reference": reference}
+        arg = {"customerID": customer_id, "orderID": order_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_project_category(
-        self, project_category: str, system_language_code: str, order_id: int
-    ) -> Result:
+    def get_order_object2(self, order_number: str) -> OrderResult:
         """
-        Set the the project category of the order, specified by its name.
-
-
-        For a full list of your project categories, see Admin | Miscellaneous |
-        Project category.
+        Method returns an instance of OrderResult, which contains an instance of Order.
 
 
-        :param project_category: str
-        :param system_language_code: str
-        :param order_id: int
-        :return: Result
+        :param order_number: str
+        :return: OrderResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setProjectCategory
-        response_model = Result
-
-        arg = {
-            "projectCategory": project_category,
-            "systemLanguageCode": system_language_code,
-            "orderID": order_id,
-        }
+        proxy = self.__client.plunet_server.DataOrder30.getOrderObject2
+        response_model = OrderResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=order_number,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_project_category(
-        self, system_language_code: str, order_id: int
-    ) -> StringResult:
+    def set_creation_date(self, creation_date: datetime, order_id: int) -> Result:
         """
-        Get the name (in the language specified) of the project category of
-        the order.
-
-        For a full list of your project categories, see Admin | Miscellaneous |
-        Project category.
+        Sets the creation date for the currently selected project.
 
 
-        :param system_language_code: str
+        :param creation_date: datetime
         :param order_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getProjectCategory
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataOrder30.setCreationDate
+        response_model = Result
 
-        arg = {"systemLanguageCode": system_language_code, "orderID": order_id}
+        arg = {"creationDate": creation_date, "orderID": order_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_customer_id(self, customer_id: int, order_id: int) -> Result:
+    def get_template_list(
+        self,
+    ) -> TemplateListResult:
         """
-        Sets the customerID for the currently selected project.
+        Method returns an instance of TemplateListResult, which contains a list
+        of template objects which can be accessed by the user.
 
 
-        :param customer_id: int
-        :param order_id: int
-        :return: Result
+        :return: TemplateListResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setCustomerID
-        response_model = Result
-
-        arg = {"customerID": customer_id, "orderID": order_id}
+        proxy = self.__client.plunet_server.DataOrder30.getTemplateList
+        response_model = TemplateListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=None,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def deregister_callback_observer(self, order_id: int) -> Result:
+    def get_order_date(self, order_id: int) -> DateResult:
         """
-        Deletes an observer.
-        (observer can only deleted by the user who has created them)
+        Get the order date.
 
 
         :param order_id: int
-        :return: Result
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.deregisterCallback_Observer
-        response_model = Result
+        proxy = self.__client.plunet_server.DataOrder30.getOrderDate
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def register_callback_notify(
-        self,
-        server_authentication_string: str,
-        server_address: str,
-        event_type: Union[EventType, int],
-    ) -> Result:
+    def set_project_status(self, order_id: int, project_status: int) -> Result:
         """
-        Register to get notified when the specified EventType occurs
-        for any order.
-
-        If the EventType occurs PBM will call the callback web service,
-        which is hosted within your environment. Please check
-        CallbackOrder30 for the exact specification for this service.
-        (each user can only create one notifier per event)
-
-
-        The  must match one of the following formats:
-
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
-
-        In the first two cases, the address will be autocompleted by appending
-        the corresponding directory "CallbackOrder30?wsdl".
-
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+        Method allows to set the ArchivStatus to ARCHIVED(3).
+        Other status changes are not supported due to underlying automated workflows.
+        Please note that the current status must be either COMPLETED(6) or COMPLETED_ARCHIVABLE(2).
 
 
-        :param server_authentication_string: str
-        :param server_address: str
-        :param event_type: EventType
+        :param order_id: int
+        :param project_status: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.registerCallback_Notify
+        proxy = self.__client.plunet_server.DataOrder30.setProjectStatus
         response_model = Result
 
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
-        else:
-            event_type = int(event_type)
-
-        arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "EventType": event_type,
-        }
+        arg = {"orderID": order_id, "projectStatus": project_status}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
+    def set_order_date(self, order_date: datetime, order_id: int) -> Result:
         """
-        Deletes an registered notify request.
-        Notify requests can only be deleted by the user who has created them
+        Set the order date.
 
 
-        :param event_type: EventType
+        :param order_date: datetime
+        :param order_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.deregisterCallback_Notify
+        proxy = self.__client.plunet_server.DataOrder30.setOrderDate
         response_model = Result
 
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
-        else:
-            event_type = int(event_type)
+        arg = {"orderDate": order_date, "orderID": order_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=event_type,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def register_callback_observer(
-        self, server_authentication_string: str, server_address: str, order_id: int
-    ) -> Result:
+    def get_project_status(self, order_id: int) -> IntegerResult:
         """
-        Register to observe a specific object for any supported
-        EventType.
-
-        As soon as any supported event occurs, PBM will call the callback web
-        service, which is hosted within your environment. Please check
-        CallbackOrder30 for the exact specification for this service.
-        (each user can only create one observer per id)
-
-
-        The  must match one of the following formats:
-
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
-
-        In the first two cases, the address will be autocompleted by appending
-        the corresponding directory "CallbackOrder30?wsdl".
-
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+        Returns an instance of IntegerResult, which contains the ArchivStatus.
 
 
-        :param server_authentication_string: str
-        :param server_address: str
         :param order_id: int
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.registerCallback_Observer
-        response_model = Result
-
-        arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "OrderID": order_id,
-        }
+        proxy = self.__client.plunet_server.DataOrder30.getProjectStatus
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=order_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def insert_by_template(
-        self, order_in: Union[OrderIN, dict], template_id: int
-    ) -> IntegerResult:
+    def get_links(
+        self, order_id: int, project_type: Union[ProjectType, int]
+    ) -> LinkListResult:
         """
-        Method to create a order depending on the transfered templateID and OrderIN object.
-        (object values will overwrite information set by the template)
-        #setOrderID(int) will be ignored as it
-        will be auto generated by the system.
+        Outputs all incoming and outgoing links for an order.
 
 
-        :param order_in: OrderIN
-        :param template_id: int
-        :return: IntegerResult
+        :param order_id: int
+        :param project_type: ProjectType
+        :return: LinkListResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.insert_byTemplate
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataOrder30.getLinks
+        response_model = LinkListResult
 
-        if type(order_in) != OrderIN:
-            order_in = OrderIN(**order_in).dict()
+        if type(project_type) == ProjectType:
+            project_type = project_type.value
+        elif type(project_type) == int:
+            project_type = project_type
         else:
-            order_in = order_in.dict()
+            project_type = int(project_type)
 
-        arg = {"OrderIN": order_in, "TemplateID": template_id}
+        arg = {"orderId": order_id, "projectType": project_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_reference_number(self, order_id: int) -> StringResult:
+    def get_action_link(
+        self, order_id: int, user_id: int, action_link_type: int
+    ) -> StringResult:
         """
-        Method returns the reference number by order ID.
+        Method to obtain any kind of order related action link.
 
 
         :param order_id: int
+        :param user_id: int
+        :param action_link_type: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getReferenceNumber
+        proxy = self.__client.plunet_server.DataOrder30.getActionLink
         response_model = StringResult
 
+        arg = {
+            "orderID": order_id,
+            "userID": user_id,
+            "actionLinkType": action_link_type,
+        }
+
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=order_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_project_manager_memo(self, order_id: int) -> StringResult:
+    def get_customer_id(self, order_id: int) -> IntegerResult:
         """
-        Method returns project-manager memo for order by orderID.
+        Returns an instance of IntegerResult, which contains the customer id.
 
 
         :param order_id: int
-        :return: StringResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getProjectManagerMemo
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataOrder30.getCustomerID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_master_project_id(self, order_id: int) -> IntegerResult:
+    def get_order_id(self, display_no: str) -> IntegerResult:
         """
-        Method to get the MasterProjectID of the specified order.
+        Method returns an instance of IntegerResult, which contains an order ID.
 
 
-        :param order_id: int
+        :param display_no: str
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getMasterProjectID
+        proxy = self.__client.plunet_server.DataOrder30.getOrderID
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=order_id,
+            argument=display_no,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_master_project_id(self, order_id: int, master_project_id: int) -> Result:
+    def set_reference_number(self, order_id: int, reference: str) -> Result:
         """
-        Method to set the MasterProjectID of the specified order.
+        Method set reference number for order by orderID.
 
 
         :param order_id: int
-        :param master_project_id: int
+        :param reference: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setMasterProjectID
+        proxy = self.__client.plunet_server.DataOrder30.setReferenceNumber
         response_model = Result
 
-        arg = {"orderID": order_id, "MasterProjectID": master_project_id}
+        arg = {"orderID": order_id, "reference": reference}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_project_manager_memo(self, order_id: int, memo: str) -> Result:
-        """
-        Method set the project-manager Memo for order by orderID.
-
-
-        :param order_id: int
-        :param memo: str
-        :return: Result
+    def set_project_category(
+        self, project_category: str, system_language_code: str, order_id: int
+    ) -> Result:
         """
+        Set the the project category of the order, specified by its name.
 
-        proxy = self.__client.plunet_server.DataOrder30.setProjectManagerMemo
-        response_model = Result
-
-        arg = {"orderID": order_id, "memo": memo}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
 
-    def set_delivery_deadline(
-        self, delivery_deadline: datetime, order_id: int
-    ) -> Result:
-        """
-        Sets the delivery deadline for the currently selected project.
+        For a full list of your project categories, see Admin | Miscellaneous |
+        Project category.
 
 
-        :param delivery_deadline: datetime
+        :param project_category: str
+        :param system_language_code: str
         :param order_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setDeliveryDeadline
+        proxy = self.__client.plunet_server.DataOrder30.setProjectCategory
         response_model = Result
 
-        arg = {"deliveryDeadline": delivery_deadline, "orderID": order_id}
+        arg = {
+            "projectCategory": project_category,
+            "systemLanguageCode": system_language_code,
+            "orderID": order_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_delivery_deadline(self, order_id: int) -> DateResult:
-        """
-        Returns an instance of DateResult, which contains the delivery deadline.
-
-
-        :param order_id: int
-        :return: DateResult
+    def get_project_category(
+        self, system_language_code: str, order_id: int
+    ) -> StringResult:
         """
+        Get the name (in the language specified) of the project category of
+        the order.
 
-        proxy = self.__client.plunet_server.DataOrder30.getDeliveryDeadline
-        response_model = DateResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=order_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def get_order_confirmations(self, order_id: int) -> StringArrayResult:
-        """
-        Returns an instance of StringArrayResult, which contains a list of relative
-        network paths to all existing order confirmation documents.
-        Info: For content based file up/download please use DataDocument30
+        For a full list of your project categories, see Admin | Miscellaneous |
+        Project category.
 
 
+        :param system_language_code: str
         :param order_id: int
-        :return: StringArrayResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getOrderConfirmations
-        response_model = StringArrayResult
+        proxy = self.__client.plunet_server.DataOrder30.getProjectCategory
+        response_model = StringResult
+
+        arg = {"systemLanguageCode": system_language_code, "orderID": order_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=order_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_en15038_requested(self, is_en15038: bool, order_id: int) -> Result:
+    def set_master_project_id(self, order_id: int, master_project_id: int) -> Result:
         """
-        Method to mark a project, that the clients wants the project to correspond to the EN 10538 standard.
+        Method to set the MasterProjectID of the specified order.
 
 
-        :param is_en15038: bool
         :param order_id: int
+        :param master_project_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setEN15038Requested
+        proxy = self.__client.plunet_server.DataOrder30.setMasterProjectID
         response_model = Result
 
-        arg = {"isEN15038": is_en15038, "orderID": order_id}
+        arg = {"orderID": order_id, "MasterProjectID": master_project_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_language_combination(self, order_id: int) -> StringArrayResult:
+    def insert_by_template(
+        self, order_in: Union[OrderIN, dict], template_id: int
+    ) -> IntegerResult:
         """
-        Returns an instance of StringArrayResult which contains a list.
+        Method to create a order depending on the transfered templateID and OrderIN object.
+        (object values will overwrite information set by the template)
+        #setOrderID(int) will be ignored as it
+        will be auto generated by the system.
 
 
-        :param order_id: int
-        :return: StringArrayResult
+        :param order_in: OrderIN
+        :param template_id: int
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getLanguageCombination
-        response_model = StringArrayResult
+        proxy = self.__client.plunet_server.DataOrder30.insert_byTemplate
+        response_model = IntegerResult
+
+        if type(order_in) != OrderIN:
+            order_in = OrderIN(**order_in).dict()
+        else:
+            order_in = order_in.dict()
+
+        arg = {"OrderIN": order_in, "TemplateID": template_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=order_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_delivery_comment(self, order_id: int) -> StringResult:
+    def get_project_manager_memo(self, order_id: int) -> StringResult:
         """
-        Method returns an instance of StringResult, which contains the delivery comment.
+        Method returns project-manager memo for order by orderID.
 
 
         :param order_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getDeliveryComment
+        proxy = self.__client.plunet_server.DataOrder30.getProjectManagerMemo
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_order_object_list(
-        self, order_id_list: Union[IntegerList, dict]
-    ) -> OrderListResult:
+    def set_project_manager_memo(self, order_id: int, memo: str) -> Result:
         """
-        Method returns an instance of OrderListResult, which contains a list of order objects.
+        Method set the project-manager Memo for order by orderID.
 
 
-        :param order_id_list: IntegerList
-        :return: OrderListResult
+        :param order_id: int
+        :param memo: str
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getOrderObjectList
-        response_model = OrderListResult
+        proxy = self.__client.plunet_server.DataOrder30.setProjectManagerMemo
+        response_model = Result
 
-        if type(order_id_list) != IntegerList:
-            order_id_list = IntegerList(**order_id_list).dict()
-        else:
-            order_id_list = order_id_list.dict()
+        arg = {"orderID": order_id, "memo": memo}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=order_id_list,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_projectmanager_id(self, order_id: int) -> IntegerResult:
+    def get_reference_number(self, order_id: int) -> StringResult:
         """
-        Returns an instance of IntegerResult, which contains the resource id.
+        Method returns the reference number by order ID.
 
 
         :param order_id: int
-        :return: IntegerResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getProjectmanagerID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataOrder30.getReferenceNumber
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_order_closing_date(self, order_id: int) -> DateResult:
+    def get_master_project_id(self, order_id: int) -> IntegerResult:
         """
-        Method returns an instance of DateResult, which contains the order closing date.
+        Method to get the MasterProjectID of the specified order.
 
 
         :param order_id: int
-        :return: DateResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getOrderClosingDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataOrder30.getMasterProjectID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_projectmanager_id(self, resource_id: int, order_id: int) -> Result:
+    def set_external_id(self, order_id: int, external_id: str) -> Result:
         """
-        Sets the resourceID of the project manager for defined order.
+        Method set ExternalID of Order by orderID
 
 
-        :param resource_id: int
         :param order_id: int
+        :param external_id: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setProjectmanagerID
+        proxy = self.__client.plunet_server.DataOrder30.setExternalID
         response_model = Result
 
-        arg = {"resourceID": resource_id, "orderID": order_id}
+        arg = {"orderID": order_id, "externalID": external_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_en15038_requested(self, order_id: int) -> BooleanResult:
+    def insert2(self, order_in: Union[OrderIN, dict]) -> IntegerResult:
         """
-        Method returns an instance of BooleanResult, which contains the information,
-        whether the client requests the EN15038 standard.
+        Method to create a order depending on the transfered object.
 
 
-        :param order_id: int
-        :return: BooleanResult
+        :param order_in: OrderIN
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getEN15038Requested
-        response_model = BooleanResult
+        proxy = self.__client.plunet_server.DataOrder30.insert2
+        response_model = IntegerResult
+
+        if type(order_in) != OrderIN:
+            order_in = OrderIN(**order_in).dict()
+        else:
+            order_in = order_in.dict()
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=order_id,
+            argument=order_in,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_order_object(self, order_id: int) -> OrderResult:
+    def get_external_id(self, order_id: int) -> StringResult:
         """
-        Method returns an instance of OrderResult, which contains an instance of Order.
+        Method returns the ExternalID by orderID
 
 
         :param order_id: int
-        :return: OrderResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getOrderObject
-        response_model = OrderResult
+        proxy = self.__client.plunet_server.DataOrder30.getExternalID
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_order_object2(self, order_number: str) -> OrderResult:
-        """
-        Method returns an instance of OrderResult, which contains an instance of Order.
-
-
-        :param order_number: str
-        :return: OrderResult
-        """
-
-        proxy = self.__client.plunet_server.DataOrder30.getOrderObject2
-        response_model = OrderResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=order_number,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def get_template_list(
-        self,
-    ) -> TemplateListResult:
+    def get_request_id(self, order_id: int) -> IntegerResult:
         """
-        Method returns an instance of TemplateListResult, which contains a list
-        of template objects which can be accessed by the user.
+        Returns an instance of IntegerResult, which contains the requestId.
 
 
-        :return: TemplateListResult
+        :param order_id: int
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getTemplateList
-        response_model = TemplateListResult
+        proxy = self.__client.plunet_server.DataOrder30.getRequestId
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=None,
+            argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_customer_contact_id(
-        self, customer_contact_id: int, order_id: int
-    ) -> Result:
+    def set_request_id(self, order_id: int, request_id: int) -> Result:
         """
-        Sets the customer contact ID for the currently selected project.
+        Method to set the project related request ID.
 
 
-        :param customer_contact_id: int
         :param order_id: int
+        :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setCustomerContactID
+        proxy = self.__client.plunet_server.DataOrder30.setRequestID
         response_model = Result
 
-        arg = {"customerContactID": customer_contact_id, "orderID": order_id}
+        arg = {"orderID": order_id, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_customer_contact_id(self, order_id: int) -> IntegerResult:
-        """
-        Returns an instance of IntegerResult, which contains the customer contact id.
-
-
-        :param order_id: int
-        :return: IntegerResult
-        """
-
-        proxy = self.__client.plunet_server.DataOrder30.getCustomerContactID
-        response_model = IntegerResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=order_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def set_project_status(self, order_id: int, project_status: int) -> Result:
+    def set_project_name(self, name: str, order_id: int) -> Result:
         """
-        Method allows to set the ArchivStatus to ARCHIVED(3).
-        Other status changes are not supported due to underlying automated workflows.
-        Please note that the current status must be either COMPLETED(6) or COMPLETED_ARCHIVABLE(2).
+        Sets the project name for the currently selected project. Returns an instance of Result.
 
 
+        :param name: str
         :param order_id: int
-        :param project_status: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setProjectStatus
+        proxy = self.__client.plunet_server.DataOrder30.setProjectName
         response_model = Result
 
-        arg = {"orderID": order_id, "projectStatus": project_status}
+        arg = {"name": name, "orderID": order_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_project_status(self, order_id: int) -> IntegerResult:
+    def get_project_name(self, order_id: int) -> StringResult:
         """
-        Returns an instance of IntegerResult, which contains the ArchivStatus.
+        Returns an instance of String Result, which contains the project name.
 
 
         :param order_id: int
-        :return: IntegerResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getProjectStatus
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataOrder30.getProjectName
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_action_link(
-        self, order_id: int, user_id: int, action_link_type: int
-    ) -> StringResult:
+    def get_subject(self, order_id: int) -> StringResult:
         """
-        Method to obtain any kind of order related action link.
+        Returns an instance of StringResult, which contains the subject.
 
 
         :param order_id: int
-        :param user_id: int
-        :param action_link_type: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getActionLink
+        proxy = self.__client.plunet_server.DataOrder30.getSubject
         response_model = StringResult
 
-        arg = {
-            "orderID": order_id,
-            "userID": user_id,
-            "actionLinkType": action_link_type,
-        }
-
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=order_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_links(
-        self, order_id: int, project_type: Union[ProjectType, int]
-    ) -> LinkListResult:
+    def set_subject(self, subject: str, order_id: int) -> Result:
         """
-        Outputs all incoming and outgoing links for an order.
+        Sets the subject for the currently selected project.
 
 
+        :param subject: str
         :param order_id: int
-        :param project_type: ProjectType
-        :return: LinkListResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getLinks
-        response_model = LinkListResult
-
-        if type(project_type) == ProjectType:
-            project_type = project_type.value
-        elif type(project_type) == int:
-            project_type = project_type
-        else:
-            project_type = int(project_type)
+        proxy = self.__client.plunet_server.DataOrder30.setSubject
+        response_model = Result
 
-        arg = {"orderId": order_id, "projectType": project_type}
+        arg = {"subject": subject, "orderID": order_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_order_date(self, order_id: int) -> DateResult:
+    def get_creation_date(self, order_id: int) -> DateResult:
         """
-        Get the order date.
+        Returns an instance of DateResult, which contains the creation date.
 
 
         :param order_id: int
         :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getOrderDate
+        proxy = self.__client.plunet_server.DataOrder30.getCreationDate
         response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_order_date(self, order_date: datetime, order_id: int) -> Result:
+    def get_order_object(self, order_id: int) -> OrderResult:
         """
-        Set the order date.
+        Method returns an instance of OrderResult, which contains an instance of Order.
 
 
-        :param order_date: datetime
         :param order_id: int
-        :return: Result
+        :return: OrderResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setOrderDate
-        response_model = Result
-
-        arg = {"orderDate": order_date, "orderID": order_id}
+        proxy = self.__client.plunet_server.DataOrder30.getOrderObject
+        response_model = OrderResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=order_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
     def check_en15038(self, order_id: int) -> BooleanResult:
         """
         Method returns an instance of BooleanResult, which contains the information,
         whether a project corresponds the EN15038 standard or not.
 
@@ -1326,265 +1282,311 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_creation_date(self, creation_date: datetime, order_id: int) -> Result:
+    def get_rate(self, order_id: int) -> DoubleResult:
         """
-        Sets the creation date for the currently selected project.
+        Returns an instance of DoubleResult, which contains the rate.
 
 
-        :param creation_date: datetime
         :param order_id: int
-        :return: Result
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setCreationDate
-        response_model = Result
-
-        arg = {"creationDate": creation_date, "orderID": order_id}
+        proxy = self.__client.plunet_server.DataOrder30.getRate
+        response_model = DoubleResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=order_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_order_no_for_view(self, order_id: int) -> StringResult:
+    def get_item_status(
+        self, source_language: str, target_language: str, order_id: int
+    ) -> IntegerResult:
         """
-        Returns an instance of StringResult, which contains the formatted order number.
+        Method returns the status of a project item associated to a specific language combination.
 
 
+        :param source_language: str
+        :param target_language: str
         :param order_id: int
-        :return: StringResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getOrderNo_for_View
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataOrder30.getItemStatus
+        response_model = IntegerResult
+
+        arg = {
+            "sourceLanguage": source_language,
+            "targetLanguage": target_language,
+            "orderID": order_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=order_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_currency_and_rate(
-        self, order_id: int, currency_iso_code: str, rate: float
+    def set_customer_contact_id(
+        self, customer_contact_id: int, order_id: int
     ) -> Result:
         """
-        Method to change the currency and rate for the current project.
-        The rate refers to the default currency / domestic currency,
-        which is configured in the admin section of the Plunet BusinessManager.
-        Changing the currency / rate will cause a recalculation of item prices.
+        Sets the customer contact ID for the currently selected project.
 
 
+        :param customer_contact_id: int
         :param order_id: int
-        :param currency_iso_code: str
-        :param rate: float
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setCurrencyAndRate
+        proxy = self.__client.plunet_server.DataOrder30.setCustomerContactID
         response_model = Result
 
-        arg = {"orderID": order_id, "currencyIsoCode": currency_iso_code, "rate": rate}
+        arg = {"customerContactID": customer_contact_id, "orderID": order_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_documents_within_source_folder(self, order_id: int) -> StringArrayResult:
+    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
         """
-        Deprecated. Please use DataDocument30.getFileList(String, int, int) with Folder Type = 6 instead
-        for compatibility reasons with DataDocument30.
-
-        Returns an instance of StringArrayResult, which contains a list
-        of network paths to source files.
-        Info: For content based file up/download please use DataDocument30
+        Deletes an registered notify request.
+        Notify requests can only be deleted by the user who has created them
 
 
-        :param order_id: int
-        :return: StringArrayResult
+        :param event_type: EventType
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getDocuments_Within_SourceFolder
-        response_model = StringArrayResult
+        proxy = self.__client.plunet_server.DataOrder30.deregisterCallback_Notify
+        response_model = Result
+
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
+        else:
+            event_type = int(event_type)
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=order_id,
+            argument=event_type,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_documents_within_final_folder(self, order_id: int) -> StringArrayResult:
+    def register_callback_notify(
+        self,
+        server_authentication_string: str,
+        server_address: str,
+        event_type: Union[EventType, int],
+    ) -> Result:
         """
-        Deprecated. Please use DataDocument30.getFileList(String, int, int) with Folder Type = 12 instead
-        for compatibility reasons with DataDocument30.
+        Register to get notified when the specified EventType occurs
+        for any order.
 
-        Returns an instance of StringArrayResult, which contains a list of network
-        paths to all documents located in the final folder.
-        Info: For content based file up/download please use DataDocument30
+        If the EventType occurs PBM will call the callback web service,
+        which is hosted within your environment. Please check
+        CallbackOrder30 for the exact specification for this service.
+        (each user can only create one notifier per event)
 
 
-        :param order_id: int
-        :return: StringArrayResult
-        """
+        The  must match one of the following formats:
 
-        proxy = self.__client.plunet_server.DataOrder30.getDocuments_Within_FinalFolder
-        response_model = StringArrayResult
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
 
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=order_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
+        In the first two cases, the address will be autocompleted by appending
+        the corresponding directory "CallbackOrder30?wsdl".
 
-    def create_order_confirmation(
-        self, template: str, format_id: int, order_id: int
-    ) -> StringResult:
-        """
-        Method creates the order confirmation as rtf-file and returns an instance of StringResult,
-        which contains the network path where the file is located.
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
 
 
-        :param template: str
-        :param format_id: int
-        :param order_id: int
-        :return: StringResult
+        :param server_authentication_string: str
+        :param server_address: str
+        :param event_type: EventType
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.createOrderConfirmation
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataOrder30.registerCallback_Notify
+        response_model = Result
 
-        arg = {"template": template, "formatId": format_id, "orderID": order_id}
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
+        else:
+            event_type = int(event_type)
+
+        arg = {
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "EventType": event_type,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def insert2(self, order_in: Union[OrderIN, dict]) -> IntegerResult:
+    def register_callback_observer(
+        self, server_authentication_string: str, server_address: str, order_id: int
+    ) -> Result:
         """
-        Method to create a order depending on the transfered object.
+        Register to observe a specific object for any supported
+        EventType.
 
+        As soon as any supported event occurs, PBM will call the callback web
+        service, which is hosted within your environment. Please check
+        CallbackOrder30 for the exact specification for this service.
+        (each user can only create one observer per id)
 
-        :param order_in: OrderIN
-        :return: IntegerResult
+
+        The  must match one of the following formats:
+
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
+
+        In the first two cases, the address will be autocompleted by appending
+        the corresponding directory "CallbackOrder30?wsdl".
+
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
+
+
+        :param server_authentication_string: str
+        :param server_address: str
+        :param order_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.insert2
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataOrder30.registerCallback_Observer
+        response_model = Result
 
-        if type(order_in) != OrderIN:
-            order_in = OrderIN(**order_in).dict()
-        else:
-            order_in = order_in.dict()
+        arg = {
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "OrderID": order_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=order_in,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_external_id(self, order_id: int, external_id: str) -> Result:
+    def deregister_callback_observer(self, order_id: int) -> Result:
         """
-        Method set ExternalID of Order by orderID
+        Deletes an observer.
+        (observer can only deleted by the user who has created them)
 
 
         :param order_id: int
-        :param external_id: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.setExternalID
+        proxy = self.__client.plunet_server.DataOrder30.deregisterCallback_Observer
         response_model = Result
 
-        arg = {"orderID": order_id, "externalID": external_id}
-
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=order_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_external_id(self, order_id: int) -> StringResult:
+    def get_delivery_deadline(self, order_id: int) -> DateResult:
         """
-        Method returns the ExternalID by orderID
+        Returns an instance of DateResult, which contains the delivery deadline.
 
 
         :param order_id: int
-        :return: StringResult
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getExternalID
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataOrder30.getDeliveryDeadline
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_order_id(self, display_no: str) -> IntegerResult:
+    def set_delivery_deadline(
+        self, delivery_deadline: datetime, order_id: int
+    ) -> Result:
         """
-        Method returns an instance of IntegerResult, which contains an order ID.
+        Sets the delivery deadline for the currently selected project.
 
 
-        :param display_no: str
-        :return: IntegerResult
+        :param delivery_deadline: datetime
+        :param order_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getOrderID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataOrder30.setDeliveryDeadline
+        response_model = Result
+
+        arg = {"deliveryDeadline": delivery_deadline, "orderID": order_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=display_no,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_documents_within_reference_folder(self, order_id: int) -> StringArrayResult:
+    def add_language_combination(
+        self, source_language: str, target_language: str, order_id: int
+    ) -> IntegerResult:
         """
-        Deprecated. Please use DataDocument30.getFileList(String, int, int) with Folder Type = 5 instead
-        for compatibility reasons with DataDocument30.
-
-        Returns an instance of StringArrayResult, which contains a list of network
-        paths to the reference files.
-        Info: For content based file up/download please use DataDocument30
+        Adds a language combination to the specified order.
+        All language descriptions were expected in English language or as ISO-Code.
+        Returns an instance of Result.
 
 
+        :param source_language: str
+        :param target_language: str
         :param order_id: int
-        :return: StringArrayResult
+        :return: IntegerResult
         """
 
-        proxy = (
-            self.__client.plunet_server.DataOrder30.getDocuments_Within_ReferenceFolder
-        )
-        response_model = StringArrayResult
+        proxy = self.__client.plunet_server.DataOrder30.addLanguageCombination
+        response_model = IntegerResult
+
+        arg = {
+            "sourceLanguage": source_language,
+            "targetLanguage": target_language,
+            "orderID": order_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=order_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
     def get_documents_within_source_folder_by_language(
         self, language: str, order_id: int
     ) -> StringArrayResult:
         """
         Deprecated. Please use DataDocument30.getFileList(String, int, int) with Folder Type = 6 instead
@@ -1641,54 +1643,51 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_customer_id(self, order_id: int) -> IntegerResult:
+    def get_documents_within_reference_folder(self, order_id: int) -> StringArrayResult:
         """
-        Returns an instance of IntegerResult, which contains the customer id.
+        Deprecated. Please use DataDocument30.getFileList(String, int, int) with Folder Type = 5 instead
+        for compatibility reasons with DataDocument30.
+
+        Returns an instance of StringArrayResult, which contains a list of network
+        paths to the reference files.
+        Info: For content based file up/download please use DataDocument30
 
 
         :param order_id: int
-        :return: IntegerResult
+        :return: StringArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getCustomerID
-        response_model = IntegerResult
+        proxy = (
+            self.__client.plunet_server.DataOrder30.getDocuments_Within_ReferenceFolder
+        )
+        response_model = StringArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=order_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_item_status(
-        self, source_language: str, target_language: str, order_id: int
-    ) -> IntegerResult:
+    def get_customer_contact_id(self, order_id: int) -> IntegerResult:
         """
-        Method returns the status of a project item associated to a specific language combination.
+        Returns an instance of IntegerResult, which contains the customer contact id.
 
 
-        :param source_language: str
-        :param target_language: str
         :param order_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOrder30.getItemStatus
+        proxy = self.__client.plunet_server.DataOrder30.getCustomerContactID
         response_model = IntegerResult
 
-        arg = {
-            "sourceLanguage": source_language,
-            "targetLanguage": target_language,
-            "orderID": order_id,
-        }
-
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=order_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_outgoing_invoice30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_outgoing_invoice30.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,62 +26,20 @@
     StringArrayResult,
     StringResult,
     TaxListResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataOutgoingInvoice30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
-    def get_subject(self, invoice_id: int) -> StringResult:
-        """
-        Returns an instance of StringResult, which contains the subject.
-
-
-        :param invoice_id: int
-        :return: StringResult
-        """
-
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getSubject
-        response_model = StringResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=invoice_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def set_subject(self, subject: str, invoice_id: int) -> Result:
-        """
-        Sets the subject.
-
-
-        :param subject: str
-        :param invoice_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setSubject
-        response_model = Result
-
-        arg = {"subject": subject, "invoiceID": invoice_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
     def delete(self, invoice_id: int) -> Result:
         """
         Deletes a invoice identified by invoice ID.
 
 
         :param invoice_id: int
         :return: Result
@@ -119,134 +77,61 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=search_filter,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_invoice_documents(self, invoice_id: int) -> StringArrayResult:
-        """
-        Returns an instance of StringArrayResult, which contains an array of
-        relative network paths for all available invoice documents.
-
-
-        :param invoice_id: int
-        :return: StringArrayResult
-        """
-
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceDocuments
-        response_model = StringArrayResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=invoice_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def set_receivable_account(self, account_id: int, invoice_id: int) -> Result:
-        """
-        Sets the receivable account.
-
-
-        :param account_id: int
-        :param invoice_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setReceivableAccount
-        response_model = Result
-
-        arg = {"accountID": account_id, "invoiceID": invoice_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def get_revenue_account(self, invoice_id: int) -> StringResult:
+    def get_currency_code(self, invoice_id: int) -> StringResult:
         """
-        Returns the revenue account.
+        Returns an instance of StringResult, which contains the currency code
+        of the currently selected invoice (the amount is standard currency).
 
 
         :param invoice_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getRevenueAccount
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getCurrencyCode
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def create_invoice_document(
-        self, template: str, format_id: int, invoice_id: int
-    ) -> StringResult:
-        """
-        Method creates an invoice document as rtf-file and returns the unc
-        path where the file is located.
-
-
-        :param template: str
-        :param format_id: int
-        :param invoice_id: int
-        :return: StringResult
-        """
-
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.createInvoiceDocument
-        response_model = StringResult
-
-        arg = {"template": template, "formatId": format_id, "invoiceID": invoice_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def get_receivable_account(self, invoice_id: int) -> StringResult:
+    def get_outstanding_by_currency_type(
+        self, invoice_id: int, currency_type: Union[CurrencyType, int]
+    ) -> DoubleResult:
         """
-        Returns the receivable account.
+        Returns an instance of DoubleResult, which contains the outstanding
+        amount in the specified (project or home) currency.
+        Default currency is the project currency.
 
 
         :param invoice_id: int
-        :return: StringResult
+        :param currency_type: CurrencyType
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getReceivableAccount
-        response_model = StringResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=invoice_id,
-            response_model=response_model,
-            unpack_dict=False,
+        proxy = (
+            self.__client.plunet_server.DataOutgoingInvoice30.getOutstandingByCurrencyType
         )
+        response_model = DoubleResult
 
-    def set_revenue_account(self, account_id: int, invoice_id: int) -> Result:
-        """
-        Sets the revenue account.
-
-
-        :param account_id: int
-        :param invoice_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setRevenueAccount
-        response_model = Result
+        if type(currency_type) == CurrencyType:
+            currency_type = currency_type.value
+        elif type(currency_type) == int:
+            currency_type = currency_type
+        else:
+            currency_type = int(currency_type)
 
-        arg = {"accountID": account_id, "invoiceID": invoice_id}
+        arg = {"invoiceID": invoice_id, "currencyType": currency_type}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
@@ -295,14 +180,63 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_item,
             response_model=response_model,
             unpack_dict=False,
         )
 
+    def get_tax_by_type_and_currency_type(
+        self,
+        invoice_id: int,
+        currency_type: Union[CurrencyType, int],
+        taxtypes: Union[TaxType, int],
+    ) -> DoubleResult:
+        """
+        Returns an instance of DoubleResult, which contains the specified TaxValue (project or home) currency.
+        Possible
+
+
+        :param invoice_id: int
+        :param currency_type: CurrencyType
+        :param taxtypes: TaxType
+        :return: DoubleResult
+        """
+
+        proxy = (
+            self.__client.plunet_server.DataOutgoingInvoice30.getTaxByTypeAndCurrencyType
+        )
+        response_model = DoubleResult
+
+        if type(currency_type) == CurrencyType:
+            currency_type = currency_type.value
+        elif type(currency_type) == int:
+            currency_type = currency_type
+        else:
+            currency_type = int(currency_type)
+
+        if type(taxtypes) == TaxType:
+            taxtypes = taxtypes.value
+        elif type(taxtypes) == int:
+            taxtypes = taxtypes
+        else:
+            taxtypes = int(taxtypes)
+
+        arg = {
+            "invoiceID": invoice_id,
+            "currencyType": currency_type,
+            "taxtypes": taxtypes,
+        }
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
     def update_invoice_item(
         self,
         invoice_item: Union[InvoiceItemIN, dict],
         enable_null_or_empty_values: bool,
     ) -> Result:
         """
         Updates a existing invoice item.
@@ -329,29 +263,28 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_paid_by_currency_type(
+    def get_gross_by_currency_type(
         self, invoice_id: int, currency_type: Union[CurrencyType, int]
     ) -> DoubleResult:
         """
-        Returns an instance of DoubleResult, which contains the invoice amount
-        in the specified (project or home) currency.
+        Returns an instance of DoubleResult, which contains the invoice amount in the specified (project or home) currency.
         Default currency is the project currency.
 
 
         :param invoice_id: int
         :param currency_type: CurrencyType
         :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPaidByCurrencyType
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getGrossByCurrencyType
         response_model = DoubleResult
 
         if type(currency_type) == CurrencyType:
             currency_type = currency_type.value
         elif type(currency_type) == int:
             currency_type = currency_type
         else:
@@ -362,28 +295,29 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_tax_by_currency_type(
+    def get_paid_by_currency_type(
         self, invoice_id: int, currency_type: Union[CurrencyType, int]
     ) -> DoubleResult:
         """
-        Returns an instance of DoubleResult, which contains the summed up taxes in the specified (project or home) currency.
+        Returns an instance of DoubleResult, which contains the invoice amount
+        in the specified (project or home) currency.
         Default currency is the project currency.
 
 
         :param invoice_id: int
         :param currency_type: CurrencyType
         :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getTaxByCurrencyType
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPaidByCurrencyType
         response_model = DoubleResult
 
         if type(currency_type) == CurrencyType:
             currency_type = currency_type.value
         elif type(currency_type) == int:
             currency_type = currency_type
         else:
@@ -394,97 +328,66 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_tax_by_type_and_currency_type(
-        self,
-        invoice_id: int,
-        currency_type: Union[CurrencyType, int],
-        taxtypes: Union[TaxType, int],
-    ) -> DoubleResult:
+    def get_invoice_item_list(self, invoice_id: int) -> InvoiceItemResult:
         """
-        Returns an instance of DoubleResult, which contains the specified TaxValue (project or home) currency.
-        Possible
+        Returns a list of all invoice items.
 
 
         :param invoice_id: int
-        :param currency_type: CurrencyType
-        :param taxtypes: TaxType
-        :return: DoubleResult
+        :return: InvoiceItemResult
         """
 
-        proxy = (
-            self.__client.plunet_server.DataOutgoingInvoice30.getTaxByTypeAndCurrencyType
-        )
-        response_model = DoubleResult
-
-        if type(currency_type) == CurrencyType:
-            currency_type = currency_type.value
-        elif type(currency_type) == int:
-            currency_type = currency_type
-        else:
-            currency_type = int(currency_type)
-
-        if type(taxtypes) == TaxType:
-            taxtypes = taxtypes.value
-        elif type(taxtypes) == int:
-            taxtypes = taxtypes
-        else:
-            taxtypes = int(taxtypes)
-
-        arg = {
-            "invoiceID": invoice_id,
-            "currencyType": currency_type,
-            "taxtypes": taxtypes,
-        }
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceItemList
+        response_model = InvoiceItemResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=invoice_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_payment_due_date(self, invoice_id: int) -> DateResult:
+    def get_is_invoice_exported(self, invoice_id: int) -> BooleanResult:
         """
-        Retuns the date the invoice is payed.
+        Returns if the invoice is already exported.
 
 
         :param invoice_id: int
-        :return: DateResult
+        :return: BooleanResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPaymentDueDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getIsInvoiceExported
+        response_model = BooleanResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_net_by_currency_type(
+    def get_tax_by_currency_type(
         self, invoice_id: int, currency_type: Union[CurrencyType, int]
     ) -> DoubleResult:
         """
-        Returns an instance of DoubleResult, which contains the net amount in the specified (project or home) currency.
+        Returns an instance of DoubleResult, which contains the summed up taxes in the specified (project or home) currency.
         Default currency is the project currency.
-        NetAmount includes any discounts
 
 
         :param invoice_id: int
         :param currency_type: CurrencyType
         :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getNetByCurrencyType
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getTaxByCurrencyType
         response_model = DoubleResult
 
         if type(currency_type) == CurrencyType:
             currency_type = currency_type.value
         elif type(currency_type) == int:
             currency_type = currency_type
         else:
@@ -495,63 +398,49 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_gross_by_currency_type(
-        self, invoice_id: int, currency_type: Union[CurrencyType, int]
-    ) -> DoubleResult:
+    def get_invoice_tax_types(self, invoice_id: int) -> TaxListResult:
         """
-        Returns an instance of DoubleResult, which contains the invoice amount in the specified (project or home) currency.
-        Default currency is the project currency.
+        Returns a list of all tax types which are used within the transfered invoice.
+        Possible currency codes can be configured over Admin|Settings|Comany Code
 
 
         :param invoice_id: int
-        :param currency_type: CurrencyType
-        :return: DoubleResult
+        :return: TaxListResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getGrossByCurrencyType
-        response_model = DoubleResult
-
-        if type(currency_type) == CurrencyType:
-            currency_type = currency_type.value
-        elif type(currency_type) == int:
-            currency_type = currency_type
-        else:
-            currency_type = int(currency_type)
-
-        arg = {"invoiceID": invoice_id, "currencyType": currency_type}
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceTaxTypes
+        response_model = TaxListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=invoice_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_outstanding_by_currency_type(
+    def get_net_by_currency_type(
         self, invoice_id: int, currency_type: Union[CurrencyType, int]
     ) -> DoubleResult:
         """
-        Returns an instance of DoubleResult, which contains the outstanding
-        amount in the specified (project or home) currency.
+        Returns an instance of DoubleResult, which contains the net amount in the specified (project or home) currency.
         Default currency is the project currency.
+        NetAmount includes any discounts
 
 
         :param invoice_id: int
         :param currency_type: CurrencyType
         :return: DoubleResult
         """
 
-        proxy = (
-            self.__client.plunet_server.DataOutgoingInvoice30.getOutstandingByCurrencyType
-        )
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getNetByCurrencyType
         response_model = DoubleResult
 
         if type(currency_type) == CurrencyType:
             currency_type = currency_type.value
         elif type(currency_type) == int:
             currency_type = currency_type
         else:
@@ -584,948 +473,1058 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_is_invoice_exported(self, invoice_id: int) -> BooleanResult:
+    def get_payment_due_date(self, invoice_id: int) -> DateResult:
         """
-        Returns if the invoice is already exported.
+        Retuns the date the invoice is payed.
 
 
         :param invoice_id: int
-        :return: BooleanResult
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getIsInvoiceExported
-        response_model = BooleanResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPaymentDueDate
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_invoice_tax_types(self, invoice_id: int) -> TaxListResult:
+    def delete_invoice_item(self, invoice_item_id: int) -> Result:
         """
-        Returns a list of all tax types which are used within the transfered invoice.
-        Possible currency codes can be configured over Admin|Settings|Comany Code
+        Delets an existing invoice item.
 
 
-        :param invoice_id: int
-        :return: TaxListResult
+        :param invoice_item_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceTaxTypes
-        response_model = TaxListResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.deleteInvoiceItem
+        response_model = Result
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=invoice_id,
+            argument=invoice_item_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_invoice_item_list(self, invoice_id: int) -> InvoiceItemResult:
+    def set_address_id(self, invoice_id: int, address_id: int) -> Result:
         """
-        Returns a list of all invoice items.
+        Sets the addressID which has to be related to the invoice related customer.
+        Address information can be obtained over
+        DataCustomerAddress30
 
 
         :param invoice_id: int
-        :return: InvoiceItemResult
+        :param address_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceItemList
-        response_model = InvoiceItemResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setAddressID
+        response_model = Result
+
+        arg = {"invoiceID": invoice_id, "addressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=invoice_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def delete_invoice_item(self, invoice_item_id: int) -> Result:
+    def set_customer_id(self, customer_id: int, invoice_id: int) -> Result:
         """
-        Delets an existing invoice item.
+        Sets the customer ID for the specified invoice.
 
 
-        :param invoice_item_id: int
+        :param customer_id: int
+        :param invoice_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.deleteInvoiceItem
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setCustomerID
         response_model = Result
 
+        arg = {"customerID": customer_id, "invoiceID": invoice_id}
+
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=invoice_item_id,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def update_price_line(
+        self, invoice_item_id: int, price_line_in: Union[PriceLineIN, dict]
+    ) -> PriceLineResult:
+        """
+        Updates a existing PriceLine.
+
+
+        :param invoice_item_id: int
+        :param price_line_in: PriceLineIN
+        :return: PriceLineResult
+        """
+
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.updatePriceLine
+        response_model = PriceLineResult
+
+        if type(price_line_in) != PriceLineIN:
+            price_line_in = PriceLineIN(**price_line_in).dict()
+        else:
+            price_line_in = price_line_in.dict()
+
+        arg = {"invoiceItemID": invoice_item_id, "priceLineIN": price_line_in}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def get_services_list(self, language_code: str) -> StringArrayResult:
+        """
+        Deprecated. Please use DataAdmin30.getAvailableServices(String, String) instead.
+        Returns a list of all available services.
+
+
+        :param language_code: str
+        :return: StringArrayResult
+        """
+
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getServices_List
+        response_model = StringArrayResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=language_code,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_currency_code(self, invoice_id: int) -> StringResult:
+    def get_pricelist(self, invoice_item_id: int) -> PricelistResult:
         """
-        Returns an instance of StringResult, which contains the currency code
-        of the currently selected invoice (the amount is standard currency).
+        Returns the current selected Pricelist for the specified invoice item.
 
 
-        :param invoice_id: int
-        :return: StringResult
+        :param invoice_item_id: int
+        :return: PricelistResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getCurrencyCode
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPricelist
+        response_model = PricelistResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=invoice_id,
+            argument=invoice_item_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_invoice_id(self, display_name: str, company_code_id: int) -> IntegerResult:
+    def get_price_unit(self, price_unit_id: int, language_code: str) -> PriceUnitResult:
         """
-        Get the invoiceId based on the display number and company code of the invoice.
+        Returns a PriceUnitResult object.
+        Possible PriceUnitÂ´s can be obtained over DataItem30.getPriceUnit_List(java.lang.String, java.lang.String, java.lang.String)
 
 
-        :param display_name: str
-        :param company_code_id: int
-        :return: IntegerResult
+        :param price_unit_id: int
+        :param language_code: str
+        :return: PriceUnitResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceId
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPriceUnit
+        response_model = PriceUnitResult
 
-        arg = {"displayName": display_name, "companyCodeId": company_code_id}
+        arg = {"PriceUnitID": price_unit_id, "languageCode": language_code}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_customer_id(self, customer_id: int, invoice_id: int) -> Result:
+    def insert_price_line(
+        self,
+        invoice_item_id: int,
+        price_line_in: Union[PriceLineIN, dict],
+        create_as_first_item: bool,
+    ) -> PriceLineResult:
         """
-        Sets the customer ID for the specified invoice.
+        Inserts a new PriceLine to the specified invoice item
 
 
-        :param customer_id: int
-        :param invoice_id: int
-        :return: Result
+        :param invoice_item_id: int
+        :param price_line_in: PriceLineIN
+        :param create_as_first_item: bool
+        :return: PriceLineResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setCustomerID
-        response_model = Result
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.insertPriceLine
+        response_model = PriceLineResult
 
-        arg = {"customerID": customer_id, "invoiceID": invoice_id}
+        if type(price_line_in) != PriceLineIN:
+            price_line_in = PriceLineIN(**price_line_in).dict()
+        else:
+            price_line_in = price_line_in.dict()
+
+        arg = {
+            "invoiceItemID": invoice_item_id,
+            "priceLineIN": price_line_in,
+            "createAsFirstItem": create_as_first_item,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_address_id(self, invoice_id: int, address_id: int) -> Result:
+    def set_pricelist(self, invoice_item_id: int, price_list_id: int) -> Result:
         """
-        Sets the addressID which has to be related to the invoice related customer.
-        Address information can be obtained over
-        DataCustomerAddress30
+        SetÂ´s the selected Pricelist for the specified invoice item.
 
 
-        :param invoice_id: int
-        :param address_id: int
+        :param invoice_item_id: int
+        :param price_list_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setAddressID
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setPricelist
         response_model = Result
 
-        arg = {"invoiceID": invoice_id, "addressID": address_id}
+        arg = {"InvoiceItemID": invoice_item_id, "priceListID": price_list_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_price_line_list(self, invoice_item_id: int) -> PriceLineListResult:
+    def delete_price_line(self, invoice_item_id: int, price_line_id: int) -> Result:
         """
-        Returns a list of all job related PriceLine
+        Deletes an existing PriceLine
 
 
         :param invoice_item_id: int
-        :return: PriceLineListResult
+        :param price_line_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPriceLine_List
-        response_model = PriceLineListResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.deletePriceLine
+        response_model = Result
+
+        arg = {"invoiceItemID": invoice_item_id, "priceLineID": price_line_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=invoice_item_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_price_unit_list(
-        self, language_code: str, service: str
-    ) -> PriceUnitListResult:
+    def get_invoice_nr(self, invoice_id: int) -> StringResult:
         """
-        Returns a list of priceUnit related to the specified service.
-        Possible services can be obtained over DataAdmin30.getAvailableServices(String, String)
+        Returns an instance of StringResult, which contains the invoice
+        number.
 
 
-        :param language_code: str
-        :param service: str
-        :return: PriceUnitListResult
+        :param invoice_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPriceUnit_List
-        response_model = PriceUnitListResult
-
-        arg = {"languageCode": language_code, "service": service}
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceNr
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=invoice_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_pricelist_entry_list(
-        self, pricelist_id: int, source_language: str, target_language: str
-    ) -> PricelistEntryList:
+    def get_net(self, invoice_id: int) -> DoubleResult:
         """
-        Provides all price entries which are related to the Pricelist
-        regarding the transfered source and target language.
+        Returns an instance of DoubleResult, which contains the net amount (in project currency).
+        NetAmount includes any discounts
 
 
-        :param pricelist_id: int
-        :param source_language: str
-        :param target_language: str
-        :return: PricelistEntryList
+        :param invoice_id: int
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPricelistEntry_List
-        response_model = PricelistEntryList
-
-        arg = {
-            "PricelistID": pricelist_id,
-            "SourceLanguage": source_language,
-            "TargetLanguage": target_language,
-        }
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getNet
+        response_model = DoubleResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=invoice_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_pricelist_list(self, invoice_item_id: int) -> PricelistListResult:
+    def get_gross(self, invoice_id: int) -> DoubleResult:
         """
-        Returns all avaliable Pricelist for this invoice item.
-        Note: This is dependent on the related project and the selected customer
+        Returns an instance of DoubleResult, which contains the invoice amount (in project currency).
 
 
-        :param invoice_item_id: int
-        :return: PricelistListResult
+        :param invoice_id: int
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPricelist_List
-        response_model = PricelistListResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getGross
+        response_model = DoubleResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=invoice_item_id,
+            argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_status(self, invoice_id: int) -> IntegerResult:
+    def get_outstanding(self, invoice_id: int) -> DoubleResult:
         """
-        Returns an instance of IntegerResult, which contains the status.
+        Returns an instance of DoubleResult, which contains the outstanding
+        amount (in project currency).
 
 
         :param invoice_id: int
-        :return: IntegerResult
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getStatus
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getOutstanding
+        response_model = DoubleResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_status(self, status: int, invoice_id: int) -> Result:
+    def get_paid(self, invoice_id: int) -> DoubleResult:
         """
-        Sets the status.
+        Returns an instance of DoubleResult, which contains the invoice amount
+        (in project currency).
 
 
-        :param status: int
         :param invoice_id: int
-        :return: Result
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setStatus
-        response_model = Result
-
-        arg = {"Status": status, "invoiceID": invoice_id}
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPaid
+        response_model = DoubleResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=invoice_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_brief_description(self, invoice_id: int) -> StringResult:
+    def get_tax(self, invoice_id: int) -> DoubleResult:
         """
-        Returns the brief description.
+        Returns an instance of DoubleResult, which contains all taxes as summed up values (in project currency).
 
 
         :param invoice_id: int
-        :return: StringResult
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getBriefDescription
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getTax
+        response_model = DoubleResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_brief_description(self, description: str, invoice_id: int) -> Result:
+    def get_order_i_ds(self, invoice_id: int) -> IntegerArrayResult:
         """
-        Sets the brief description.
+        Returns an instances of IntegerArrayResult, which contains the order
+        IDs.
 
 
-        :param description: str
         :param invoice_id: int
-        :return: Result
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setBriefDescription
-        response_model = Result
-
-        arg = {"description": description, "invoiceID": invoice_id}
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getOrderIDs
+        response_model = IntegerArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=invoice_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_contact_person_id(self, invoice_id: int) -> IntegerResult:
+    def get_invoice_date(self, invoice_id: int) -> DateResult:
         """
-        Returns the id to the invoice realted contact person (customer).
-        Contact Person details can be obtained over
-        DataCustomerContact30
+        Returns an instance of DateResult, which contains the invoice
+        date.
 
 
         :param invoice_id: int
-        :return: IntegerResult
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getContactPersonID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceDate
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_contact_person_id(self, invoice_id: int, contact_person_id: int) -> Result:
+    def set_value_date(self, value_date: datetime, invoice_id: int) -> Result:
         """
-        Sets the customer depended contact person for the specified invoice.
-        Contact Person details can be obtained over
-        DataCustomerContact30
+        Sets the value date of the currently selected invoice.
 
 
+        :param value_date: datetime
         :param invoice_id: int
-        :param contact_person_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setContactPersonID
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setValueDate
         response_model = Result
 
-        arg = {"invoiceID": invoice_id, "contactPersonID": contact_person_id}
+        arg = {"valueDate": value_date, "invoiceID": invoice_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def update_price_line(
-        self, invoice_item_id: int, price_line_in: Union[PriceLineIN, dict]
-    ) -> PriceLineResult:
+    def set_invoice_date(self, invoice_date: datetime, invoice_id: int) -> Result:
         """
-        Updates a existing PriceLine.
+        Sets the invoice date.
 
 
-        :param invoice_item_id: int
-        :param price_line_in: PriceLineIN
-        :return: PriceLineResult
+        :param invoice_date: datetime
+        :param invoice_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.updatePriceLine
-        response_model = PriceLineResult
-
-        if type(price_line_in) != PriceLineIN:
-            price_line_in = PriceLineIN(**price_line_in).dict()
-        else:
-            price_line_in = price_line_in.dict()
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setInvoiceDate
+        response_model = Result
 
-        arg = {"invoiceItemID": invoice_item_id, "priceLineIN": price_line_in}
+        arg = {"invoiceDate": invoice_date, "invoiceID": invoice_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_pricelist(self, invoice_item_id: int) -> PricelistResult:
+    def get_invoice_object(self, invoice_id: int) -> InvoiceResult:
         """
-        Returns the current selected Pricelist for the specified invoice item.
+        Method returns an instance of InvoiceResult, which contains an
+        instance of Invoice.
 
 
-        :param invoice_item_id: int
-        :return: PricelistResult
+        :param invoice_id: int
+        :return: InvoiceResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPricelist
-        response_model = PricelistResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceObject
+        response_model = InvoiceResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=invoice_item_id,
+            argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_pricelist(self, invoice_item_id: int, price_list_id: int) -> Result:
+    def get_value_date(self, invoice_id: int) -> DateResult:
         """
-        SetÂ´s the selected Pricelist for the specified invoice item.
+        Returns an instance of DateResult, which contains the value date.
 
 
-        :param invoice_item_id: int
-        :param price_list_id: int
-        :return: Result
+        :param invoice_id: int
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setPricelist
-        response_model = Result
-
-        arg = {"InvoiceItemID": invoice_item_id, "priceListID": price_list_id}
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getValueDate
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=invoice_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_services_list(self, language_code: str) -> StringArrayResult:
+    def get_company_code(self, invoice_id: int) -> IntegerResult:
         """
-        Deprecated. Please use DataAdmin30.getAvailableServices(String, String) instead.
-        Returns a list of all available services.
+        Returns the type dependent company code, related to the specified
+        invoice.
 
 
-        :param language_code: str
-        :return: StringArrayResult
+        :param invoice_id: int
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getServices_List
-        response_model = StringArrayResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getCompanyCode
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=language_code,
+            argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_price_unit(self, price_unit_id: int, language_code: str) -> PriceUnitResult:
+    def get_invoice_id(self, display_name: str, company_code_id: int) -> IntegerResult:
         """
-        Returns a PriceUnitResult object.
-        Possible PriceUnitÂ´s can be obtained over DataItem30.getPriceUnit_List(java.lang.String, java.lang.String, java.lang.String)
+        Get the invoiceId based on the display number and company code of the invoice.
 
 
-        :param price_unit_id: int
-        :param language_code: str
-        :return: PriceUnitResult
+        :param display_name: str
+        :param company_code_id: int
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPriceUnit
-        response_model = PriceUnitResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceId
+        response_model = IntegerResult
 
-        arg = {"PriceUnitID": price_unit_id, "languageCode": language_code}
+        arg = {"displayName": display_name, "companyCodeId": company_code_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def insert_price_line(
-        self,
-        invoice_item_id: int,
-        price_line_in: Union[PriceLineIN, dict],
-        create_as_first_item: bool,
-    ) -> PriceLineResult:
+    def get_adress_id(self, invoice_id: int) -> IntegerResult:
         """
-        Inserts a new PriceLine to the specified invoice item
+        Return the ID of the customer address entry this invoice is mapped to.
+        Address information can be obtained over
+        DataCustomerAddress30
 
 
-        :param invoice_item_id: int
-        :param price_line_in: PriceLineIN
-        :param create_as_first_item: bool
-        :return: PriceLineResult
+        :param invoice_id: int
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.insertPriceLine
-        response_model = PriceLineResult
-
-        if type(price_line_in) != PriceLineIN:
-            price_line_in = PriceLineIN(**price_line_in).dict()
-        else:
-            price_line_in = price_line_in.dict()
-
-        arg = {
-            "invoiceItemID": invoice_item_id,
-            "priceLineIN": price_line_in,
-            "createAsFirstItem": create_as_first_item,
-        }
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getAdressID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=invoice_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def delete_price_line(self, invoice_item_id: int, price_line_id: int) -> Result:
+    def set_paid_date(self, invoice_id: int, paid_date: datetime) -> Result:
         """
-        Deletes an existing PriceLine
+        Defines the date the invoice is payed.
 
 
-        :param invoice_item_id: int
-        :param price_line_id: int
+        :param invoice_id: int
+        :param paid_date: datetime
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.deletePriceLine
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setPaidDate
         response_model = Result
 
-        arg = {"invoiceItemID": invoice_item_id, "priceLineID": price_line_id}
+        arg = {"invoiceID": invoice_id, "paidDate": paid_date}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_po_number(self, invoice_id: int, po_number: str) -> Result:
+    def get_paid_date(self, invoice_id: int) -> DateResult:
         """
-        Defines if the invoice is already exported.
+        Retuns the date the invoice is payed.
 
 
         :param invoice_id: int
-        :param po_number: str
-        :return: Result
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setPONumber
-        response_model = Result
-
-        arg = {"invoiceID": invoice_id, "poNumber": po_number}
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPaidDate
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=invoice_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_outstanding(self, invoice_id: int) -> DoubleResult:
+    def get_po_number(self, invoice_id: int) -> StringResult:
         """
-        Returns an instance of DoubleResult, which contains the outstanding
-        amount (in project currency).
+        Returns if the PO-number
 
 
         :param invoice_id: int
-        :return: DoubleResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getOutstanding
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPONumber
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_gross(self, invoice_id: int) -> DoubleResult:
+    def set_status(self, status: int, invoice_id: int) -> Result:
         """
-        Returns an instance of DoubleResult, which contains the invoice amount (in project currency).
+        Sets the status.
 
 
+        :param status: int
         :param invoice_id: int
-        :return: DoubleResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getGross
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setStatus
+        response_model = Result
+
+        arg = {"Status": status, "invoiceID": invoice_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=invoice_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_order_i_ds(self, invoice_id: int) -> IntegerArrayResult:
+    def get_customer_id(self, invoice_id: int) -> IntegerResult:
         """
-        Returns an instances of IntegerArrayResult, which contains the order
-        IDs.
+        Returns an instance of IntegerResult, which contains the customer
+        ID.
 
 
         :param invoice_id: int
-        :return: IntegerArrayResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getOrderIDs
-        response_model = IntegerArrayResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getCustomerID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_net(self, invoice_id: int) -> DoubleResult:
+    def get_pricelist_list(self, invoice_item_id: int) -> PricelistListResult:
         """
-        Returns an instance of DoubleResult, which contains the net amount (in project currency).
-        NetAmount includes any discounts
+        Returns all avaliable Pricelist for this invoice item.
+        Note: This is dependent on the related project and the selected customer
 
 
-        :param invoice_id: int
-        :return: DoubleResult
+        :param invoice_item_id: int
+        :return: PricelistListResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getNet
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPricelist_List
+        response_model = PricelistListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=invoice_id,
+            argument=invoice_item_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_paid(self, invoice_id: int) -> DoubleResult:
+    def get_pricelist_entry_list(
+        self, pricelist_id: int, source_language: str, target_language: str
+    ) -> PricelistEntryList:
         """
-        Returns an instance of DoubleResult, which contains the invoice amount
-        (in project currency).
+        Provides all price entries which are related to the Pricelist
+        regarding the transfered source and target language.
 
 
-        :param invoice_id: int
-        :return: DoubleResult
+        :param pricelist_id: int
+        :param source_language: str
+        :param target_language: str
+        :return: PricelistEntryList
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPaid
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPricelistEntry_List
+        response_model = PricelistEntryList
+
+        arg = {
+            "PricelistID": pricelist_id,
+            "SourceLanguage": source_language,
+            "TargetLanguage": target_language,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=invoice_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_value_date(self, invoice_id: int) -> DateResult:
+    def get_price_line_list(self, invoice_item_id: int) -> PriceLineListResult:
         """
-        Returns an instance of DateResult, which contains the value date.
+        Returns a list of all job related PriceLine
 
 
-        :param invoice_id: int
-        :return: DateResult
+        :param invoice_item_id: int
+        :return: PriceLineListResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getValueDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPriceLine_List
+        response_model = PriceLineListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=invoice_id,
+            argument=invoice_item_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_invoice_date(self, invoice_id: int) -> DateResult:
+    def get_price_unit_list(
+        self, language_code: str, service: str
+    ) -> PriceUnitListResult:
         """
-        Returns an instance of DateResult, which contains the invoice
-        date.
+        Returns a list of priceUnit related to the specified service.
+        Possible services can be obtained over DataAdmin30.getAvailableServices(String, String)
+
+
+        :param language_code: str
+        :param service: str
+        :return: PriceUnitListResult
+        """
+
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPriceUnit_List
+        response_model = PriceUnitListResult
+
+        arg = {"languageCode": language_code, "service": service}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def get_status(self, invoice_id: int) -> IntegerResult:
+        """
+        Returns an instance of IntegerResult, which contains the status.
 
 
         :param invoice_id: int
-        :return: DateResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getStatus
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_invoice_nr(self, invoice_id: int) -> StringResult:
+    def get_subject(self, invoice_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the invoice
-        number.
+        Returns an instance of StringResult, which contains the subject.
 
 
         :param invoice_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceNr
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getSubject
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_invoice_date(self, invoice_date: datetime, invoice_id: int) -> Result:
+    def set_subject(self, subject: str, invoice_id: int) -> Result:
         """
-        Sets the invoice date.
+        Sets the subject.
 
 
-        :param invoice_date: datetime
+        :param subject: str
         :param invoice_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setInvoiceDate
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setSubject
         response_model = Result
 
-        arg = {"invoiceDate": invoice_date, "invoiceID": invoice_id}
+        arg = {"subject": subject, "invoiceID": invoice_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_tax(self, invoice_id: int) -> DoubleResult:
+    def set_po_number(self, invoice_id: int, po_number: str) -> Result:
         """
-        Returns an instance of DoubleResult, which contains all taxes as summed up values (in project currency).
+        Defines if the invoice is already exported.
 
 
         :param invoice_id: int
-        :return: DoubleResult
+        :param po_number: str
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getTax
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setPONumber
+        response_model = Result
+
+        arg = {"invoiceID": invoice_id, "poNumber": po_number}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=invoice_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_invoice_object(self, invoice_id: int) -> InvoiceResult:
+    def get_brief_description(self, invoice_id: int) -> StringResult:
         """
-        Method returns an instance of InvoiceResult, which contains an
-        instance of Invoice.
+        Returns the brief description.
 
 
         :param invoice_id: int
-        :return: InvoiceResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceObject
-        response_model = InvoiceResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getBriefDescription
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_value_date(self, value_date: datetime, invoice_id: int) -> Result:
+    def set_brief_description(self, description: str, invoice_id: int) -> Result:
         """
-        Sets the value date of the currently selected invoice.
+        Sets the brief description.
 
 
-        :param value_date: datetime
+        :param description: str
         :param invoice_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setValueDate
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setBriefDescription
         response_model = Result
 
-        arg = {"valueDate": value_date, "invoiceID": invoice_id}
+        arg = {"description": description, "invoiceID": invoice_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_customer_id(self, invoice_id: int) -> IntegerResult:
+    def get_revenue_account(self, invoice_id: int) -> StringResult:
         """
-        Returns an instance of IntegerResult, which contains the customer
-        ID.
+        Returns the revenue account.
 
 
         :param invoice_id: int
-        :return: IntegerResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getCustomerID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getRevenueAccount
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_adress_id(self, invoice_id: int) -> IntegerResult:
+    def create_invoice_document(
+        self, template: str, format_id: int, invoice_id: int
+    ) -> StringResult:
         """
-        Return the ID of the customer address entry this invoice is mapped to.
-        Address information can be obtained over
-        DataCustomerAddress30
+        Method creates an invoice document as rtf-file and returns the unc
+        path where the file is located.
 
 
+        :param template: str
+        :param format_id: int
         :param invoice_id: int
-        :return: IntegerResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getAdressID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.createInvoiceDocument
+        response_model = StringResult
+
+        arg = {"template": template, "formatId": format_id, "invoiceID": invoice_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=invoice_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_paid_date(self, invoice_id: int) -> DateResult:
+    def get_receivable_account(self, invoice_id: int) -> StringResult:
         """
-        Retuns the date the invoice is payed.
+        Returns the receivable account.
 
 
         :param invoice_id: int
-        :return: DateResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPaidDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getReceivableAccount
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_po_number(self, invoice_id: int) -> StringResult:
+    def set_receivable_account(self, account_id: int, invoice_id: int) -> Result:
         """
-        Returns if the PO-number
+        Sets the receivable account.
 
 
+        :param account_id: int
         :param invoice_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getPONumber
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setReceivableAccount
+        response_model = Result
+
+        arg = {"accountID": account_id, "invoiceID": invoice_id}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def get_invoice_documents(self, invoice_id: int) -> StringArrayResult:
+        """
+        Returns an instance of StringArrayResult, which contains an array of
+        relative network paths for all available invoice documents.
+
+
+        :param invoice_id: int
+        :return: StringArrayResult
+        """
+
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getInvoiceDocuments
+        response_model = StringArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_paid_date(self, invoice_id: int, paid_date: datetime) -> Result:
+    def set_revenue_account(self, account_id: int, invoice_id: int) -> Result:
         """
-        Defines the date the invoice is payed.
+        Sets the revenue account.
 
 
+        :param account_id: int
         :param invoice_id: int
-        :param paid_date: datetime
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setPaidDate
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setRevenueAccount
         response_model = Result
 
-        arg = {"invoiceID": invoice_id, "paidDate": paid_date}
+        arg = {"accountID": account_id, "invoiceID": invoice_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_company_code(self, invoice_id: int) -> IntegerResult:
+    def get_contact_person_id(self, invoice_id: int) -> IntegerResult:
         """
-        Returns the type dependent company code, related to the specified
-        invoice.
+        Returns the id to the invoice realted contact person (customer).
+        Contact Person details can be obtained over
+        DataCustomerContact30
 
 
         :param invoice_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getCompanyCode
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.getContactPersonID
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=invoice_id,
             response_model=response_model,
             unpack_dict=False,
         )
+
+    def set_contact_person_id(self, invoice_id: int, contact_person_id: int) -> Result:
+        """
+        Sets the customer depended contact person for the specified invoice.
+        Contact Person details can be obtained over
+        DataCustomerContact30
+
+
+        :param invoice_id: int
+        :param contact_person_id: int
+        :return: Result
+        """
+
+        proxy = self.__client.plunet_server.DataOutgoingInvoice30.setContactPersonID
+        response_model = Result
+
+        arg = {"invoiceID": invoice_id, "contactPersonID": contact_person_id}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_payable30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_payable30.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,18 @@
     StringArrayResult,
     StringResult,
     TaxListResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataPayable30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
     def search(
         self, search_filter: Union[SearchFilter_Payable, dict]
     ) -> IntegerArrayResult:
         """
         No description of search in docs.
@@ -55,157 +54,90 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=search_filter,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_payment_due_date(self, payables_id: int) -> DateResult:
+    def get_currency(self, payables_id: int) -> StringResult:
         """
-        Retuns the date the invoice is payed.
+        Returns the currency of the payable.
 
 
         :param payables_id: int
-        :return: DateResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getPaymentDueDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataPayable30.getCurrency
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_payment_due_date(self, payables_id: int, due_date: datetime) -> Result:
+    def delete_payment_item(self, payment_item_id: int) -> Result:
         """
-        Defines the date the invoice is payed.
+        Deletes an payment Item
 
 
-        :param payables_id: int
-        :param due_date: datetime
+        :param payment_item_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.setPaymentDueDate
+        proxy = self.__client.plunet_server.DataPayable30.deletePaymentItem
         response_model = Result
 
-        arg = {"payablesID": payables_id, "dueDate": due_date}
-
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def get_invoice_tax_types(self, payables_id: int) -> TaxListResult:
-        """
-        Returns a list of all tax types which are used within the transfered invoice..
-        Possible currency codes can be configured over Admin|Settings|Comany Code
-
-
-        :param payables_id: int
-        :return: TaxListResult
-        """
-
-        proxy = self.__client.plunet_server.DataPayable30.getInvoiceTaxTypes
-        response_model = TaxListResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=payables_id,
+            argument=payment_item_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_creditor_account(self, payables_id: int) -> StringResult:
+    def get_expense_account(self, payables_id: int) -> StringResult:
         """
-        Returns the creditor account.
+        Returns the expense account.
 
 
         :param payables_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getCreditorAccount
+        proxy = self.__client.plunet_server.DataPayable30.getExpenseAccount
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_external_invoice_number(self, payables_id: int) -> StringResult:
+    def get_account_statement(self, payables_id: int) -> StringResult:
         """
-        Returns the revenue account.
+        Returns the account statement.
 
 
         :param payables_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getExternalInvoiceNumber
+        proxy = self.__client.plunet_server.DataPayable30.getAccountStatement
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_creditor_account(self, account_id: str, payables_id: int) -> Result:
-        """
-        Defines the creditor account.
-
-
-        :param account_id: str
-        :param payables_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataPayable30.setCreditorAccount
-        response_model = Result
-
-        arg = {"accountID": account_id, "payablesID": payables_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def set_account_statement(self, payables_id: int, accountstatement: str) -> Result:
-        """
-        Defines the po number of the related credit note.
-
-
-        :param payables_id: int
-        :param accountstatement: str
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataPayable30.setAccountStatement
-        response_model = Result
-
-        arg = {"payablesID": payables_id, "accountstatement": accountstatement}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
     def get_total_tax_amount(
         self, payables_id: int, currency_tpe: int, tax_type: Union[TaxType, int]
     ) -> DoubleResult:
         """
         Returns the total tax price of the payment.
 
 
@@ -234,36 +166,14 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_total_net_amount(self, payables_id: int, currency_tpe: int) -> DoubleResult:
-        """
-        Returns the total net price of the payment,
-
-
-        :param payables_id: int
-        :param currency_tpe: int
-        :return: DoubleResult
-        """
-
-        proxy = self.__client.plunet_server.DataPayable30.getTotalNetAmount
-        response_model = DoubleResult
-
-        arg = {"payablesID": payables_id, "currencyTpe": currency_tpe}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
     def update_payment_item(
         self,
         payment_item_in: Union[PayableItemIN, dict],
         payment_item_id: int,
         enable_null_or_empty_values: bool,
     ) -> Result:
         """
@@ -293,283 +203,265 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def delete_payment_item(self, payment_item_id: int) -> Result:
+    def get_payment_item_list(self, payables_id: int) -> PayableItemResultList:
         """
-        Deletes an payment Item
+        Retuns a list of all paymentent relevant items
 
 
-        :param payment_item_id: int
-        :return: Result
+        :param payables_id: int
+        :return: PayableItemResultList
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.deletePaymentItem
-        response_model = Result
+        proxy = self.__client.plunet_server.DataPayable30.getPaymentItemList
+        response_model = PayableItemResultList
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=payment_item_id,
+            argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_expense_account(self, payables_id: int) -> StringResult:
+    def get_total_net_amount(self, payables_id: int, currency_tpe: int) -> DoubleResult:
         """
-        Returns the expense account.
+        Returns the total net price of the payment,
 
 
         :param payables_id: int
-        :return: StringResult
+        :param currency_tpe: int
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getExpenseAccount
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataPayable30.getTotalNetAmount
+        response_model = DoubleResult
+
+        arg = {"payablesID": payables_id, "currencyTpe": currency_tpe}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=payables_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_payment_item_list(self, payables_id: int) -> PayableItemResultList:
+    def get_payment_creator_resource_id(self, payables_id: int) -> IntegerResult:
         """
-        Retuns a list of all paymentent relevant items
+        Returns the resourceID of the for the creation responsible resource.
 
 
         :param payables_id: int
-        :return: PayableItemResultList
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getPaymentItemList
-        response_model = PayableItemResultList
+        proxy = self.__client.plunet_server.DataPayable30.getPaymentCreatorResourceID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_account_statement(self, payables_id: int) -> StringResult:
+    def set_creditor_account(self, account_id: str, payables_id: int) -> Result:
         """
-        Returns the account statement.
+        Defines the creditor account.
 
 
+        :param account_id: str
         :param payables_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getAccountStatement
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataPayable30.setCreditorAccount
+        response_model = Result
+
+        arg = {"accountID": account_id, "payablesID": payables_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=payables_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def insert_payment_item(
-        self, payment_item_in: Union[PayableItemIN, dict]
-    ) -> IntegerResult:
+    def get_invoice_tax_types(self, payables_id: int) -> TaxListResult:
         """
-        Inserts a new payment item
+        Returns a list of all tax types which are used within the transfered invoice..
+        Possible currency codes can be configured over Admin|Settings|Comany Code
 
 
-        :param payment_item_in: PayableItemIN
-        :return: IntegerResult
+        :param payables_id: int
+        :return: TaxListResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.insertPaymentItem
-        response_model = IntegerResult
-
-        if type(payment_item_in) != PayableItemIN:
-            payment_item_in = PayableItemIN(**payment_item_in).dict()
-        else:
-            payment_item_in = payment_item_in.dict()
+        proxy = self.__client.plunet_server.DataPayable30.getInvoiceTaxTypes
+        response_model = TaxListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=payment_item_in,
+            argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_payment_creator_resource_id(self, payables_id: int) -> IntegerResult:
+    def get_external_invoice_number(self, payables_id: int) -> StringResult:
         """
-        Returns the resourceID of the for the creation responsible resource.
+        Returns the revenue account.
 
 
         :param payables_id: int
-        :return: IntegerResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getPaymentCreatorResourceID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataPayable30.getExternalInvoiceNumber
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_external_invoice_number(
-        self, payables_id: int, external_number: str
-    ) -> Result:
+    def set_account_statement(self, payables_id: int, accountstatement: str) -> Result:
         """
-        Defines the revenue account.
+        Defines the po number of the related credit note.
 
 
         :param payables_id: int
-        :param external_number: str
+        :param accountstatement: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.setExternalInvoiceNumber
+        proxy = self.__client.plunet_server.DataPayable30.setAccountStatement
         response_model = Result
 
-        arg = {"payablesID": payables_id, "externalNumber": external_number}
+        arg = {"payablesID": payables_id, "accountstatement": accountstatement}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_currency(self, payables_id: int) -> StringResult:
+    def get_creditor_account(self, payables_id: int) -> StringResult:
         """
-        Returns the currency of the payable.
+        Returns the creditor account.
 
 
         :param payables_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getCurrency
+        proxy = self.__client.plunet_server.DataPayable30.getCreditorAccount
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_payment_method(self, payables_id: int) -> IntegerResult:
+    def set_payment_due_date(self, payables_id: int, due_date: datetime) -> Result:
         """
-        Returns the payment method, represented by its FA value.
-
-        See Admin | Miscellaneous | Payment method | FA value.
+        Defines the date the invoice is payed.
 
 
         :param payables_id: int
-        :return: IntegerResult
+        :param due_date: datetime
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getPaymentMethod
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataPayable30.setPaymentDueDate
+        response_model = Result
+
+        arg = {"payablesID": payables_id, "dueDate": due_date}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=payables_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_price_line_list(self, payables_item_id: int) -> PriceLineListResult:
+    def get_payment_due_date(self, payables_id: int) -> DateResult:
         """
-        Returns a list of all job related PriceLine
+        Retuns the date the invoice is payed.
 
 
-        :param payables_item_id: int
-        :return: PriceLineListResult
+        :param payables_id: int
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getPriceLine_List
-        response_model = PriceLineListResult
+        proxy = self.__client.plunet_server.DataPayable30.getPaymentDueDate
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=payables_item_id,
+            argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_price_unit_list(
-        self, language_code: str, service: str
-    ) -> PriceUnitListResult:
+    def set_external_invoice_number(
+        self, payables_id: int, external_number: str
+    ) -> Result:
         """
-        Returns a list of priceUnit related to the specified service.
-        Possible services can be obtained over DataAdmin30.getAvailableServices(String, String)
+        Defines the revenue account.
 
 
-        :param language_code: str
-        :param service: str
-        :return: PriceUnitListResult
+        :param payables_id: int
+        :param external_number: str
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getPriceUnit_List
-        response_model = PriceUnitListResult
+        proxy = self.__client.plunet_server.DataPayable30.setExternalInvoiceNumber
+        response_model = Result
 
-        arg = {"languageCode": language_code, "service": service}
+        arg = {"payablesID": payables_id, "externalNumber": external_number}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_status(self, payables_id: int) -> IntegerResult:
+    def insert_payment_item(
+        self, payment_item_in: Union[PayableItemIN, dict]
+    ) -> IntegerResult:
         """
-        Returns an instance of IntegerResult, which contains the
-        PayableStatus.
+        Inserts a new payment item
 
 
-        :param payables_id: int
+        :param payment_item_in: PayableItemIN
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getStatus
+        proxy = self.__client.plunet_server.DataPayable30.insertPaymentItem
         response_model = IntegerResult
 
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=payables_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def set_status(self, status: int, payables_id: int) -> Result:
-        """
-        Defines the PayableStatus.
-
-
-        :param status: int
-        :param payables_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataPayable30.setStatus
-        response_model = Result
-
-        arg = {"Status": status, "payablesID": payables_id}
+        if type(payment_item_in) != PayableItemIN:
+            payment_item_in = PayableItemIN(**payment_item_in).dict()
+        else:
+            payment_item_in = payment_item_in.dict()
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=payment_item_in,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
     def update_price_line(
         self, payables_item_id: int, price_line_in: Union[PriceLineIN, dict]
     ) -> PriceLineResult:
         """
         Updates a existing PriceLine.
@@ -714,51 +606,54 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=item_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_value_date(self, payables_id: int) -> DateResult:
+    def get_invoice_date(self, payables_id: int) -> DateResult:
         """
-        Returns an instance of DateResult, which contains the value date.
+        Returns an instance of DateResult, which contains the invoice
+        date.
 
 
         :param payables_id: int
         :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getValueDate
+        proxy = self.__client.plunet_server.DataPayable30.getInvoiceDate
         response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_invoice_date(self, payables_id: int) -> DateResult:
+    def set_value_date(self, value_date: datetime, payables_id: int) -> Result:
         """
-        Returns an instance of DateResult, which contains the invoice
-        date.
+        Defines the value date of the currently selected invoice.
 
 
+        :param value_date: datetime
         :param payables_id: int
-        :return: DateResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getInvoiceDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataPayable30.setValueDate
+        response_model = Result
+
+        arg = {"valueDate": value_date, "payablesID": payables_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=payables_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
     def set_invoice_date(self, invoice_date: datetime, payables_id: int) -> Result:
         """
         Defines the invoice date.
 
 
@@ -775,66 +670,107 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_value_date(self, value_date: datetime, payables_id: int) -> Result:
+    def get_value_date(self, payables_id: int) -> DateResult:
         """
-        Defines the value date of the currently selected invoice.
+        Returns an instance of DateResult, which contains the value date.
+
+
+        :param payables_id: int
+        :return: DateResult
+        """
+
+        proxy = self.__client.plunet_server.DataPayable30.getValueDate
+        response_model = DateResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=payables_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_memo(self, payables_id: int) -> StringResult:
+        """
+        Returns the memo field value
+
+
+        :param payables_id: int
+        :return: StringResult
+        """
+
+        proxy = self.__client.plunet_server.DataPayable30.getMemo
+        response_model = StringResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=payables_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def set_memo(self, payables_id: int, memo: str) -> Result:
+        """
+        Defines the memo field value
 
 
-        :param value_date: datetime
         :param payables_id: int
+        :param memo: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.setValueDate
+        proxy = self.__client.plunet_server.DataPayable30.setMemo
         response_model = Result
 
-        arg = {"valueDate": value_date, "payablesID": payables_id}
+        arg = {"payablesID": payables_id, "memo": memo}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_resource_id(self, payables_id: int) -> IntegerResult:
+    def get_company_code(self, payables_id: int) -> IntegerResult:
         """
-        Returns the resourceID the payment is related to.
+        Returns the type dependent company code, related to the specified
+        invoice.
 
 
         :param payables_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getResourceID
+        proxy = self.__client.plunet_server.DataPayable30.getCompanyCode
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_is_exported(self, payables_id: int) -> BooleanResult:
+    def get_payment_method(self, payables_id: int) -> IntegerResult:
         """
-        Returns if the invoice is already exported.
+        Returns the payment method, represented by its FA value.
+
+        See Admin | Miscellaneous | Payment method | FA value.
 
 
         :param payables_id: int
-        :return: BooleanResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getIsExported
-        response_model = BooleanResult
+        proxy = self.__client.plunet_server.DataPayable30.getPaymentMethod
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
@@ -857,25 +793,47 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_memo(self, payables_id: int) -> StringResult:
+    def set_paid_date(self, payables_id: int, paid_date: datetime) -> Result:
         """
-        Returns the memo field value
+        Defines the date the invoice is payed.
 
 
         :param payables_id: int
-        :return: StringResult
+        :param paid_date: datetime
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getMemo
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataPayable30.setPaidDate
+        response_model = Result
+
+        arg = {"payablesID": payables_id, "paidDate": paid_date}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def get_is_exported(self, payables_id: int) -> BooleanResult:
+        """
+        Returns if the invoice is already exported.
+
+
+        :param payables_id: int
+        :return: BooleanResult
+        """
+
+        proxy = self.__client.plunet_server.DataPayable30.getIsExported
+        response_model = BooleanResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
@@ -895,69 +853,110 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_memo(self, payables_id: int, memo: str) -> Result:
+    def set_status(self, status: int, payables_id: int) -> Result:
         """
-        Defines the memo field value
+        Defines the PayableStatus.
 
 
+        :param status: int
         :param payables_id: int
-        :param memo: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.setMemo
+        proxy = self.__client.plunet_server.DataPayable30.setStatus
         response_model = Result
 
-        arg = {"payablesID": payables_id, "memo": memo}
+        arg = {"Status": status, "payablesID": payables_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_paid_date(self, payables_id: int, paid_date: datetime) -> Result:
+    def get_resource_id(self, payables_id: int) -> IntegerResult:
         """
-        Defines the date the invoice is payed.
+        Returns the resourceID the payment is related to.
 
 
         :param payables_id: int
-        :param paid_date: datetime
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.setPaidDate
-        response_model = Result
+        proxy = self.__client.plunet_server.DataPayable30.getResourceID
+        response_model = IntegerResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=payables_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_price_line_list(self, payables_item_id: int) -> PriceLineListResult:
+        """
+        Returns a list of all job related PriceLine
 
-        arg = {"payablesID": payables_id, "paidDate": paid_date}
+
+        :param payables_item_id: int
+        :return: PriceLineListResult
+        """
+
+        proxy = self.__client.plunet_server.DataPayable30.getPriceLine_List
+        response_model = PriceLineListResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=payables_item_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_price_unit_list(
+        self, language_code: str, service: str
+    ) -> PriceUnitListResult:
+        """
+        Returns a list of priceUnit related to the specified service.
+        Possible services can be obtained over DataAdmin30.getAvailableServices(String, String)
+
+
+        :param language_code: str
+        :param service: str
+        :return: PriceUnitListResult
+        """
+
+        proxy = self.__client.plunet_server.DataPayable30.getPriceUnit_List
+        response_model = PriceUnitListResult
+
+        arg = {"languageCode": language_code, "service": service}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_company_code(self, payables_id: int) -> IntegerResult:
+    def get_status(self, payables_id: int) -> IntegerResult:
         """
-        Returns the type dependent company code, related to the specified
-        invoice.
+        Returns an instance of IntegerResult, which contains the
+        PayableStatus.
 
 
         :param payables_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataPayable30.getCompanyCode
+        proxy = self.__client.plunet_server.DataPayable30.getStatus
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=payables_id,
             response_model=response_model,
             unpack_dict=False,
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_quote30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_quote30.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,314 +17,305 @@
     SearchFilter_Quote,
     StringResult,
     TemplateListResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataQuote30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
-    def add_language_combination(
-        self, source_language: str, target_language: str, quote_id: int
-    ) -> IntegerResult:
+    def get_projectmanager_id(self, quote_id: int) -> IntegerResult:
         """
-        Adds a language combination to the specified quote.
-        All language descriptions were expected in English language or as ISO-Code.
-        Returns an instance of Result.
+        Returns an instance of IntegerResult, which contains the resource id.
 
 
-        :param source_language: str
-        :param target_language: str
         :param quote_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.addLanguageCombination
+        proxy = self.__client.plunet_server.DataQuote30.getProjectmanagerID
         response_model = IntegerResult
 
-        arg = {
-            "sourceLanguage": source_language,
-            "targetLanguage": target_language,
-            "quoteID": quote_id,
-        }
-
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=quote_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_rate(self, quote_id: int) -> DoubleResult:
+    def set_projectmanager_id(self, resource_id: int, quote_id: int) -> Result:
         """
-        Returns an instance of DoubleResult, which contains the rate
+        Sets the resourceID of the project manager to the given quote.
 
 
+        :param resource_id: int
         :param quote_id: int
-        :return: DoubleResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getRate
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataQuote30.setProjectmanagerID
+        response_model = Result
+
+        arg = {"resourceID": resource_id, "quoteID": quote_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=quote_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_request_id(self, quote_id: int) -> IntegerResult:
+    def update(
+        self, quote_in: Union[QuoteIN, dict], enable_null_or_empty_values: bool
+    ) -> Result:
         """
-        Returns an instance of IntegerResult, which contains the requestId
+        updates the quote by the transfered object
+        Use EnableNullOrEmptyValues to decide if Null or empty Strings are saved
+        into Plunet or ignored.
 
 
-        :param quote_id: int
-        :return: IntegerResult
+        :param quote_in: QuoteIN
+        :param enable_null_or_empty_values: bool
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getRequestId
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataQuote30.update
+        response_model = Result
+
+        if type(quote_in) != QuoteIN:
+            quote_in = QuoteIN(**quote_in).dict()
+        else:
+            quote_in = quote_in.dict()
+
+        arg = {
+            "QuoteIN": quote_in,
+            "enableNullOrEmptyValues": enable_null_or_empty_values,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=quote_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_project_name(self, project_name: str, quote_id: int) -> Result:
+    def delete(self, quote_id: int) -> Result:
         """
-        Sets the project name.
+        Method to delete an quote via ID
 
 
-        :param project_name: str
         :param quote_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.setProjectName
+        proxy = self.__client.plunet_server.DataQuote30.delete
         response_model = Result
 
-        arg = {"ProjectName": project_name, "quoteID": quote_id}
-
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=quote_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_subject(self, quote_id: int) -> StringResult:
+    def insert(
+        self,
+    ) -> IntegerResult:
         """
-        Returns an instance of StringResult, which contains the subject.
+        Method to create a new, empty quote.
+        The method will return an instance
+        of IntegerResult, which contains the quote id.
+        Further api calls via this port will maninpulate this quote
+        (except methods with an quote id as parameter ),
+        until another quote is fetched or the session is invalidated.
 
 
-        :param quote_id: int
-        :return: StringResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getSubject
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataQuote30.insert
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=quote_id,
+            argument=None,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_subject(self, subject: str, quote_id: int) -> Result:
+    def search(
+        self, search_filter: Union[SearchFilter_Quote, dict]
+    ) -> IntegerArrayResult:
         """
-        Sets the subject
+        Search implementation to filter for any existing quotes based on
+        specific criteria.
 
 
-        :param subject: str
-        :param quote_id: int
-        :return: Result
+        :param search_filter: SearchFilter_Quote
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.setSubject
-        response_model = Result
+        proxy = self.__client.plunet_server.DataQuote30.search
+        response_model = IntegerArrayResult
 
-        arg = {"subject": subject, "quoteID": quote_id}
+        if type(search_filter) != SearchFilter_Quote:
+            search_filter = SearchFilter_Quote(**search_filter).dict()
+        else:
+            search_filter = search_filter.dict()
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=search_filter,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_project_name(self, quote_id: int) -> StringResult:
+    def get_currency(self, quote_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the project name
+        Returns the currency
 
 
         :param quote_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getProjectName
+        proxy = self.__client.plunet_server.DataQuote30.getCurrency
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=quote_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_request_id(self, quote_id: int, request_id: int) -> Result:
+    def set_customer_id(self, customer_id: int, quote_id: int) -> Result:
         """
-        Method to set the project related request ID.
+        Sets the customerID
 
 
+        :param customer_id: int
         :param quote_id: int
-        :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.setRequestID
+        proxy = self.__client.plunet_server.DataQuote30.setCustomerID
         response_model = Result
 
-        arg = {"quoteID": quote_id, "requestID": request_id}
+        arg = {"customerID": customer_id, "quoteID": quote_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_creation_date(self, quote_id: int) -> DateResult:
+    def set_creation_date(self, date: datetime, quote_id: int) -> Result:
         """
-        Returns an instance of DateResult, which contains the creation date
+        Sets the creation date
 
 
+        :param date: datetime
         :param quote_id: int
-        :return: DateResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getCreationDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataQuote30.setCreationDate
+        response_model = Result
+
+        arg = {"date": date, "quoteID": quote_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=quote_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def update(
-        self, quote_in: Union[QuoteIN, dict], enable_null_or_empty_values: bool
-    ) -> Result:
+    def get_quote_document(self, quote_id: int) -> StringResult:
         """
-        updates the quote by the transfered object
-        Use EnableNullOrEmptyValues to decide if Null or empty Strings are saved
-        into Plunet or ignored.
+        Returns an instance of StringResult, which contains the relative network path to the quote document.
+        Files can also directly be downloaded as file content over
+        DataDocument30.download_Document(String, int, int, String)
 
 
-        :param quote_in: QuoteIN
-        :param enable_null_or_empty_values: bool
-        :return: Result
+        :param quote_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.update
-        response_model = Result
-
-        if type(quote_in) != QuoteIN:
-            quote_in = QuoteIN(**quote_in).dict()
-        else:
-            quote_in = quote_in.dict()
-
-        arg = {
-            "QuoteIN": quote_in,
-            "enableNullOrEmptyValues": enable_null_or_empty_values,
-        }
+        proxy = self.__client.plunet_server.DataQuote30.getQuoteDocument
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=quote_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def delete(self, quote_id: int) -> Result:
+    def get_template_list(
+        self,
+    ) -> TemplateListResult:
         """
-        Method to delete an quote via ID
+        Method returns an instance of TemplateListResult, which contains a list
+        of template objects which can be accessed by the user.
 
 
-        :param quote_id: int
-        :return: Result
+        :return: TemplateListResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.delete
-        response_model = Result
+        proxy = self.__client.plunet_server.DataQuote30.getTemplateList
+        response_model = TemplateListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=quote_id,
+            argument=None,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def insert(
-        self,
-    ) -> IntegerResult:
+    def get_quote_object(self, quote_id: int) -> QuoteResult:
         """
-        Method to create a new, empty quote.
-        The method will return an instance
-        of IntegerResult, which contains the quote id.
-        Further api calls via this port will maninpulate this quote
-        (except methods with an quote id as parameter ),
-        until another quote is fetched or the session is invalidated.
+        Method returns an instance of QuoteResult, which contains an instance of Quote.
 
 
-        :return: IntegerResult
+        :param quote_id: int
+        :return: QuoteResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.insert
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataQuote30.getQuoteObject
+        response_model = QuoteResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=None,
+            argument=quote_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def search(
-        self, search_filter: Union[SearchFilter_Quote, dict]
-    ) -> IntegerArrayResult:
+    def get_quote_object2(self, quote_number: str) -> QuoteResult:
         """
-        Search implementation to filter for any existing quotes based on
-        specific criteria.
+        Method returns an instance of QuoteResult, which contains an instance of Quote.
 
 
-        :param search_filter: SearchFilter_Quote
-        :return: IntegerArrayResult
+        :param quote_number: str
+        :return: QuoteResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.search
-        response_model = IntegerArrayResult
-
-        if type(search_filter) != SearchFilter_Quote:
-            search_filter = SearchFilter_Quote(**search_filter).dict()
-        else:
-            search_filter = search_filter.dict()
+        proxy = self.__client.plunet_server.DataQuote30.getQuoteObject2
+        response_model = QuoteResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=search_filter,
+            argument=quote_number,
             response_model=response_model,
             unpack_dict=False,
         )
 
     def request_order(self, quote_id: int) -> Result:
         """
         Request and order to the provided quoteID
@@ -366,33 +357,118 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=project_class_type,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_currency(self, quote_id: int) -> StringResult:
+    def set_project_status(self, quote_id: int, project_status: int) -> Result:
         """
-        Returns the currency
+        Method allows to set the ArchivStatus to ARCHIVED (3).
+        Other status changes are not supported due to underlying automated workflows.
+        Please note that the current status must be either COMPLETED(6) or COMPLETED_ARCHIVABLE(2).
 
 
         :param quote_id: int
-        :return: StringResult
+        :param project_status: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getCurrency
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataQuote30.setProjectStatus
+        response_model = Result
+
+        arg = {"quoteID": quote_id, "projectStatus": project_status}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def get_project_status(self, quote_id: int) -> IntegerResult:
+        """
+        Returns an instance of IntegerResult, which contains the
+        ArchivStatus.
+
+
+        :param quote_id: int
+        :return: IntegerResult
+        """
+
+        proxy = self.__client.plunet_server.DataQuote30.getProjectStatus
+        response_model = IntegerResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=quote_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def set_status(self, status: int, quote_id: int) -> Result:
+        """
+        Sets the QuoteStatusType.
+
+
+        :param status: int
+        :param quote_id: int
+        :return: Result
+        """
+
+        proxy = self.__client.plunet_server.DataQuote30.setStatus
+        response_model = Result
+
+        arg = {"Status": status, "quoteID": quote_id}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def get_customer_id(self, quote_id: int) -> IntegerResult:
+        """
+        Returns an instance of customer id, which contains the customer id
+
+
+        :param quote_id: int
+        :return: IntegerResult
+        """
+
+        proxy = self.__client.plunet_server.DataQuote30.getCustomerID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=quote_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
+    def get_quote_id(self, display_no: str) -> IntegerResult:
+        """
+        Method returns an instance of IntegerResult, which contains the Quote ID.
+
+
+        :param display_no: str
+        :return: IntegerResult
+        """
+
+        proxy = self.__client.plunet_server.DataQuote30.getQuoteID
+        response_model = IntegerResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=display_no,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
     def set_reference_number(self, quote_id: int, reference: str) -> Result:
         """
         Method set reference number for quote by quoteID.
 
 
         :param quote_id: int
         :param reference: str
@@ -468,181 +544,101 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_customer_id(self, customer_id: int, quote_id: int) -> Result:
-        """
-        Sets the customerID
-
-
-        :param customer_id: int
-        :param quote_id: int
-        :return: Result
+    def get_order_id_first_item(self, quote_id: int) -> IntegerResult:
         """
+        If the currently selected quote is already changed to an order, this
+        method returns the order ID by checking the first quote item.
 
-        proxy = self.__client.plunet_server.DataQuote30.setCustomerID
-        response_model = Result
-
-        arg = {"customerID": customer_id, "quoteID": quote_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def deregister_callback_observer(self, quote_id: int) -> Result:
-        """
-        Deletes a observer.
-        observer can only deleted by the user who has created them.
+        Returns an instance of IntegerResult.
 
 
         :param quote_id: int
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.deregisterCallback_Observer
-        response_model = Result
+        proxy = self.__client.plunet_server.DataQuote30.getOrderIDFirstItem
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=quote_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def register_callback_notify(
-        self,
-        server_authentication_string: str,
-        server_address: str,
-        event_type: Union[EventType, int],
-    ) -> Result:
+    def get_quote_no_for_view(self, quote_id: int) -> StringResult:
         """
-        Register to get notified when the specified EventType occurs
-        for any quote.
-
-        If the EventType occurs PBM will call the callback web service,
-        which is hosted within your environment. Please check
-        CallbackQuote30 for the exact specification for this service.
-        (each user can only create one notifier per event)
-
-
-        The  must match one of the following formats:
-
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
-
-        In the first two cases, the address will be autocompleted by appending
-        the corresponding directory "CallbackQuote30?wsdl".
-
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+        Returns an instance of StringResult, which contains the formatted quote number,
+        which appears in the forms used by BusinessManager.
 
 
-        :param server_authentication_string: str
-        :param server_address: str
-        :param event_type: EventType
-        :return: Result
+        :param quote_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.registerCallback_Notify
-        response_model = Result
-
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
-        else:
-            event_type = int(event_type)
-
-        arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "EventType": event_type,
-        }
+        proxy = self.__client.plunet_server.DataQuote30.getQuoteNo_for_View
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=quote_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
+    def get_quote_object_list(
+        self, quote_id_list: Union[IntegerList, dict]
+    ) -> QuoteListResult:
         """
-        Deletes an already registered notify request
-        (notify requests can only be deleted by the user who has created them)
+        Method returns an instance of QuoteListResult, which contains a list of quote objects.
 
 
-        :param event_type: EventType
-        :return: Result
+        :param quote_id_list: IntegerList
+        :return: QuoteListResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.deregisterCallback_Notify
-        response_model = Result
+        proxy = self.__client.plunet_server.DataQuote30.getQuoteObjectList
+        response_model = QuoteListResult
 
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
+        if type(quote_id_list) != IntegerList:
+            quote_id_list = IntegerList(**quote_id_list).dict()
         else:
-            event_type = int(event_type)
+            quote_id_list = quote_id_list.dict()
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=event_type,
+            argument=quote_id_list,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def register_callback_observer(
-        self, server_authentication_string: str, server_address: str, quote_id: int
-    ) -> Result:
+    def create_quote_document(
+        self, template: str, format_id: int, quote_id: int
+    ) -> StringResult:
         """
-        Register to observe a specific object for any supported
-        EventType.
-
-        As soon as any supported event occurs, PBM will call the callback web
-        service, which is hosted within your environment. Please check
-        CallbackQuote30 for the exact specification for this service.
-        (each user can only create one observer per id)
-
-
-        The  must match one of the following formats:
-
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
-
-        In the first two cases, the address will be autocompleted by appending
-        the corresponding directory "CallbackQuote30?wsdl".
-
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+        Method creates a quote document as rtf-file and returns the unc path where the file is located.
+        Files can also directly be uploaded as file content over
+        DataDocument30.upload_Document(String, int, int, byte[], String, long)
 
 
-        :param server_authentication_string: str
-        :param server_address: str
+        :param template: str
+        :param format_id: int
         :param quote_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.registerCallback_Observer
-        response_model = Result
+        proxy = self.__client.plunet_server.DataQuote30.createQuoteDocument
+        response_model = StringResult
 
-        arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "QuoteID": quote_id,
-        }
+        arg = {"template": template, "formatId": format_id, "quoteID": quote_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
@@ -675,33 +671,14 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_reference_number(self, quote_id: int) -> StringResult:
-        """
-        Method returns the reference number by quote ID.
-
-
-        :param quote_id: int
-        :return: StringResult
-        """
-
-        proxy = self.__client.plunet_server.DataQuote30.getReferenceNumber
-        response_model = StringResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=quote_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
     def get_project_manager_memo(self, quote_id: int) -> StringResult:
         """
         Method returns project-manager memo for order by quoteID.
 
 
         :param quote_id: int
         :return: StringResult
@@ -735,475 +712,497 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_status(self, quote_id: int) -> IntegerResult:
+    def get_reference_number(self, quote_id: int) -> StringResult:
         """
-        Returns an instance of IntegerResult, which contains the QuoteStatusType.
+        Method returns the reference number by quote ID.
 
 
         :param quote_id: int
-        :return: IntegerResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getStatus
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataQuote30.getReferenceNumber
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=quote_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_status(self, status: int, quote_id: int) -> Result:
-        """
-        Sets the QuoteStatusType.
-
-
-        :param status: int
-        :param quote_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataQuote30.setStatus
-        response_model = Result
-
-        arg = {"Status": status, "quoteID": quote_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def get_projectmanager_id(self, quote_id: int) -> IntegerResult:
+    def get_status(self, quote_id: int) -> IntegerResult:
         """
-        Returns an instance of IntegerResult, which contains the resource id.
+        Returns an instance of IntegerResult, which contains the QuoteStatusType.
 
 
         :param quote_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getProjectmanagerID
+        proxy = self.__client.plunet_server.DataQuote30.getStatus
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=quote_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_projectmanager_id(self, resource_id: int, quote_id: int) -> Result:
+    def set_external_id(self, quote_id: int, external_id: str) -> Result:
         """
-        Sets the resourceID of the project manager to the given quote.
+        Methode set External ID for Quote by quoteID
 
 
-        :param resource_id: int
         :param quote_id: int
+        :param external_id: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.setProjectmanagerID
+        proxy = self.__client.plunet_server.DataQuote30.setExternalID
         response_model = Result
 
-        arg = {"resourceID": resource_id, "quoteID": quote_id}
+        arg = {"quoteID": quote_id, "externalID": external_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_template_list(
-        self,
-    ) -> TemplateListResult:
+    def insert2(self, quote_in: Union[QuoteIN, dict]) -> IntegerResult:
         """
-        Method returns an instance of TemplateListResult, which contains a list
-        of template objects which can be accessed by the user.
+        Method to create a quote depending on the transfered object
 
 
-        :return: TemplateListResult
+        :param quote_in: QuoteIN
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getTemplateList
-        response_model = TemplateListResult
+        proxy = self.__client.plunet_server.DataQuote30.insert2
+        response_model = IntegerResult
+
+        if type(quote_in) != QuoteIN:
+            quote_in = QuoteIN(**quote_in).dict()
+        else:
+            quote_in = quote_in.dict()
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=None,
+            argument=quote_in,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_customer_contact_id(
-        self, customer_contact_id: int, quote_id: int
-    ) -> Result:
+    def get_external_id(self, quote_id: int) -> StringResult:
         """
-        Sets the customer contact ID for the currently selected project.
+        Method retuns ExternalID from Qute by quoteID
 
 
-        :param customer_contact_id: int
         :param quote_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.setCustomerContactID
-        response_model = Result
-
-        arg = {"customerContactID": customer_contact_id, "quoteID": quote_id}
+        proxy = self.__client.plunet_server.DataQuote30.getExternalID
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=quote_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_customer_contact_id(self, quote_id: int) -> IntegerResult:
+    def get_request_id(self, quote_id: int) -> IntegerResult:
         """
-        Returns an instance of IntegerResult, which contains the customer
-        contact id.
+        Returns an instance of IntegerResult, which contains the requestId
 
 
         :param quote_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getCustomerContactID
+        proxy = self.__client.plunet_server.DataQuote30.getRequestId
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=quote_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_project_status(self, quote_id: int, project_status: int) -> Result:
+    def set_request_id(self, quote_id: int, request_id: int) -> Result:
         """
-        Method allows to set the ArchivStatus to ARCHIVED (3).
-        Other status changes are not supported due to underlying automated workflows.
-        Please note that the current status must be either COMPLETED(6) or COMPLETED_ARCHIVABLE(2).
+        Method to set the project related request ID.
 
 
         :param quote_id: int
-        :param project_status: int
+        :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.setProjectStatus
+        proxy = self.__client.plunet_server.DataQuote30.setRequestID
         response_model = Result
 
-        arg = {"quoteID": quote_id, "projectStatus": project_status}
+        arg = {"quoteID": quote_id, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_project_status(self, quote_id: int) -> IntegerResult:
+    def set_project_name(self, project_name: str, quote_id: int) -> Result:
         """
-        Returns an instance of IntegerResult, which contains the
-        ArchivStatus.
+        Sets the project name.
 
 
+        :param project_name: str
         :param quote_id: int
-        :return: IntegerResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getProjectStatus
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataQuote30.setProjectName
+        response_model = Result
+
+        arg = {"ProjectName": project_name, "quoteID": quote_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=quote_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_quote_object(self, quote_id: int) -> QuoteResult:
+    def get_project_name(self, quote_id: int) -> StringResult:
         """
-        Method returns an instance of QuoteResult, which contains an instance of Quote.
+        Returns an instance of StringResult, which contains the project name
 
 
         :param quote_id: int
-        :return: QuoteResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getQuoteObject
-        response_model = QuoteResult
+        proxy = self.__client.plunet_server.DataQuote30.getProjectName
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=quote_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_quote_document(self, quote_id: int) -> StringResult:
+    def get_subject(self, quote_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the relative network path to the quote document.
-        Files can also directly be downloaded as file content over
-        DataDocument30.download_Document(String, int, int, String)
+        Returns an instance of StringResult, which contains the subject.
 
 
         :param quote_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getQuoteDocument
+        proxy = self.__client.plunet_server.DataQuote30.getSubject
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=quote_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_creation_date(self, date: datetime, quote_id: int) -> Result:
+    def set_subject(self, subject: str, quote_id: int) -> Result:
         """
-        Sets the creation date
+        Sets the subject
 
 
-        :param date: datetime
+        :param subject: str
         :param quote_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.setCreationDate
+        proxy = self.__client.plunet_server.DataQuote30.setSubject
         response_model = Result
 
-        arg = {"date": date, "quoteID": quote_id}
+        arg = {"subject": subject, "quoteID": quote_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_quote_object2(self, quote_number: str) -> QuoteResult:
+    def get_creation_date(self, quote_id: int) -> DateResult:
         """
-        Method returns an instance of QuoteResult, which contains an instance of Quote.
+        Returns an instance of DateResult, which contains the creation date
 
 
-        :param quote_number: str
-        :return: QuoteResult
+        :param quote_id: int
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getQuoteObject2
-        response_model = QuoteResult
+        proxy = self.__client.plunet_server.DataQuote30.getCreationDate
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=quote_number,
+            argument=quote_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_order_id_first_item(self, quote_id: int) -> IntegerResult:
+    def get_rate(self, quote_id: int) -> DoubleResult:
         """
-        If the currently selected quote is already changed to an order, this
-        method returns the order ID by checking the first quote item.
-
-        Returns an instance of IntegerResult.
+        Returns an instance of DoubleResult, which contains the rate
 
 
         :param quote_id: int
-        :return: IntegerResult
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getOrderIDFirstItem
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataQuote30.getRate
+        response_model = DoubleResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=quote_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_quote_no_for_view(self, quote_id: int) -> StringResult:
+    def set_customer_contact_id(
+        self, customer_contact_id: int, quote_id: int
+    ) -> Result:
         """
-        Returns an instance of StringResult, which contains the formatted quote number,
-        which appears in the forms used by BusinessManager.
+        Sets the customer contact ID for the currently selected project.
 
 
+        :param customer_contact_id: int
         :param quote_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getQuoteNo_for_View
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataQuote30.setCustomerContactID
+        response_model = Result
+
+        arg = {"customerContactID": customer_contact_id, "quoteID": quote_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=quote_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_quote_object_list(
-        self, quote_id_list: Union[IntegerList, dict]
-    ) -> QuoteListResult:
+    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
         """
-        Method returns an instance of QuoteListResult, which contains a list of quote objects.
+        Deletes an already registered notify request
+        (notify requests can only be deleted by the user who has created them)
 
 
-        :param quote_id_list: IntegerList
-        :return: QuoteListResult
+        :param event_type: EventType
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getQuoteObjectList
-        response_model = QuoteListResult
+        proxy = self.__client.plunet_server.DataQuote30.deregisterCallback_Notify
+        response_model = Result
 
-        if type(quote_id_list) != IntegerList:
-            quote_id_list = IntegerList(**quote_id_list).dict()
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
         else:
-            quote_id_list = quote_id_list.dict()
+            event_type = int(event_type)
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=quote_id_list,
+            argument=event_type,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def create_quote_document(
-        self, template: str, format_id: int, quote_id: int
-    ) -> StringResult:
+    def register_callback_notify(
+        self,
+        server_authentication_string: str,
+        server_address: str,
+        event_type: Union[EventType, int],
+    ) -> Result:
         """
-        Method creates a quote document as rtf-file and returns the unc path where the file is located.
-        Files can also directly be uploaded as file content over
-        DataDocument30.upload_Document(String, int, int, byte[], String, long)
+        Register to get notified when the specified EventType occurs
+        for any quote.
 
+        If the EventType occurs PBM will call the callback web service,
+        which is hosted within your environment. Please check
+        CallbackQuote30 for the exact specification for this service.
+        (each user can only create one notifier per event)
 
-        :param template: str
-        :param format_id: int
-        :param quote_id: int
-        :return: StringResult
+
+        The  must match one of the following formats:
+
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
+
+        In the first two cases, the address will be autocompleted by appending
+        the corresponding directory "CallbackQuote30?wsdl".
+
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
+
+
+        :param server_authentication_string: str
+        :param server_address: str
+        :param event_type: EventType
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.createQuoteDocument
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataQuote30.registerCallback_Notify
+        response_model = Result
 
-        arg = {"template": template, "formatId": format_id, "quoteID": quote_id}
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
+        else:
+            event_type = int(event_type)
+
+        arg = {
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "EventType": event_type,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def insert2(self, quote_in: Union[QuoteIN, dict]) -> IntegerResult:
+    def register_callback_observer(
+        self, server_authentication_string: str, server_address: str, quote_id: int
+    ) -> Result:
         """
-        Method to create a quote depending on the transfered object
+        Register to observe a specific object for any supported
+        EventType.
 
+        As soon as any supported event occurs, PBM will call the callback web
+        service, which is hosted within your environment. Please check
+        CallbackQuote30 for the exact specification for this service.
+        (each user can only create one observer per id)
 
-        :param quote_in: QuoteIN
-        :return: IntegerResult
-        """
 
-        proxy = self.__client.plunet_server.DataQuote30.insert2
-        response_model = IntegerResult
+        The  must match one of the following formats:
 
-        if type(quote_in) != QuoteIN:
-            quote_in = QuoteIN(**quote_in).dict()
-        else:
-            quote_in = quote_in.dict()
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
 
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=quote_in,
-            response_model=response_model,
-            unpack_dict=False,
-        )
+        In the first two cases, the address will be autocompleted by appending
+        the corresponding directory "CallbackQuote30?wsdl".
 
-    def set_external_id(self, quote_id: int, external_id: str) -> Result:
-        """
-        Methode set External ID for Quote by quoteID
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
 
 
+        :param server_authentication_string: str
+        :param server_address: str
         :param quote_id: int
-        :param external_id: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.setExternalID
+        proxy = self.__client.plunet_server.DataQuote30.registerCallback_Observer
         response_model = Result
 
-        arg = {"quoteID": quote_id, "externalID": external_id}
+        arg = {
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "QuoteID": quote_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_external_id(self, quote_id: int) -> StringResult:
+    def deregister_callback_observer(self, quote_id: int) -> Result:
         """
-        Method retuns ExternalID from Qute by quoteID
+        Deletes a observer.
+        observer can only deleted by the user who has created them.
 
 
         :param quote_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getExternalID
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataQuote30.deregisterCallback_Observer
+        response_model = Result
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=quote_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_quote_id(self, display_no: str) -> IntegerResult:
+    def add_language_combination(
+        self, source_language: str, target_language: str, quote_id: int
+    ) -> IntegerResult:
         """
-        Method returns an instance of IntegerResult, which contains the Quote ID.
+        Adds a language combination to the specified quote.
+        All language descriptions were expected in English language or as ISO-Code.
+        Returns an instance of Result.
 
 
-        :param display_no: str
+        :param source_language: str
+        :param target_language: str
+        :param quote_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getQuoteID
+        proxy = self.__client.plunet_server.DataQuote30.addLanguageCombination
         response_model = IntegerResult
 
+        arg = {
+            "sourceLanguage": source_language,
+            "targetLanguage": target_language,
+            "quoteID": quote_id,
+        }
+
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=display_no,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_customer_id(self, quote_id: int) -> IntegerResult:
+    def get_customer_contact_id(self, quote_id: int) -> IntegerResult:
         """
-        Returns an instance of customer id, which contains the customer id
+        Returns an instance of IntegerResult, which contains the customer
+        contact id.
 
 
         :param quote_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataQuote30.getCustomerID
+        proxy = self.__client.plunet_server.DataQuote30.getCustomerContactID
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=quote_id,
             response_model=response_model,
             unpack_dict=False,
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_request30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_request30.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,105 +17,55 @@
     Result,
     SearchFilter_Request,
     StringResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataRequest30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
-    def add_language_combination(
-        self, source_language: str, target_language: str, request_id: int
-    ) -> Result:
-        """
-        Adds a language combination to the specified request.
-        All language descriptions were expected in english language or as ISO-Code.
-        Returns an instance of Result.
-
-
-        :param source_language: str
-        :param target_language: str
-        :param request_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataRequest30.addLanguageCombination
-        response_model = Result
-
-        arg = {
-            "sourceLanguage": source_language,
-            "targetLanguage": target_language,
-            "requestID": request_id,
-        }
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
-
-    def get_subject(self, request_id: int) -> StringResult:
-        """
-        Returns an instance of StringResult, which contains the subject of the
-        current request and general status information.
-
-
-        :param request_id: int
-        :return: StringResult
-        """
-
-        proxy = self.__client.plunet_server.DataRequest30.getSubject
-        response_model = StringResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=request_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def set_subject(self, subject: str, request_id: int) -> Result:
+    def set_en15038_requested(self, is_en15038: bool, request_id: int) -> Result:
         """
-        Sets the subject of the current request. Returns an instance of Result.
+        Method to mark a request, that the client wants the request to correspond
+        to the EN 10538 standard.
 
 
-        :param subject: str
+        :param is_en15038: bool
         :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setSubject
+        proxy = self.__client.plunet_server.DataRequest30.setEN15038Requested
         response_model = Result
 
-        arg = {"subject": subject, "requestID": request_id}
+        arg = {"isEN15038": is_en15038, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_creation_date(self, request_id: int) -> DateResult:
+    def get_en15038_requested(self, request_id: int) -> BooleanResult:
         """
-        Returns an instance of DateResult, containing the creation date of the specified request.
+        Method returns an instance of BooleanResult, which contains the information,
+        whether the client requests the EN15038 standard.
 
 
         :param request_id: int
-        :return: DateResult
+        :return: BooleanResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getCreationDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataRequest30.getEN15038Requested
+        response_model = BooleanResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
@@ -274,1308 +224,1357 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=search_filter,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_rush_request(self, is_rush_request: bool, request_id: int) -> Result:
+    def add_service(self, service: str, request_id: int) -> Result:
         """
-        Sets the flag for rush request.
+        Adds a service type to the specified request.
+        Service types were expected in english language.
+        Returns an instance of Result.
 
 
-        :param is_rush_request: bool
+        :param service: str
         :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setRushRequest
+        proxy = self.__client.plunet_server.DataRequest30.addService
         response_model = Result
 
-        arg = {"IsRushRequest": is_rush_request, "requestID": request_id}
+        arg = {"service": service, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_type_of_project(self, request_id: int, type_of_project: str) -> Result:
+    def set_customer_id(self, customer_id: int, request_id: int) -> Result:
         """
-        Method to set the type of the project.
-        Info: Type of Project does not displays the standard project-types like
-        order, request... and can be configured within the admin area of
-        business manager.
+        Sets the customer id for the specified request.
 
 
+        :param customer_id: int
         :param request_id: int
-        :param type_of_project: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setTypeOfProject
+        proxy = self.__client.plunet_server.DataRequest30.setCustomerID
         response_model = Result
 
-        arg = {"requestID": request_id, "TypeOfProject": type_of_project}
+        arg = {"customerID": customer_id, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_workflow_id(self, request_id: int) -> IntegerResult:
+    def set_creation_date(self, date: datetime, request_id: int) -> Result:
         """
-        Method to get the workflowID of the specified request
+        Sets the creation date of the specified request.
 
 
+        :param date: datetime
         :param request_id: int
-        :return: IntegerResult
-        """
-
-        proxy = self.__client.plunet_server.DataRequest30.getWorkflowID
-        response_model = IntegerResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=request_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def quote_request(self, request_id: int) -> IntegerResult:
+        :return: Result
         """
-        Method to create a quote from the specified request.
-        Language combinations and items will be created.
-        Also the source/reference files will be copied to the created quote.
-        Returns an instance of IntegerResult, which contains the identifier of the new quote.
-
 
-        :param request_id: int
-        :return: IntegerResult
-        """
+        proxy = self.__client.plunet_server.DataRequest30.setCreationDate
+        response_model = Result
 
-        proxy = self.__client.plunet_server.DataRequest30.quoteRequest
-        response_model = IntegerResult
+        arg = {"date": date, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=request_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_type_of_project(self, request_id: int) -> StringResult:
+    def get_customer_ref_no(self, request_id: int) -> StringResult:
         """
-        Method to get the type of the project
-        Info: Type of Project does not displays the standard project-types like
-        order, request... and can be configured within the admin area of
-        business manager.
+        Method returns an instance of StringResult, which contains the customer
+        reference number of the definied request.
 
 
         :param request_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getTypeOfProject
+        proxy = self.__client.plunet_server.DataRequest30.getCustomerRefNo
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_workflow_id(self, request_id: int, workflow_id: int) -> Result:
+    def set_order_id(self, order_id: int, request_id: int) -> Result:
         """
-        Method to set the workflowID of the specified request
-
-        A workflowID equals -1 will remove the workflow currently set for the
-        request.
+        Deprecated.
 
 
+        :param order_id: int
         :param request_id: int
-        :param workflow_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setWorkflowID
+        proxy = self.__client.plunet_server.DataRequest30.setOrderID
         response_model = Result
 
-        arg = {"requestID": request_id, "workflowID": workflow_id}
+        arg = {"orderID": order_id, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_rush_request(self, request_id: int) -> BooleanResult:
+    def get_order_id_list(self, request_id: int) -> IntegerArrayResult:
         """
-        Returns an instance of StringResult, containing the project name and
-        further status information.
+        Method returns an instance of IntegerArrayResult, containing all order
+        ID's for the specified request.
 
 
         :param request_id: int
-        :return: BooleanResult
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getRushRequest
-        response_model = BooleanResult
+        proxy = self.__client.plunet_server.DataRequest30.getOrderIDList
+        response_model = IntegerArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def order_request_by_template(
-        self, request_id: int, order_template_id: int
-    ) -> IntegerResult:
+    def get_all_requests(
+        self,
+    ) -> IntegerArrayResult:
         """
-        Method to order the specified request, using the transfered template.
-        Language combinations and items will be created.
-        Also the source/reference files will be copied to the created order.
-        Returns an instance of IntegerResult, which contains the identifier of the new order.
-        OrderTemplateID can be 0, to not use any template.
+        Method returns an instance of IntegerArrayResult, which contains a list of request ids.
+        System will search for all request, which were connected to the user, which is currently logged in.
+        For a customer user, this method will return all requests from this customer
 
 
-        :param request_id: int
-        :param order_template_id: int
-        :return: IntegerResult
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.orderRequest_byTemplate
-        response_model = IntegerResult
-
-        arg = {"requestID": request_id, "OrderTemplateID": order_template_id}
+        proxy = self.__client.plunet_server.DataRequest30.getAll_Requests
+        response_model = IntegerArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=None,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def quote_request_by_template(
-        self, request_id: int, quote_template_id: int
-    ) -> IntegerResult:
+    def set_delivery_date(self, date: datetime, request_id: int) -> Result:
         """
-        Method to quote the specified request using the transfered template.
-        Language combinations and items will be created.
-        Also the source/reference files will be copied to the created quote.
-        Returns an instance of IntegerResult, which contains the identifier of the new quote.
-        QuoteTemplateID can be 0, to not use any template.
+        Sets the delivery date of the current request. Returns an instance of Result
 
 
+        :param date: datetime
         :param request_id: int
-        :param quote_template_id: int
-        :return: IntegerResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.quoteRequest_byTemplate
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataRequest30.setDeliveryDate
+        response_model = Result
 
-        arg = {"requestID": request_id, "QuoteTemplateID": quote_template_id}
+        arg = {"date": date, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def add_service(self, service: str, request_id: int) -> Result:
+    def set_customer_ref_no(self, customer_ref_no: str, request_id: int) -> Result:
         """
-        Adds a service type to the specified request.
-        Service types were expected in english language.
-        Returns an instance of Result.
+        Method to set the customer reference number.
 
 
-        :param service: str
+        :param customer_ref_no: str
         :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.addService
+        proxy = self.__client.plunet_server.DataRequest30.setCustomerRefNo
         response_model = Result
 
-        arg = {"service": service, "requestID": request_id}
+        arg = {"CustomerRefNo": customer_ref_no, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_customer_id(self, customer_id: int, request_id: int) -> Result:
+    def set_price(self, price: float, request_id: int) -> Result:
         """
-        Sets the customer id for the specified request.
+        Method to set the price. Returns an instance of Result.
+        This value is available for free use.
 
 
-        :param customer_id: int
+        :param price: float
         :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setCustomerID
+        proxy = self.__client.plunet_server.DataRequest30.setPrice
         response_model = Result
 
-        arg = {"customerID": customer_id, "requestID": request_id}
+        arg = {"price": price, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def deregister_callback_observer(self, request_id: int) -> Result:
+    def get_quotation_date(self, request_id: int) -> DateResult:
         """
-        Deletes an observer
-
-        Observer can only deleted by the user who has created them
+        Returns an instance of DateResult, containing the quotation date of the
+        current request
 
 
         :param request_id: int
-        :return: Result
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.deregisterCallback_Observer
-        response_model = Result
+        proxy = self.__client.plunet_server.DataRequest30.getQuotationDate
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def register_callback_notify(
-        self,
-        server_authentication_string: str,
-        server_address: str,
-        event_type: Union[EventType, int],
-    ) -> Result:
+    def get_delivery_date(self, request_id: int) -> DateResult:
         """
-        Register to get notified when the specified EventType occurs
-        for any request.
-
-        If the EventType occurs PBM will call the callback web service,
-        which is hosted within your environment. Also each user can only create
-        one notify request per event.
-
-        Please check CallbackRequest30 for the exact specification for
-        this service.
+        Returns an instance of DateResult, containing the delivery date of the current request
 
 
-        The  must match one of the following formats:
+        :param request_id: int
+        :return: DateResult
+        """
 
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
+        proxy = self.__client.plunet_server.DataRequest30.getDeliveryDate
+        response_model = DateResult
 
-        In the first two cases, the address will be autocompleted by appending
-        the corresponding directory "CallbackRequest30?wsdl".
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=request_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
 
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+    def set_quotation_date(self, date: datetime, request_id: int) -> Result:
+        """
+        Sets the quotation date of the current request. Returns an instance of Result.
 
 
-        :param server_authentication_string: str
-        :param server_address: str
-        :param event_type: EventType
+        :param date: datetime
+        :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.registerCallback_Notify
+        proxy = self.__client.plunet_server.DataRequest30.setQuotationDate
         response_model = Result
 
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
-        else:
-            event_type = int(event_type)
-
-        arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "EventType": event_type,
-        }
+        arg = {"date": date, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
+    def get_price(self, request_id: int) -> DoubleResult:
         """
-        Deletes an registered notify request
-        Notify requests can only be deleted by the user who has created them.
+        Method returns an instance of DoubleResult, which contains the price of
+        the currently definied request.
 
 
-        :param event_type: EventType
-        :return: Result
+        :param request_id: int
+        :return: DoubleResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.deregisterCallback_Notify
-        response_model = Result
-
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
-        else:
-            event_type = int(event_type)
+        proxy = self.__client.plunet_server.DataRequest30.getPrice
+        response_model = DoubleResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=event_type,
+            argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def register_callback_observer(
-        self, server_authentication_string: str, server_address: str, request_id: int
-    ) -> Result:
+    def order_request(self, request_id: int) -> IntegerResult:
         """
-        Register to observe a specific object for any supported
-        EventType.
-
-        As soon as any supported event occurs, PBM will call the callback web
-        service, which is hosted within your environment.
-
-        Please check CallbackRequest30 for the exact specification for
-        this service.
+        Method to order the specified request.
+        Language combinations and items will be created.
+        Also the source/reference files will be copied to the created order.
+        Returns an instance of IntegerResult, which contains the identifier of the new order.
 
 
-        The  must match one of the following formats:
+        :param request_id: int
+        :return: IntegerResult
+        """
 
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
+        proxy = self.__client.plunet_server.DataRequest30.orderRequest
+        response_model = IntegerResult
 
-        In the first two cases, the address will be autocompleted by appending
-        the corresponding directory "CallbackRequest30?wsdl".
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=request_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
 
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+    def get_quote_id_list(self, request_id: int) -> IntegerArrayResult:
+        """
+        Method returns an instance of IntegerArrayResult, containing all quote
+        ID's for the specified request.
 
 
-        :param server_authentication_string: str
-        :param server_address: str
         :param request_id: int
-        :return: Result
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.registerCallback_Observer
-        response_model = Result
-
-        arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "RequestID": request_id,
-        }
+        proxy = self.__client.plunet_server.DataRequest30.getQuoteIDList
+        response_model = IntegerArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=request_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_master_project_id(self, request_id: int) -> IntegerResult:
+    def get_request_object(self, request_id: int) -> RequestResult:
         """
-        Method to get the MasterProjectID of the specified request
+        Method returns an instance of RequestResult, which contains an instance of Request.
+        Do not loop through an array of requestIDs using this call. Use getRequestObjectList(String, IntegerList) instead.
 
 
         :param request_id: int
-        :return: IntegerResult
+        :return: RequestResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getMasterProjectID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataRequest30.getRequestObject
+        response_model = RequestResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_master_project_id(self, request_id: int, master_project_id: int) -> Result:
+    def set_quote_id(self, quote_id: int, request_id: int) -> Result:
         """
-        Method to set the MasterProjectID of the specified request
+        Deprecated.
 
 
+        :param quote_id: int
         :param request_id: int
-        :param master_project_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setMasterProjectID
+        proxy = self.__client.plunet_server.DataRequest30.setQuoteID
         response_model = Result
 
-        arg = {"requestID": request_id, "MasterProjectID": master_project_id}
+        arg = {"quoteID": quote_id, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_status(self, request_id: int) -> IntegerResult:
+    def quote_request(self, request_id: int) -> IntegerResult:
         """
-        Returns an instance of IntegerResult, which contains the RequestStatusType.
+        Method to create a quote from the specified request.
+        Language combinations and items will be created.
+        Also the source/reference files will be copied to the created quote.
+        Returns an instance of IntegerResult, which contains the identifier of the new quote.
 
 
         :param request_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getStatus
+        proxy = self.__client.plunet_server.DataRequest30.quoteRequest
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_status(self, status: int, request_id: int) -> Result:
+    def get_workflow_id(self, request_id: int) -> IntegerResult:
         """
-        Sets the RequestStatusType. Returns an instance of Result.
+        Method to get the workflowID of the specified request
 
 
-        :param status: int
         :param request_id: int
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setStatus
-        response_model = Result
+        proxy = self.__client.plunet_server.DataRequest30.getWorkflowID
+        response_model = IntegerResult
 
-        arg = {"Status": status, "requestID": request_id}
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=request_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_type_of_project(self, request_id: int) -> StringResult:
+        """
+        Method to get the type of the project
+        Info: Type of Project does not displays the standard project-types like
+        order, request... and can be configured within the admin area of
+        business manager.
+
+
+        :param request_id: int
+        :return: StringResult
+        """
+
+        proxy = self.__client.plunet_server.DataRequest30.getTypeOfProject
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=request_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_brief_description(self, request_id: int) -> StringResult:
+    def get_rush_request(self, request_id: int) -> BooleanResult:
         """
         Returns an instance of StringResult, containing the project name and
         further status information.
 
 
         :param request_id: int
-        :return: StringResult
+        :return: BooleanResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getBriefDescription
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataRequest30.getRushRequest
+        response_model = BooleanResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_brief_description(self, brief_description: str, request_id: int) -> Result:
+    def set_type_of_project(self, request_id: int, type_of_project: str) -> Result:
         """
-        Sets the project name.
+        Method to set the type of the project.
+        Info: Type of Project does not displays the standard project-types like
+        order, request... and can be configured within the admin area of
+        business manager.
 
 
-        :param brief_description: str
         :param request_id: int
+        :param type_of_project: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setBriefDescription
+        proxy = self.__client.plunet_server.DataRequest30.setTypeOfProject
         response_model = Result
 
-        arg = {"briefDescription": brief_description, "requestID": request_id}
+        arg = {"requestID": request_id, "TypeOfProject": type_of_project}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_en15038_requested(self, is_en15038: bool, request_id: int) -> Result:
+    def set_rush_request(self, is_rush_request: bool, request_id: int) -> Result:
         """
-        Method to mark a request, that the client wants the request to correspond
-        to the EN 10538 standard.
+        Sets the flag for rush request.
 
 
-        :param is_en15038: bool
+        :param is_rush_request: bool
         :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setEN15038Requested
+        proxy = self.__client.plunet_server.DataRequest30.setRushRequest
         response_model = Result
 
-        arg = {"isEN15038": is_en15038, "requestID": request_id}
+        arg = {"IsRushRequest": is_rush_request, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_en15038_requested(self, request_id: int) -> BooleanResult:
+    def set_workflow_id(self, request_id: int, workflow_id: int) -> Result:
         """
-        Method returns an instance of BooleanResult, which contains the information,
-        whether the client requests the EN15038 standard.
+        Method to set the workflowID of the specified request
+
+        A workflowID equals -1 will remove the workflow currently set for the
+        request.
 
 
         :param request_id: int
-        :return: BooleanResult
+        :param workflow_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getEN15038Requested
-        response_model = BooleanResult
+        proxy = self.__client.plunet_server.DataRequest30.setWorkflowID
+        response_model = Result
+
+        arg = {"requestID": request_id, "workflowID": workflow_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=request_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_customer_contact_id(
-        self, request_id: int, customer_contact_id: int
-    ) -> Result:
+    def set_status(self, status: int, request_id: int) -> Result:
         """
-        Method to set the customer contact for the specified request.
+        Sets the RequestStatusType. Returns an instance of Result.
 
 
+        :param status: int
         :param request_id: int
-        :param customer_contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setCustomerContactID
+        proxy = self.__client.plunet_server.DataRequest30.setStatus
         response_model = Result
 
-        arg = {"requestID": request_id, "customerContactID": customer_contact_id}
+        arg = {"Status": status, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_customer_contact_id(self, request_id: int) -> IntegerResult:
+    def get_customer_id(self, request_id: int) -> IntegerResult:
         """
-        Method to get the customer contact for the specified request.
+        Returns an instance of IntegerResult, which contains the customer id of
+        the current request and general status information.
 
 
         :param request_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getCustomerContactID
+        proxy = self.__client.plunet_server.DataRequest30.getCustomerID
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_order_id_list(self, request_id: int) -> IntegerArrayResult:
+    def get_order_id(self, request_id: int) -> IntegerResult:
         """
-        Method returns an instance of IntegerArrayResult, containing all order
-        ID's for the specified request.
+        Deprecated.
 
 
         :param request_id: int
-        :return: IntegerArrayResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getOrderIDList
-        response_model = IntegerArrayResult
+        proxy = self.__client.plunet_server.DataRequest30.getOrderID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_delivery_date(self, date: datetime, request_id: int) -> Result:
+    def get_request_id(self, display_no: str) -> IntegerResult:
         """
-        Sets the delivery date of the current request. Returns an instance of Result
+        Method returns an instance of IntegerResult, containing the ID of the current request.
 
 
-        :param date: datetime
-        :param request_id: int
-        :return: Result
+        :param display_no: str
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setDeliveryDate
-        response_model = Result
-
-        arg = {"date": date, "requestID": request_id}
+        proxy = self.__client.plunet_server.DataRequest30.getRequestID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=display_no,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_delivery_date(self, request_id: int) -> DateResult:
+    def get_quote_id(self, request_id: int) -> IntegerResult:
         """
-        Returns an instance of DateResult, containing the delivery date of the current request
+        Deprecated.
 
 
         :param request_id: int
-        :return: DateResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getDeliveryDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataRequest30.getQuoteID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_price(self, price: float, request_id: int) -> Result:
+    def get_word_count(self, request_id: int) -> IntegerResult:
         """
-        Method to set the price. Returns an instance of Result.
-        This value is available for free use.
+        Method returns an instance of IntegerResult, which contains the word
+        count for the currently fetched request.
 
 
-        :param price: float
         :param request_id: int
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setPrice
-        response_model = Result
-
-        arg = {"price": price, "requestID": request_id}
+        proxy = self.__client.plunet_server.DataRequest30.getWordCount
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=request_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_quotation_date(self, date: datetime, request_id: int) -> Result:
+    def set_word_count(self, word_count: int, request_id: int) -> Result:
         """
-        Sets the quotation date of the current request. Returns an instance of Result.
+        Method to set the word count. Returns an instance of Result.
+        This value is available for free use.
 
 
-        :param date: datetime
+        :param word_count: int
         :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setQuotationDate
+        proxy = self.__client.plunet_server.DataRequest30.setWordCount
         response_model = Result
 
-        arg = {"date": date, "requestID": request_id}
+        arg = {"wordCount": word_count, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_customer_ref_no(self, customer_ref_no: str, request_id: int) -> Result:
+    def get_customer_ref_no_prev_order(self, request_id: int) -> StringResult:
         """
-        Method to set the customer reference number.
+        Method returns an instance of StringResult, which contains the
+        customer reference number of the previous order.
 
 
-        :param customer_ref_no: str
         :param request_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setCustomerRefNo
-        response_model = Result
-
-        arg = {"CustomerRefNo": customer_ref_no, "requestID": request_id}
+        proxy = self.__client.plunet_server.DataRequest30.getCustomerRefNo_PrevOrder
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=request_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_quote_id(self, quote_id: int, request_id: int) -> Result:
+    def get_request_no_for_view(self, request_id: int) -> StringResult:
         """
-        Deprecated.
+        Returns an instance of StringResult, containing status information and
+        the formatted request number, which appears in the forms of the
+        BusinessManager ( donât confuse it with the request id, which
+        looks similar to the request number ).
 
 
-        :param quote_id: int
         :param request_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setQuoteID
-        response_model = Result
+        proxy = self.__client.plunet_server.DataRequest30.getRequestNo_for_View
+        response_model = StringResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=request_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def get_request_object2(self, request_number: str) -> RequestResult:
+        """
+        Method returns an instance of RequestResult, which contains an instance of Request.
 
-        arg = {"quoteID": quote_id, "requestID": request_id}
+
+        :param request_number: str
+        :return: RequestResult
+        """
+
+        proxy = self.__client.plunet_server.DataRequest30.getRequestObject2
+        response_model = RequestResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=request_number,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_quote_id_list(self, request_id: int) -> IntegerArrayResult:
+    def get_request_object_list(
+        self, request_id_list: Union[IntegerList, dict]
+    ) -> RequestListResult:
         """
-        Method returns an instance of IntegerArrayResult, containing all quote
-        ID's for the specified request.
+        Method returns an instance of RequestListResult, which contains a list of Request objects.
+        WARNING: This call can cause performance issues. It has been optimized from Plunet version 8.15
 
 
-        :param request_id: int
-        :return: IntegerArrayResult
+        :param request_id_list: IntegerList
+        :return: RequestListResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getQuoteIDList
-        response_model = IntegerArrayResult
+        proxy = self.__client.plunet_server.DataRequest30.getRequestObjectList
+        response_model = RequestListResult
+
+        if type(request_id_list) != IntegerList:
+            request_id_list = IntegerList(**request_id_list).dict()
+        else:
+            request_id_list = request_id_list.dict()
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=request_id,
+            argument=request_id_list,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_creation_date(self, date: datetime, request_id: int) -> Result:
+    def copy_document_to_reference_folder(
+        self, ref_language: str, unc_file_name: str, request_id: int
+    ) -> Result:
         """
-        Sets the creation date of the specified request.
+        Deprecated. Please use DataDocument30.upload_Document(String, int, int, byte[], String, long) instead.
+        Please note that this call is now deactivated by default. For Reactivation please contact Support@plunet.com.
+
+        Copies a file to the reference folder.
+        In general "uncFileName" describes the location of a file, which is
+        located within the local network.Usually the path has the following format:
+        \\ComputerName\SharedFolder\Resource
+        It is also possible to commit an URL (http://... / https://...) to a
+        file on an external server via "uncFileName". The URL must end with the filename.
+        The reference language description is expected in english language or as ISO-Code.
+        Method returns an instance of Result
+        Files can also directly be uploaded as file content over
+        DataDocument30.upload_Document(String, int, int, byte[], String, long)
 
 
-        :param date: datetime
+        :param ref_language: str
+        :param unc_file_name: str
         :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setCreationDate
+        proxy = self.__client.plunet_server.DataRequest30.copyDocument_toReferenceFolder
         response_model = Result
 
-        arg = {"date": date, "requestID": request_id}
+        arg = {
+            "refLanguage": ref_language,
+            "uncFileName": unc_file_name,
+            "requestID": request_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_order_id(self, order_id: int, request_id: int) -> Result:
+    def copy_document_to_source_folder(
+        self, source_language: str, unc_file_name: str, request_id: int
+    ) -> Result:
         """
-        Deprecated.
+        Deprecated. Please use DataDocument30.upload_Document(String, int, int, byte[], String, long) instead.
 
+        Copies a file to the source folder.
+        In general "uncFileName" describes the location of a file, which is located within the local network.
+        Usually the path has the following format:
+        \\ComputerName\SharedFolder\Resource
+        It is also possible to commit an URL (http://... / https://...) to a
+        file on an external server via "uncFileName". The URL must end with the filename.
+        The source language description is expected in english language or as ISO-Code.
+        Returns an instance of Result.
+        Files can also directly be uploaded as file content over
+        DataDocument30.upload_Document(String, int, int, byte[], String, long)
 
-        :param order_id: int
+
+        :param source_language: str
+        :param unc_file_name: str
         :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setOrderID
+        proxy = self.__client.plunet_server.DataRequest30.copyDocument_toSourceFolder
         response_model = Result
 
-        arg = {"orderID": order_id, "requestID": request_id}
+        arg = {
+            "sourceLanguage": source_language,
+            "uncFileName": unc_file_name,
+            "requestID": request_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_quotation_date(self, request_id: int) -> DateResult:
+    def set_customer_ref_no_prev_order(
+        self, customer_ref_no_previous_order: str, request_id: int
+    ) -> Result:
         """
-        Returns an instance of DateResult, containing the quotation date of the
-        current request
+        Method to set the customer reference number of the previous order.
+        Retuns an instance of Result. This value is available for free use.
 
 
+        :param customer_ref_no_previous_order: str
         :param request_id: int
-        :return: DateResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getQuotationDate
-        response_model = DateResult
+        proxy = self.__client.plunet_server.DataRequest30.setCustomerRefNo_PrevOrder
+        response_model = Result
+
+        arg = {
+            "CustomerRefNo_PreviousOrder": customer_ref_no_previous_order,
+            "requestID": request_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=request_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_request_object(self, request_id: int) -> RequestResult:
+    def set_master_project_id(self, request_id: int, master_project_id: int) -> Result:
         """
-        Method returns an instance of RequestResult, which contains an instance of Request.
-        Do not loop through an array of requestIDs using this call. Use getRequestObjectList(String, IntegerList) instead.
+        Method to set the MasterProjectID of the specified request
 
 
         :param request_id: int
-        :return: RequestResult
+        :param master_project_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getRequestObject
-        response_model = RequestResult
+        proxy = self.__client.plunet_server.DataRequest30.setMasterProjectID
+        response_model = Result
+
+        arg = {"requestID": request_id, "MasterProjectID": master_project_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=request_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_customer_ref_no(self, request_id: int) -> StringResult:
+    def get_master_project_id(self, request_id: int) -> IntegerResult:
         """
-        Method returns an instance of StringResult, which contains the customer
-        reference number of the definied request.
+        Method to get the MasterProjectID of the specified request
 
 
         :param request_id: int
-        :return: StringResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getCustomerRefNo
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataRequest30.getMasterProjectID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_price(self, request_id: int) -> DoubleResult:
+    def get_status(self, request_id: int) -> IntegerResult:
         """
-        Method returns an instance of DoubleResult, which contains the price of
-        the currently definied request.
+        Returns an instance of IntegerResult, which contains the RequestStatusType.
 
 
         :param request_id: int
-        :return: DoubleResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getPrice
-        response_model = DoubleResult
+        proxy = self.__client.plunet_server.DataRequest30.getStatus
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def order_request(self, request_id: int) -> IntegerResult:
+    def insert2(self, request_in: Union[RequestIN, dict]) -> IntegerResult:
         """
-        Method to order the specified request.
-        Language combinations and items will be created.
-        Also the source/reference files will be copied to the created order.
-        Returns an instance of IntegerResult, which contains the identifier of the new order.
+        Method to create a quote depending on the transfered object
 
 
-        :param request_id: int
+        :param request_in: RequestIN
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.orderRequest
+        proxy = self.__client.plunet_server.DataRequest30.insert2
         response_model = IntegerResult
 
+        if type(request_in) != RequestIN:
+            request_in = RequestIN(**request_in).dict()
+        else:
+            request_in = request_in.dict()
+
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=request_id,
+            argument=request_in,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_all_requests(
-        self,
-    ) -> IntegerArrayResult:
+    def get_subject(self, request_id: int) -> StringResult:
         """
-        Method returns an instance of IntegerArrayResult, which contains a list of request ids.
-        System will search for all request, which were connected to the user, which is currently logged in.
-        For a customer user, this method will return all requests from this customer
+        Returns an instance of StringResult, which contains the subject of the
+        current request and general status information.
 
 
-        :return: IntegerArrayResult
+        :param request_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getAll_Requests
-        response_model = IntegerArrayResult
+        proxy = self.__client.plunet_server.DataRequest30.getSubject
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=None,
+            argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_customer_ref_no_prev_order(
-        self, customer_ref_no_previous_order: str, request_id: int
-    ) -> Result:
+    def set_subject(self, subject: str, request_id: int) -> Result:
         """
-        Method to set the customer reference number of the previous order.
-        Retuns an instance of Result. This value is available for free use.
+        Sets the subject of the current request. Returns an instance of Result.
 
 
-        :param customer_ref_no_previous_order: str
+        :param subject: str
         :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setCustomerRefNo_PrevOrder
+        proxy = self.__client.plunet_server.DataRequest30.setSubject
         response_model = Result
 
-        arg = {
-            "CustomerRefNo_PreviousOrder": customer_ref_no_previous_order,
-            "requestID": request_id,
-        }
+        arg = {"subject": subject, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_customer_ref_no_prev_order(self, request_id: int) -> StringResult:
+    def get_creation_date(self, request_id: int) -> DateResult:
         """
-        Method returns an instance of StringResult, which contains the
-        customer reference number of the previous order.
+        Returns an instance of DateResult, containing the creation date of the specified request.
 
 
         :param request_id: int
-        :return: StringResult
+        :return: DateResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getCustomerRefNo_PrevOrder
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataRequest30.getCreationDate
+        response_model = DateResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def copy_document_to_reference_folder(
-        self, ref_language: str, unc_file_name: str, request_id: int
+    def set_customer_contact_id(
+        self, request_id: int, customer_contact_id: int
     ) -> Result:
         """
-        Deprecated. Please use DataDocument30.upload_Document(String, int, int, byte[], String, long) instead.
-        Please note that this call is now deactivated by default. For Reactivation please contact Support@plunet.com.
-
-        Copies a file to the reference folder.
-        In general "uncFileName" describes the location of a file, which is
-        located within the local network.Usually the path has the following format:
-        \\ComputerName\SharedFolder\Resource
-        It is also possible to commit an URL (http://... / https://...) to a
-        file on an external server via "uncFileName". The URL must end with the filename.
-        The reference language description is expected in english language or as ISO-Code.
-        Method returns an instance of Result
-        Files can also directly be uploaded as file content over
-        DataDocument30.upload_Document(String, int, int, byte[], String, long)
+        Method to set the customer contact for the specified request.
 
 
-        :param ref_language: str
-        :param unc_file_name: str
         :param request_id: int
+        :param customer_contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.copyDocument_toReferenceFolder
+        proxy = self.__client.plunet_server.DataRequest30.setCustomerContactID
         response_model = Result
 
-        arg = {
-            "refLanguage": ref_language,
-            "uncFileName": unc_file_name,
-            "requestID": request_id,
-        }
+        arg = {"requestID": request_id, "customerContactID": customer_contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def copy_document_to_source_folder(
-        self, source_language: str, unc_file_name: str, request_id: int
-    ) -> Result:
+    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
         """
-        Deprecated. Please use DataDocument30.upload_Document(String, int, int, byte[], String, long) instead.
-
-        Copies a file to the source folder.
-        In general "uncFileName" describes the location of a file, which is located within the local network.
-        Usually the path has the following format:
-        \\ComputerName\SharedFolder\Resource
-        It is also possible to commit an URL (http://... / https://...) to a
-        file on an external server via "uncFileName". The URL must end with the filename.
-        The source language description is expected in english language or as ISO-Code.
-        Returns an instance of Result.
-        Files can also directly be uploaded as file content over
-        DataDocument30.upload_Document(String, int, int, byte[], String, long)
+        Deletes an registered notify request
+        Notify requests can only be deleted by the user who has created them.
 
 
-        :param source_language: str
-        :param unc_file_name: str
-        :param request_id: int
+        :param event_type: EventType
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.copyDocument_toSourceFolder
+        proxy = self.__client.plunet_server.DataRequest30.deregisterCallback_Notify
         response_model = Result
 
-        arg = {
-            "sourceLanguage": source_language,
-            "uncFileName": unc_file_name,
-            "requestID": request_id,
-        }
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
+        else:
+            event_type = int(event_type)
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=event_type,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_request_object2(self, request_number: str) -> RequestResult:
+    def register_callback_notify(
+        self,
+        server_authentication_string: str,
+        server_address: str,
+        event_type: Union[EventType, int],
+    ) -> Result:
         """
-        Method returns an instance of RequestResult, which contains an instance of Request.
+        Register to get notified when the specified EventType occurs
+        for any request.
 
+        If the EventType occurs PBM will call the callback web service,
+        which is hosted within your environment. Also each user can only create
+        one notify request per event.
 
-        :param request_number: str
-        :return: RequestResult
+        Please check CallbackRequest30 for the exact specification for
+        this service.
+
+
+        The  must match one of the following formats:
+
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
+
+        In the first two cases, the address will be autocompleted by appending
+        the corresponding directory "CallbackRequest30?wsdl".
+
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
+
+
+        :param server_authentication_string: str
+        :param server_address: str
+        :param event_type: EventType
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getRequestObject2
-        response_model = RequestResult
+        proxy = self.__client.plunet_server.DataRequest30.registerCallback_Notify
+        response_model = Result
+
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
+        else:
+            event_type = int(event_type)
+
+        arg = {
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "EventType": event_type,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=request_number,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_request_no_for_view(self, request_id: int) -> StringResult:
+    def register_callback_observer(
+        self, server_authentication_string: str, server_address: str, request_id: int
+    ) -> Result:
         """
-        Returns an instance of StringResult, containing status information and
-        the formatted request number, which appears in the forms of the
-        BusinessManager ( donât confuse it with the request id, which
-        looks similar to the request number ).
+        Register to observe a specific object for any supported
+        EventType.
+
+        As soon as any supported event occurs, PBM will call the callback web
+        service, which is hosted within your environment.
 
+        Please check CallbackRequest30 for the exact specification for
+        this service.
 
+
+        The  must match one of the following formats:
+
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
+
+        In the first two cases, the address will be autocompleted by appending
+        the corresponding directory "CallbackRequest30?wsdl".
+
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
+
+
+        :param server_authentication_string: str
+        :param server_address: str
         :param request_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getRequestNo_for_View
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataRequest30.registerCallback_Observer
+        response_model = Result
+
+        arg = {
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "RequestID": request_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=request_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_request_object_list(
-        self, request_id_list: Union[IntegerList, dict]
-    ) -> RequestListResult:
+    def deregister_callback_observer(self, request_id: int) -> Result:
         """
-        Method returns an instance of RequestListResult, which contains a list of Request objects.
-        WARNING: This call can cause performance issues. It has been optimized from Plunet version 8.15
+        Deletes an observer
 
+        Observer can only deleted by the user who has created them
 
-        :param request_id_list: IntegerList
-        :return: RequestListResult
-        """
 
-        proxy = self.__client.plunet_server.DataRequest30.getRequestObjectList
-        response_model = RequestListResult
+        :param request_id: int
+        :return: Result
+        """
 
-        if type(request_id_list) != IntegerList:
-            request_id_list = IntegerList(**request_id_list).dict()
-        else:
-            request_id_list = request_id_list.dict()
+        proxy = self.__client.plunet_server.DataRequest30.deregisterCallback_Observer
+        response_model = Result
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=request_id_list,
+            argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def insert2(self, request_in: Union[RequestIN, dict]) -> IntegerResult:
+    def get_brief_description(self, request_id: int) -> StringResult:
         """
-        Method to create a quote depending on the transfered object
+        Returns an instance of StringResult, containing the project name and
+        further status information.
 
 
-        :param request_in: RequestIN
-        :return: IntegerResult
+        :param request_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.insert2
-        response_model = IntegerResult
-
-        if type(request_in) != RequestIN:
-            request_in = RequestIN(**request_in).dict()
-        else:
-            request_in = request_in.dict()
+        proxy = self.__client.plunet_server.DataRequest30.getBriefDescription
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=request_in,
+            argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_word_count(self, word_count: int, request_id: int) -> Result:
+    def set_brief_description(self, brief_description: str, request_id: int) -> Result:
         """
-        Method to set the word count. Returns an instance of Result.
-        This value is available for free use.
+        Sets the project name.
 
 
-        :param word_count: int
+        :param brief_description: str
         :param request_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.setWordCount
+        proxy = self.__client.plunet_server.DataRequest30.setBriefDescription
         response_model = Result
 
-        arg = {"wordCount": word_count, "requestID": request_id}
+        arg = {"briefDescription": brief_description, "requestID": request_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_word_count(self, request_id: int) -> IntegerResult:
+    def add_language_combination(
+        self, source_language: str, target_language: str, request_id: int
+    ) -> Result:
         """
-        Method returns an instance of IntegerResult, which contains the word
-        count for the currently fetched request.
+        Adds a language combination to the specified request.
+        All language descriptions were expected in english language or as ISO-Code.
+        Returns an instance of Result.
 
 
+        :param source_language: str
+        :param target_language: str
         :param request_id: int
-        :return: IntegerResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getWordCount
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataRequest30.addLanguageCombination
+        response_model = Result
+
+        arg = {
+            "sourceLanguage": source_language,
+            "targetLanguage": target_language,
+            "requestID": request_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=request_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_quote_id(self, request_id: int) -> IntegerResult:
+    def order_request_by_template(
+        self, request_id: int, order_template_id: int
+    ) -> IntegerResult:
         """
-        Deprecated.
+        Method to order the specified request, using the transfered template.
+        Language combinations and items will be created.
+        Also the source/reference files will be copied to the created order.
+        Returns an instance of IntegerResult, which contains the identifier of the new order.
+        OrderTemplateID can be 0, to not use any template.
 
 
         :param request_id: int
+        :param order_template_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getQuoteID
+        proxy = self.__client.plunet_server.DataRequest30.orderRequest_byTemplate
         response_model = IntegerResult
 
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=request_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def get_request_id(self, display_no: str) -> IntegerResult:
-        """
-        Method returns an instance of IntegerResult, containing the ID of the current request.
-
-
-        :param display_no: str
-        :return: IntegerResult
-        """
-
-        proxy = self.__client.plunet_server.DataRequest30.getRequestID
-        response_model = IntegerResult
+        arg = {"requestID": request_id, "OrderTemplateID": order_template_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=display_no,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_order_id(self, request_id: int) -> IntegerResult:
+    def quote_request_by_template(
+        self, request_id: int, quote_template_id: int
+    ) -> IntegerResult:
         """
-        Deprecated.
+        Method to quote the specified request using the transfered template.
+        Language combinations and items will be created.
+        Also the source/reference files will be copied to the created quote.
+        Returns an instance of IntegerResult, which contains the identifier of the new quote.
+        QuoteTemplateID can be 0, to not use any template.
 
 
         :param request_id: int
+        :param quote_template_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getOrderID
+        proxy = self.__client.plunet_server.DataRequest30.quoteRequest_byTemplate
         response_model = IntegerResult
 
+        arg = {"requestID": request_id, "QuoteTemplateID": quote_template_id}
+
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=request_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_customer_id(self, request_id: int) -> IntegerResult:
+    def get_customer_contact_id(self, request_id: int) -> IntegerResult:
         """
-        Returns an instance of IntegerResult, which contains the customer id of
-        the current request and general status information.
+        Method to get the customer contact for the specified request.
 
 
         :param request_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataRequest30.getCustomerID
+        proxy = self.__client.plunet_server.DataRequest30.getCustomerContactID
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_resource30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_resource30.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,18 @@
     Result,
     SearchFilter_Resource,
     StringResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataResource30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
     def update(
         self, resource_in: Union[ResourceIN, dict], enable_null_or_empty_values: bool
     ) -> Result:
         """
         Updates a resource per Object.
@@ -185,14 +184,34 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
+    def get_full_name(self, resource_id: int) -> StringResult:
+        """
+        Returns an instance of StringResult, which contains the full name
+        depending on the resourceID .
+
+
+        :param resource_id: int
+        :return: StringResult
+        """
+
+        proxy = self.__client.plunet_server.DataResource30.getFullName
+        response_model = StringResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=resource_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
     def set_supervisor1(self, login_name: str, resource_id: int) -> Result:
         """
         Method to set the supervisor 1.
 
 
         :param login_name: str
         :param resource_id: int
@@ -207,34 +226,66 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_supervisor1(self, resource_id: int) -> StringResult:
+    def get_working_status(self, resource_id: int) -> IntegerResult:
         """
-        Returns an instance of StringResult, which contains the loginname
-        of the supervisor 1.
+        Returns an instance of IntegerResult, which contains the
+        WorkingStatus of the currently fetched resource.
 
 
         :param resource_id: int
-        :return: StringResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getSupervisor1
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResource30.getWorkingStatus
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
+    def set_resource_type(
+        self, resource_type: Union[ResourceType, int], resource_id: int
+    ) -> Result:
+        """
+        Method to set the ResourceType. Returns an instance of
+        Result.
+
+
+        :param resource_type: ResourceType
+        :param resource_id: int
+        :return: Result
+        """
+
+        proxy = self.__client.plunet_server.DataResource30.setResourceType
+        response_model = Result
+
+        if type(resource_type) == ResourceType:
+            resource_type = resource_type.value
+        elif type(resource_type) == int:
+            resource_type = resource_type
+        else:
+            resource_type = int(resource_type)
+
+        arg = {"ResourceType": resource_type, "resourceID": resource_id}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
     def set_supervisor2(self, login_name: str, resource_id: int) -> Result:
         """
         Method to set the supervisor 2.
 
 
         :param login_name: str
         :param resource_id: int
@@ -249,81 +300,71 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_supervisor2(self, resource_id: int) -> StringResult:
+    def get_supervisor1(self, resource_id: int) -> StringResult:
         """
         Returns an instance of StringResult, which contains the loginname
-        of the supervisor 2.
+        of the supervisor 1.
 
 
         :param resource_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getSupervisor2
+        proxy = self.__client.plunet_server.DataResource30.getSupervisor1
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_resource_type(self, resource_id: int) -> IntegerResult:
+    def get_supervisor2(self, resource_id: int) -> StringResult:
         """
-        Returns the ResourceType of the selected resource.
+        Returns an instance of StringResult, which contains the loginname
+        of the supervisor 2.
 
 
         :param resource_id: int
-        :return: IntegerResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getResourceType
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataResource30.getSupervisor2
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_pricelists2(
-        self, sourcelanguage: str, targetlanguage: str, resource_id: int
-    ) -> PricelistListResult:
+    def get_resource_type(self, resource_id: int) -> IntegerResult:
         """
-        Method to get all pricelists from a resource, depending on source and/or
-        target-language.
+        Returns the ResourceType of the selected resource.
 
 
-        :param sourcelanguage: str
-        :param targetlanguage: str
         :param resource_id: int
-        :return: PricelistListResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getPricelists2
-        response_model = PricelistListResult
-
-        arg = {
-            "sourcelanguage": sourcelanguage,
-            "targetlanguage": targetlanguage,
-            "resourceID": resource_id,
-        }
+        proxy = self.__client.plunet_server.DataResource30.getResourceType
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=resource_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
     def set_working_status(
         self, working_status: Union[WorkingStatus, int], resource_id: int
     ) -> Result:
         """
         Method to set the WorkingStatus. Returns an instance of
@@ -350,58 +391,36 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_working_status(self, resource_id: int) -> IntegerResult:
-        """
-        Returns an instance of IntegerResult, which contains the
-        WorkingStatus of the currently fetched resource.
-
-
-        :param resource_id: int
-        :return: IntegerResult
-        """
-
-        proxy = self.__client.plunet_server.DataResource30.getWorkingStatus
-        response_model = IntegerResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=resource_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def set_resource_type(
-        self, resource_type: Union[ResourceType, int], resource_id: int
-    ) -> Result:
+    def get_pricelists2(
+        self, sourcelanguage: str, targetlanguage: str, resource_id: int
+    ) -> PricelistListResult:
         """
-        Method to set the ResourceType. Returns an instance of
-        Result.
+        Method to get all pricelists from a resource, depending on source and/or
+        target-language.
 
 
-        :param resource_type: ResourceType
+        :param sourcelanguage: str
+        :param targetlanguage: str
         :param resource_id: int
-        :return: Result
+        :return: PricelistListResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setResourceType
-        response_model = Result
-
-        if type(resource_type) == ResourceType:
-            resource_type = resource_type.value
-        elif type(resource_type) == int:
-            resource_type = resource_type
-        else:
-            resource_type = int(resource_type)
+        proxy = self.__client.plunet_server.DataResource30.getPricelists2
+        response_model = PricelistListResult
 
-        arg = {"ResourceType": resource_type, "resourceID": resource_id}
+        arg = {
+            "sourcelanguage": sourcelanguage,
+            "targetlanguage": targetlanguage,
+            "resourceID": resource_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
@@ -421,575 +440,477 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_payment_information(
-        self, resource_id: int, payment_info: Union[PaymentInfo, dict]
-    ) -> Result:
+    def get_account(self, account_id: int) -> AccountResult:
         """
-        Allows to transfer a PaymentInfo object so change multiple payment
-        related values.
-
-        External-resources are not allowed to change the account information.
+        Allows the access to account details dependent on the transfered
+        accountID, which is part of PaymentInfo.
 
 
-        :param resource_id: int
-        :param payment_info: PaymentInfo
-        :return: Result
+        :param account_id: int
+        :return: AccountResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setPaymentInformation
-        response_model = Result
-
-        if type(payment_info) != PaymentInfo:
-            payment_info = PaymentInfo(**payment_info).dict()
-        else:
-            payment_info = payment_info.dict()
-
-        arg = {"resourceID": resource_id, "paymentInfo": payment_info}
+        proxy = self.__client.plunet_server.DataResource30.getAccount
+        response_model = AccountResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=account_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_payment_information(self, resource_id: int) -> PaymentInfoResult:
+    def insert_object(self, resource_in: Union[ResourceIN, dict]) -> IntegerResult:
         """
-        Returns an PaymentInfo included within the result, which contains
-        information like IBAN, bank-code or credit account.
+        Method to create a new resource dataset by Object.
 
+        The method will return an instance of IntegerResult, which contains
+        the identifier of the new generated resource. Further API calls via this port
+        will manipulate this resource (except methods with an resource id as
+        parameter ), until another resource is fetched or the session is invalidated.
 
-        :param resource_id: int
-        :return: PaymentInfoResult
+
+        :param resource_in: ResourceIN
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getPaymentInformation
-        response_model = PaymentInfoResult
+        proxy = self.__client.plunet_server.DataResource30.insertObject
+        response_model = IntegerResult
+
+        if type(resource_in) != ResourceIN:
+            resource_in = ResourceIN(**resource_in).dict()
+        else:
+            resource_in = resource_in.dict()
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=resource_id,
+            argument=resource_in,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_available_payment_method_list(
-        self,
-    ) -> IntegerArrayResult:
+    def seek_by_external_id(self, external_id: str) -> IntegerResult:
         """
-        Returns a list of all available payment methods.
+        Method returns an instance of IntegerResult, which contains the ID
+        of the resource dataset, which was identified via the external id.
 
 
-        :return: IntegerArrayResult
+        :param external_id: str
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getAvailablePaymentMethodList
-        response_model = IntegerArrayResult
+        proxy = self.__client.plunet_server.DataResource30.seekByExternalID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=None,
+            argument=external_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_payment_method_description(
-        self, payment_method_id: int, system_language_code: str
-    ) -> StringResult:
+    def set_cost_center(self, cost_center: str, resource_id: int) -> Result:
         """
-        Returns the description of the transfered payment method in the specified
-        language.
+        Method to set the cost center. Returns an instance of Result.
 
 
-        :param payment_method_id: int
-        :param system_language_code: str
-        :return: StringResult
+        :param cost_center: str
+        :param resource_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getPaymentMethodDescription
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResource30.setCostCenter
+        response_model = Result
 
-        arg = {
-            "paymentMethodID": payment_method_id,
-            "systemLanguageCode": system_language_code,
-        }
+        arg = {"CostCenter": cost_center, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def deregister_callback_observer(self, resource_id: int) -> Result:
+    def get_cost_center(self, resource_id: int) -> StringResult:
         """
-        Deletes an observer.
-
-        Warning:
-
-
-        Observer can only deleted by the user who has created them.
+        Returns an instance of StringResult, which contains the cost
+        center depending on the resourceID.
 
 
         :param resource_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.deregisterCallback_Observer
-        response_model = Result
+        proxy = self.__client.plunet_server.DataResource30.getCostCenter
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def register_callback_notify(
-        self,
-        server_authentication_string: str,
-        server_address: str,
-        event_type: Union[EventType, int],
-    ) -> Result:
+    def get_user_id(self, resource_id: int) -> IntegerResult:
         """
-        Register to get notified when the specified EventType occurs
-        for any resource.
-
-        If the EventType occurs PBM will call the callback web service,
-        which is hosted within your environment. Also each user can only create
-        one notify request per event type.
-
-
-        Please check CallbackResource30 for the exact specification for
-        this service.
+        Returns an instance of IntegerResult, which contains the user id
+        of the selected resource.
 
 
-        The  must match one of the following formats:
+        :param resource_id: int
+        :return: IntegerResult
+        """
 
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
+        proxy = self.__client.plunet_server.DataResource30.getUserId
+        response_model = IntegerResult
 
-        In the first two cases, the address will be autocompleted by appending
-        the corresponding directory "CallbackResource30?wsdl".
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=resource_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
 
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+    def set_status(self, status: int, resource_id: int) -> Result:
+        """
+        Method to set the ResourceStatus of the resource. Returns an
+        instance of Result.
 
 
-        :param server_authentication_string: str
-        :param server_address: str
-        :param event_type: EventType
+        :param status: int
+        :param resource_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.registerCallback_Notify
+        proxy = self.__client.plunet_server.DataResource30.setStatus
         response_model = Result
 
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
-        else:
-            event_type = int(event_type)
-
-        arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "EventType": event_type,
-        }
+        arg = {"Status": status, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_available_account_id_list(
-        self,
-    ) -> IntegerArrayResult:
+    def get_status(self, resource_id: int) -> IntegerResult:
         """
-        Returns a list of all available accountIDÂ´s.
+        Returns an instance of IntegerResult, which contains the
+        ResourceStatus as integer.
 
 
-        :return: IntegerArrayResult
+        :param resource_id: int
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getAvailableAccountIDList
-        response_model = IntegerArrayResult
+        proxy = self.__client.plunet_server.DataResource30.getStatus
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=None,
+            argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
+    def get_skype_id(self, resource_id: int) -> StringResult:
         """
-        Deletes an registered notify request.
-
-        Warning:
-
-
-        Notify requests can only be deleted by the user who has created them).
+        Returns an instance of StringResult, which contains the SkypeID
+        depending on the resourceID.
 
 
-        :param event_type: EventType
-        :return: Result
+        :param resource_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.deregisterCallback_Notify
-        response_model = Result
-
-        if type(event_type) == EventType:
-            event_type = event_type.value
-        elif type(event_type) == int:
-            event_type = event_type
-        else:
-            event_type = int(event_type)
+        proxy = self.__client.plunet_server.DataResource30.getSkypeID
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=event_type,
+            argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def register_callback_observer(
-        self, server_authentication_string: str, server_address: str, resource_id: int
-    ) -> Result:
+    def set_academic_title(self, academic_title: str, resource_id: int) -> Result:
         """
-        Register to observe a specific object for any supported
-        EventType.
-
-        As soon as any supported EventType occurs, PBM will call the
-        callback web service, which is hosted within your environment.
-
-
-        Please check CallbackResource30 for the exact specification for
-        this service.
-
-
-        The  must match one of the following formats:
-
-        http://mypath
-        http://mypath/
-        http://mypath/subfolder?wsdl
-
-        In the first two cases, the address will be autocompleted by appending
-        the corresponding directory "CallbackResource30?wsdl".
-
-        A list of all registered callbacks can be accessed with
-        DataAdmin30.getListOfRegisteredCallbacks(String)
+        Method to set the academic title. Returns an instance of Result.
 
 
-        :param server_authentication_string: str
-        :param server_address: str
+        :param academic_title: str
         :param resource_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.registerCallback_Observer
+        proxy = self.__client.plunet_server.DataResource30.setAcademicTitle
         response_model = Result
 
-        arg = {
-            "ServerAuthenticationString": server_authentication_string,
-            "ServerAddress": server_address,
-            "ResourceID": resource_id,
-        }
+        arg = {"AcademicTitle": academic_title, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_full_name(self, resource_id: int) -> StringResult:
+    def get_academic_title(self, resource_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the full name
-        depending on the resourceID .
+        Returns an instance of StringResult, which contains the academic
+        title depending on the resourceID.
 
 
         :param resource_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getFullName
+        proxy = self.__client.plunet_server.DataResource30.getAcademicTitle
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_status(self, resource_id: int) -> IntegerResult:
+    def set_opening(self, opening: str, resource_id: int) -> Result:
         """
-        Returns an instance of IntegerResult, which contains the
-        ResourceStatus as integer.
+        Method to set the opening. Returns an instance of Result.
 
 
+        :param opening: str
         :param resource_id: int
-        :return: IntegerResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getStatus
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataResource30.setOpening
+        response_model = Result
+
+        arg = {"Opening": opening, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=resource_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_status(self, status: int, resource_id: int) -> Result:
+    def set_name1(self, name: str, resource_id: int) -> Result:
         """
-        Method to set the ResourceStatus of the resource. Returns an
-        instance of Result.
+        Method to set name1 (last name). Returns an instance of Result.
 
 
-        :param status: int
+        :param name: str
         :param resource_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setStatus
+        proxy = self.__client.plunet_server.DataResource30.setName1
         response_model = Result
 
-        arg = {"Status": status, "resourceID": resource_id}
+        arg = {"Name": name, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_all_resource_objects2(
-        self,
-        working_status_list: Union[IntegerList, dict],
-        status_list: Union[IntegerList, dict],
-    ) -> ResourceListResult:
+    def set_phone(self, phone_number: str, resource_id: int) -> Result:
         """
-        Returns an instance of ResourceListResult, which contains a list
-        of resource objects, which are filtered by the ResourceStatus and the
-        WorkingStatus.
+        Method to set the phone number. Returns an instance of Result.
 
 
-        :param working_status_list: IntegerList
-        :param status_list: IntegerList
-        :return: ResourceListResult
+        :param phone_number: str
+        :param resource_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getAllResourceObjects2
-        response_model = ResourceListResult
-
-        if type(working_status_list) != IntegerList:
-            working_status_list = IntegerList(**working_status_list).dict()
-        else:
-            working_status_list = working_status_list.dict()
-
-        if type(status_list) != IntegerList:
-            status_list = IntegerList(**status_list).dict()
-        else:
-            status_list = status_list.dict()
+        proxy = self.__client.plunet_server.DataResource30.setPhone
+        response_model = Result
 
-        arg = {"WorkingStatusList": working_status_list, "StatusList": status_list}
+        arg = {"PhoneNumber": phone_number, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_all_resource_objects(
-        self, working_status: Union[WorkingStatus, int], status: int
-    ) -> ResourceListResult:
+    def set_mobile_phone(self, phone_number: str, resource_id: int) -> Result:
         """
-        Returns an instance of ResourceListResult, which contains a list
-        of resource objects, which are filtered by the ResourceStatus and the
-        WorkingStatus.
+        Method to set the mobile number. Returns an instance of
+        Result.
 
 
-        :param working_status: WorkingStatus
-        :param status: int
-        :return: ResourceListResult
+        :param phone_number: str
+        :param resource_id: int
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getAllResourceObjects
-        response_model = ResourceListResult
-
-        if type(working_status) == WorkingStatus:
-            working_status = working_status.value
-        elif type(working_status) == int:
-            working_status = working_status
-        else:
-            working_status = int(working_status)
+        proxy = self.__client.plunet_server.DataResource30.setMobilePhone
+        response_model = Result
 
-        arg = {"WorkingStatus": working_status, "Status": status}
+        arg = {"PhoneNumber": phone_number, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_resource_object(self, resource_id: int) -> ResourceResult:
+    def get_name1(self, resource_id: int) -> StringResult:
         """
-        Returns an instance of ResourceResult, which contains an instance
-        of resource.
+        Returns an instance of StringResult, which contains name1 (last
+        name).
 
 
         :param resource_id: int
-        :return: ResourceResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getResourceObject
-        response_model = ResourceResult
+        proxy = self.__client.plunet_server.DataResource30.getName1
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_saml_external_id(self, resource_id: int, saml_external_id: str) -> Result:
+    def set_external_id(self, external_id: str, resource_id: int) -> Result:
         """
-        Method to set the samlExternalId of a resource.
+        Method to set the external ID. Returns an instance of Result.
 
 
+        :param external_id: str
         :param resource_id: int
-        :param saml_external_id: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setSamlExternalId
+        proxy = self.__client.plunet_server.DataResource30.setExternalID
         response_model = Result
 
-        arg = {"resourceId": resource_id, "samlExternalId": saml_external_id}
+        arg = {"ExternalID": external_id, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_saml_external_id(self, resource_id: int) -> StringResult:
+    def set_fax(self, fax: str, resource_id: int) -> Result:
         """
-        Method to get the samlExternalId of a resource
+        Method to set the fax address. Returns an instance of Result.
 
 
+        :param fax: str
         :param resource_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getSamlExternalId
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResource30.setFax
+        response_model = Result
+
+        arg = {"Fax": fax, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=resource_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def insert_object(self, resource_in: Union[ResourceIN, dict]) -> IntegerResult:
+    def get_mobile_phone(self, resource_id: int) -> StringResult:
         """
-        Method to create a new resource dataset by Object.
-
-        The method will return an instance of IntegerResult, which contains
-        the identifier of the new generated resource. Further API calls via this port
-        will manipulate this resource (except methods with an resource id as
-        parameter ), until another resource is fetched or the session is invalidated.
+        Returns an instance of StringResult, which contains the mobile
+        phone number depending on the resourceID.
 
 
-        :param resource_in: ResourceIN
-        :return: IntegerResult
+        :param resource_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.insertObject
-        response_model = IntegerResult
-
-        if type(resource_in) != ResourceIN:
-            resource_in = ResourceIN(**resource_in).dict()
-        else:
-            resource_in = resource_in.dict()
+        proxy = self.__client.plunet_server.DataResource30.getMobilePhone
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=resource_in,
+            argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_account(self, account_id: int) -> AccountResult:
+    def get_fax(self, resource_id: int) -> StringResult:
         """
-        Allows the access to account details dependent on the transfered
-        accountID, which is part of PaymentInfo.
+        Returns an instance of StringResult, which contains the fax
+        address depending on the resourceID.
 
 
-        :param account_id: int
-        :return: AccountResult
+        :param resource_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getAccount
-        response_model = AccountResult
+        proxy = self.__client.plunet_server.DataResource30.getFax
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=account_id,
+            argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_fax(self, resource_id: int) -> StringResult:
+    def set_email(self, e_mail: str, resource_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains the fax
-        address depending on the resourceID.
+        Method to set the e-mail address. Returns an instance of
+        Result.
 
 
+        :param e_mail: str
         :param resource_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getFax
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResource30.setEmail
+        response_model = Result
+
+        arg = {"EMail": e_mail, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=resource_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_name1(self, resource_id: int) -> StringResult:
+    def get_phone(self, resource_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains name1 (last
-        name).
+        Returns an instance of StringResult, which contains the phone
+        number depending on the resourceID.
 
 
         :param resource_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getName1
+        proxy = self.__client.plunet_server.DataResource30.getPhone
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
@@ -1014,532 +935,610 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_form_of_address(self, resource_id: int) -> IntegerResult:
+    def get_email(self, resource_id: int) -> StringResult:
         """
-        Returns an instance of IntegerResult, which contains the
-        FormOfAddressType.
+        Returns an instance of StringResult, which contains the e-mail
+        address depending on the resourceID.
 
 
         :param resource_id: int
-        :return: IntegerResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getFormOfAddress
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataResource30.getEmail
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_website(self, website: str, resource_id: int) -> Result:
+    def set_name2(self, name: str, resource_id: int) -> Result:
         """
-        Method to set the website. Returns an instance of Result.
+        Method to set name2 (first name). Returns an instance of Result.
 
 
-        :param website: str
+        :param name: str
         :param resource_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setWebsite
+        proxy = self.__client.plunet_server.DataResource30.setName2
         response_model = Result
 
-        arg = {"Website": website, "resourceID": resource_id}
+        arg = {"Name": name, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_fax(self, fax: str, resource_id: int) -> Result:
+    def get_name2(self, resource_id: int) -> StringResult:
         """
-        Method to set the fax address. Returns an instance of Result.
+        Returns an instance of StringResult, which contains name2 (first
+        name).
 
 
-        :param fax: str
         :param resource_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setFax
-        response_model = Result
-
-        arg = {"Fax": fax, "resourceID": resource_id}
+        proxy = self.__client.plunet_server.DataResource30.getName2
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=resource_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_skype_id(self, skype_id: str, resource_id: int) -> Result:
+    def get_external_id(self, resource_id: int) -> StringResult:
         """
-        Method to set the SkypeID. Returns an instance of Result.
+        Returns an instance of StringResult, which contains the external
+        ID depending on the resourceID .
 
 
-        :param skype_id: str
         :param resource_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setSkypeID
-        response_model = Result
-
-        arg = {"SkypeID": skype_id, "resourceID": resource_id}
+        proxy = self.__client.plunet_server.DataResource30.getExternalID
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=resource_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_skype_id(self, resource_id: int) -> StringResult:
+    def get_form_of_address(self, resource_id: int) -> IntegerResult:
         """
-        Returns an instance of StringResult, which contains the SkypeID
-        depending on the resourceID.
+        Returns an instance of IntegerResult, which contains the
+        FormOfAddressType.
 
 
         :param resource_id: int
-        :return: StringResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getSkypeID
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResource30.getFormOfAddress
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_academic_title(self, resource_id: int) -> StringResult:
+    def set_website(self, website: str, resource_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains the academic
-        title depending on the resourceID.
+        Method to set the website. Returns an instance of Result.
 
 
+        :param website: str
         :param resource_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getAcademicTitle
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResource30.setWebsite
+        response_model = Result
+
+        arg = {"Website": website, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=resource_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_phone(self, resource_id: int) -> StringResult:
+    def get_website(self, resource_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the phone
-        number depending on the resourceID.
+        Returns an instance of StringResult, which contains the website
+        depending on the resourceID.
 
 
         :param resource_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getPhone
+        proxy = self.__client.plunet_server.DataResource30.getWebsite
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_name1(self, name: str, resource_id: int) -> Result:
+    def set_skype_id(self, skype_id: str, resource_id: int) -> Result:
         """
-        Method to set name1 (last name). Returns an instance of Result.
+        Method to set the SkypeID. Returns an instance of Result.
 
 
-        :param name: str
+        :param skype_id: str
         :param resource_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setName1
+        proxy = self.__client.plunet_server.DataResource30.setSkypeID
         response_model = Result
 
-        arg = {"Name": name, "resourceID": resource_id}
+        arg = {"SkypeID": skype_id, "resourceID": resource_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_mobile_phone(self, resource_id: int) -> StringResult:
+    def get_opening(self, resource_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the mobile
-        phone number depending on the resourceID.
+        Returns an instance of StringResult, which contains the opening
+        depending on the resourceID.
 
 
         :param resource_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getMobilePhone
+        proxy = self.__client.plunet_server.DataResource30.getOpening
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_website(self, resource_id: int) -> StringResult:
+    def get_saml_external_id(self, resource_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the website
-        depending on the resourceID.
+        Method to get the samlExternalId of a resource
 
 
         :param resource_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getWebsite
+        proxy = self.__client.plunet_server.DataResource30.getSamlExternalId
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_external_id(self, external_id: str, resource_id: int) -> Result:
+    def set_saml_external_id(self, resource_id: int, saml_external_id: str) -> Result:
         """
-        Method to set the external ID. Returns an instance of Result.
+        Method to set the samlExternalId of a resource.
 
 
-        :param external_id: str
         :param resource_id: int
+        :param saml_external_id: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setExternalID
+        proxy = self.__client.plunet_server.DataResource30.setSamlExternalId
         response_model = Result
 
-        arg = {"ExternalID": external_id, "resourceID": resource_id}
+        arg = {"resourceId": resource_id, "samlExternalId": saml_external_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_cost_center(self, cost_center: str, resource_id: int) -> Result:
+    def get_all_resource_objects2(
+        self,
+        working_status_list: Union[IntegerList, dict],
+        status_list: Union[IntegerList, dict],
+    ) -> ResourceListResult:
         """
-        Method to set the cost center. Returns an instance of Result.
+        Returns an instance of ResourceListResult, which contains a list
+        of resource objects, which are filtered by the ResourceStatus and the
+        WorkingStatus.
 
 
-        :param cost_center: str
-        :param resource_id: int
-        :return: Result
+        :param working_status_list: IntegerList
+        :param status_list: IntegerList
+        :return: ResourceListResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setCostCenter
-        response_model = Result
+        proxy = self.__client.plunet_server.DataResource30.getAllResourceObjects2
+        response_model = ResourceListResult
 
-        arg = {"CostCenter": cost_center, "resourceID": resource_id}
+        if type(working_status_list) != IntegerList:
+            working_status_list = IntegerList(**working_status_list).dict()
+        else:
+            working_status_list = working_status_list.dict()
+
+        if type(status_list) != IntegerList:
+            status_list = IntegerList(**status_list).dict()
+        else:
+            status_list = status_list.dict()
+
+        arg = {"WorkingStatusList": working_status_list, "StatusList": status_list}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_user_id(self, resource_id: int) -> IntegerResult:
+    def get_resource_object(self, resource_id: int) -> ResourceResult:
         """
-        Returns an instance of IntegerResult, which contains the user id
-        of the selected resource.
+        Returns an instance of ResourceResult, which contains an instance
+        of resource.
 
 
         :param resource_id: int
-        :return: IntegerResult
+        :return: ResourceResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getUserId
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataResource30.getResourceObject
+        response_model = ResourceResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_name2(self, name: str, resource_id: int) -> Result:
+    def get_all_resource_objects(
+        self, working_status: Union[WorkingStatus, int], status: int
+    ) -> ResourceListResult:
         """
-        Method to set name2 (first name). Returns an instance of Result.
+        Returns an instance of ResourceListResult, which contains a list
+        of resource objects, which are filtered by the ResourceStatus and the
+        WorkingStatus.
 
 
-        :param name: str
-        :param resource_id: int
-        :return: Result
+        :param working_status: WorkingStatus
+        :param status: int
+        :return: ResourceListResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setName2
-        response_model = Result
+        proxy = self.__client.plunet_server.DataResource30.getAllResourceObjects
+        response_model = ResourceListResult
 
-        arg = {"Name": name, "resourceID": resource_id}
+        if type(working_status) == WorkingStatus:
+            working_status = working_status.value
+        elif type(working_status) == int:
+            working_status = working_status
+        else:
+            working_status = int(working_status)
+
+        arg = {"WorkingStatus": working_status, "Status": status}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_email(self, e_mail: str, resource_id: int) -> Result:
+    def deregister_callback_notify(self, event_type: Union[EventType, int]) -> Result:
         """
-        Method to set the e-mail address. Returns an instance of
-        Result.
+        Deletes an registered notify request.
 
+        Warning:
 
-        :param e_mail: str
-        :param resource_id: int
+
+        Notify requests can only be deleted by the user who has created them).
+
+
+        :param event_type: EventType
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setEmail
+        proxy = self.__client.plunet_server.DataResource30.deregisterCallback_Notify
         response_model = Result
 
-        arg = {"EMail": e_mail, "resourceID": resource_id}
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
+        else:
+            event_type = int(event_type)
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=event_type,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_opening(self, resource_id: int) -> StringResult:
+    def get_payment_information(self, resource_id: int) -> PaymentInfoResult:
         """
-        Returns an instance of StringResult, which contains the opening
-        depending on the resourceID.
+        Returns an PaymentInfo included within the result, which contains
+        information like IBAN, bank-code or credit account.
 
 
         :param resource_id: int
-        :return: StringResult
+        :return: PaymentInfoResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getOpening
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResource30.getPaymentInformation
+        response_model = PaymentInfoResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_academic_title(self, academic_title: str, resource_id: int) -> Result:
+    def get_payment_method_description(
+        self, payment_method_id: int, system_language_code: str
+    ) -> StringResult:
         """
-        Method to set the academic title. Returns an instance of Result.
+        Returns the description of the transfered payment method in the specified
+        language.
 
 
-        :param academic_title: str
-        :param resource_id: int
-        :return: Result
+        :param payment_method_id: int
+        :param system_language_code: str
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setAcademicTitle
-        response_model = Result
+        proxy = self.__client.plunet_server.DataResource30.getPaymentMethodDescription
+        response_model = StringResult
 
-        arg = {"AcademicTitle": academic_title, "resourceID": resource_id}
+        arg = {
+            "paymentMethodID": payment_method_id,
+            "systemLanguageCode": system_language_code,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_opening(self, opening: str, resource_id: int) -> Result:
+    def get_available_account_id_list(
+        self,
+    ) -> IntegerArrayResult:
         """
-        Method to set the opening. Returns an instance of Result.
+        Returns a list of all available accountIDÂ´s.
 
 
-        :param opening: str
-        :param resource_id: int
-        :return: Result
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setOpening
-        response_model = Result
-
-        arg = {"Opening": opening, "resourceID": resource_id}
+        proxy = self.__client.plunet_server.DataResource30.getAvailableAccountIDList
+        response_model = IntegerArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=None,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_phone(self, phone_number: str, resource_id: int) -> Result:
+    def register_callback_notify(
+        self,
+        server_authentication_string: str,
+        server_address: str,
+        event_type: Union[EventType, int],
+    ) -> Result:
         """
-        Method to set the phone number. Returns an instance of Result.
+        Register to get notified when the specified EventType occurs
+        for any resource.
 
+        If the EventType occurs PBM will call the callback web service,
+        which is hosted within your environment. Also each user can only create
+        one notify request per event type.
 
-        :param phone_number: str
-        :param resource_id: int
+
+        Please check CallbackResource30 for the exact specification for
+        this service.
+
+
+        The  must match one of the following formats:
+
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
+
+        In the first two cases, the address will be autocompleted by appending
+        the corresponding directory "CallbackResource30?wsdl".
+
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
+
+
+        :param server_authentication_string: str
+        :param server_address: str
+        :param event_type: EventType
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setPhone
+        proxy = self.__client.plunet_server.DataResource30.registerCallback_Notify
         response_model = Result
 
-        arg = {"PhoneNumber": phone_number, "resourceID": resource_id}
+        if type(event_type) == EventType:
+            event_type = event_type.value
+        elif type(event_type) == int:
+            event_type = event_type
+        else:
+            event_type = int(event_type)
+
+        arg = {
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "EventType": event_type,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_email(self, resource_id: int) -> StringResult:
+    def get_available_payment_method_list(
+        self,
+    ) -> IntegerArrayResult:
         """
-        Returns an instance of StringResult, which contains the e-mail
-        address depending on the resourceID.
+        Returns a list of all available payment methods.
 
 
-        :param resource_id: int
-        :return: StringResult
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getEmail
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResource30.getAvailablePaymentMethodList
+        response_model = IntegerArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=resource_id,
+            argument=None,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_external_id(self, resource_id: int) -> StringResult:
+    def register_callback_observer(
+        self, server_authentication_string: str, server_address: str, resource_id: int
+    ) -> Result:
         """
-        Returns an instance of StringResult, which contains the external
-        ID depending on the resourceID .
+        Register to observe a specific object for any supported
+        EventType.
 
+        As soon as any supported EventType occurs, PBM will call the
+        callback web service, which is hosted within your environment.
 
-        :param resource_id: int
-        :return: StringResult
-        """
 
-        proxy = self.__client.plunet_server.DataResource30.getExternalID
-        response_model = StringResult
+        Please check CallbackResource30 for the exact specification for
+        this service.
 
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=resource_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
 
-    def set_mobile_phone(self, phone_number: str, resource_id: int) -> Result:
-        """
-        Method to set the mobile number. Returns an instance of
-        Result.
+        The  must match one of the following formats:
 
+        http://mypath
+        http://mypath/
+        http://mypath/subfolder?wsdl
 
-        :param phone_number: str
+        In the first two cases, the address will be autocompleted by appending
+        the corresponding directory "CallbackResource30?wsdl".
+
+        A list of all registered callbacks can be accessed with
+        DataAdmin30.getListOfRegisteredCallbacks(String)
+
+
+        :param server_authentication_string: str
+        :param server_address: str
         :param resource_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.setMobilePhone
+        proxy = self.__client.plunet_server.DataResource30.registerCallback_Observer
         response_model = Result
 
-        arg = {"PhoneNumber": phone_number, "resourceID": resource_id}
+        arg = {
+            "ServerAuthenticationString": server_authentication_string,
+            "ServerAddress": server_address,
+            "ResourceID": resource_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_name2(self, resource_id: int) -> StringResult:
+    def deregister_callback_observer(self, resource_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains name2 (first
-        name).
+        Deletes an observer.
+
+        Warning:
+
+
+        Observer can only deleted by the user who has created them.
 
 
         :param resource_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResource30.getName2
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResource30.deregisterCallback_Observer
+        response_model = Result
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def seek_by_external_id(self, external_id: str) -> IntegerResult:
-        """
-        Method returns an instance of IntegerResult, which contains the ID
-        of the resource dataset, which was identified via the external id.
-
-
-        :param external_id: str
-        :return: IntegerResult
+    def set_payment_information(
+        self, resource_id: int, payment_info: Union[PaymentInfo, dict]
+    ) -> Result:
         """
+        Allows to transfer a PaymentInfo object so change multiple payment
+        related values.
 
-        proxy = self.__client.plunet_server.DataResource30.seekByExternalID
-        response_model = IntegerResult
+        External-resources are not allowed to change the account information.
 
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=external_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
 
-    def get_cost_center(self, resource_id: int) -> StringResult:
+        :param resource_id: int
+        :param payment_info: PaymentInfo
+        :return: Result
         """
-        Returns an instance of StringResult, which contains the cost
-        center depending on the resourceID.
 
+        proxy = self.__client.plunet_server.DataResource30.setPaymentInformation
+        response_model = Result
 
-        :param resource_id: int
-        :return: StringResult
-        """
+        if type(payment_info) != PaymentInfo:
+            payment_info = PaymentInfo(**payment_info).dict()
+        else:
+            payment_info = payment_info.dict()
 
-        proxy = self.__client.plunet_server.DataResource30.getCostCenter
-        response_model = StringResult
+        arg = {"resourceID": resource_id, "paymentInfo": payment_info}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=resource_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_resource_address30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_resource_address30.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 from typing import TYPE_CHECKING, List, Union
 
 from ..enums import AddressType
 from ..models import AddressIN, IntegerArrayResult, IntegerResult, Result, StringResult
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataResourceAddress30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
     def update(
         self, address_in: Union[AddressIN, dict], enable_null_or_empty_values: bool
     ) -> Result:
         """
         updates an resource address per Object.
@@ -148,32 +147,34 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_address_type(self, address_id: int) -> IntegerResult:
+    def set_description(self, description: str, address_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains the AddressType of
-        the currently selected Resource.
+        Method to set the address description. Returns an instance of Result.
 
 
+        :param description: str
         :param address_id: int
-        :return: IntegerResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.getAddressType
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataResourceAddress30.setDescription
+        response_model = Result
+
+        arg = {"Description": description, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=address_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
     def get_description(self, address_id: int) -> StringResult:
         """
         Returns an instance of StringResult, which contains the address description.
 
 
@@ -187,328 +188,348 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=address_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_description(self, description: str, address_id: int) -> Result:
+    def get_zip(self, address_id: int) -> StringResult:
         """
-        Method to set the address description. Returns an instance of Result.
+        Returns an instance of StringResult, which contains the zip code
 
 
-        :param description: str
         :param address_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.setDescription
-        response_model = Result
-
-        arg = {"Description": description, "AddressID": address_id}
+        proxy = self.__client.plunet_server.DataResourceAddress30.getZip
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=address_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_address_type(
-        self, address_type: Union[AddressType, int], address_id: int
-    ) -> Result:
+    def get_city(self, address_id: int) -> StringResult:
         """
-        Method to set the AddressType. Returns an instance of Result.
+        Returns an instance of StringResult, which contains the city.
 
 
-        :param address_type: AddressType
         :param address_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.setAddressType
-        response_model = Result
-
-        if type(address_type) == AddressType:
-            address_type = address_type.value
-        elif type(address_type) == int:
-            address_type = address_type
-        else:
-            address_type = int(address_type)
-
-        arg = {"AddressType": address_type, "addressID": address_id}
+        proxy = self.__client.plunet_server.DataResourceAddress30.getCity
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=address_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_street2(self, street2: str, address_id: int) -> Result:
+    def set_country(self, country: str, address_id: int) -> Result:
         """
-        Method to set street 2. Returns an instance of Result.
+        Method to set the country. Returns an instance of Result.
 
 
-        :param street2: str
+        :param country: str
         :param address_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.setStreet2
+        proxy = self.__client.plunet_server.DataResourceAddress30.setCountry
         response_model = Result
 
-        arg = {"Street2": street2, "AddressID": address_id}
+        arg = {"Country": country, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_street2(self, address_id: int) -> StringResult:
+    def get_all_addresses(self, resource_id: int) -> IntegerArrayResult:
         """
-        Returns an instance of StringResult, which contains street 2
+        Returns an instance of IntegerArrayResult, which contains a list of all available addressIDs
+        for this resource address
 
 
-        :param address_id: int
-        :return: StringResult
+        :param resource_id: int
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.getStreet2
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResourceAddress30.getAllAddresses
+        response_model = IntegerArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=address_id,
+            argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_city(self, city: str, address_id: int) -> Result:
+    def set_office(self, external_id: str, address_id: int) -> Result:
         """
-        Method to set city.
-
-        Returns an instance of Result.
+        Method to set the office name. Returns an instance of Result.
 
 
-        :param city: str
+        :param external_id: str
         :param address_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.setCity
+        proxy = self.__client.plunet_server.DataResourceAddress30.setOffice
         response_model = Result
 
-        arg = {"City": city, "AddressID": address_id}
+        arg = {"ExternalID": external_id, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_city(self, address_id: int) -> StringResult:
+    def get_street(self, address_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the city.
+        Returns an instance of StringResult, which contains street
 
 
         :param address_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.getCity
+        proxy = self.__client.plunet_server.DataResourceAddress30.getStreet
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=address_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_country(self, country: str, address_id: int) -> Result:
+    def set_city(self, city: str, address_id: int) -> Result:
         """
-        Method to set the country. Returns an instance of Result.
+        Method to set city.
 
+        Returns an instance of Result.
 
-        :param country: str
+
+        :param city: str
         :param address_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.setCountry
+        proxy = self.__client.plunet_server.DataResourceAddress30.setCity
         response_model = Result
 
-        arg = {"Country": country, "AddressID": address_id}
+        arg = {"City": city, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_all_addresses(self, resource_id: int) -> IntegerArrayResult:
+    def get_address_id(self, address_id: int) -> IntegerResult:
         """
-        Returns an instance of IntegerArrayResult, which contains a list of all available addressIDs
-        for this resource address
+        Returns an instance of IntegerResult, which contains the addressID of the currently fetched
+        address.
 
 
-        :param resource_id: int
-        :return: IntegerArrayResult
+        :param address_id: int
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.getAllAddresses
-        response_model = IntegerArrayResult
+        proxy = self.__client.plunet_server.DataResourceAddress30.getAddressID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=resource_id,
+            argument=address_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_address_id(self, address_id: int) -> IntegerResult:
+    def get_office(self, address_id: int) -> StringResult:
         """
-        Returns an instance of IntegerResult, which contains the addressID of the currently fetched
-        address.
+        Returns an instance of StringResult, which contains the office name
 
 
         :param address_id: int
-        :return: IntegerResult
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.getAddressID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataResourceAddress30.getOffice
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=address_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_office(self, external_id: str, address_id: int) -> Result:
+    def set_street(self, street: str, address_id: int) -> Result:
         """
-        Method to set the office name. Returns an instance of Result.
+        Method to set street. Returns an instance of Result.
 
 
-        :param external_id: str
+        :param street: str
         :param address_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.setOffice
+        proxy = self.__client.plunet_server.DataResourceAddress30.setStreet
         response_model = Result
 
-        arg = {"ExternalID": external_id, "AddressID": address_id}
+        arg = {"Street": street, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_street(self, address_id: int) -> StringResult:
+    def set_street2(self, street2: str, address_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains street
+        Method to set street 2. Returns an instance of Result.
+
+
+        :param street2: str
+        :param address_id: int
+        :return: Result
+        """
+
+        proxy = self.__client.plunet_server.DataResourceAddress30.setStreet2
+        response_model = Result
+
+        arg = {"Street2": street2, "AddressID": address_id}
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def get_street2(self, address_id: int) -> StringResult:
+        """
+        Returns an instance of StringResult, which contains street 2
 
 
         :param address_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.getStreet
+        proxy = self.__client.plunet_server.DataResourceAddress30.getStreet2
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=address_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_street(self, street: str, address_id: int) -> Result:
+    def set_zip(self, zip: str, address_id: int) -> Result:
         """
-        Method to set street. Returns an instance of Result.
+        Method to set zip code. Returns an instance of Result.
 
 
-        :param street: str
+        :param zip: str
         :param address_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.setStreet
+        proxy = self.__client.plunet_server.DataResourceAddress30.setZip
         response_model = Result
 
-        arg = {"Street": street, "AddressID": address_id}
+        arg = {"Zip": zip, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_zip(self, address_id: int) -> StringResult:
+    def get_address_type(self, address_id: int) -> IntegerResult:
         """
-        Returns an instance of StringResult, which contains the zip code
+        Returns an instance of StringResult, which contains the AddressType of
+        the currently selected Resource.
 
 
         :param address_id: int
-        :return: StringResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.getZip
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResourceAddress30.getAddressType
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=address_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_office(self, address_id: int) -> StringResult:
+    def set_address_type(
+        self, address_type: Union[AddressType, int], address_id: int
+    ) -> Result:
         """
-        Returns an instance of StringResult, which contains the office name
+        Method to set the AddressType. Returns an instance of Result.
 
 
+        :param address_type: AddressType
         :param address_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.getOffice
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResourceAddress30.setAddressType
+        response_model = Result
+
+        if type(address_type) == AddressType:
+            address_type = address_type.value
+        elif type(address_type) == int:
+            address_type = address_type
+        else:
+            address_type = int(address_type)
+
+        arg = {"AddressType": address_type, "addressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=address_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_zip(self, zip: str, address_id: int) -> Result:
+    def set_name1(self, name: str, address_id: int) -> Result:
         """
-        Method to set zip code. Returns an instance of Result.
+        Method to set the name1 / last name. Returns an instance of Result.
 
 
-        :param zip: str
+        :param name: str
         :param address_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceAddress30.setZip
+        proxy = self.__client.plunet_server.DataResourceAddress30.setName1
         response_model = Result
 
-        arg = {"Zip": zip, "AddressID": address_id}
+        arg = {"Name": name, "AddressID": address_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
@@ -556,36 +577,14 @@
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
-
-    def set_name1(self, name: str, address_id: int) -> Result:
-        """
-        Method to set the name1 / last name. Returns an instance of Result.
-
-
-        :param name: str
-        :param address_id: int
-        :return: Result
-        """
-
-        proxy = self.__client.plunet_server.DataResourceAddress30.setName1
-        response_model = Result
-
-        arg = {"Name": name, "AddressID": address_id}
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=arg,
-            response_model=response_model,
-            unpack_dict=True,
-        )
 
     def set_name2(self, name: str, address_id: int) -> Result:
         """
         Method to set the name2 / first name. Returns an instance of Result.
 
 
         :param name: str
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_resource_contact30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_resource_contact30.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,18 @@
     ResourceContactResult,
     Result,
     StringResult,
 )
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataResourceContact30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
     def update(
         self,
         resource_contact_in: Union[ResourceContactIN, dict],
         enable_null_or_empty_values: bool,
     ) -> Result:
@@ -73,53 +72,55 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=None,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_resource_id(self, resource_id: int, contact_id: int) -> Result:
+    def get_address_id(self, contact_id: int) -> IntegerResult:
         """
-        Method to set the resourceId. Returns an instance of Result.
+        Returns an instance of IntegerResult, which contains the address id of the resource contact. Use
+        the DataResourceAddress25 service, to manage addresses for this resource contact.
 
 
-        :param resource_id: int
         :param contact_id: int
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setResourceID
-        response_model = Result
-
-        arg = {"ResourceID": resource_id, "ContactID": contact_id}
+        proxy = self.__client.plunet_server.DataResourceContact30.getAddressID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=contact_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_contact_object(self, contact_id: int) -> ResourceContactResult:
+    def set_address_id(self, address_id: int, contact_id: int) -> Result:
         """
-        Returns an instance of ResourceContactResult, which contains a specific resource contact object.
+        Method to set the default addres for this resource contact. Use the DataResourceAddress25
+        service, to manage addresses for this resource contact.
 
 
+        :param address_id: int
         :param contact_id: int
-        :return: ResourceContactResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getContactObject
-        response_model = ResourceContactResult
+        proxy = self.__client.plunet_server.DataResourceContact30.setAddressID
+        response_model = Result
+
+        arg = {"AddressID": address_id, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=contact_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
     def get_all_contacts(self, resource_id: int) -> IntegerArrayResult:
         """
         Returns an instance of IntegerArrayResult, which contains a list of all available resource
         contact IDs.
 
@@ -134,56 +135,70 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_address_id(self, address_id: int, contact_id: int) -> Result:
+    def get_contact_object(self, contact_id: int) -> ResourceContactResult:
         """
-        Method to set the default addres for this resource contact. Use the DataResourceAddress25
-        service, to manage addresses for this resource contact.
+        Returns an instance of ResourceContactResult, which contains a specific resource contact object.
 
 
-        :param address_id: int
+        :param contact_id: int
+        :return: ResourceContactResult
+        """
+
+        proxy = self.__client.plunet_server.DataResourceContact30.getContactObject
+        response_model = ResourceContactResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=contact_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def set_resource_id(self, resource_id: int, contact_id: int) -> Result:
+        """
+        Method to set the resourceId. Returns an instance of Result.
+
+
+        :param resource_id: int
         :param contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setAddressID
+        proxy = self.__client.plunet_server.DataResourceContact30.setResourceID
         response_model = Result
 
-        arg = {"AddressID": address_id, "ContactID": contact_id}
+        arg = {"ResourceID": resource_id, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_status(self, contact_id: int) -> IntegerResult:
+    def seek_by_external_id(self, external_id: str) -> IntegerArrayResult:
         """
-        Returns an instance of IntegerResult, which contains the status id as integer.
-        Status codes:
-
-        0 = not active
-        1 = active
+        Returns an instance of IntegerArrayResult, which contains a list of resource contact IDs.
 
 
-        :param contact_id: int
-        :return: IntegerResult
+        :param external_id: str
+        :return: IntegerArrayResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getStatus
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataResourceContact30.seekByExternalID
+        response_model = IntegerArrayResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=contact_id,
+            argument=external_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
     def set_status(self, status: int, contact_id: int) -> Result:
         """
         Method to set the status of the resource contact. Returns an instance of Result. Status
@@ -206,262 +221,265 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_saml_external_id(self, contact_id: int, saml_external_id: str) -> Result:
+    def get_resource_id(self, contact_id: int) -> IntegerResult:
         """
-        Sets the samlExternalId for a contact person.
+        Returns an instance of IntegerResult, which contains resourceId
 
 
         :param contact_id: int
-        :param saml_external_id: str
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setSamlExternalId
-        response_model = Result
-
-        arg = {"ContactID": contact_id, "SamlExternalID": saml_external_id}
+        proxy = self.__client.plunet_server.DataResourceContact30.getResourceID
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=contact_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_saml_external_id(self, contact_id: int) -> StringResult:
+    def get_status(self, contact_id: int) -> IntegerResult:
         """
-        Gets the samlExternalId for a contact person.
+        Returns an instance of IntegerResult, which contains the status id as integer.
+        Status codes:
+
+        0 = not active
+        1 = active
 
 
         :param contact_id: int
-        :return: StringResult
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getSamlExternalId
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResourceContact30.getStatus
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_all_contact_objects(self, resource_id: int) -> ResourceContactListResult:
+    def get_skype_id(self, contact_id: int) -> StringResult:
         """
-        Returns an instance of ResourceContactListResult, which contains a list of all available resource contact objects.
+        Returns an instance of StringResult, which contains the SkypeID
 
 
-        :param resource_id: int
-        :return: ResourceContactListResult
+        :param contact_id: int
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getAllContactObjects
-        response_model = ResourceContactListResult
+        proxy = self.__client.plunet_server.DataResourceContact30.getSkypeID
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=resource_id,
+            argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_address_id(self, contact_id: int) -> IntegerResult:
+    def set_academic_title(self, academic_title: str, contact_id: int) -> Result:
         """
-        Returns an instance of IntegerResult, which contains the address id of the resource contact. Use
-        the DataResourceAddress25 service, to manage addresses for this resource contact.
+        Method to set the academic title. Returns an instance of Result.
 
 
+        :param academic_title: str
         :param contact_id: int
-        :return: IntegerResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getAddressID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataResourceContact30.setAcademicTitle
+        response_model = Result
+
+        arg = {"AcademicTitle": academic_title, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=contact_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_fax(self, contact_id: int) -> StringResult:
+    def get_academic_title(self, contact_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the fax address
+        Returns an instance of StringResult, which contains the academic title
 
 
         :param contact_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getFax
+        proxy = self.__client.plunet_server.DataResourceContact30.getAcademicTitle
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_name1(self, contact_id: int) -> StringResult:
+    def set_opening(self, opening: str, contact_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains the name1 / last name
+        Method to set the opening. Returns an instance of Result.
 
 
+        :param opening: str
         :param contact_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getName1
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResourceContact30.setOpening
+        response_model = Result
+
+        arg = {"Opening": opening, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=contact_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_form_of_address(self, form_of_address: int, contact_id: int) -> Result:
+    def set_name1(self, name: str, contact_id: int) -> Result:
         """
-        Method to set the form of address. Returns an instance of Result. Form of address:
-
-        1 = Mr
-        2 = Mrs
-        3 = Company
+        Method to set the name1 / last name. Returns an instance of Result.
 
 
-        :param form_of_address: int
+        :param name: str
         :param contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setFormOfAddress
+        proxy = self.__client.plunet_server.DataResourceContact30.setName1
         response_model = Result
 
-        arg = {"FormOfAddress": form_of_address, "ContactID": contact_id}
+        arg = {"Name": name, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_form_of_address(self, contact_id: int) -> IntegerResult:
+    def set_phone(self, phone_number: str, contact_id: int) -> Result:
         """
-        Returns an instance of IntegerResult, which contains the id of the form of address.
-        Form of address:
-
-        1 = Mr
-        2 = Mrs
-        3 = Company
+        Method to set phone number. Returns an instance of Result.
 
 
+        :param phone_number: str
         :param contact_id: int
-        :return: IntegerResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getFormOfAddress
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataResourceContact30.setPhone
+        response_model = Result
+
+        arg = {"PhoneNumber": phone_number, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=contact_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def set_fax(self, fax: str, contact_id: int) -> Result:
+    def set_mobile_phone(self, phone_number: str, contact_id: int) -> Result:
         """
-        Method to set the fax address. Returns an instance of Result.
+        Method to set mobile number. Returns an instance of Result.
 
 
-        :param fax: str
+        :param phone_number: str
         :param contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setFax
+        proxy = self.__client.plunet_server.DataResourceContact30.setMobilePhone
         response_model = Result
 
-        arg = {"Fax": fax, "ContactID": contact_id}
+        arg = {"PhoneNumber": phone_number, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_skype_id(self, skype_id: str, contact_id: int) -> Result:
+    def get_name1(self, contact_id: int) -> StringResult:
         """
-        Method to set the SkypeID. Returns an instance of Result.
+        Returns an instance of StringResult, which contains the name1 / last name
 
 
-        :param skype_id: str
         :param contact_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setSkypeID
-        response_model = Result
-
-        arg = {"SkypeID": skype_id, "ContactID": contact_id}
+        proxy = self.__client.plunet_server.DataResourceContact30.getName1
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=contact_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def get_skype_id(self, contact_id: int) -> StringResult:
+    def set_external_id(self, external_id: str, contact_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains the SkypeID
+        Method to set the external ID. Returns an instance of Result.
 
 
+        :param external_id: str
         :param contact_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getSkypeID
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResourceContact30.setExternalID
+        response_model = Result
+
+        arg = {"ExternalID": external_id, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=contact_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
-    def get_academic_title(self, contact_id: int) -> StringResult:
+    def set_fax(self, fax: str, contact_id: int) -> Result:
         """
-        Returns an instance of StringResult, which contains the academic title
+        Method to set the fax address. Returns an instance of Result.
 
 
+        :param fax: str
         :param contact_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getAcademicTitle
-        response_model = StringResult
+        proxy = self.__client.plunet_server.DataResourceContact30.setFax
+        response_model = Result
+
+        arg = {"Fax": fax, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=contact_id,
+            argument=arg,
             response_model=response_model,
-            unpack_dict=False,
+            unpack_dict=True,
         )
 
     def insert2(
         self, resource_contact_in: Union[ResourceContactIN, dict]
     ) -> IntegerResult:
         """
         Method to create a new resource depending on transfered object
@@ -482,334 +500,315 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_contact_in,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_phone(self, contact_id: int) -> StringResult:
+    def get_mobile_phone(self, contact_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the phone number
+        Returns an instance of StringResult, which contains the mobile phone number
 
 
         :param contact_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getPhone
+        proxy = self.__client.plunet_server.DataResourceContact30.getMobilePhone
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_name1(self, name: str, contact_id: int) -> Result:
+    def get_fax(self, contact_id: int) -> StringResult:
         """
-        Method to set the name1 / last name. Returns an instance of Result.
+        Returns an instance of StringResult, which contains the fax address
 
 
-        :param name: str
+        :param contact_id: int
+        :return: StringResult
+        """
+
+        proxy = self.__client.plunet_server.DataResourceContact30.getFax
+        response_model = StringResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=contact_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def set_email(self, e_mail: str, contact_id: int) -> Result:
+        """
+        Method to set the e-mail address. Returns an instance of Result.
+
+
+        :param e_mail: str
         :param contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setName1
+        proxy = self.__client.plunet_server.DataResourceContact30.setEmail
         response_model = Result
 
-        arg = {"Name": name, "ContactID": contact_id}
+        arg = {"EMail": e_mail, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_mobile_phone(self, contact_id: int) -> StringResult:
+    def get_phone(self, contact_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the mobile phone number
+        Returns an instance of StringResult, which contains the phone number
 
 
         :param contact_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getMobilePhone
+        proxy = self.__client.plunet_server.DataResourceContact30.getPhone
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_external_id(self, external_id: str, contact_id: int) -> Result:
+    def set_form_of_address(self, form_of_address: int, contact_id: int) -> Result:
         """
-        Method to set the external ID. Returns an instance of Result.
+        Method to set the form of address. Returns an instance of Result. Form of address:
+
+        1 = Mr
+        2 = Mrs
+        3 = Company
 
 
-        :param external_id: str
+        :param form_of_address: int
         :param contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setExternalID
+        proxy = self.__client.plunet_server.DataResourceContact30.setFormOfAddress
         response_model = Result
 
-        arg = {"ExternalID": external_id, "ContactID": contact_id}
+        arg = {"FormOfAddress": form_of_address, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def set_name2(self, name: str, contact_id: int) -> Result:
+    def get_email(self, contact_id: int) -> StringResult:
         """
-        Method to set the name2 / first name. Returns an instance of Result.
+        Returns an instance of StringResult, which contains the e-mail address
 
 
-        :param name: str
         :param contact_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setName2
-        response_model = Result
-
-        arg = {"Name": name, "ContactID": contact_id}
+        proxy = self.__client.plunet_server.DataResourceContact30.getEmail
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=contact_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_email(self, e_mail: str, contact_id: int) -> Result:
+    def set_name2(self, name: str, contact_id: int) -> Result:
         """
-        Method to set the e-mail address. Returns an instance of Result.
+        Method to set the name2 / first name. Returns an instance of Result.
 
 
-        :param e_mail: str
+        :param name: str
         :param contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setEmail
+        proxy = self.__client.plunet_server.DataResourceContact30.setName2
         response_model = Result
 
-        arg = {"EMail": e_mail, "ContactID": contact_id}
+        arg = {"Name": name, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_opening(self, contact_id: int) -> StringResult:
+    def get_name2(self, contact_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the opening
+        Returns an instance of StringResult, which contains the name2 / first name
 
 
         :param contact_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getOpening
+        proxy = self.__client.plunet_server.DataResourceContact30.getName2
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_academic_title(self, academic_title: str, contact_id: int) -> Result:
+    def get_external_id(self, contact_id: int) -> StringResult:
         """
-        Method to set the academic title. Returns an instance of Result.
+        Returns an instance of StringResult, which contains the external id
 
 
-        :param academic_title: str
         :param contact_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setAcademicTitle
-        response_model = Result
-
-        arg = {"AcademicTitle": academic_title, "ContactID": contact_id}
+        proxy = self.__client.plunet_server.DataResourceContact30.getExternalID
+        response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=contact_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_opening(self, opening: str, contact_id: int) -> Result:
+    def get_form_of_address(self, contact_id: int) -> IntegerResult:
         """
-        Method to set the opening. Returns an instance of Result.
+        Returns an instance of IntegerResult, which contains the id of the form of address.
+        Form of address:
+
+        1 = Mr
+        2 = Mrs
+        3 = Company
 
 
-        :param opening: str
         :param contact_id: int
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setOpening
-        response_model = Result
-
-        arg = {"Opening": opening, "ContactID": contact_id}
+        proxy = self.__client.plunet_server.DataResourceContact30.getFormOfAddress
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=contact_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_phone(self, phone_number: str, contact_id: int) -> Result:
+    def set_skype_id(self, skype_id: str, contact_id: int) -> Result:
         """
-        Method to set phone number. Returns an instance of Result.
+        Method to set the SkypeID. Returns an instance of Result.
 
 
-        :param phone_number: str
+        :param skype_id: str
         :param contact_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setPhone
+        proxy = self.__client.plunet_server.DataResourceContact30.setSkypeID
         response_model = Result
 
-        arg = {"PhoneNumber": phone_number, "ContactID": contact_id}
+        arg = {"SkypeID": skype_id, "ContactID": contact_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_email(self, contact_id: int) -> StringResult:
+    def get_opening(self, contact_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the e-mail address
+        Returns an instance of StringResult, which contains the opening
 
 
         :param contact_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getEmail
+        proxy = self.__client.plunet_server.DataResourceContact30.getOpening
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_external_id(self, contact_id: int) -> StringResult:
+    def get_saml_external_id(self, contact_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the external id
+        Gets the samlExternalId for a contact person.
 
 
         :param contact_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getExternalID
+        proxy = self.__client.plunet_server.DataResourceContact30.getSamlExternalId
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=contact_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_mobile_phone(self, phone_number: str, contact_id: int) -> Result:
+    def set_saml_external_id(self, contact_id: int, saml_external_id: str) -> Result:
         """
-        Method to set mobile number. Returns an instance of Result.
+        Sets the samlExternalId for a contact person.
 
 
-        :param phone_number: str
         :param contact_id: int
+        :param saml_external_id: str
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.setMobilePhone
+        proxy = self.__client.plunet_server.DataResourceContact30.setSamlExternalId
         response_model = Result
 
-        arg = {"PhoneNumber": phone_number, "ContactID": contact_id}
+        arg = {"ContactID": contact_id, "SamlExternalID": saml_external_id}
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_name2(self, contact_id: int) -> StringResult:
-        """
-        Returns an instance of StringResult, which contains the name2 / first name
-
-
-        :param contact_id: int
-        :return: StringResult
-        """
-
-        proxy = self.__client.plunet_server.DataResourceContact30.getName2
-        response_model = StringResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=contact_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def seek_by_external_id(self, external_id: str) -> IntegerArrayResult:
-        """
-        Returns an instance of IntegerArrayResult, which contains a list of resource contact IDs.
-
-
-        :param external_id: str
-        :return: IntegerArrayResult
-        """
-
-        proxy = self.__client.plunet_server.DataResourceContact30.seekByExternalID
-        response_model = IntegerArrayResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=external_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def get_resource_id(self, contact_id: int) -> IntegerResult:
+    def get_all_contact_objects(self, resource_id: int) -> ResourceContactListResult:
         """
-        Returns an instance of IntegerResult, which contains resourceId
+        Returns an instance of ResourceContactListResult, which contains a list of all available resource contact objects.
 
 
-        :param contact_id: int
-        :return: IntegerResult
+        :param resource_id: int
+        :return: ResourceContactListResult
         """
 
-        proxy = self.__client.plunet_server.DataResourceContact30.getResourceID
-        response_model = IntegerResult
+        proxy = self.__client.plunet_server.DataResourceContact30.getAllContactObjects
+        response_model = ResourceContactListResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=contact_id,
+            argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/data_user30.py` & `pyplunet-0.8.0/src/pyplunet/services/data_user30.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,37 +3,36 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, List, Union
 
 from ..models import UserListResult, UserResult
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class DataUser30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
-    def get_user_by_login_name(self, user_login_name: str) -> UserResult:
+    def get_user_by_id(self, user_id: int) -> UserResult:
         """
         Returns a UserResult if a user can be found
-        depending on the transfered login-name
+        depending on the transfered user id
 
 
-        :param user_login_name: str
+        :param user_id: int
         :return: UserResult
         """
 
-        proxy = self.__client.plunet_server.DataUser30.getUserByLoginName
+        proxy = self.__client.plunet_server.DataUser30.getUserByID
         response_model = UserResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=user_login_name,
+            argument=user_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
     def get_user_list_by_resource_id(self, resource_id: int) -> UserListResult:
         """
         Returns a List of all resource related userÂ´s
@@ -49,26 +48,26 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=resource_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_user_by_id(self, user_id: int) -> UserResult:
+    def get_user_by_login_name(self, user_login_name: str) -> UserResult:
         """
         Returns a UserResult if a user can be found
-        depending on the transfered user id
+        depending on the transfered login-name
 
 
-        :param user_id: int
+        :param user_login_name: str
         :return: UserResult
         """
 
-        proxy = self.__client.plunet_server.DataUser30.getUserByID
+        proxy = self.__client.plunet_server.DataUser30.getUserByLoginName
         response_model = UserResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=user_id,
+            argument=user_login_name,
             response_model=response_model,
             unpack_dict=False,
         )
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/report_customer30.py` & `pyplunet-0.8.0/src/pyplunet/services/report_customer30.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, List, Union
 
 from ..models import IntegerArrayResult, SearchFilter_Customer
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class ReportCustomer30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
     def search(
         self, search_filter_customer: Union[SearchFilter_Customer, dict]
     ) -> IntegerArrayResult:
         """
         Search for all customers which fulfill the requirements of the provided search-object.
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/report_job30.py` & `pyplunet-0.8.0/src/pyplunet/services/report_job30.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, List, Union
 
 from ..models import IntegerArrayResult, SearchFilter_Job
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class ReportJob30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
     def search(
         self, search_filter_job: Union[SearchFilter_Job, dict]
     ) -> IntegerArrayResult:
         """
         Search for all jobs which fulfill the requirements of the provided search-object.
```

### Comparing `pyplunet-0.7.0/src/pyplunet/services/request_doc_text30.py` & `pyplunet-0.8.0/src/pyplunet/services/request_doc_text30.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, List, Union
 
 from ..models import IntegerArrayResult, IntegerResult, Result, StringResult
 
 if TYPE_CHECKING:
     from ..client import PlunetClient
-    from ..retrying_client import RetryingPlunetClient
 
 
 class RequestDocText30:
-    def __init__(self, client: Union[PlunetClient, RetryingPlunetClient]):
+    def __init__(self, client: PlunetClient):
         self.__client = client
 
     def update(self, request_doc_text_id: int) -> Result:
         """
         Commits all changes for the currently selected request text to database. Returns an instance of Result.
 
 
@@ -73,150 +72,109 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_additional_info(
-        self, additional_info: str, request_doc_text_id: int
-    ) -> Result:
+    def get_word_count(self, request_doc_text_id: int) -> IntegerResult:
         """
-        Method to add additional information to the currently fetched request text.
-        Returns an instance of Result.
+        Returns an instance of IntegerResult, which contains the word count of the currently fetched text.
 
 
-        :param additional_info: str
         :param request_doc_text_id: int
-        :return: Result
+        :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.RequestDocText30.setAdditionalInfo
-        response_model = Result
-
-        arg = {
-            "additionalInfo": additional_info,
-            "requestDocTextID": request_doc_text_id,
-        }
+        proxy = self.__client.plunet_server.RequestDocText30.getWordCount
+        response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=arg,
+            argument=request_doc_text_id,
             response_model=response_model,
-            unpack_dict=True,
+            unpack_dict=False,
         )
 
-    def set_customer_text_id(
-        self, customer_text_id: int, request_doc_text_id: int
-    ) -> Result:
+    def get_target_text(
+        self, target_language: str, request_doc_text_id: int
+    ) -> StringResult:
         """
-        Method to set the customer text id of the currently fetched request text.
-        This value is an external identifier,
-        which is available for free use.
-        Returns an instance of Result.
+        Method to return the target text, of the currently fetched request text.
+        Method will return an instance of StringResult, which contains
+        the target text for a specific language.
+        System will search the target file within the target-folder of the order item.
+        All language descriptions were expected in english language or as ISO-Code.
 
 
-        :param customer_text_id: int
+        :param target_language: str
         :param request_doc_text_id: int
-        :return: Result
+        :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.RequestDocText30.setCustomerTextID
-        response_model = Result
+        proxy = self.__client.plunet_server.RequestDocText30.getTargetText
+        response_model = StringResult
 
         arg = {
-            "customerTextID": customer_text_id,
+            "targetLanguage": target_language,
             "requestDocTextID": request_doc_text_id,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_customer_text_id(self, request_doc_text_id: int) -> IntegerResult:
-        """
-        Returns an instance of IntegerResult, which contains the customer text id.
-
-
-        :param request_doc_text_id: int
-        :return: IntegerResult
-        """
-
-        proxy = self.__client.plunet_server.RequestDocText30.getCustomerTextID
-        response_model = IntegerResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=request_doc_text_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def get_all_by_request_id(self, request_id: int) -> IntegerArrayResult:
-        """
-        Returns an instance of IntegerArrayResult, which contains a list of request text identifier for a specific request.
-
-
-        :param request_id: int
-        :return: IntegerArrayResult
-        """
-
-        proxy = self.__client.plunet_server.RequestDocText30.getAll_ByRequestID
-        response_model = IntegerArrayResult
-
-        return self.__client.make_request(
-            operation_proxy=proxy,
-            argument=request_id,
-            response_model=response_model,
-            unpack_dict=False,
-        )
-
-    def get_additional_info(self, request_doc_text_id: int) -> StringResult:
+    def get_source_text(self, request_doc_text_id: int) -> StringResult:
         """
-        Returns an instance of StringResult, which contains the additional information of the currently fetched request text.
+        Method returns an instance of StringResult, which contains the sourcetext of the currently fetched request text.
 
 
         :param request_doc_text_id: int
         :return: StringResult
         """
 
-        proxy = self.__client.plunet_server.RequestDocText30.getAdditionalInfo
+        proxy = self.__client.plunet_server.RequestDocText30.getSourceText
         response_model = StringResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_doc_text_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_target_text(
-        self, target_language: str, request_doc_text_id: int
-    ) -> StringResult:
+    def set_source_text2(
+        self, source_text: str, encoding: str, request_doc_text_id: int
+    ) -> Result:
         """
-        Method to return the target text, of the currently fetched request text.
-        Method will return an instance of StringResult, which contains
-        the target text for a specific language.
-        System will search the target file within the target-folder of the order item.
-        All language descriptions were expected in english language or as ISO-Code.
+        Method returns an instance of StringResult, which contains the sourcetext of the currently fetched request text.
+        With the encoding parameter, it is possible to choose the encoding type for the created source file.
+        Valid encoding:
 
+        UTF-8
+        UTF-16LE
+        UTF-16BE
+        ANSI
 
-        :param target_language: str
+
+        :param source_text: str
+        :param encoding: str
         :param request_doc_text_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.RequestDocText30.getTargetText
-        response_model = StringResult
+        proxy = self.__client.plunet_server.RequestDocText30.setSourceText2
+        response_model = Result
 
         arg = {
-            "targetLanguage": target_language,
+            "sourceText": source_text,
+            "encoding": encoding,
             "requestDocTextID": request_doc_text_id,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
@@ -265,78 +223,119 @@
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
             unpack_dict=True,
         )
 
-    def get_source_text(self, request_doc_text_id: int) -> StringResult:
+    def set_additional_info(
+        self, additional_info: str, request_doc_text_id: int
+    ) -> Result:
         """
-        Method returns an instance of StringResult, which contains the sourcetext of the currently fetched request text.
+        Method to add additional information to the currently fetched request text.
+        Returns an instance of Result.
 
 
+        :param additional_info: str
         :param request_doc_text_id: int
-        :return: StringResult
+        :return: Result
         """
 
-        proxy = self.__client.plunet_server.RequestDocText30.getSourceText
-        response_model = StringResult
+        proxy = self.__client.plunet_server.RequestDocText30.setAdditionalInfo
+        response_model = Result
+
+        arg = {
+            "additionalInfo": additional_info,
+            "requestDocTextID": request_doc_text_id,
+        }
 
         return self.__client.make_request(
             operation_proxy=proxy,
-            argument=request_doc_text_id,
+            argument=arg,
+            response_model=response_model,
+            unpack_dict=True,
+        )
+
+    def get_all_by_request_id(self, request_id: int) -> IntegerArrayResult:
+        """
+        Returns an instance of IntegerArrayResult, which contains a list of request text identifier for a specific request.
+
+
+        :param request_id: int
+        :return: IntegerArrayResult
+        """
+
+        proxy = self.__client.plunet_server.RequestDocText30.getAll_ByRequestID
+        response_model = IntegerArrayResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=request_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def get_word_count(self, request_doc_text_id: int) -> IntegerResult:
+    def get_customer_text_id(self, request_doc_text_id: int) -> IntegerResult:
         """
-        Returns an instance of IntegerResult, which contains the word count of the currently fetched text.
+        Returns an instance of IntegerResult, which contains the customer text id.
 
 
         :param request_doc_text_id: int
         :return: IntegerResult
         """
 
-        proxy = self.__client.plunet_server.RequestDocText30.getWordCount
+        proxy = self.__client.plunet_server.RequestDocText30.getCustomerTextID
         response_model = IntegerResult
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=request_doc_text_id,
             response_model=response_model,
             unpack_dict=False,
         )
 
-    def set_source_text2(
-        self, source_text: str, encoding: str, request_doc_text_id: int
-    ) -> Result:
+    def get_additional_info(self, request_doc_text_id: int) -> StringResult:
         """
-        Method returns an instance of StringResult, which contains the sourcetext of the currently fetched request text.
-        With the encoding parameter, it is possible to choose the encoding type for the created source file.
-        Valid encoding:
+        Returns an instance of StringResult, which contains the additional information of the currently fetched request text.
 
-        UTF-8
-        UTF-16LE
-        UTF-16BE
-        ANSI
 
+        :param request_doc_text_id: int
+        :return: StringResult
+        """
 
-        :param source_text: str
-        :param encoding: str
+        proxy = self.__client.plunet_server.RequestDocText30.getAdditionalInfo
+        response_model = StringResult
+
+        return self.__client.make_request(
+            operation_proxy=proxy,
+            argument=request_doc_text_id,
+            response_model=response_model,
+            unpack_dict=False,
+        )
+
+    def set_customer_text_id(
+        self, customer_text_id: int, request_doc_text_id: int
+    ) -> Result:
+        """
+        Method to set the customer text id of the currently fetched request text.
+        This value is an external identifier,
+        which is available for free use.
+        Returns an instance of Result.
+
+
+        :param customer_text_id: int
         :param request_doc_text_id: int
         :return: Result
         """
 
-        proxy = self.__client.plunet_server.RequestDocText30.setSourceText2
+        proxy = self.__client.plunet_server.RequestDocText30.setCustomerTextID
         response_model = Result
 
         arg = {
-            "sourceText": source_text,
-            "encoding": encoding,
+            "customerTextID": customer_text_id,
             "requestDocTextID": request_doc_text_id,
         }
 
         return self.__client.make_request(
             operation_proxy=proxy,
             argument=arg,
             response_model=response_model,
```

### Comparing `pyplunet-0.7.0/src/pyplunet/venv/bin/activate_this.py` & `pyplunet-0.8.0/src/pyplunet/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/src/pyplunet.egg-info/PKG-INFO` & `pyplunet-0.8.0/src/pyplunet.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: pyplunet
-Version: 0.7.0
+Version: 0.8.0
 Summary: Client for the Plunet 3.0 SOAP API.
 Author-email: Henrik Kühnemann <hello@yellownape.se>
 Project-URL: Homepage, https://github.com/kuhnemann/pyplunet
 Keywords: plunet,api,translation,localization,tms
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: retry
 License-File: LICENCE
 
 <div id="top"></div>
 
 
 <!-- PROJECT SHIELDS -->
 
@@ -53,17 +52,17 @@
 
 - Implements all services and methods as per Plunet 9.2 (the latest version of ApiDocs available)
 - Fully typed for validation and code completion support
 - Fully documented methods with complete content of the Plunet JavaDocs.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-### New in 0.7.0
-- Retrying client that uses tenacity to retry on ConnectionError from zeep/requests
-- Improved typing for enums - all are still not covered but getting there
+### New in 0.8.0
+- Decided to remove the retrying client 
+- Improved flexibility for enums, which now accept both integers and strings that are possible to cast as ints
 
 ### Built With
 
 * [zeep](https://docs.python-zeep.org/en/master/)
 * [pydantic](https://docs.pydantic.dev/)
 * [plunetapi](https://github.com/kuhnemann/plunetapi/)
 
@@ -81,19 +80,14 @@
 
 Install via pip
 
    ```sh
    pip install pyplunet
    ```
 
-To include tenacity:
-   ```sh
-   pip install pyplunet[retry] 
-   ```
-
 Or clone the repo
 
    ```sh
    git clone https://github.com/kuhnemann/pyplunet.git
    ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,37 +1,36 @@
-Metadata-Version: 2.1 Name: pyplunet Version: 0.7.0 Summary: Client for the
+Metadata-Version: 2.1 Name: pyplunet Version: 0.8.0 Summary: Client for the
 Plunet 3.0 SOAP API. Author-email: Henrik KÃ¼hnemann
 yellownape.se> Project-URL: Homepage, https://github.com/kuhnemann/pyplunet
 Keywords: plunet,api,translation,localization,tms Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.9 Description-Content-
-Type: text/markdown Provides-Extra: dev Provides-Extra: retry License-File:
-LICENCE
+Type: text/markdown Provides-Extra: dev License-File: LICENCE
  [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url] [![MIT License][license-shield]]
 [license-url] [![LinkedIn][linkedin-shield]][linkedin-url]
                               **** PyPlunet ****
       Modern Python client for interacting with the Plunet SOAP 3.0 API.
  ## About The Project Modern Python client for interacting with the Plunet SOAP
 API, without having to deal with any of the soapiness. Ready to use out of the
 box, you can jump directly into the business logic. Pip install, import and
 start working. It really is as easy as that! - Implements all services and
 methods as per Plunet 9.2 (the latest version of ApiDocs available) - Fully
 typed for validation and code completion support - Fully documented methods
 with complete content of the Plunet JavaDocs.
                                                                   (back_to_top)
-### New in 0.7.0 - Retrying client that uses tenacity to retry on
-ConnectionError from zeep/requests - Improved typing for enums - all are still
-not covered but getting there ### Built With * [zeep](https://docs.python-
-zeep.org/en/master/) * [pydantic](https://docs.pydantic.dev/) * [plunetapi]
-(https://github.com/kuhnemann/plunetapi/)
+### New in 0.8.0 - Decided to remove the retrying client - Improved flexibility
+for enums, which now accept both integers and strings that are possible to cast
+as ints ### Built With * [zeep](https://docs.python-zeep.org/en/master/) *
+[pydantic](https://docs.pydantic.dev/) * [plunetapi](https://github.com/
+kuhnemann/plunetapi/)
                                                                   (back_to_top)
  ## Getting Started ### Installation Install via pip ```sh pip install pyplunet
-``` To include tenacity: ```sh pip install pyplunet[retry] ``` Or clone the
-repo ```sh git clone https://github.com/kuhnemann/pyplunet.git ```
+``` Or clone the repo ```sh git clone https://github.com/kuhnemann/pyplunet.git
+```
                                                                   (back_to_top)
  ## Usage Install using pip like so: ```sh pip install pyplunet ``` Initialize
 the client with the base URL of your Plunet instance, authenticate and start
 doing whatever you aim to do. ```sh from pyplunet import PlunetClient
 plunet_client = PlunetClient(base_url="YOUR_URL") plunet_client.login
 (username=username, password=password) order_result =
 plunet_client.order.get_order_object(order_id=1234) ``` Complex types and enums
```

### Comparing `pyplunet-0.7.0/src/pyplunet.egg-info/SOURCES.txt` & `pyplunet-0.8.0/src/pyplunet.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,8 +58,9 @@
 tests/test_DataResourceAddress30.py
 tests/test_DataResourceContact30.py
 tests/test_DataUser30.py
 tests/test_PlunetAPI.py
 tests/test_ReportCustomer30.py
 tests/test_ReportJob30.py
 tests/test_RequestDocText30.py
-tests/test_client_factory.py
+tests/test_client_factory.py
+tests/test_enums.py
```

### Comparing `pyplunet-0.7.0/src/venv/bin/activate_this.py` & `pyplunet-0.8.0/src/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataAdmin30.py` & `pyplunet-0.8.0/tests/test_DataAdmin30.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,18 +144,14 @@
 
 if __name__ == '__main__':
     test_clients = [
         test_client_factory.get_test_client,
         test_client_factory.get_test_client_inmemory_cache,
         test_client_factory.get_test_configured_sql_cache,
         test_client_factory.get_test_client_no_caching,
-        test_client_factory.get_test_retrying_client,
-        test_client_factory.get_test_retrying_client_inmemory_cache,
-        test_client_factory.get_test_retrying_configured_sql_cache,
-        test_client_factory.get_test_retrying_client_no_caching,
     ]
     test_set = get_test_set()
     for client in test_clients:
         print(client.__name__)
         pc = client()
         test_DataAdmin30_get_domestic_currency(pc, test_set)
         test_DataAdmin30_get_available_document_templates(pc, test_set)
```

### Comparing `pyplunet-0.7.0/tests/test_DataCreditNote30.py` & `pyplunet-0.8.0/tests/test_DataCreditNote30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataCustomFields30.py` & `pyplunet-0.8.0/tests/test_DataCustomFields30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataCustomer30.py` & `pyplunet-0.8.0/tests/test_DataCustomer30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataCustomerAddress30.py` & `pyplunet-0.8.0/tests/test_DataCustomerAddress30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataCustomerContact30.py` & `pyplunet-0.8.0/tests/test_DataCustomerContact30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataDocument30.py` & `pyplunet-0.8.0/tests/test_DataDocument30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataItem30.py` & `pyplunet-0.8.0/tests/test_DataItem30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataJob30.py` & `pyplunet-0.8.0/tests/test_DataJob30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataJobRound30.py` & `pyplunet-0.8.0/tests/test_DataJobRound30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataOrder30.py` & `pyplunet-0.8.0/tests/test_DataOrder30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataOutgoingInvoice30.py` & `pyplunet-0.8.0/tests/test_DataOutgoingInvoice30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataPayable30.py` & `pyplunet-0.8.0/tests/test_DataPayable30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataQuote30.py` & `pyplunet-0.8.0/tests/test_DataQuote30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataRequest30.py` & `pyplunet-0.8.0/tests/test_DataRequest30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataResource30.py` & `pyplunet-0.8.0/tests/test_DataResource30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataResourceAddress30.py` & `pyplunet-0.8.0/tests/test_DataResourceAddress30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataResourceContact30.py` & `pyplunet-0.8.0/tests/test_DataResourceContact30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_DataUser30.py` & `pyplunet-0.8.0/tests/test_DataUser30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_PlunetAPI.py` & `pyplunet-0.8.0/tests/test_PlunetAPI.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_ReportCustomer30.py` & `pyplunet-0.8.0/tests/test_ReportCustomer30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_ReportJob30.py` & `pyplunet-0.8.0/tests/test_ReportJob30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_RequestDocText30.py` & `pyplunet-0.8.0/tests/test_RequestDocText30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.7.0/tests/test_client_factory.py` & `pyplunet-0.8.0/tests/test_client_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.pyplunet import PlunetClient, RetryingPlunetClient
+from src.pyplunet import PlunetClient
 import os
 from dotenv import load_dotenv
 load_dotenv()
 from zeep.cache import SqliteCache, InMemoryCache
 from zeep import Transport
 
 def get_test_client(logged_in: bool = True) -> PlunetClient:
@@ -26,33 +26,7 @@
 
 def get_test_configured_sql_cache(logged_in: bool = True) -> PlunetClient:
     cache = SqliteCache(path="test_zeep.db")
     pc = PlunetClient(base_url=os.getenv("TEST_URL"), cache_wsdl=False, transport_options={"cache": cache})
     if logged_in:
         pc.login(os.getenv("TEST_USER"), os.getenv("TEST_PW"))
     return pc
-
-def get_test_retrying_client(logged_in: bool = True) -> PlunetClient:
-    pc = RetryingPlunetClient(base_url=os.getenv("TEST_URL"))
-    if logged_in:
-        pc.login(os.getenv("TEST_USER"), os.getenv("TEST_PW"))
-    return pc
-
-def get_test_retrying_client_no_caching(logged_in: bool = True) -> PlunetClient:
-    pc = RetryingPlunetClient(base_url=os.getenv("TEST_URL"), cache_wsdl=False)
-    if logged_in:
-        pc.login(os.getenv("TEST_USER"), os.getenv("TEST_PW"))
-    return pc
-
-def get_test_retrying_client_inmemory_cache(logged_in: bool = True) -> PlunetClient:
-    transport = Transport(cache=InMemoryCache())
-    pc = RetryingPlunetClient(base_url=os.getenv("TEST_URL"), cache_wsdl=False, transport_options={"transport": transport})
-    if logged_in:
-        pc.login(os.getenv("TEST_USER"), os.getenv("TEST_PW"))
-    return pc
-
-def get_test_retrying_configured_sql_cache(logged_in: bool = True) -> PlunetClient:
-    cache = SqliteCache(path="test_zeep.db")
-    pc = RetryingPlunetClient(base_url=os.getenv("TEST_URL"), cache_wsdl=False, transport_options={"cache": cache})
-    if logged_in:
-        pc.login(os.getenv("TEST_USER"), os.getenv("TEST_PW"))
-    return pc
```

