# Comparing `tmp/spotON_sdk-0.0.4.4.tar.gz` & `tmp/spotON_sdk-0.0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.4.4.tar", last modified: Wed May 17 21:33:55 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.4.5.tar", last modified: Wed May 17 21:54:13 2023, max compression
```

## Comparing `spotON_sdk-0.0.4.4.tar` & `spotON_sdk-0.0.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.4.4/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.4/LICENSE
--rw-r--r--   0        0        0      319 2023-05-17 20:34:33.623695 spotON_sdk-0.0.4.4/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-17 21:12:08.438361 spotON_sdk-0.0.4.4/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.4.4/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      122 2023-05-17 20:39:45.544124 spotON_sdk-0.0.4.4/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.4.4/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0     3477 2023-05-13 09:52:05.827466 spotON_sdk-0.0.4.4/spotON_sdk/data_helpers/entsoe_query.py
--rw-r--r--   0        0        0     3863 2023-05-16 22:30:07.960999 spotON_sdk-0.0.4.4/spotON_sdk/settings/Config/Config.py
--rw-r--r--   0        0        0      163 2023-05-13 12:09:52.903536 spotON_sdk-0.0.4.4/spotON_sdk/settings/Config/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.4/spotON_sdk/settings/Config/bidding_zones.py
--rw-r--r--   0        0        0     4796 2023-05-17 20:32:32.318040 spotON_sdk-0.0.4.4/spotON_sdk/settings/Config/countries.py
--rw-r--r--   0        0        0     2351 2023-05-17 21:12:02.442054 spotON_sdk-0.0.4.4/spotON_sdk/settings/Config/markets.py
--rw-r--r--   0        0        0     6875 2023-05-17 21:31:51.983935 spotON_sdk-0.0.4.4/spotON_sdk/settings/Config/spotON_Areas.py
--rw-r--r--   0        0        0      424 2023-05-13 12:13:49.881633 spotON_sdk-0.0.4.4/spotON_sdk/settings/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.4/spotON_sdk/settings/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.4/spotON_sdk/settings/Feedback/Units.py
--rw-r--r--   0        0        0      132 2023-05-13 12:05:25.975505 spotON_sdk-0.0.4.4/spotON_sdk/settings/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-16 22:28:41.467762 spotON_sdk-0.0.4.4/spotON_sdk/settings/Switchtypes/Switchtypes.py
--rw-r--r--   0        0        0       91 2023-05-13 12:09:16.378665 spotON_sdk-0.0.4.4/spotON_sdk/settings/Switchtypes/__init__.py
--rw-r--r--   0        0        0      137 2023-05-13 12:11:13.611869 spotON_sdk-0.0.4.4/spotON_sdk/settings/__init__.py
--rw-r--r--   0        0        0      342 2023-05-13 12:13:23.297526 spotON_sdk-0.0.4.4/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      218 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.4.5/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.5/LICENSE
+-rw-r--r--   0        0        0      319 2023-05-17 20:34:33.623695 spotON_sdk-0.0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-17 21:54:07.821850 spotON_sdk-0.0.4.5/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.4.5/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      122 2023-05-17 20:39:45.544124 spotON_sdk-0.0.4.5/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.4.5/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0     3477 2023-05-13 09:52:05.827466 spotON_sdk-0.0.4.5/spotON_sdk/data_helpers/entsoe_query.py
+-rw-r--r--   0        0        0     3863 2023-05-16 22:30:07.960999 spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/Config.py
+-rw-r--r--   0        0        0      163 2023-05-13 12:09:52.903536 spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/bidding_zones.py
+-rw-r--r--   0        0        0     4796 2023-05-17 20:32:32.318040 spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/countries.py
+-rw-r--r--   0        0        0     2351 2023-05-17 21:53:53.693111 spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/markets.py
+-rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/spotON_Areas.py
+-rw-r--r--   0        0        0      424 2023-05-13 12:13:49.881633 spotON_sdk-0.0.4.5/spotON_sdk/settings/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.5/spotON_sdk/settings/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.5/spotON_sdk/settings/Feedback/Units.py
+-rw-r--r--   0        0        0      132 2023-05-13 12:05:25.975505 spotON_sdk-0.0.4.5/spotON_sdk/settings/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-16 22:28:41.467762 spotON_sdk-0.0.4.5/spotON_sdk/settings/Switchtypes/Switchtypes.py
+-rw-r--r--   0        0        0       91 2023-05-13 12:09:16.378665 spotON_sdk-0.0.4.5/spotON_sdk/settings/Switchtypes/__init__.py
+-rw-r--r--   0        0        0      137 2023-05-13 12:11:13.611869 spotON_sdk-0.0.4.5/spotON_sdk/settings/__init__.py
+-rw-r--r--   0        0        0      342 2023-05-13 12:13:23.297526 spotON_sdk-0.0.4.5/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      218 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.5/PKG-INFO
```

### Comparing `spotON_sdk-0.0.4.4/.gitignore` & `spotON_sdk-0.0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.4/LICENSE` & `spotON_sdk-0.0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.4/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.4.5/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.4/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.4.5/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.4/spotON_sdk/data_helpers/entsoe_query.py` & `spotON_sdk-0.0.4.5/spotON_sdk/data_helpers/entsoe_query.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.4/spotON_sdk/settings/Config/Config.py` & `spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/Config.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.4/spotON_sdk/settings/Config/bidding_zones.py` & `spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.4/spotON_sdk/settings/Config/countries.py` & `spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.4/spotON_sdk/settings/Config/markets.py` & `spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.4/spotON_sdk/settings/Config/spotON_Areas.py` & `spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/spotON_Areas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from dataclasses import dataclass
 from enum import Enum
 
 @dataclass
 class Area_details():
-    name : str
+    name:str
     code: str
     tz: str
+    # How can i add a name: str with the Object name example : name :str = AL
 
-class spotON_Area(Enum):
+@dataclass
+class spotON_Area():
     AL = Area_details('AL','10YAL-KESH-----5','Europe/Tirane')
     AT = Area_details('AT','10YAT-APG------L','Europe/Vienna')
     BA = Area_details('BA','10YBA-JPCC-----D','Europe/Sarajevo')
     BE = Area_details('BE','10YBE----------2','Europe/Brussels')
     BG = Area_details('BG','10YCA-BULGARIA-R','Europe/Sofia')
     BY = Area_details('BY','10Y1001A1001A51S','Europe/Minsk')
     CH = Area_details('CH','10YCH-SWISSGRIDZ','Europe/Zurich')
@@ -102,8 +104,8 @@
     TR = Area_details('TR','10YTR-TEIAS----W','Europe/Istanbul')
     UA = Area_details('UA','10Y1001C--00003F','Europe/Kiev')
     UA_BEI = Area_details('UA_BEI','10YUA-WEPS-----0','Europe/Kiev')
     UA_DOBTPP = Area_details('UA_DOBTPP','10Y1001A1001A869','Europe/Kiev')
     UA_IPS = Area_details('UA_IPS','10Y1001C--000182','Europe/Kiev')
     UK = Area_details('UK','10Y1001A1001A92E','Europe/London')
     XK = Area_details('XK','10Y1001C--00100H','Europe/Rome')
-    pass
+    pass
```

