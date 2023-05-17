# Comparing `tmp/django-oscar-wfrs-5.1.2.tar.gz` & `tmp/django-oscar-wfrs-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oscar-wfrs-5.1.2.tar", last modified: Wed May 10 22:09:57 2023, max compression
+gzip compressed data, was "django-oscar-wfrs-5.1.3.tar", last modified: Wed May 17 17:48:17 2023, max compression
```

## Comparing `django-oscar-wfrs-5.1.2.tar` & `django-oscar-wfrs-5.1.3.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.980434 django-oscar-wfrs-5.1.2/
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1820 2023-05-10 22:09:57.980434 django-oscar-wfrs-5.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1514 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-05-10 22:09:57.980434 django-oscar-wfrs-5.1.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2257 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.917427 django-oscar-wfrs-5.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.927428 django-oscar-wfrs-5.1.2/src/django_oscar_wfrs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1820 2023-05-10 22:09:57.000000 django-oscar-wfrs-5.1.2/src/django_oscar_wfrs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7966 2023-05-10 22:09:57.000000 django-oscar-wfrs-5.1.2/src/django_oscar_wfrs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 22:09:57.000000 django-oscar-wfrs-5.1.2/src/django_oscar_wfrs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      535 2023-05-10 22:09:57.000000 django-oscar-wfrs-5.1.2/src/django_oscar_wfrs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-10 22:09:57.000000 django-oscar-wfrs-5.1.2/src/django_oscar_wfrs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.930428 django-oscar-wfrs-5.1.2/src/wellsfargo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2401 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.931429 django-oscar-wfrs-5.1.2/src/wellsfargo/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2796 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/api/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/api/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    13924 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)    14193 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.934429 django-oscar-wfrs-5.1.2/src/wellsfargo/connector/
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/connector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5576 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/connector/accounts.py
--rw-rw-rw-   0 root         (0) root         (0)     6837 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/connector/applications.py
--rw-rw-rw-   0 root         (0) root         (0)     6238 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/connector/client.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/connector/health.py
--rw-rw-rw-   0 root         (0) root         (0)     2925 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/connector/prequal.py
--rw-rw-rw-   0 root         (0) root         (0)     3936 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/connector/transactions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.936429 django-oscar-wfrs-5.1.2/src/wellsfargo/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8087 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/core/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/core/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1958 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/core/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/core/signals.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/core/structures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.937429 django-oscar-wfrs-5.1.2/src/wellsfargo/dashboard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/dashboard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3695 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/dashboard/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     3263 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/dashboard/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     9524 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/dashboard/tables.py
--rw-rw-rw-   0 root         (0) root         (0)    19657 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/dashboard/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.938429 django-oscar-wfrs-5.1.2/src/wellsfargo/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/fixtures/wfrs-test.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.939429 django-oscar-wfrs-5.1.2/src/wellsfargo/fraud/
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/fraud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10440 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/fraud/cybersource.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/fraud/dummy.py
--rw-rw-rw-   0 root         (0) root         (0)     1172 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.919427 django-oscar-wfrs-5.1.2/src/wellsfargo/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.919427 django-oscar-wfrs-5.1.2/src/wellsfargo/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.939429 django-oscar-wfrs-5.1.2/src/wellsfargo/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    43450 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/locale/es/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     9352 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/methods.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.953431 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    66475 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0001_squash_060.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0002_transfermetadata_credentials.py
--rw-rw-rw-   0 root         (0) root         (0)    11940 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0003_auto_20170510_1633.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0004_auto_20170510_1712.py
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0005_financingplan_fine_print_superscript.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0006_financingplan_product_price_threshold.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0007_financingplan_advertising_enabled.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0008_fraudscreenresult.py
--rw-rw-rw-   0 root         (0) root         (0)     1206 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0009_auto_20171005_1541.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0010_fraudscreenresult_reference.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0011_auto_20171204_1506.py
--rw-rw-rw-   0 root         (0) root         (0)     4716 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0012_auto_20180102_1147.py
--rw-rw-rw-   0 root         (0) root         (0)     6304 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0013_prequalificationrequest_prequalificationresponse.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0014_auto_20180222_1432.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0015_prequalificationresponse_reported_datetime.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0016_prequalificationresponse_customer_order.py
--rw-rw-rw-   0 root         (0) root         (0)     1759 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0017_auto_20180302_1843.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0018_auto_20181019_1924.py
--rw-rw-rw-   0 root         (0) root         (0)      534 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0019_prequalificationrequest_customer_initiated.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0020_prequalificationsdkapplicationresult.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0021_auto_20181105_1602.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0022_auto_20181220_1057.py
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0023_auto_20190125_1153.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0024_auto_20190125_1248.py
--rw-rw-rw-   0 root         (0) root         (0)     3674 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0025_auto_20190208_1431.py
--rw-rw-rw-   0 root         (0) root         (0)     1438 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0026_auto_20190208_1629.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0027_auto_20190208_1635.py
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0028_auto_20190401_1213.py
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0029_auto_20190401_1233.py
--rw-rw-rw-   0 root         (0) root         (0)     4601 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0030_auto_20190719_1500.py
--rw-rw-rw-   0 root         (0) root         (0)     3024 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0031_creditappindex.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0032_auto_20191209_1348.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0033_auto_20191209_1358.py
--rw-rw-rw-   0 root         (0) root         (0)    18229 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0034_auto_20200326_1411.py
--rw-rw-rw-   0 root         (0) root         (0)    13104 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0035_auto_20200326_1412.py
--rw-rw-rw-   0 root         (0) root         (0)     7646 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0036_auto_20200326_1430.py
--rw-rw-rw-   0 root         (0) root         (0)     3875 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0037_auto_20200402_1108.py
--rw-rw-rw-   0 root         (0) root         (0)     6532 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0038_auto_20200415_1233.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0039_auto_20200420_1719.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.956431 django-oscar-wfrs-5.1.2/src/wellsfargo/models/
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1959 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/models/accounts.py
--rw-rw-rw-   0 root         (0) root         (0)     9179 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/models/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1383 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/models/fraud.py
--rw-rw-rw-   0 root         (0) root         (0)     1631 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/models/merchants.py
--rw-rw-rw-   0 root         (0) root         (0)     1664 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/models/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     4754 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/models/plans.py
--rw-rw-rw-   0 root         (0) root         (0)     9744 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/models/prequal.py
--rw-rw-rw-   0 root         (0) root         (0)     3002 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/models/transfers.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/models/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.957431 django-oscar-wfrs-5.1.2/src/wellsfargo/security/
--rw-rw-rw-   0 root         (0) root         (0)     1647 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/security/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1215 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/security/fernet.py
--rw-rw-rw-   0 root         (0) root         (0)     2443 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/security/kms.py
--rw-rw-rw-   0 root         (0) root         (0)     2052 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/security/multi.py
--rw-rw-rw-   0 root         (0) root         (0)     2449 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.921427 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.921427 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/oscar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.921427 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/oscar/dashboard/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.958431 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/oscar/dashboard/users/
--rw-rw-rw-   0 root         (0) root         (0)     1533 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/oscar/dashboard/users/detail.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.922428 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.969433 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/
--rw-rw-rw-   0 root         (0) root         (0)     2510 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_detail_applicant.html
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_row_account_number.html
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_row_actions.html
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_row_credit_limit.html
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_row_main_applicant_name.html
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_row_order_delay.html
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_row_order_merchant_name.html
--rw-rw-rw-   0 root         (0) root         (0)      276 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_row_order_total.html
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_row_purchase_price.html
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_row_secondary_applicant_name.html
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_row_submitting_user.html
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_row_type.html
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_row_user.html
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_prequal_row_address.html
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_prequal_row_credit_limit.html
--rw-rw-rw-   0 root         (0) root         (0)      542 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_prequal_row_order_delay.html
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_prequal_row_order_total.html
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_sdk_application_row_prequal_link.html
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_transfer_row_order.html
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_transfer_row_user.html
--rw-rw-rw-   0 root         (0) root         (0)     4059 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/application_detail.html
--rw-rw-rw-   0 root         (0) root         (0)     4392 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/application_list.html
--rw-rw-rw-   0 root         (0) root         (0)     1715 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/benefit_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/benefit_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2089 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/benefit_list.html
--rw-rw-rw-   0 root         (0) root         (0)     2190 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/form_base.html
--rw-rw-rw-   0 root         (0) root         (0)     2035 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/plan_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     1983 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/plan_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2936 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/plan_list.html
--rw-rw-rw-   0 root         (0) root         (0)    10410 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/prequal_detail.html
--rw-rw-rw-   0 root         (0) root         (0)     4259 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/prequal_list.html
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/responsive-table.html
--rw-rw-rw-   0 root         (0) root         (0)     4237 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/sdk_application_list.html
--rw-rw-rw-   0 root         (0) root         (0)     4115 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/transfer_detail.html
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/transfer_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.971433 django-oscar-wfrs-5.1.2/src/wellsfargo/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templatetags/wfrs_credit_apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templatetags/wfrs_default_plan.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/templatetags/wfrs_filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.973433 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.976433 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14760 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/test_api_checkout.py
--rw-rw-rw-   0 root         (0) root         (0)     9442 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/test_api_credit_app.py
--rw-rw-rw-   0 root         (0) root         (0)     3290 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/test_estimated_payments.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2686 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/test_inquiry.py
--rw-rw-rw-   0 root         (0) root         (0)    12352 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/test_prequal.py
--rw-rw-rw-   0 root         (0) root         (0)    11591 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.978434 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8300 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/test_accounts.py
--rw-rw-rw-   0 root         (0) root         (0)     9324 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/test_applications.py
--rw-rw-rw-   0 root         (0) root         (0)     2944 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/test_health.py
--rw-rw-rw-   0 root         (0) root         (0)     4136 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/test_prequal.py
--rw-rw-rw-   0 root         (0) root         (0)     4521 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/test_transactions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.979434 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/dashboard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/dashboard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3003 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/dashboard/test_forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 22:09:57.980434 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/responses/
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/responses/cybersource_accept.xml
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/responses/cybersource_reject.xml
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/responses/cybersource_review.xml
--rw-rw-rw-   0 root         (0) root         (0)      452 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/responses.py
--rw-rw-rw-   0 root         (0) root         (0)     3969 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/test_fraud.py
--rw-rw-rw-   0 root         (0) root         (0)    15522 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     8171 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/test_security.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-10 22:09:44.000000 django-oscar-wfrs-5.1.2/src/wellsfargo/utils.py
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-10 22:09:57.000000 django-oscar-wfrs-5.1.2/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.859216 django-oscar-wfrs-5.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-05-17 17:48:17.859216 django-oscar-wfrs-5.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1514 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-05-17 17:48:17.860216 django-oscar-wfrs-5.1.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2257 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.829216 django-oscar-wfrs-5.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.833216 django-oscar-wfrs-5.1.3/src/django_oscar_wfrs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-05-17 17:48:17.000000 django-oscar-wfrs-5.1.3/src/django_oscar_wfrs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7966 2023-05-17 17:48:17.000000 django-oscar-wfrs-5.1.3/src/django_oscar_wfrs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 17:48:17.000000 django-oscar-wfrs-5.1.3/src/django_oscar_wfrs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      535 2023-05-17 17:48:17.000000 django-oscar-wfrs-5.1.3/src/django_oscar_wfrs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-17 17:48:17.000000 django-oscar-wfrs-5.1.3/src/django_oscar_wfrs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.834216 django-oscar-wfrs-5.1.3/src/wellsfargo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.835216 django-oscar-wfrs-5.1.3/src/wellsfargo/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/api/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13924 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)    14193 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.836216 django-oscar-wfrs-5.1.3/src/wellsfargo/connector/
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/connector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5576 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/connector/accounts.py
+-rw-rw-rw-   0 root         (0) root         (0)     6837 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/connector/applications.py
+-rw-rw-rw-   0 root         (0) root         (0)     6238 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/connector/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/connector/health.py
+-rw-rw-rw-   0 root         (0) root         (0)     3012 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/connector/prequal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3936 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/connector/transactions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.837216 django-oscar-wfrs-5.1.3/src/wellsfargo/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8087 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/core/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/core/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1958 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/core/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/core/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/core/structures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.838216 django-oscar-wfrs-5.1.3/src/wellsfargo/dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/dashboard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3695 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/dashboard/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3263 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/dashboard/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     9524 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/dashboard/tables.py
+-rw-rw-rw-   0 root         (0) root         (0)    19657 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/dashboard/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.838216 django-oscar-wfrs-5.1.3/src/wellsfargo/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/fixtures/wfrs-test.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.839216 django-oscar-wfrs-5.1.3/src/wellsfargo/fraud/
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/fraud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10440 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/fraud/cybersource.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/fraud/dummy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1172 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.830216 django-oscar-wfrs-5.1.3/src/wellsfargo/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.830216 django-oscar-wfrs-5.1.3/src/wellsfargo/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.839216 django-oscar-wfrs-5.1.3/src/wellsfargo/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    43450 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/locale/es/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     9352 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/methods.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.846216 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    66475 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0001_squash_060.py
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0002_transfermetadata_credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)    11940 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0003_auto_20170510_1633.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0004_auto_20170510_1712.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0005_financingplan_fine_print_superscript.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0006_financingplan_product_price_threshold.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0007_financingplan_advertising_enabled.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0008_fraudscreenresult.py
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0009_auto_20171005_1541.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0010_fraudscreenresult_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0011_auto_20171204_1506.py
+-rw-rw-rw-   0 root         (0) root         (0)     4716 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0012_auto_20180102_1147.py
+-rw-rw-rw-   0 root         (0) root         (0)     6304 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0013_prequalificationrequest_prequalificationresponse.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0014_auto_20180222_1432.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0015_prequalificationresponse_reported_datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0016_prequalificationresponse_customer_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     1759 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0017_auto_20180302_1843.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0018_auto_20181019_1924.py
+-rw-rw-rw-   0 root         (0) root         (0)      534 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0019_prequalificationrequest_customer_initiated.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0020_prequalificationsdkapplicationresult.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0021_auto_20181105_1602.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0022_auto_20181220_1057.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0023_auto_20190125_1153.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0024_auto_20190125_1248.py
+-rw-rw-rw-   0 root         (0) root         (0)     3674 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0025_auto_20190208_1431.py
+-rw-rw-rw-   0 root         (0) root         (0)     1438 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0026_auto_20190208_1629.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0027_auto_20190208_1635.py
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0028_auto_20190401_1213.py
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0029_auto_20190401_1233.py
+-rw-rw-rw-   0 root         (0) root         (0)     4601 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0030_auto_20190719_1500.py
+-rw-rw-rw-   0 root         (0) root         (0)     3024 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0031_creditappindex.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0032_auto_20191209_1348.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0033_auto_20191209_1358.py
+-rw-rw-rw-   0 root         (0) root         (0)    18229 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0034_auto_20200326_1411.py
+-rw-rw-rw-   0 root         (0) root         (0)    13104 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0035_auto_20200326_1412.py
+-rw-rw-rw-   0 root         (0) root         (0)     7646 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0036_auto_20200326_1430.py
+-rw-rw-rw-   0 root         (0) root         (0)     3875 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0037_auto_20200402_1108.py
+-rw-rw-rw-   0 root         (0) root         (0)     6532 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0038_auto_20200415_1233.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0039_auto_20200420_1719.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.847216 django-oscar-wfrs-5.1.3/src/wellsfargo/models/
+-rw-rw-rw-   0 root         (0) root         (0)      274 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1959 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/models/accounts.py
+-rw-rw-rw-   0 root         (0) root         (0)     9179 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/models/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1383 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/models/fraud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/models/merchants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1664 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/models/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     4754 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/models/plans.py
+-rw-rw-rw-   0 root         (0) root         (0)     9744 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/models/prequal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3002 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/models/transfers.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/models/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.848216 django-oscar-wfrs-5.1.3/src/wellsfargo/security/
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/security/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/security/fernet.py
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/security/kms.py
+-rw-rw-rw-   0 root         (0) root         (0)     2052 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/security/multi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2449 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.831216 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.831216 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/oscar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.831216 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/oscar/dashboard/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.848216 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/oscar/dashboard/users/
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/oscar/dashboard/users/detail.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.831216 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.854216 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_detail_applicant.html
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_row_account_number.html
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_row_actions.html
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_row_credit_limit.html
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_row_main_applicant_name.html
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_row_order_delay.html
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_row_order_merchant_name.html
+-rw-rw-rw-   0 root         (0) root         (0)      276 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_row_order_total.html
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_row_purchase_price.html
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_row_secondary_applicant_name.html
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_row_submitting_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_row_type.html
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_row_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_prequal_row_address.html
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_prequal_row_credit_limit.html
+-rw-rw-rw-   0 root         (0) root         (0)      542 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_prequal_row_order_delay.html
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_prequal_row_order_total.html
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_sdk_application_row_prequal_link.html
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_transfer_row_order.html
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_transfer_row_user.html
+-rw-rw-rw-   0 root         (0) root         (0)     4059 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/application_detail.html
+-rw-rw-rw-   0 root         (0) root         (0)     4392 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/application_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     1715 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/benefit_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/benefit_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2089 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/benefit_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/form_base.html
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/plan_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1983 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/plan_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2936 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/plan_list.html
+-rw-rw-rw-   0 root         (0) root         (0)    10410 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/prequal_detail.html
+-rw-rw-rw-   0 root         (0) root         (0)     4259 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/prequal_list.html
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/responsive-table.html
+-rw-rw-rw-   0 root         (0) root         (0)     4237 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/sdk_application_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     4115 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/transfer_detail.html
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/transfer_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.855216 django-oscar-wfrs-5.1.3/src/wellsfargo/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templatetags/wfrs_credit_apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templatetags/wfrs_default_plan.py
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/templatetags/wfrs_filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.856216 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.857216 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14760 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/test_api_checkout.py
+-rw-rw-rw-   0 root         (0) root         (0)     9442 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/test_api_credit_app.py
+-rw-rw-rw-   0 root         (0) root         (0)     3290 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/test_estimated_payments.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2686 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/test_inquiry.py
+-rw-rw-rw-   0 root         (0) root         (0)    12352 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/test_prequal.py
+-rw-rw-rw-   0 root         (0) root         (0)    11591 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.858216 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8300 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/test_accounts.py
+-rw-rw-rw-   0 root         (0) root         (0)     9324 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/test_applications.py
+-rw-rw-rw-   0 root         (0) root         (0)     2944 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/test_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/test_health.py
+-rw-rw-rw-   0 root         (0) root         (0)     4138 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/test_prequal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4521 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/test_transactions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.858216 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/dashboard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3003 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/dashboard/test_forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:48:17.859216 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/responses/
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/responses/cybersource_accept.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/responses/cybersource_reject.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/responses/cybersource_review.xml
+-rw-rw-rw-   0 root         (0) root         (0)      452 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)     3969 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/test_fraud.py
+-rw-rw-rw-   0 root         (0) root         (0)    15522 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     8171 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/test_security.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-17 17:48:07.000000 django-oscar-wfrs-5.1.3/src/wellsfargo/utils.py
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-17 17:48:17.000000 django-oscar-wfrs-5.1.3/version.txt
```

### Comparing `django-oscar-wfrs-5.1.2/LICENSE` & `django-oscar-wfrs-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/PKG-INFO` & `django-oscar-wfrs-5.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-wfrs
-Version: 5.1.2
+Version: 5.1.3
 Summary: An extension on-top of django-oscar-api-checkout to allow interfacing with Wells Fargo Retail Services.
 Home-page: https://gitlab.com/thelabnyc/django-oscar-wfrs
 Author: thelabnyc
 Author-email: thelabdev@thelabnyc.com
 License: ISC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-oscar-wfrs-5.1.2/README.rst` & `django-oscar-wfrs-5.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/requirements.txt` & `django-oscar-wfrs-5.1.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/setup.py` & `django-oscar-wfrs-5.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/django_oscar_wfrs.egg-info/PKG-INFO` & `django-oscar-wfrs-5.1.3/src/django_oscar_wfrs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-wfrs
-Version: 5.1.2
+Version: 5.1.3
 Summary: An extension on-top of django-oscar-api-checkout to allow interfacing with Wells Fargo Retail Services.
 Home-page: https://gitlab.com/thelabnyc/django-oscar-wfrs
 Author: thelabnyc
 Author-email: thelabdev@thelabnyc.com
 License: ISC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-oscar-wfrs-5.1.2/src/django_oscar_wfrs.egg-info/SOURCES.txt` & `django-oscar-wfrs-5.1.3/src/django_oscar_wfrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/django_oscar_wfrs.egg-info/requires.txt` & `django-oscar-wfrs-5.1.3/src/django_oscar_wfrs.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/admin.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/api/apps.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/api/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/api/exceptions.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/api/serializers.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/api/views.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/api/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/connector/accounts.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/connector/accounts.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/connector/applications.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/connector/applications.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/connector/client.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/connector/client.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/connector/prequal.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/connector/prequal.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
             "merchant_number": creds.merchant_num,
             "transaction_code": PREQUAL_TRANS_CODE_MERCHANT_INITIATED_PRESCREEN,
             "main_applicant": {
                 "first_name": prequal_request.first_name,
                 "middle_initial": prequal_request.middle_initial,
                 "last_name": prequal_request.last_name,
                 "phone_number": format_phone(prequal_request.phone),
-                "email": prequal_request.email,
+                # Email is no longer allowed to be sent for the P1 transaction type.
+                # "email": prequal_request.email,
                 "last_four_ssn": None,
                 "address": {
                     "address_line_1": prequal_request.line1,
                     "address_line_2": prequal_request.line2,
                     "city": prequal_request.city,
                     "state_code": prequal_request.state,
                     "postal_code": prequal_request.postcode,
```

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/connector/transactions.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/connector/transactions.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/core/constants.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/core/constants.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/core/fields.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/core/fields.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/dashboard/apps.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/dashboard/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/dashboard/forms.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/dashboard/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/dashboard/tables.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/dashboard/tables.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/dashboard/views.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/dashboard/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/fraud/__init__.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/fraud/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/fraud/cybersource.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/fraud/cybersource.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/fraud/dummy.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/fraud/dummy.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/handlers.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/handlers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/locale/es/LC_MESSAGES/django.po` & `django-oscar-wfrs-5.1.3/src/wellsfargo/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/methods.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/methods.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0001_squash_060.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0001_squash_060.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0002_transfermetadata_credentials.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0002_transfermetadata_credentials.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0003_auto_20170510_1633.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0003_auto_20170510_1633.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0004_auto_20170510_1712.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0004_auto_20170510_1712.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0005_financingplan_fine_print_superscript.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0005_financingplan_fine_print_superscript.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0006_financingplan_product_price_threshold.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0006_financingplan_product_price_threshold.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0007_financingplan_advertising_enabled.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0007_financingplan_advertising_enabled.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0008_fraudscreenresult.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0008_fraudscreenresult.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0009_auto_20171005_1541.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0009_auto_20171005_1541.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0010_fraudscreenresult_reference.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0010_fraudscreenresult_reference.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0011_auto_20171204_1506.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0011_auto_20171204_1506.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0012_auto_20180102_1147.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0012_auto_20180102_1147.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0013_prequalificationrequest_prequalificationresponse.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0013_prequalificationrequest_prequalificationresponse.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0014_auto_20180222_1432.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0014_auto_20180222_1432.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0015_prequalificationresponse_reported_datetime.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0015_prequalificationresponse_reported_datetime.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0016_prequalificationresponse_customer_order.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0016_prequalificationresponse_customer_order.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0017_auto_20180302_1843.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0017_auto_20180302_1843.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0018_auto_20181019_1924.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0018_auto_20181019_1924.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0019_prequalificationrequest_customer_initiated.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0019_prequalificationrequest_customer_initiated.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0020_prequalificationsdkapplicationresult.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0020_prequalificationsdkapplicationresult.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0021_auto_20181105_1602.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0021_auto_20181105_1602.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0022_auto_20181220_1057.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0022_auto_20181220_1057.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0024_auto_20190125_1248.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0024_auto_20190125_1248.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0025_auto_20190208_1431.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0025_auto_20190208_1431.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0026_auto_20190208_1629.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0026_auto_20190208_1629.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0027_auto_20190208_1635.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0027_auto_20190208_1635.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0028_auto_20190401_1213.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0028_auto_20190401_1213.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0029_auto_20190401_1233.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0029_auto_20190401_1233.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0030_auto_20190719_1500.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0030_auto_20190719_1500.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0031_creditappindex.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0031_creditappindex.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0032_auto_20191209_1348.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0032_auto_20191209_1348.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0033_auto_20191209_1358.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0033_auto_20191209_1358.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0034_auto_20200326_1411.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0034_auto_20200326_1411.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0035_auto_20200326_1412.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0035_auto_20200326_1412.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0036_auto_20200326_1430.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0036_auto_20200326_1430.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0037_auto_20200402_1108.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0037_auto_20200402_1108.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0038_auto_20200415_1233.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0038_auto_20200415_1233.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/migrations/0039_auto_20200420_1719.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/migrations/0039_auto_20200420_1719.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/models/accounts.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/models/accounts.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/models/apps.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/models/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/models/fraud.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/models/fraud.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/models/merchants.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/models/merchants.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/models/mixins.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/models/mixins.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/models/plans.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/models/plans.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/models/prequal.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/models/prequal.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/models/transfers.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/models/transfers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/security/__init__.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/security/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/security/fernet.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/security/fernet.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/security/kms.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/security/kms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/security/multi.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/security/multi.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/settings.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/settings.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/oscar/dashboard/users/detail.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/oscar/dashboard/users/detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_detail_applicant.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_detail_applicant.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_application_row_order_delay.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_application_row_order_delay.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/_prequal_row_order_delay.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/_prequal_row_order_delay.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/application_detail.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/application_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/application_list.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/application_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/benefit_delete.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/benefit_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/benefit_form.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/benefit_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/benefit_list.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/benefit_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/form_base.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/form_base.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/plan_delete.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/plan_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/plan_form.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/plan_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/plan_list.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/plan_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/prequal_detail.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/prequal_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/prequal_list.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/prequal_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/sdk_application_list.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/sdk_application_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/transfer_detail.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/transfer_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templates/wfrs/dashboard/transfer_list.html` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templates/wfrs/dashboard/transfer_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templatetags/wfrs_credit_apps.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templatetags/wfrs_credit_apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templatetags/wfrs_default_plan.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templatetags/wfrs_default_plan.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/templatetags/wfrs_filters.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/templatetags/wfrs_filters.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/test_api_checkout.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/test_api_checkout.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/test_api_credit_app.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/test_api_credit_app.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/test_estimated_payments.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/test_estimated_payments.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/test_exceptions.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/test_inquiry.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/test_inquiry.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/api/test_prequal.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/api/test_prequal.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/base.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/test_accounts.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/test_accounts.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/test_applications.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/test_applications.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/test_client.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/test_client.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/test_health.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/test_health.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/test_prequal.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/test_prequal.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                 {
                     "merchant_number": "1111111111111111",
                     "transaction_code": "P1",
                     "main_applicant": {
                         "first_name": "Demo",
                         "last_name": "Tester",
                         "phone_number": "2122091333",
-                        "email": "demo@wellsfargo.com",
+                        # "email": "demo@wellsfargo.com",
                         "address": {
                             "address_line_1": "800 Walnut St",
                             "city": "Des Moines",
                             "state_code": "IA",
                             "postal_code": "50309",
                         },
                     },
```

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/connector/test_transactions.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/connector/test_transactions.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/dashboard/test_forms.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/dashboard/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/responses/cybersource_accept.xml` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/responses/cybersource_accept.xml`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/responses/cybersource_reject.xml` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/responses/cybersource_reject.xml`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/responses/cybersource_review.xml` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/responses/cybersource_review.xml`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/test_fraud.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/test_fraud.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/test_models.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/test_security.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/tests/test_tags.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `django-oscar-wfrs-5.1.2/src/wellsfargo/utils.py` & `django-oscar-wfrs-5.1.3/src/wellsfargo/utils.py`

 * *Files identical despite different names*

