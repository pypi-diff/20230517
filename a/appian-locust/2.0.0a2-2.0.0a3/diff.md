# Comparing `tmp/appian-locust-2.0.0a2.tar.gz` & `tmp/appian-locust-2.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appian-locust-2.0.0a2.tar", last modified: Mon May 15 17:27:05 2023, max compression
+gzip compressed data, was "appian-locust-2.0.0a3.tar", last modified: Wed May 17 15:57:16 2023, max compression
```

## Comparing `appian-locust-2.0.0a2.tar` & `appian-locust-2.0.0a3.tar`

### file list

```diff
@@ -1,53 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 17:27:05.440197 appian-locust-2.0.0a2/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5403 2023-05-15 17:27:05.440197 appian-locust-2.0.0a2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4829 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 17:27:05.438197 appian-locust-2.0.0a2/appian_locust/
--rw-rw-rw-   0 root         (0) root         (0)      775 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9541 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2479 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_design.py
--rw-rw-rw-   0 root         (0) root         (0)     6206 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_feature_toggle_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7830 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_grid_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)    53252 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)     5171 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_locust_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7765 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_news.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_portals.py
--rw-rw-rw-   0 root         (0) root         (0)    16297 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_records.py
--rw-rw-rw-   0 root         (0) root         (0)     7380 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_records_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7185 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     3016 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_save_request_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    10948 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_sites.py
--rw-rw-rw-   0 root         (0) root         (0)     4514 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_task_opener.py
--rw-rw-rw-   0 root         (0) root         (0)     7644 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/_ui_reconciler.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/actions_info.py
--rw-rw-rw-   0 root         (0) root         (0)    14485 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/appianclient.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/application_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/design_object_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/design_object_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     4998 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/design_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/feature_flag.py
--rw-rw-rw-   0 root         (0) root         (0)    16278 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/helper.py
--rwxrwxrwx   0 root         (0) root         (0)     1431 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/loadDriverUtils.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     2749 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/news_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1941 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/record_list_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     1320 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/record_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/records_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1472 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/reports_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1364 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/site_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1408 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/tasks_info.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/tempo_navigator.py
--rw-rw-rw-   0 root         (0) root         (0)    73573 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/uiform.py
--rw-rw-rw-   0 root         (0) root         (0)    13955 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/appian_locust/visitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 17:27:05.439197 appian-locust-2.0.0a2/appian_locust.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5403 2023-05-15 17:27:05.000000 appian-locust-2.0.0a2/appian_locust.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1403 2023-05-15 17:27:05.000000 appian-locust-2.0.0a2/appian_locust.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 17:27:05.000000 appian-locust-2.0.0a2/appian_locust.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-15 17:27:05.000000 appian-locust-2.0.0a2/appian_locust.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-15 17:27:05.000000 appian-locust-2.0.0a2/appian_locust.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-15 17:27:05.440197 appian-locust-2.0.0a2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-05-15 17:26:54.000000 appian-locust-2.0.0a2/setup.py
+drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-17 15:57:16.951041 appian-locust-2.0.0a3/
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    11358 2022-02-17 16:44:14.000000 appian-locust-2.0.0a3/LICENSE
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     5403 2023-05-17 15:57:16.951230 appian-locust-2.0.0a3/PKG-INFO
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     4829 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/README.rst
+drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-17 15:57:16.919757 appian-locust-2.0.0a3/appian_locust/
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      775 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/__init__.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     9541 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_actions.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      786 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_admin.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2479 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_base.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     5721 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_design.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     6206 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_feature_toggle_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     7830 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_grid_interactor.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    53252 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_interactor.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     5171 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_locust_error_handler.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     7765 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_news.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1025 2023-05-15 14:44:16.000000 appian-locust-2.0.0a3/appian_locust/_portals.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    16297 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_records.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     7380 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_records_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     7185 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_reports.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     3016 2023-04-27 17:42:07.000000 appian-locust-2.0.0a3/appian_locust/_save_request_builder.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    10948 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_sites.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     4514 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_task_opener.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     7644 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/_tasks.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2365 2022-02-17 16:44:14.000000 appian-locust-2.0.0a3/appian_locust/_ui_reconciler.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1372 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/actions_info.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    14485 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/appianclient.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1981 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/application_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      205 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/design_object_type.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1068 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/design_object_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     4998 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/design_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      859 2022-02-17 16:44:14.000000 appian-locust-2.0.0a3/appian_locust/exceptions.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1792 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/feature_flag.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    16278 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/helper.py
+-rwxr-xr-x   0 harry.wilton   (502) staff       (20)     1431 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/loadDriverUtils.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      862 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/logger.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2749 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/news_info.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1941 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/record_list_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1320 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/record_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      547 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/records_info.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1546 2023-05-17 15:35:49.000000 appian-locust-2.0.0a3/appian_locust/reports_info.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1364 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/site_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1408 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/tasks_info.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2254 2023-05-17 15:37:08.000000 appian-locust-2.0.0a3/appian_locust/tempo_navigator.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    73573 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/appian_locust/uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    13955 2023-05-15 14:44:16.000000 appian-locust-2.0.0a3/appian_locust/visitor.py
+drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-17 15:57:16.923795 appian-locust-2.0.0a3/appian_locust.egg-info/
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     5403 2023-05-17 15:57:16.000000 appian-locust-2.0.0a3/appian_locust.egg-info/PKG-INFO
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2175 2023-05-17 15:57:16.000000 appian-locust-2.0.0a3/appian_locust.egg-info/SOURCES.txt
+-rw-r--r--   0 harry.wilton   (502) staff       (20)        1 2023-05-17 15:57:16.000000 appian-locust-2.0.0a3/appian_locust.egg-info/dependency_links.txt
+-rw-r--r--   0 harry.wilton   (502) staff       (20)       15 2023-05-17 15:57:16.000000 appian-locust-2.0.0a3/appian_locust.egg-info/requires.txt
+-rw-r--r--   0 harry.wilton   (502) staff       (20)       14 2023-05-17 15:57:16.000000 appian-locust-2.0.0a3/appian_locust.egg-info/top_level.txt
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      100 2023-02-28 19:42:15.000000 appian-locust-2.0.0a3/pyproject.toml
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      595 2023-05-17 15:57:16.951997 appian-locust-2.0.0a3/setup.cfg
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1088 2023-05-15 17:00:04.000000 appian-locust-2.0.0a3/setup.py
+drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-17 15:57:16.950113 appian-locust-2.0.0a3/tests/
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     6106 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_actions.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1053 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_admin.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     6785 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_app_importer.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    11018 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_appianclient.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1667 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_application_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2981 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_design.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1632 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_design_object_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2596 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_design_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    12722 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_feature_toggle_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     7834 2022-06-20 13:00:59.000000 appian-locust-2.0.0a3/tests/test_grid_interactor.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2936 2022-06-08 19:05:09.000000 appian-locust-2.0.0a3/tests/test_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    19580 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_interactor.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1458 2022-02-17 16:44:14.000000 appian-locust-2.0.0a3/tests/test_libraries_utils.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      891 2022-02-17 16:44:14.000000 appian-locust-2.0.0a3/tests/test_locust_error_handler.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     4727 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_news.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2391 2023-05-15 14:44:16.000000 appian-locust-2.0.0a3/tests/test_portals.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1844 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_record_list_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     4349 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_record_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    13429 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_records.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2334 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_records_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     5554 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_reports.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     3664 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_save_request_builder.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2257 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_site_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     6235 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_sites.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     4184 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_tasks.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2360 2022-02-17 16:44:14.000000 appian-locust-2.0.0a3/tests/test_ui_reconciler.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    61599 2023-05-11 19:17:00.000000 appian-locust-2.0.0a3/tests/test_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      784 2022-02-17 16:44:14.000000 appian-locust-2.0.0a3/tests/test_utils.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    22517 2023-05-15 14:44:16.000000 appian-locust-2.0.0a3/tests/test_visitor.py
```

### Comparing `appian-locust-2.0.0a2/LICENSE` & `appian-locust-2.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/PKG-INFO` & `appian-locust-2.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a2
+Version: 2.0.0a3
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.0.0a2/README.rst` & `appian-locust-2.0.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/__init__.py` & `appian-locust-2.0.0a3/appian_locust/__init__.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_actions.py` & `appian-locust-2.0.0a3/appian_locust/_actions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_admin.py` & `appian-locust-2.0.0a3/appian_locust/_admin.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_base.py` & `appian-locust-2.0.0a3/appian_locust/_base.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_design.py` & `appian-locust-2.0.0a3/appian_locust/_design.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_feature_toggle_helper.py` & `appian-locust-2.0.0a3/appian_locust/_feature_toggle_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_grid_interactor.py` & `appian-locust-2.0.0a3/appian_locust/_grid_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_interactor.py` & `appian-locust-2.0.0a3/appian_locust/_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_locust_error_handler.py` & `appian-locust-2.0.0a3/appian_locust/_locust_error_handler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_news.py` & `appian-locust-2.0.0a3/appian_locust/_news.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_portals.py` & `appian-locust-2.0.0a3/appian_locust/_portals.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_records.py` & `appian-locust-2.0.0a3/appian_locust/_records.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_records_helper.py` & `appian-locust-2.0.0a3/appian_locust/_records_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_reports.py` & `appian-locust-2.0.0a3/appian_locust/_reports.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_save_request_builder.py` & `appian-locust-2.0.0a3/appian_locust/_save_request_builder.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_sites.py` & `appian-locust-2.0.0a3/appian_locust/_sites.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_task_opener.py` & `appian-locust-2.0.0a3/appian_locust/_task_opener.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_tasks.py` & `appian-locust-2.0.0a3/appian_locust/_tasks.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/_ui_reconciler.py` & `appian-locust-2.0.0a3/appian_locust/_ui_reconciler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/actions_info.py` & `appian-locust-2.0.0a3/appian_locust/actions_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/appianclient.py` & `appian-locust-2.0.0a3/appian_locust/appianclient.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/application_uiform.py` & `appian-locust-2.0.0a3/appian_locust/application_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/design_object_uiform.py` & `appian-locust-2.0.0a3/appian_locust/design_object_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/design_uiform.py` & `appian-locust-2.0.0a3/appian_locust/design_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/exceptions.py` & `appian-locust-2.0.0a3/appian_locust/exceptions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/feature_flag.py` & `appian-locust-2.0.0a3/appian_locust/feature_flag.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/helper.py` & `appian-locust-2.0.0a3/appian_locust/helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/loadDriverUtils.py` & `appian-locust-2.0.0a3/appian_locust/loadDriverUtils.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/logger.py` & `appian-locust-2.0.0a3/appian_locust/logger.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/news_info.py` & `appian-locust-2.0.0a3/appian_locust/news_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/record_list_uiform.py` & `appian-locust-2.0.0a3/appian_locust/record_list_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/record_uiform.py` & `appian-locust-2.0.0a3/appian_locust/record_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/records_info.py` & `appian-locust-2.0.0a3/appian_locust/records_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/reports_info.py` & `appian-locust-2.0.0a3/appian_locust/reports_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from ._reports import _Reports
 
 
 class ReportsInfo:
     """
     Class which provides metadata about available reports from the Tempo Reports tab
     """
 
     def __init__(self, reports: _Reports):
         self.__reports = reports
 
-    def get_all_available_reports(self) -> Dict[str, Any]:
+    def get_all_available_reports(self, search_string: Optional[str] = None) -> Dict[str, Any]:
         """
         Retrieves all the available "reports" and associated metadata from "Appian-Tempo-Reports"
 
         Returns (dict): List of reports and associated metadata
 
         Examples:
 
             >>> reports_info.get_all_available_reports()
 
         """
-        return self.__reports.get_all()
+        return self.__reports.get_all(search_string=search_string)
 
     def get_report_info(self, report_name: str, exact_match: bool = True) -> Dict[str, Any]:
         """
         Get the information about specific report by name.
 
         Args:
             report_name (str): Name of the action
```

### Comparing `appian-locust-2.0.0a2/appian_locust/site_helper.py` & `appian-locust-2.0.0a3/appian_locust/site_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/tasks_info.py` & `appian-locust-2.0.0a3/appian_locust/tasks_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/tempo_navigator.py` & `appian-locust-2.0.0a3/appian_locust/tempo_navigator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from ._interactor import _Interactor
 from .news_info import NewsInfo
 from .actions_info import ActionsInfo
 from .records_info import RecordsInfo
 from .reports_info import ReportsInfo
 from .tasks_info import TasksInfo
 from ._actions import _Actions
 from ._interactor import _Interactor
```

### Comparing `appian-locust-2.0.0a2/appian_locust/uiform.py` & `appian-locust-2.0.0a3/appian_locust/uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust/visitor.py` & `appian-locust-2.0.0a3/appian_locust/visitor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/appian_locust.egg-info/PKG-INFO` & `appian-locust-2.0.0a3/appian_locust.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a2
+Version: 2.0.0a3
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.0.0a2/setup.cfg` & `appian-locust-2.0.0a3/setup.cfg`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a2/setup.py` & `appian-locust-2.0.0a3/setup.py`

 * *Files identical despite different names*

