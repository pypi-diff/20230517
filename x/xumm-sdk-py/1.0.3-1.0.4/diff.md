# Comparing `tmp/xumm-sdk-py-1.0.3.tar.gz` & `tmp/xumm-sdk-py-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xumm-sdk-py-1.0.3.tar", last modified: Tue Jan 24 11:11:12 2023, max compression
+gzip compressed data, was "xumm-sdk-py-1.0.4.tar", last modified: Wed May 17 12:29:24 2023, max compression
```

## Comparing `xumm-sdk-py-1.0.3.tar` & `xumm-sdk-py-1.0.4.tar`

### file list

```diff
@@ -1,66 +1,75 @@
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-01-24 11:11:12.283578 xumm-sdk-py-1.0.3/
--rw-r--r--   0 av         (501) staff       (20)     1078 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/LICENSE
--rw-r--r--   0 av         (501) staff       (20)    18927 2023-01-24 11:11:12.283378 xumm-sdk-py-1.0.3/PKG-INFO
--rw-r--r--   0 av         (501) staff       (20)    18215 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/README.md
--rw-r--r--   0 av         (501) staff       (20)      102 2022-02-01 11:04:09.000000 xumm-sdk-py-1.0.3/pyproject.toml
--rw-r--r--   0 av         (501) staff       (20)       38 2023-01-24 11:11:12.283615 xumm-sdk-py-1.0.3/setup.cfg
--rw-r--r--   0 av         (501) staff       (20)     1558 2023-01-24 11:07:50.000000 xumm-sdk-py-1.0.3/setup.py
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-01-24 11:11:12.277679 xumm-sdk-py-1.0.3/xumm/
--rw-r--r--   0 av         (501) staff       (20)      322 2022-02-01 11:04:09.000000 xumm-sdk-py-1.0.3/xumm/__init__.py
--rw-r--r--   0 av         (501) staff       (20)     6337 2022-02-08 13:20:57.000000 xumm-sdk-py-1.0.3/xumm/client.py
--rw-r--r--   0 av         (501) staff       (20)     1331 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/error.py
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-01-24 11:11:12.279143 xumm-sdk-py-1.0.3/xumm/resource/
--rw-r--r--   0 av         (501) staff       (20)     5033 2022-02-01 11:04:09.000000 xumm-sdk-py-1.0.3/xumm/resource/__init__.py
--rw-r--r--   0 av         (501) staff       (20)     4986 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/xumm/resource/base.py
--rw-r--r--   0 av         (501) staff       (20)      419 2022-02-08 10:42:27.000000 xumm-sdk-py-1.0.3/xumm/resource/curated_assets.py
--rw-r--r--   0 av         (501) staff       (20)      757 2022-02-08 10:48:00.000000 xumm-sdk-py-1.0.3/xumm/resource/kyc_status.py
--rw-r--r--   0 av         (501) staff       (20)     8737 2022-02-07 12:47:32.000000 xumm-sdk-py-1.0.3/xumm/resource/payload.py
--rw-r--r--   0 av         (501) staff       (20)      424 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/ping.py
--rw-r--r--   0 av         (501) staff       (20)     1549 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/xumm/resource/push.py
--rw-r--r--   0 av         (501) staff       (20)      522 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/rates.py
--rw-r--r--   0 av         (501) staff       (20)     2120 2022-02-08 10:13:01.000000 xumm-sdk-py-1.0.3/xumm/resource/storage.py
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-01-24 11:11:12.279422 xumm-sdk-py-1.0.3/xumm/resource/types/
--rw-r--r--   0 av         (501) staff       (20)     1869 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/xumm/resource/types/__init__.py
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-01-24 11:11:12.280487 xumm-sdk-py-1.0.3/xumm/resource/types/meta/
--rw-r--r--   0 av         (501) staff       (20)        0 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/types/meta/__init__.py
--rw-r--r--   0 av         (501) staff       (20)     9861 2022-02-01 11:04:09.000000 xumm-sdk-py-1.0.3/xumm/resource/types/meta/application_details.py
--rw-r--r--   0 av         (501) staff       (20)    13176 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/types/meta/curated_assets_response.py
--rw-r--r--   0 av         (501) staff       (20)     2309 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/types/meta/kyc_info_response.py
--rw-r--r--   0 av         (501) staff       (20)     3562 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/types/meta/kyc_status_response.py
--rw-r--r--   0 av         (501) staff       (20)     2167 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/types/meta/pong.py
--rw-r--r--   0 av         (501) staff       (20)     7598 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/types/meta/rates_response.py
--rw-r--r--   0 av         (501) staff       (20)     5574 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/xumm/resource/types/meta/user_tokens.py
--rw-r--r--   0 av         (501) staff       (20)     6511 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/types/meta/xrpl_transaction.py
--rw-r--r--   0 av         (501) staff       (20)    42110 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/xumm/resource/types/misc.py
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-01-24 11:11:12.281044 xumm-sdk-py-1.0.3/xumm/resource/types/payload/
--rw-r--r--   0 av         (501) staff       (20)        0 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/types/payload/__init__.py
--rw-r--r--   0 av         (501) staff       (20)      297 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/types/payload/on_payload_event.py
--rw-r--r--   0 av         (501) staff       (20)     5031 2022-02-08 13:12:29.000000 xumm-sdk-py-1.0.3/xumm/resource/types/payload/payload_and_subscription.py
--rw-r--r--   0 av         (501) staff       (20)     4086 2022-02-08 13:12:14.000000 xumm-sdk-py-1.0.3/xumm/resource/types/payload/payload_subscription.py
--rw-r--r--   0 av         (501) staff       (20)     3853 2022-02-07 14:10:19.000000 xumm-sdk-py-1.0.3/xumm/resource/types/payload/subscription_callback_params.py
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-01-24 11:11:12.281595 xumm-sdk-py-1.0.3/xumm/resource/types/push/
--rw-r--r--   0 av         (501) staff       (20)        0 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/xumm/resource/types/push/__init__.py
--rw-r--r--   0 av         (501) staff       (20)     1909 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/xumm/resource/types/push/push_event_response.py
--rw-r--r--   0 av         (501) staff       (20)     1346 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/xumm/resource/types/push/push_push_response.py
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-01-24 11:11:12.282262 xumm-sdk-py-1.0.3/xumm/resource/types/storage/
--rw-r--r--   0 av         (501) staff       (20)        0 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/types/storage/__init__.py
--rw-r--r--   0 av         (501) staff       (20)     3282 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/types/storage/storage_delete_response.py
--rw-r--r--   0 av         (501) staff       (20)     2343 2022-02-08 10:17:56.000000 xumm-sdk-py-1.0.3/xumm/resource/types/storage/storage_get_response.py
--rw-r--r--   0 av         (501) staff       (20)     2107 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/types/storage/storage_response.py
--rw-r--r--   0 av         (501) staff       (20)     3185 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/resource/types/storage/storage_set_response.py
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-01-24 11:11:12.282452 xumm-sdk-py-1.0.3/xumm/resource/types/xapp/
--rw-r--r--   0 av         (501) staff       (20)        0 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/xumm/resource/types/xapp/__init__.py
--rw-r--r--   0 av         (501) staff       (20)    16899 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/xumm/resource/types/xapp/xapp_ott_response.py
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-01-24 11:11:12.282576 xumm-sdk-py-1.0.3/xumm/resource/types/xumm_api/
--rw-r--r--   0 av         (501) staff       (20)    60063 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/xumm/resource/types/xumm_api/__init__.py
--rw-r--r--   0 av         (501) staff       (20)      472 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/xumm/resource/user_tokens.py
--rw-r--r--   0 av         (501) staff       (20)      927 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.3/xumm/resource/xapp.py
--rw-r--r--   0 av         (501) staff       (20)      500 2022-02-08 11:02:49.000000 xumm-sdk-py-1.0.3/xumm/resource/xrpl_tx.py
--rw-r--r--   0 av         (501) staff       (20)      471 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.3/xumm/util.py
--rw-r--r--   0 av         (501) staff       (20)    10141 2022-02-01 11:04:09.000000 xumm-sdk-py-1.0.3/xumm/ws_client.py
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-01-24 11:11:12.283185 xumm-sdk-py-1.0.3/xumm_sdk_py.egg-info/
--rw-r--r--   0 av         (501) staff       (20)    18927 2023-01-24 11:11:12.000000 xumm-sdk-py-1.0.3/xumm_sdk_py.egg-info/PKG-INFO
--rw-r--r--   0 av         (501) staff       (20)     1804 2023-01-24 11:11:12.000000 xumm-sdk-py-1.0.3/xumm_sdk_py.egg-info/SOURCES.txt
--rw-r--r--   0 av         (501) staff       (20)        1 2023-01-24 11:11:12.000000 xumm-sdk-py-1.0.3/xumm_sdk_py.egg-info/dependency_links.txt
--rw-r--r--   0 av         (501) staff       (20)      156 2023-01-24 11:11:12.000000 xumm-sdk-py-1.0.3/xumm_sdk_py.egg-info/requires.txt
--rw-r--r--   0 av         (501) staff       (20)        5 2023-01-24 11:11:12.000000 xumm-sdk-py-1.0.3/xumm_sdk_py.egg-info/top_level.txt
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-05-17 12:29:24.367264 xumm-sdk-py-1.0.4/
+-rw-r--r--   0 av         (501) staff       (20)     1078 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/LICENSE
+-rw-r--r--   0 av         (501) staff       (20)    18927 2023-05-17 12:29:24.367081 xumm-sdk-py-1.0.4/PKG-INFO
+-rw-r--r--   0 av         (501) staff       (20)    18215 2023-05-17 12:23:44.000000 xumm-sdk-py-1.0.4/README.md
+-rw-r--r--   0 av         (501) staff       (20)      102 2022-02-01 11:04:09.000000 xumm-sdk-py-1.0.4/pyproject.toml
+-rw-r--r--   0 av         (501) staff       (20)       38 2023-05-17 12:29:24.367308 xumm-sdk-py-1.0.4/setup.cfg
+-rw-r--r--   0 av         (501) staff       (20)     1594 2023-05-17 12:27:40.000000 xumm-sdk-py-1.0.4/setup.py
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-05-17 12:29:24.360991 xumm-sdk-py-1.0.4/tests/
+-rw-r--r--   0 av         (501) staff       (20)     1557 2022-02-08 12:33:19.000000 xumm-sdk-py-1.0.4/tests/test_app_storage.py
+-rw-r--r--   0 av         (501) staff       (20)     6391 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.4/tests/test_common.py
+-rw-r--r--   0 av         (501) staff       (20)     3063 2022-02-08 12:35:05.000000 xumm-sdk-py-1.0.4/tests/test_payload_cancel.py
+-rw-r--r--   0 av         (501) staff       (20)     1968 2022-02-08 12:39:02.000000 xumm-sdk-py-1.0.4/tests/test_payload_create.py
+-rw-r--r--   0 av         (501) staff       (20)     2203 2022-02-08 12:39:45.000000 xumm-sdk-py-1.0.4/tests/test_payload_get.py
+-rw-r--r--   0 av         (501) staff       (20)    10352 2022-02-08 12:42:03.000000 xumm-sdk-py-1.0.4/tests/test_payload_subscribe.py
+-rw-r--r--   0 av         (501) staff       (20)     1477 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.4/tests/test_push.py
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-05-17 12:29:24.361560 xumm-sdk-py-1.0.4/xumm/
+-rw-r--r--   0 av         (501) staff       (20)      362 2023-05-17 12:23:44.000000 xumm-sdk-py-1.0.4/xumm/__init__.py
+-rw-r--r--   0 av         (501) staff       (20)     6499 2023-05-17 12:23:44.000000 xumm-sdk-py-1.0.4/xumm/client.py
+-rw-r--r--   0 av         (501) staff       (20)     1331 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/error.py
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-05-17 12:29:24.362890 xumm-sdk-py-1.0.4/xumm/resource/
+-rw-r--r--   0 av         (501) staff       (20)     5145 2023-05-17 12:23:44.000000 xumm-sdk-py-1.0.4/xumm/resource/__init__.py
+-rw-r--r--   0 av         (501) staff       (20)     4994 2023-05-17 12:23:44.000000 xumm-sdk-py-1.0.4/xumm/resource/base.py
+-rw-r--r--   0 av         (501) staff       (20)      419 2022-02-08 10:42:27.000000 xumm-sdk-py-1.0.4/xumm/resource/curated_assets.py
+-rw-r--r--   0 av         (501) staff       (20)      757 2022-02-08 10:48:00.000000 xumm-sdk-py-1.0.4/xumm/resource/kyc_status.py
+-rw-r--r--   0 av         (501) staff       (20)     2451 2023-05-17 12:23:44.000000 xumm-sdk-py-1.0.4/xumm/resource/oauth2.py
+-rw-r--r--   0 av         (501) staff       (20)     8737 2022-02-07 12:47:32.000000 xumm-sdk-py-1.0.4/xumm/resource/payload.py
+-rw-r--r--   0 av         (501) staff       (20)      424 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/ping.py
+-rw-r--r--   0 av         (501) staff       (20)     1549 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.4/xumm/resource/push.py
+-rw-r--r--   0 av         (501) staff       (20)      522 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/rates.py
+-rw-r--r--   0 av         (501) staff       (20)     2120 2022-02-08 10:13:01.000000 xumm-sdk-py-1.0.4/xumm/resource/storage.py
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-05-17 12:29:24.363117 xumm-sdk-py-1.0.4/xumm/resource/types/
+-rw-r--r--   0 av         (501) staff       (20)     1967 2023-05-17 12:23:44.000000 xumm-sdk-py-1.0.4/xumm/resource/types/__init__.py
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-05-17 12:29:24.364118 xumm-sdk-py-1.0.4/xumm/resource/types/meta/
+-rw-r--r--   0 av         (501) staff       (20)        0 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/types/meta/__init__.py
+-rw-r--r--   0 av         (501) staff       (20)     9861 2022-02-01 11:04:09.000000 xumm-sdk-py-1.0.4/xumm/resource/types/meta/application_details.py
+-rw-r--r--   0 av         (501) staff       (20)    13176 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/types/meta/curated_assets_response.py
+-rw-r--r--   0 av         (501) staff       (20)     2309 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/types/meta/kyc_info_response.py
+-rw-r--r--   0 av         (501) staff       (20)     3562 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/types/meta/kyc_status_response.py
+-rw-r--r--   0 av         (501) staff       (20)     2167 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/types/meta/pong.py
+-rw-r--r--   0 av         (501) staff       (20)     7598 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/types/meta/rates_response.py
+-rw-r--r--   0 av         (501) staff       (20)     5574 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.4/xumm/resource/types/meta/user_tokens.py
+-rw-r--r--   0 av         (501) staff       (20)     6511 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/types/meta/xrpl_transaction.py
+-rw-r--r--   0 av         (501) staff       (20)    42110 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.4/xumm/resource/types/misc.py
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-05-17 12:29:24.364633 xumm-sdk-py-1.0.4/xumm/resource/types/oauth2/
+-rw-r--r--   0 av         (501) staff       (20)        0 2023-05-17 12:23:44.000000 xumm-sdk-py-1.0.4/xumm/resource/types/oauth2/__init__.py
+-rw-r--r--   0 av         (501) staff       (20)     4808 2023-05-17 12:23:44.000000 xumm-sdk-py-1.0.4/xumm/resource/types/oauth2/oauth2_token_response.py
+-rw-r--r--   0 av         (501) staff       (20)     9318 2023-05-17 12:23:44.000000 xumm-sdk-py-1.0.4/xumm/resource/types/oauth2/oauth2_user_info_response.py
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-05-17 12:29:24.365244 xumm-sdk-py-1.0.4/xumm/resource/types/payload/
+-rw-r--r--   0 av         (501) staff       (20)        0 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/types/payload/__init__.py
+-rw-r--r--   0 av         (501) staff       (20)      297 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/types/payload/on_payload_event.py
+-rw-r--r--   0 av         (501) staff       (20)     5031 2022-02-08 13:12:29.000000 xumm-sdk-py-1.0.4/xumm/resource/types/payload/payload_and_subscription.py
+-rw-r--r--   0 av         (501) staff       (20)     4086 2022-02-08 13:12:14.000000 xumm-sdk-py-1.0.4/xumm/resource/types/payload/payload_subscription.py
+-rw-r--r--   0 av         (501) staff       (20)     3853 2022-02-07 14:10:19.000000 xumm-sdk-py-1.0.4/xumm/resource/types/payload/subscription_callback_params.py
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-05-17 12:29:24.365587 xumm-sdk-py-1.0.4/xumm/resource/types/push/
+-rw-r--r--   0 av         (501) staff       (20)        0 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.4/xumm/resource/types/push/__init__.py
+-rw-r--r--   0 av         (501) staff       (20)     1909 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.4/xumm/resource/types/push/push_event_response.py
+-rw-r--r--   0 av         (501) staff       (20)     1346 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.4/xumm/resource/types/push/push_push_response.py
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-05-17 12:29:24.366141 xumm-sdk-py-1.0.4/xumm/resource/types/storage/
+-rw-r--r--   0 av         (501) staff       (20)        0 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/types/storage/__init__.py
+-rw-r--r--   0 av         (501) staff       (20)     3282 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/types/storage/storage_delete_response.py
+-rw-r--r--   0 av         (501) staff       (20)     2343 2022-02-08 10:17:56.000000 xumm-sdk-py-1.0.4/xumm/resource/types/storage/storage_get_response.py
+-rw-r--r--   0 av         (501) staff       (20)     2107 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/types/storage/storage_response.py
+-rw-r--r--   0 av         (501) staff       (20)     3185 2022-02-01 10:08:55.000000 xumm-sdk-py-1.0.4/xumm/resource/types/storage/storage_set_response.py
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-05-17 12:29:24.366247 xumm-sdk-py-1.0.4/xumm/resource/types/xumm_api/
+-rw-r--r--   0 av         (501) staff       (20)    60063 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.4/xumm/resource/types/xumm_api/__init__.py
+-rw-r--r--   0 av         (501) staff       (20)      472 2023-01-18 17:02:16.000000 xumm-sdk-py-1.0.4/xumm/resource/user_tokens.py
+-rw-r--r--   0 av         (501) staff       (20)      500 2022-02-08 11:02:49.000000 xumm-sdk-py-1.0.4/xumm/resource/xrpl_tx.py
+-rw-r--r--   0 av         (501) staff       (20)     1029 2023-05-17 12:23:44.000000 xumm-sdk-py-1.0.4/xumm/util.py
+-rw-r--r--   0 av         (501) staff       (20)    10141 2022-02-01 11:04:09.000000 xumm-sdk-py-1.0.4/xumm/ws_client.py
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-05-17 12:29:24.366867 xumm-sdk-py-1.0.4/xumm_sdk_py.egg-info/
+-rw-r--r--   0 av         (501) staff       (20)    18927 2023-05-17 12:29:24.000000 xumm-sdk-py-1.0.4/xumm_sdk_py.egg-info/PKG-INFO
+-rw-r--r--   0 av         (501) staff       (20)     2052 2023-05-17 12:29:24.000000 xumm-sdk-py-1.0.4/xumm_sdk_py.egg-info/SOURCES.txt
+-rw-r--r--   0 av         (501) staff       (20)        1 2023-05-17 12:29:24.000000 xumm-sdk-py-1.0.4/xumm_sdk_py.egg-info/dependency_links.txt
+-rw-r--r--   0 av         (501) staff       (20)      181 2023-05-17 12:29:24.000000 xumm-sdk-py-1.0.4/xumm_sdk_py.egg-info/requires.txt
+-rw-r--r--   0 av         (501) staff       (20)        5 2023-05-17 12:29:24.000000 xumm-sdk-py-1.0.4/xumm_sdk_py.egg-info/top_level.txt
```

### Comparing `xumm-sdk-py-1.0.3/LICENSE` & `xumm-sdk-py-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/PKG-INFO` & `xumm-sdk-py-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xumm-sdk-py
-Version: 1.0.3
+Version: 1.0.4
 Summary: Xumm SDK for Python
 Home-page: https://github.com/XRPL-Labs/xumm-sdk-py
 Author: XRPL-Labs
 Author-email: support@xrpl-labs.com
 License: MIT
 Keywords: xrp,ledger,ripple,xumm,sdk
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 
 # XUMM SDK (Python) [![python version](https://badge.fury.io/py/xumm-sdk-py.svg)](https://pypi.org/project/xumm-sdk-py/) [![GitHub Actions Python status](https://github.com/XRPL-Labs/xumm-sdk-py/workflows/Python/badge.svg?branch=main)](https://github.com/XRPL-Labs/xumm-sdk-py/actions)
 
 Interact with the XUMM SDK from Python environments.
 
 #### **⚠️ Please note: The XUMM SDK (XUMM API in general) is for BACKEND USE only. Please DO NOT use your API credentials in a FRONTEND environment.**
 
-> To implement the XUMM SKD (or XUMM API directly) in your own web project, make sure your frontend calls your own backend, where the follow up communication with the XUMM SDK (or XUMM API) will take place. Your XUMM credentials should never be publicly available.
+> To implement the XUMM SDK (or XUMM API directly) in your own web project, make sure your frontend calls your own backend, where the follow up communication with the XUMM SDK (or XUMM API) will take place. Your XUMM credentials should never be publicly available.
 
 - [Getting Started](#getting-started)
 - [Usage](#usage)
   - [Payloads](#payloads)
   - [App Storage](#app-storage)
   - [Helper Methods](#helper-methods)
 - [Development](#development)
```

### Comparing `xumm-sdk-py-1.0.3/README.md` & `xumm-sdk-py-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # XUMM SDK (Python) [![python version](https://badge.fury.io/py/xumm-sdk-py.svg)](https://pypi.org/project/xumm-sdk-py/) [![GitHub Actions Python status](https://github.com/XRPL-Labs/xumm-sdk-py/workflows/Python/badge.svg?branch=main)](https://github.com/XRPL-Labs/xumm-sdk-py/actions)
 
 Interact with the XUMM SDK from Python environments.
 
 #### **⚠️ Please note: The XUMM SDK (XUMM API in general) is for BACKEND USE only. Please DO NOT use your API credentials in a FRONTEND environment.**
 
-> To implement the XUMM SKD (or XUMM API directly) in your own web project, make sure your frontend calls your own backend, where the follow up communication with the XUMM SDK (or XUMM API) will take place. Your XUMM credentials should never be publicly available.
+> To implement the XUMM SDK (or XUMM API directly) in your own web project, make sure your frontend calls your own backend, where the follow up communication with the XUMM SDK (or XUMM API) will take place. Your XUMM credentials should never be publicly available.
 
 - [Getting Started](#getting-started)
 - [Usage](#usage)
   - [Payloads](#payloads)
   - [App Storage](#app-storage)
   - [Helper Methods](#helper-methods)
 - [Development](#development)
```

### Comparing `xumm-sdk-py-1.0.3/setup.py` & `xumm-sdk-py-1.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 import os
 from setuptools import setup, find_packages
 from codecs import open
 
 NAME = "xumm-sdk-py"
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 
 # Get the long description from the README.md file
 base_dir = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(base_dir, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
@@ -21,14 +21,15 @@
     author='XRPL-Labs',
     author_email='support@xrpl-labs.com',
     url='https://github.com/XRPL-Labs/xumm-sdk-py',
     packages=find_packages(include=('xumm*',)),
     include_package_data=True,
     install_requires=[
         "requests>=2.26.0,<=2.28.2",
+        "requests-oauthlib>=1.3.1",
         "websocket-client>=1.2.3,<=1.4.2",
         "six==1.16.0",
         "python-dotenv>=0.19.2,<=0.21.1"
     ],
     extras_require={
         'develop': [
             'pytest==6.2.5',
```

### Comparing `xumm-sdk-py-1.0.3/xumm/client.py` & `xumm-sdk-py-1.0.4/xumm/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,25 +70,29 @@
         'content-type': 'application/json',
         'accept': 'application/json',
         'user-agent': "xumm-sdk/python ({}) requests".format(gethostname(),)
     }
 
 
 def get(
-    url: str
+    url: str,
+    access_token: str = None
 ) -> Dict[str, object]:
     """
     Returns the sdk GET response
 
     :param url: A string url endpoint.
     :type: str
     :return: Dict[str, object]
     """
     try:
-        res = requests.get(url, headers=get_headers())
+        headers = get_headers()
+        if isinstance(access_token, str):
+            headers['Authorization'] = f'Bearer {access_token}'
+        res = requests.get(url, headers=headers)
     except Exception as e:
         handle_request_error(e)
     return handle_response(res)
 
 
 def post(
     url: str,
```

### Comparing `xumm-sdk-py-1.0.3/xumm/error.py` & `xumm-sdk-py-1.0.4/xumm/error.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/__init__.py` & `xumm-sdk-py-1.0.4/xumm/resource/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from __future__ import unicode_literals
 
 from typing import Dict
 import pprint
 import six
 
 from xumm import client
+from xumm import oauth2_base
 
 # import logging
 # logging.basicConfig(level=logging.ERROR)
 
 
 class BaseResource(object):
 
@@ -159,12 +160,16 @@
 
 class XummResource(BaseResource):
 
     @classmethod
     def platform_url(cls) -> str:
         return client.build_url() + 'platform' + '/'
 
+    @classmethod
+    def oauth2_url(cls) -> str:
+        return oauth2_base + '/'
+
     def __init__(cls, *args, **kwargs) -> 'XummResource':
         cls.refresh_from(**kwargs)
 
     def refresh_from(cls, **kwargs):
         raise NotImplementedError
```

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/base.py` & `xumm-sdk-py-1.0.4/xumm/resource/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 from xumm.resource.kyc_status import KycStatusResource
 from xumm.resource.curated_assets import CuratedAssetsResource
 from xumm.resource.xrpl_tx import XrplTxResource
 from xumm.resource.rates import RatesResource
 from xumm.resource.payload import PayloadResource
 from xumm.resource.storage import StorageResource
 from xumm.resource.user_tokens import UserTokensResource
-from xumm.resource.xapp import XappResource
 from xumm.resource.push import PushResource
+from xumm.resource.oauth2 import OAuth2Resource
 
 
 class XummSdk(XummResource):
 
     def __init__(cls, *args) -> 'XummSdk':
 
         if len(args) == 2 and isinstance(args[0], str):
@@ -60,16 +60,16 @@
             raise error.AuthenticationError(
                 'Invalid API secret provided. (HINT: XXXXXXXX-XXXX-'
                 'XXXX-XXXX-XXXXXXXXXXXX).'
             )
 
         cls.payload = PayloadResource()
         cls.storage = StorageResource()
-        cls.xapp = XappResource()
         cls.push = PushResource()
+        cls.oauth2 = OAuth2Resource()
 
     def refresh_from(cls, **kwargs):
         return super().refresh_from(**kwargs)
 
     def ping(cls) -> PongResponse:
         """Returns the dict as a model
```

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/kyc_status.py` & `xumm-sdk-py-1.0.4/xumm/resource/kyc_status.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/payload.py` & `xumm-sdk-py-1.0.4/xumm/resource/payload.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/push.py` & `xumm-sdk-py-1.0.4/xumm/resource/push.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/rates.py` & `xumm-sdk-py-1.0.4/xumm/resource/rates.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/storage.py` & `xumm-sdk-py-1.0.4/xumm/resource/storage.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/__init__.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 from .payload.subscription_callback_params import SubscriptionCallbackParams  # noqa: F401 E501
 
 from .storage.storage_delete_response import StorageDeleteResponse  # noqa: F401 E501
 from .storage.storage_get_response import StorageGetResponse  # noqa: F401
 from .storage.storage_response import StorageResponse  # noqa: F401
 from .storage.storage_set_response import StorageSetResponse  # noqa: F401
 
-from .xapp.xapp_ott_response import XappOttResponse  # noqa: F401
-
 from .push.push_event_response import PushEventResponse  # noqa: F401
 from .push.push_push_response import PushPushResponse  # noqa: F401
 
 from .meta.user_tokens import (  # noqa: F401
     UserTokenValidity,
     UserTokenResponse,
 )
@@ -42,7 +40,10 @@
 from .xumm_api import (  # noqa: F401
     XummPostPayloadResponse as CreatedPayload,
     XummDeletePayloadResponse as DeletedPayload,
     XummGetPayloadResponse as XummPayload,
     XummWebhookBody,
     XummPushEventRequest,
 )
+
+from .oauth2.oauth2_token_response import OAuth2TokenResponse  # noqa: F401
+from .oauth2.oauth2_user_info_response import OAuth2UserInfoResponse  # noqa: F401 E501
```

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/meta/application_details.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/meta/application_details.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/meta/curated_assets_response.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/meta/curated_assets_response.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/meta/kyc_info_response.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/meta/kyc_info_response.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/meta/kyc_status_response.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/meta/kyc_status_response.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/meta/pong.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/meta/pong.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/meta/rates_response.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/meta/rates_response.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/meta/user_tokens.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/meta/user_tokens.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/meta/xrpl_transaction.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/meta/xrpl_transaction.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/misc.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/misc.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/payload/payload_and_subscription.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/payload/payload_and_subscription.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/payload/payload_subscription.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/payload/payload_subscription.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/payload/subscription_callback_params.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/payload/subscription_callback_params.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/push/push_event_response.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/push/push_event_response.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/push/push_push_response.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/push/push_push_response.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/storage/storage_delete_response.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/storage/storage_delete_response.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/storage/storage_get_response.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/storage/storage_get_response.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/storage/storage_response.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/storage/storage_response.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/storage/storage_set_response.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/storage/storage_set_response.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/resource/types/xumm_api/__init__.py` & `xumm-sdk-py-1.0.4/xumm/resource/types/xumm_api/__init__.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm/ws_client.py` & `xumm-sdk-py-1.0.4/xumm/ws_client.py`

 * *Files identical despite different names*

### Comparing `xumm-sdk-py-1.0.3/xumm_sdk_py.egg-info/PKG-INFO` & `xumm-sdk-py-1.0.4/xumm_sdk_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xumm-sdk-py
-Version: 1.0.3
+Version: 1.0.4
 Summary: Xumm SDK for Python
 Home-page: https://github.com/XRPL-Labs/xumm-sdk-py
 Author: XRPL-Labs
 Author-email: support@xrpl-labs.com
 License: MIT
 Keywords: xrp,ledger,ripple,xumm,sdk
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 
 # XUMM SDK (Python) [![python version](https://badge.fury.io/py/xumm-sdk-py.svg)](https://pypi.org/project/xumm-sdk-py/) [![GitHub Actions Python status](https://github.com/XRPL-Labs/xumm-sdk-py/workflows/Python/badge.svg?branch=main)](https://github.com/XRPL-Labs/xumm-sdk-py/actions)
 
 Interact with the XUMM SDK from Python environments.
 
 #### **⚠️ Please note: The XUMM SDK (XUMM API in general) is for BACKEND USE only. Please DO NOT use your API credentials in a FRONTEND environment.**
 
-> To implement the XUMM SKD (or XUMM API directly) in your own web project, make sure your frontend calls your own backend, where the follow up communication with the XUMM SDK (or XUMM API) will take place. Your XUMM credentials should never be publicly available.
+> To implement the XUMM SDK (or XUMM API directly) in your own web project, make sure your frontend calls your own backend, where the follow up communication with the XUMM SDK (or XUMM API) will take place. Your XUMM credentials should never be publicly available.
 
 - [Getting Started](#getting-started)
 - [Usage](#usage)
   - [Payloads](#payloads)
   - [App Storage](#app-storage)
   - [Helper Methods](#helper-methods)
 - [Development](#development)
```

### Comparing `xumm-sdk-py-1.0.3/xumm_sdk_py.egg-info/SOURCES.txt` & `xumm-sdk-py-1.0.4/xumm_sdk_py.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+tests/test_app_storage.py
+tests/test_common.py
+tests/test_payload_cancel.py
+tests/test_payload_create.py
+tests/test_payload_get.py
+tests/test_payload_subscribe.py
+tests/test_push.py
 xumm/__init__.py
 xumm/client.py
 xumm/error.py
 xumm/util.py
 xumm/ws_client.py
 xumm/resource/__init__.py
 xumm/resource/base.py
 xumm/resource/curated_assets.py
 xumm/resource/kyc_status.py
+xumm/resource/oauth2.py
 xumm/resource/payload.py
 xumm/resource/ping.py
 xumm/resource/push.py
 xumm/resource/rates.py
 xumm/resource/storage.py
 xumm/resource/user_tokens.py
-xumm/resource/xapp.py
 xumm/resource/xrpl_tx.py
 xumm/resource/types/__init__.py
 xumm/resource/types/misc.py
 xumm/resource/types/meta/__init__.py
 xumm/resource/types/meta/application_details.py
 xumm/resource/types/meta/curated_assets_response.py
 xumm/resource/types/meta/kyc_info_response.py
 xumm/resource/types/meta/kyc_status_response.py
 xumm/resource/types/meta/pong.py
 xumm/resource/types/meta/rates_response.py
 xumm/resource/types/meta/user_tokens.py
 xumm/resource/types/meta/xrpl_transaction.py
+xumm/resource/types/oauth2/__init__.py
+xumm/resource/types/oauth2/oauth2_token_response.py
+xumm/resource/types/oauth2/oauth2_user_info_response.py
 xumm/resource/types/payload/__init__.py
 xumm/resource/types/payload/on_payload_event.py
 xumm/resource/types/payload/payload_and_subscription.py
 xumm/resource/types/payload/payload_subscription.py
 xumm/resource/types/payload/subscription_callback_params.py
 xumm/resource/types/push/__init__.py
 xumm/resource/types/push/push_event_response.py
 xumm/resource/types/push/push_push_response.py
 xumm/resource/types/storage/__init__.py
 xumm/resource/types/storage/storage_delete_response.py
 xumm/resource/types/storage/storage_get_response.py
 xumm/resource/types/storage/storage_response.py
 xumm/resource/types/storage/storage_set_response.py
-xumm/resource/types/xapp/__init__.py
-xumm/resource/types/xapp/xapp_ott_response.py
 xumm/resource/types/xumm_api/__init__.py
 xumm_sdk_py.egg-info/PKG-INFO
 xumm_sdk_py.egg-info/SOURCES.txt
 xumm_sdk_py.egg-info/dependency_links.txt
 xumm_sdk_py.egg-info/requires.txt
 xumm_sdk_py.egg-info/top_level.txt
```

