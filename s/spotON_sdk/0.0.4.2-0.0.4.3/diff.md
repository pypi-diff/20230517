# Comparing `tmp/spotON_sdk-0.0.4.2.tar.gz` & `tmp/spotON_sdk-0.0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.4.2.tar", last modified: Wed May 17 20:35:41 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.4.3.tar", last modified: Wed May 17 20:40:04 2023, max compression
```

## Comparing `spotON_sdk-0.0.4.2.tar` & `spotON_sdk-0.0.4.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.4.2/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.2/LICENSE
--rw-r--r--   0        0        0      319 2023-05-17 20:34:33.623695 spotON_sdk-0.0.4.2/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-17 20:32:40.303649 spotON_sdk-0.0.4.2/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.4.2/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      150 2023-05-13 09:50:24.206287 spotON_sdk-0.0.4.2/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.4.2/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0     3477 2023-05-13 09:52:05.827466 spotON_sdk-0.0.4.2/spotON_sdk/data_helpers/entsoe_query.py
--rw-r--r--   0        0        0     3863 2023-05-16 22:30:07.960999 spotON_sdk-0.0.4.2/spotON_sdk/settings/Config/Config.py
--rw-r--r--   0        0        0      163 2023-05-13 12:09:52.903536 spotON_sdk-0.0.4.2/spotON_sdk/settings/Config/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.2/spotON_sdk/settings/Config/bidding_zones.py
--rw-r--r--   0        0        0     4796 2023-05-17 20:32:32.318040 spotON_sdk-0.0.4.2/spotON_sdk/settings/Config/countries.py
--rw-r--r--   0        0        0     2337 2023-05-17 20:32:30.819588 spotON_sdk-0.0.4.2/spotON_sdk/settings/Config/markets.py
--rw-r--r--   0        0        0     6095 2023-05-17 20:20:49.477030 spotON_sdk-0.0.4.2/spotON_sdk/settings/Config/spotON_Areas.py
--rw-r--r--   0        0        0      424 2023-05-13 12:13:49.881633 spotON_sdk-0.0.4.2/spotON_sdk/settings/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.2/spotON_sdk/settings/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.2/spotON_sdk/settings/Feedback/Units.py
--rw-r--r--   0        0        0      132 2023-05-13 12:05:25.975505 spotON_sdk-0.0.4.2/spotON_sdk/settings/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-16 22:28:41.467762 spotON_sdk-0.0.4.2/spotON_sdk/settings/Switchtypes/Switchtypes.py
--rw-r--r--   0        0        0       91 2023-05-13 12:09:16.378665 spotON_sdk-0.0.4.2/spotON_sdk/settings/Switchtypes/__init__.py
--rw-r--r--   0        0        0      137 2023-05-13 12:11:13.611869 spotON_sdk-0.0.4.2/spotON_sdk/settings/__init__.py
--rw-r--r--   0        0        0      342 2023-05-13 12:13:23.297526 spotON_sdk-0.0.4.2/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      218 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.4.3/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.3/LICENSE
+-rw-r--r--   0        0        0      319 2023-05-17 20:34:33.623695 spotON_sdk-0.0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-17 20:39:56.751321 spotON_sdk-0.0.4.3/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.4.3/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      122 2023-05-17 20:39:45.544124 spotON_sdk-0.0.4.3/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.4.3/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0     3477 2023-05-13 09:52:05.827466 spotON_sdk-0.0.4.3/spotON_sdk/data_helpers/entsoe_query.py
+-rw-r--r--   0        0        0     3863 2023-05-16 22:30:07.960999 spotON_sdk-0.0.4.3/spotON_sdk/settings/Config/Config.py
+-rw-r--r--   0        0        0      163 2023-05-13 12:09:52.903536 spotON_sdk-0.0.4.3/spotON_sdk/settings/Config/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.3/spotON_sdk/settings/Config/bidding_zones.py
+-rw-r--r--   0        0        0     4796 2023-05-17 20:32:32.318040 spotON_sdk-0.0.4.3/spotON_sdk/settings/Config/countries.py
+-rw-r--r--   0        0        0     2337 2023-05-17 20:32:30.819588 spotON_sdk-0.0.4.3/spotON_sdk/settings/Config/markets.py
+-rw-r--r--   0        0        0     6095 2023-05-17 20:20:49.477030 spotON_sdk-0.0.4.3/spotON_sdk/settings/Config/spotON_Areas.py
+-rw-r--r--   0        0        0      424 2023-05-13 12:13:49.881633 spotON_sdk-0.0.4.3/spotON_sdk/settings/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.3/spotON_sdk/settings/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.3/spotON_sdk/settings/Feedback/Units.py
+-rw-r--r--   0        0        0      132 2023-05-13 12:05:25.975505 spotON_sdk-0.0.4.3/spotON_sdk/settings/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-16 22:28:41.467762 spotON_sdk-0.0.4.3/spotON_sdk/settings/Switchtypes/Switchtypes.py
+-rw-r--r--   0        0        0       91 2023-05-13 12:09:16.378665 spotON_sdk-0.0.4.3/spotON_sdk/settings/Switchtypes/__init__.py
+-rw-r--r--   0        0        0      137 2023-05-13 12:11:13.611869 spotON_sdk-0.0.4.3/spotON_sdk/settings/__init__.py
+-rw-r--r--   0        0        0      342 2023-05-13 12:13:23.297526 spotON_sdk-0.0.4.3/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      218 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.3/PKG-INFO
```

### Comparing `spotON_sdk-0.0.4.2/.gitignore` & `spotON_sdk-0.0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.2/LICENSE` & `spotON_sdk-0.0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.2/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.4.3/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.2/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.4.3/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.2/spotON_sdk/data_helpers/entsoe_query.py` & `spotON_sdk-0.0.4.3/spotON_sdk/data_helpers/entsoe_query.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.2/spotON_sdk/settings/Config/Config.py` & `spotON_sdk-0.0.4.3/spotON_sdk/settings/Config/Config.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.2/spotON_sdk/settings/Config/bidding_zones.py` & `spotON_sdk-0.0.4.3/spotON_sdk/settings/Config/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.2/spotON_sdk/settings/Config/countries.py` & `spotON_sdk-0.0.4.3/spotON_sdk/settings/Config/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.2/spotON_sdk/settings/Config/markets.py` & `spotON_sdk-0.0.4.3/spotON_sdk/settings/Config/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.2/spotON_sdk/settings/Config/spotON_Areas.py` & `spotON_sdk-0.0.4.3/spotON_sdk/settings/Config/spotON_Areas.py`

 * *Files identical despite different names*

