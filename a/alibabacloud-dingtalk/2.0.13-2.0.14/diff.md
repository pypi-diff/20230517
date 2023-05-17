# Comparing `tmp/alibabacloud_dingtalk-2.0.13.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.13.tar", last modified: Tue May 16 02:06:51 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.14.tar", last modified: Wed May 17 02:21:50 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.13.tar` & `alibabacloud_dingtalk-2.0.14.tar`

### file list

```diff
@@ -1,357 +1,357 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/
--rw-r--r--   0 root         (0) root         (0)    19492 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21260 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23341 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90648 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138912 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   158124 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   299469 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201848 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   569113 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138814 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   331545 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35138 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101075 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85810 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110530 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   293352 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   387566 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6576 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10253 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   220322 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   547684 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45840 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    65285 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211006 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267473 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269103 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   453174 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   705965 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   312544 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   433417 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5282 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4431 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4668 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92926 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137528 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302532 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   378971 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13884 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18281 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   523174 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   756557 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   131349 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   159547 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260568 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413706 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44880 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    81308 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   147980 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53454 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   118368 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27686 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    29689 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   175082 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   370377 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11743 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/
+-rw-r--r--   0 root         (0) root         (0)    19557 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21260 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23341 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90648 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138912 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   158124 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   299469 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201848 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   569113 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138814 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   331545 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35138 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101075 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85810 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110530 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   293352 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   387566 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6576 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10253 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   220322 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   547684 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45840 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    65285 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   211006 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   267473 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269103 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   453174 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   705965 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   312544 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   433417 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5282 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92926 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137528 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302532 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   378971 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13884 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18281 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   523174 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   756557 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   131349 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   159547 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260568 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413706 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44880 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    81308 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32237 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53454 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   118368 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27686 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    29689 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   175082 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   370377 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11743 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.13/ChangeLog.md` & `alibabacloud_dingtalk-2.0.14/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-16 Version: 2.0.13
+- Update AddOfficialAccountFollower.
+
 2023-05-12 Version: 2.0.12
 - Update AddOfficialAccountFollower.
 
 2023-05-09 Version: 2.0.11
 - Update AddOfficialAccountFollower.
 
 2023-04-28 Version: 2.0.10
```

### Comparing `alibabacloud_dingtalk-2.0.13/LICENSE` & `alibabacloud_dingtalk-2.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/PKG-INFO` & `alibabacloud_dingtalk-2.0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.13
+Version: 2.0.14
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.13/README-CN.md` & `alibabacloud_dingtalk-2.0.14/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/README.md` & `alibabacloud_dingtalk-2.0.14/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2846,26 +2846,28 @@
         created_time: int = None,
         creator_id: str = None,
         detail_url: QueryOrgTodoByUserResponseBodyTodoCardsDetailUrl = None,
         due_time: int = None,
         is_done: bool = None,
         modified_time: int = None,
         priority: int = None,
+        source_ext: str = None,
         source_id: str = None,
         subject: str = None,
         task_id: str = None,
     ):
         self.biz_tag = biz_tag
         self.created_time = created_time
         self.creator_id = creator_id
         self.detail_url = detail_url
         self.due_time = due_time
         self.is_done = is_done
         self.modified_time = modified_time
         self.priority = priority
+        self.source_ext = source_ext
         self.source_id = source_id
         self.subject = subject
         self.task_id = task_id
 
     def validate(self):
         if self.detail_url:
             self.detail_url.validate()
@@ -2888,14 +2890,16 @@
             result['dueTime'] = self.due_time
         if self.is_done is not None:
             result['isDone'] = self.is_done
         if self.modified_time is not None:
             result['modifiedTime'] = self.modified_time
         if self.priority is not None:
             result['priority'] = self.priority
+        if self.source_ext is not None:
+            result['sourceExt'] = self.source_ext
         if self.source_id is not None:
             result['sourceId'] = self.source_id
         if self.subject is not None:
             result['subject'] = self.subject
         if self.task_id is not None:
             result['taskId'] = self.task_id
         return result
@@ -2915,14 +2919,16 @@
             self.due_time = m.get('dueTime')
         if m.get('isDone') is not None:
             self.is_done = m.get('isDone')
         if m.get('modifiedTime') is not None:
             self.modified_time = m.get('modifiedTime')
         if m.get('priority') is not None:
             self.priority = m.get('priority')
+        if m.get('sourceExt') is not None:
+            self.source_ext = m.get('sourceExt')
         if m.get('sourceId') is not None:
             self.source_id = m.get('sourceId')
         if m.get('subject') is not None:
             self.subject = m.get('subject')
         if m.get('taskId') is not None:
             self.task_id = m.get('taskId')
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.13
+Version: 2.0.14
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.13/setup.py` & `alibabacloud_dingtalk-2.0.14/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 16/05/2023
+Created on 17/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

