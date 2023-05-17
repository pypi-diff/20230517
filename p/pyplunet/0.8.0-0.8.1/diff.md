# Comparing `tmp/pyplunet-0.8.0.tar.gz` & `tmp/pyplunet-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplunet-0.8.0.tar", last modified: Wed May 17 21:44:53 2023, max compression
+gzip compressed data, was "pyplunet-0.8.1.tar", last modified: Wed May 17 21:51:31 2023, max compression
```

## Comparing `pyplunet-0.8.0.tar` & `pyplunet-0.8.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.841118 pyplunet-0.8.0/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1067 2022-06-16 21:31:29.000000 pyplunet-0.8.0/LICENCE
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)        0 2022-06-16 21:00:13.000000 pyplunet-0.8.0/MANIFEST.in
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6643 2023-05-17 21:44:53.840984 pyplunet-0.8.0/PKG-INFO
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6132 2023-05-17 21:41:39.000000 pyplunet-0.8.0/README.md
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1141 2023-05-17 21:44:32.000000 pyplunet-0.8.0/pyproject.toml
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       38 2023-05-17 21:44:53.841226 pyplunet-0.8.0/setup.cfg
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       38 2022-06-16 21:32:43.000000 pyplunet-0.8.0/setup.py
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.823533 pyplunet-0.8.0/src/
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.826056 pyplunet-0.8.0/src/pyplunet/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       84 2023-05-17 21:44:32.000000 pyplunet-0.8.0/src/pyplunet/__init__.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     5649 2023-05-08 14:02:53.000000 pyplunet-0.8.0/src/pyplunet/client.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     8664 2023-05-17 21:23:00.000000 pyplunet-0.8.0/src/pyplunet/enums.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    70877 2023-01-24 12:52:24.000000 pyplunet-0.8.0/src/pyplunet/exceptions.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    45076 2023-05-08 14:02:54.000000 pyplunet-0.8.0/src/pyplunet/models.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1853 2023-05-08 13:35:08.000000 pyplunet-0.8.0/src/pyplunet/retrying_client.py
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.829860 pyplunet-0.8.0/src/pyplunet/services/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1530 2023-05-08 13:35:08.000000 pyplunet-0.8.0/src/pyplunet/services/__init__.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     5312 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_admin30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    32871 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_credit_note30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     9551 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_custom_fields30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    39480 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_customer30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    20334 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_customer_address30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    22304 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_customer_contact30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     4324 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_document30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    75559 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_item30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    65279 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_job30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    11742 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_job_round30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    49290 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_order30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    44495 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_outgoing_invoice30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    26853 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_payable30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    34425 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_quote30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    47369 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_request30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    44378 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_resource30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    17453 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_resource_address30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    23191 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_resource_contact30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1970 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/data_user30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1264 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/report_customer30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1154 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/report_job30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    10527 2023-05-17 21:04:16.000000 pyplunet-0.8.0/src/pyplunet/services/request_doc_text30.py
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.823460 pyplunet-0.8.0/src/pyplunet/venv/
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.829995 pyplunet-0.8.0/src/pyplunet/venv/bin/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1176 2023-02-11 15:54:46.000000 pyplunet-0.8.0/src/pyplunet/venv/bin/activate_this.py
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.826774 pyplunet-0.8.0/src/pyplunet.egg-info/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6643 2023-05-17 21:44:53.000000 pyplunet-0.8.0/src/pyplunet.egg-info/PKG-INFO
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     2145 2023-05-17 21:44:53.000000 pyplunet-0.8.0/src/pyplunet.egg-info/SOURCES.txt
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)        1 2023-05-17 21:44:53.000000 pyplunet-0.8.0/src/pyplunet.egg-info/dependency_links.txt
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       74 2023-05-17 21:44:53.000000 pyplunet-0.8.0/src/pyplunet.egg-info/requires.txt
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       14 2023-05-17 21:44:53.000000 pyplunet-0.8.0/src/pyplunet.egg-info/top_level.txt
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.823583 pyplunet-0.8.0/src/venv/
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.831238 pyplunet-0.8.0/src/venv/bin/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1200 2022-11-22 08:52:14.000000 pyplunet-0.8.0/src/venv/bin/activate_this.py
-drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:44:53.840799 pyplunet-0.8.0/tests/
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     5667 2023-05-17 21:41:39.000000 pyplunet-0.8.0/tests/test_DataAdmin30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    32511 2023-05-08 14:14:04.000000 pyplunet-0.8.0/tests/test_DataCreditNote30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6388 2023-05-08 14:14:09.000000 pyplunet-0.8.0/tests/test_DataCustomFields30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    38127 2023-05-08 14:14:06.000000 pyplunet-0.8.0/tests/test_DataCustomer30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    21662 2023-05-08 14:14:07.000000 pyplunet-0.8.0/tests/test_DataCustomerAddress30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    23055 2023-05-08 14:14:07.000000 pyplunet-0.8.0/tests/test_DataCustomerContact30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     3475 2023-05-08 14:14:09.000000 pyplunet-0.8.0/tests/test_DataDocument30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    47839 2023-05-08 14:14:06.000000 pyplunet-0.8.0/tests/test_DataItem30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    42177 2023-05-08 14:14:04.000000 pyplunet-0.8.0/tests/test_DataJob30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    10662 2023-05-08 14:14:05.000000 pyplunet-0.8.0/tests/test_DataJobRound30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    45330 2023-05-08 14:14:05.000000 pyplunet-0.8.0/tests/test_DataOrder30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    45908 2023-05-08 14:14:04.000000 pyplunet-0.8.0/tests/test_DataOutgoingInvoice30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    28255 2023-05-08 14:14:03.000000 pyplunet-0.8.0/tests/test_DataPayable30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    32151 2023-05-08 14:14:05.000000 pyplunet-0.8.0/tests/test_DataQuote30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    42688 2023-05-08 14:14:06.000000 pyplunet-0.8.0/tests/test_DataRequest30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    40943 2023-05-08 14:14:06.000000 pyplunet-0.8.0/tests/test_DataResource30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    18933 2023-05-08 14:14:08.000000 pyplunet-0.8.0/tests/test_DataResourceAddress30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    25135 2023-05-08 14:14:07.000000 pyplunet-0.8.0/tests/test_DataResourceContact30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     2958 2023-05-08 14:14:09.000000 pyplunet-0.8.0/tests/test_DataUser30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     3128 2023-05-08 14:06:14.000000 pyplunet-0.8.0/tests/test_PlunetAPI.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1766 2023-05-08 14:14:07.000000 pyplunet-0.8.0/tests/test_ReportCustomer30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1691 2023-05-08 14:14:05.000000 pyplunet-0.8.0/tests/test_ReportJob30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    10341 2023-05-08 14:14:09.000000 pyplunet-0.8.0/tests/test_RequestDocText30.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1282 2023-05-17 21:41:52.000000 pyplunet-0.8.0/tests/test_client_factory.py
--rw-r--r--   0 henrikkuhnemann   (501) staff       (20)      438 2023-05-17 21:18:03.000000 pyplunet-0.8.0/tests/test_enums.py
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:51:31.869764 pyplunet-0.8.1/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1067 2022-06-16 21:31:29.000000 pyplunet-0.8.1/LICENCE
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)        0 2022-06-16 21:00:13.000000 pyplunet-0.8.1/MANIFEST.in
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6643 2023-05-17 21:51:31.869619 pyplunet-0.8.1/PKG-INFO
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6132 2023-05-17 21:41:39.000000 pyplunet-0.8.1/README.md
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1141 2023-05-17 21:51:20.000000 pyplunet-0.8.1/pyproject.toml
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       38 2023-05-17 21:51:31.869809 pyplunet-0.8.1/setup.cfg
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       38 2022-06-16 21:32:43.000000 pyplunet-0.8.1/setup.py
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:51:31.852366 pyplunet-0.8.1/src/
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:51:31.854845 pyplunet-0.8.1/src/pyplunet/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       84 2023-05-17 21:51:20.000000 pyplunet-0.8.1/src/pyplunet/__init__.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     5649 2023-05-08 14:02:53.000000 pyplunet-0.8.1/src/pyplunet/client.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     8615 2023-05-17 21:50:31.000000 pyplunet-0.8.1/src/pyplunet/enums.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    70877 2023-01-24 12:52:24.000000 pyplunet-0.8.1/src/pyplunet/exceptions.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    45076 2023-05-08 14:02:54.000000 pyplunet-0.8.1/src/pyplunet/models.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1853 2023-05-08 13:35:08.000000 pyplunet-0.8.1/src/pyplunet/retrying_client.py
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:51:31.861969 pyplunet-0.8.1/src/pyplunet/services/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1530 2023-05-08 13:35:08.000000 pyplunet-0.8.1/src/pyplunet/services/__init__.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     5312 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_admin30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    32871 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_credit_note30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     9551 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_custom_fields30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    39480 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_customer30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    20334 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_customer_address30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    22304 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_customer_contact30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     4324 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_document30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    75559 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_item30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    65279 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_job30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    11742 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_job_round30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    49290 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_order30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    44495 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_outgoing_invoice30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    26853 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_payable30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    34425 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_quote30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    47369 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_request30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    44378 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_resource30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    17453 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_resource_address30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    23191 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_resource_contact30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1970 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/data_user30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1264 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/report_customer30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1154 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/report_job30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    10527 2023-05-17 21:04:16.000000 pyplunet-0.8.1/src/pyplunet/services/request_doc_text30.py
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:51:31.852286 pyplunet-0.8.1/src/pyplunet/venv/
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:51:31.862226 pyplunet-0.8.1/src/pyplunet/venv/bin/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1176 2023-02-11 15:54:46.000000 pyplunet-0.8.1/src/pyplunet/venv/bin/activate_this.py
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:51:31.855577 pyplunet-0.8.1/src/pyplunet.egg-info/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6643 2023-05-17 21:51:31.000000 pyplunet-0.8.1/src/pyplunet.egg-info/PKG-INFO
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     2145 2023-05-17 21:51:31.000000 pyplunet-0.8.1/src/pyplunet.egg-info/SOURCES.txt
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)        1 2023-05-17 21:51:31.000000 pyplunet-0.8.1/src/pyplunet.egg-info/dependency_links.txt
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       74 2023-05-17 21:51:31.000000 pyplunet-0.8.1/src/pyplunet.egg-info/requires.txt
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)       14 2023-05-17 21:51:31.000000 pyplunet-0.8.1/src/pyplunet.egg-info/top_level.txt
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:51:31.852420 pyplunet-0.8.1/src/venv/
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:51:31.862471 pyplunet-0.8.1/src/venv/bin/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1200 2022-11-22 08:52:14.000000 pyplunet-0.8.1/src/venv/bin/activate_this.py
+drwxr-xr-x   0 henrikkuhnemann   (501) staff       (20)        0 2023-05-17 21:51:31.869170 pyplunet-0.8.1/tests/
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     5667 2023-05-17 21:41:39.000000 pyplunet-0.8.1/tests/test_DataAdmin30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    32511 2023-05-08 14:14:04.000000 pyplunet-0.8.1/tests/test_DataCreditNote30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     6388 2023-05-08 14:14:09.000000 pyplunet-0.8.1/tests/test_DataCustomFields30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    38127 2023-05-08 14:14:06.000000 pyplunet-0.8.1/tests/test_DataCustomer30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    21662 2023-05-08 14:14:07.000000 pyplunet-0.8.1/tests/test_DataCustomerAddress30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    23055 2023-05-08 14:14:07.000000 pyplunet-0.8.1/tests/test_DataCustomerContact30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     3475 2023-05-08 14:14:09.000000 pyplunet-0.8.1/tests/test_DataDocument30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    47839 2023-05-08 14:14:06.000000 pyplunet-0.8.1/tests/test_DataItem30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    42177 2023-05-08 14:14:04.000000 pyplunet-0.8.1/tests/test_DataJob30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    10662 2023-05-08 14:14:05.000000 pyplunet-0.8.1/tests/test_DataJobRound30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    45330 2023-05-08 14:14:05.000000 pyplunet-0.8.1/tests/test_DataOrder30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    45908 2023-05-08 14:14:04.000000 pyplunet-0.8.1/tests/test_DataOutgoingInvoice30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    28255 2023-05-08 14:14:03.000000 pyplunet-0.8.1/tests/test_DataPayable30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    32151 2023-05-08 14:14:05.000000 pyplunet-0.8.1/tests/test_DataQuote30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    42688 2023-05-08 14:14:06.000000 pyplunet-0.8.1/tests/test_DataRequest30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    40943 2023-05-08 14:14:06.000000 pyplunet-0.8.1/tests/test_DataResource30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    18933 2023-05-08 14:14:08.000000 pyplunet-0.8.1/tests/test_DataResourceAddress30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    25135 2023-05-08 14:14:07.000000 pyplunet-0.8.1/tests/test_DataResourceContact30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     2958 2023-05-08 14:14:09.000000 pyplunet-0.8.1/tests/test_DataUser30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     3128 2023-05-08 14:06:14.000000 pyplunet-0.8.1/tests/test_PlunetAPI.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1766 2023-05-08 14:14:07.000000 pyplunet-0.8.1/tests/test_ReportCustomer30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1691 2023-05-08 14:14:05.000000 pyplunet-0.8.1/tests/test_ReportJob30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)    10341 2023-05-08 14:14:09.000000 pyplunet-0.8.1/tests/test_RequestDocText30.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)     1282 2023-05-17 21:41:52.000000 pyplunet-0.8.1/tests/test_client_factory.py
+-rw-r--r--   0 henrikkuhnemann   (501) staff       (20)      438 2023-05-17 21:18:03.000000 pyplunet-0.8.1/tests/test_enums.py
```

### Comparing `pyplunet-0.8.0/LICENCE` & `pyplunet-0.8.1/LICENCE`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/PKG-INFO` & `pyplunet-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplunet
-Version: 0.8.0
+Version: 0.8.1
 Summary: Client for the Plunet 3.0 SOAP API.
 Author-email: Henrik Kühnemann <hello@yellownape.se>
 Project-URL: Homepage, https://github.com/kuhnemann/pyplunet
 Keywords: plunet,api,translation,localization,tms
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyplunet Version: 0.8.0 Summary: Client for the
+Metadata-Version: 2.1 Name: pyplunet Version: 0.8.1 Summary: Client for the
 Plunet 3.0 SOAP API. Author-email: Henrik KÃ¼hnemann
 yellownape.se> Project-URL: Homepage, https://github.com/kuhnemann/pyplunet
 Keywords: plunet,api,translation,localization,tms Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.9 Description-Content-
 Type: text/markdown Provides-Extra: dev License-File: LICENCE
  [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url]
```

### Comparing `pyplunet-0.8.0/README.md` & `pyplunet-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/pyproject.toml` & `pyplunet-0.8.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyplunet"
-version = "0.8.0"
+version = "0.8.1"
 description = "Client for the Plunet 3.0 SOAP API."
 readme = "README.md"
 authors = [{ name = "Henrik Kühnemann", email = "hello@yellownape.se" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -26,15 +26,15 @@
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/kuhnemann/pyplunet"
 
 
 [tool.bumpver]
-current_version = "0.8.0"
+current_version = "0.8.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyplunet-0.8.0/src/pyplunet/client.py` & `pyplunet-0.8.1/src/pyplunet/client.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/enums.py` & `pyplunet-0.8.1/src/pyplunet/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         try:
             int_value = int(value)
             for member in cls:
                 if member.name == value or member.value == int_value:
                     return member
         except ValueError:
             pass
-        raise ValueError(f"{value} ({type(value)}) is not a valid {cls.__name__}. Valid values: {', '.join([str(x) for x in cls])}")
+        raise ValueError(f"{value} ({type(value)}) is not a valid {cls.__name__}.")
 
 
 class SearchSelection_Resource(StrIntEnum):
     AGENCY = 9
     RESOURCE = 1
```

### Comparing `pyplunet-0.8.0/src/pyplunet/exceptions.py` & `pyplunet-0.8.1/src/pyplunet/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/models.py` & `pyplunet-0.8.1/src/pyplunet/models.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/retrying_client.py` & `pyplunet-0.8.1/src/pyplunet/retrying_client.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/__init__.py` & `pyplunet-0.8.1/src/pyplunet/services/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_admin30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_admin30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_credit_note30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_credit_note30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_custom_fields30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_custom_fields30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_customer30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_customer30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_customer_address30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_customer_address30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_customer_contact30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_customer_contact30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_document30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_document30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_item30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_item30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_job30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_job30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_job_round30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_job_round30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_order30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_order30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_outgoing_invoice30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_outgoing_invoice30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_payable30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_payable30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_quote30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_quote30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_request30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_request30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_resource30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_resource30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_resource_address30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_resource_address30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_resource_contact30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_resource_contact30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/data_user30.py` & `pyplunet-0.8.1/src/pyplunet/services/data_user30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/report_customer30.py` & `pyplunet-0.8.1/src/pyplunet/services/report_customer30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/report_job30.py` & `pyplunet-0.8.1/src/pyplunet/services/report_job30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/services/request_doc_text30.py` & `pyplunet-0.8.1/src/pyplunet/services/request_doc_text30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet/venv/bin/activate_this.py` & `pyplunet-0.8.1/src/pyplunet/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/pyplunet.egg-info/PKG-INFO` & `pyplunet-0.8.1/src/pyplunet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplunet
-Version: 0.8.0
+Version: 0.8.1
 Summary: Client for the Plunet 3.0 SOAP API.
 Author-email: Henrik Kühnemann <hello@yellownape.se>
 Project-URL: Homepage, https://github.com/kuhnemann/pyplunet
 Keywords: plunet,api,translation,localization,tms
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyplunet Version: 0.8.0 Summary: Client for the
+Metadata-Version: 2.1 Name: pyplunet Version: 0.8.1 Summary: Client for the
 Plunet 3.0 SOAP API. Author-email: Henrik KÃ¼hnemann
 yellownape.se> Project-URL: Homepage, https://github.com/kuhnemann/pyplunet
 Keywords: plunet,api,translation,localization,tms Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.9 Description-Content-
 Type: text/markdown Provides-Extra: dev License-File: LICENCE
  [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url]
```

### Comparing `pyplunet-0.8.0/src/pyplunet.egg-info/SOURCES.txt` & `pyplunet-0.8.1/src/pyplunet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/src/venv/bin/activate_this.py` & `pyplunet-0.8.1/src/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataAdmin30.py` & `pyplunet-0.8.1/tests/test_DataAdmin30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataCreditNote30.py` & `pyplunet-0.8.1/tests/test_DataCreditNote30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataCustomFields30.py` & `pyplunet-0.8.1/tests/test_DataCustomFields30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataCustomer30.py` & `pyplunet-0.8.1/tests/test_DataCustomer30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataCustomerAddress30.py` & `pyplunet-0.8.1/tests/test_DataCustomerAddress30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataCustomerContact30.py` & `pyplunet-0.8.1/tests/test_DataCustomerContact30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataDocument30.py` & `pyplunet-0.8.1/tests/test_DataDocument30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataItem30.py` & `pyplunet-0.8.1/tests/test_DataItem30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataJob30.py` & `pyplunet-0.8.1/tests/test_DataJob30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataJobRound30.py` & `pyplunet-0.8.1/tests/test_DataJobRound30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataOrder30.py` & `pyplunet-0.8.1/tests/test_DataOrder30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataOutgoingInvoice30.py` & `pyplunet-0.8.1/tests/test_DataOutgoingInvoice30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataPayable30.py` & `pyplunet-0.8.1/tests/test_DataPayable30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataQuote30.py` & `pyplunet-0.8.1/tests/test_DataQuote30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataRequest30.py` & `pyplunet-0.8.1/tests/test_DataRequest30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataResource30.py` & `pyplunet-0.8.1/tests/test_DataResource30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataResourceAddress30.py` & `pyplunet-0.8.1/tests/test_DataResourceAddress30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataResourceContact30.py` & `pyplunet-0.8.1/tests/test_DataResourceContact30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_DataUser30.py` & `pyplunet-0.8.1/tests/test_DataUser30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_PlunetAPI.py` & `pyplunet-0.8.1/tests/test_PlunetAPI.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_ReportCustomer30.py` & `pyplunet-0.8.1/tests/test_ReportCustomer30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_ReportJob30.py` & `pyplunet-0.8.1/tests/test_ReportJob30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_RequestDocText30.py` & `pyplunet-0.8.1/tests/test_RequestDocText30.py`

 * *Files identical despite different names*

### Comparing `pyplunet-0.8.0/tests/test_client_factory.py` & `pyplunet-0.8.1/tests/test_client_factory.py`

 * *Files identical despite different names*

