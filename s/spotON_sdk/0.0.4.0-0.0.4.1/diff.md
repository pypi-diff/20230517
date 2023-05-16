# Comparing `tmp/spotON_sdk-0.0.4.0.tar.gz` & `tmp/spotON_sdk-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.4.0.tar", last modified: Sat May 13 13:05:49 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.4.1.tar", last modified: Tue May 16 22:32:39 2023, max compression
```

## Comparing `spotON_sdk-0.0.4.0.tar` & `spotON_sdk-0.0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.4.0/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.0/LICENSE
--rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.4.0/pyproject.toml
--rw-r--r--   0        0        0      471 2023-05-13 12:21:23.587076 spotON_sdk-0.0.4.0/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.4.0/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      150 2023-05-13 09:50:24.206287 spotON_sdk-0.0.4.0/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.4.0/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0     3477 2023-05-13 09:52:05.827466 spotON_sdk-0.0.4.0/spotON_sdk/data_helpers/entsoe_query.py
--rw-r--r--   0        0        0     2643 2023-05-13 12:17:11.591288 spotON_sdk-0.0.4.0/spotON_sdk/settings/Config/Config.py
--rw-r--r--   0        0        0      163 2023-05-13 12:09:52.903536 spotON_sdk-0.0.4.0/spotON_sdk/settings/Config/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.0/spotON_sdk/settings/Config/bidding_zones.py
--rw-r--r--   0        0        0     4783 2023-05-13 09:44:54.918595 spotON_sdk-0.0.4.0/spotON_sdk/settings/Config/countries.py
--rw-r--r--   0        0        0     2289 2023-05-13 11:25:11.404195 spotON_sdk-0.0.4.0/spotON_sdk/settings/Config/markets.py
--rw-r--r--   0        0        0      424 2023-05-13 12:13:49.881633 spotON_sdk-0.0.4.0/spotON_sdk/settings/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.0/spotON_sdk/settings/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.0/spotON_sdk/settings/Feedback/Units.py
--rw-r--r--   0        0        0      132 2023-05-13 12:05:25.975505 spotON_sdk-0.0.4.0/spotON_sdk/settings/Feedback/__init__.py
--rw-r--r--   0        0        0       64 2023-05-13 12:09:44.848658 spotON_sdk-0.0.4.0/spotON_sdk/settings/Switchtypes/Switchtypes.py
--rw-r--r--   0        0        0       91 2023-05-13 12:09:16.378665 spotON_sdk-0.0.4.0/spotON_sdk/settings/Switchtypes/__init__.py
--rw-r--r--   0        0        0      137 2023-05-13 12:11:13.611869 spotON_sdk-0.0.4.0/spotON_sdk/settings/__init__.py
--rw-r--r--   0        0        0      342 2023-05-13 12:13:23.297526 spotON_sdk-0.0.4.0/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.4.1/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.1/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      471 2023-05-16 22:32:09.160262 spotON_sdk-0.0.4.1/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.4.1/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      150 2023-05-13 09:50:24.206287 spotON_sdk-0.0.4.1/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.4.1/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0     3477 2023-05-13 09:52:05.827466 spotON_sdk-0.0.4.1/spotON_sdk/data_helpers/entsoe_query.py
+-rw-r--r--   0        0        0     3863 2023-05-16 22:30:07.960999 spotON_sdk-0.0.4.1/spotON_sdk/settings/Config/Config.py
+-rw-r--r--   0        0        0      163 2023-05-13 12:09:52.903536 spotON_sdk-0.0.4.1/spotON_sdk/settings/Config/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.1/spotON_sdk/settings/Config/bidding_zones.py
+-rw-r--r--   0        0        0     4783 2023-05-13 09:44:54.918595 spotON_sdk-0.0.4.1/spotON_sdk/settings/Config/countries.py
+-rw-r--r--   0        0        0     2289 2023-05-13 11:25:11.404195 spotON_sdk-0.0.4.1/spotON_sdk/settings/Config/markets.py
+-rw-r--r--   0        0        0      424 2023-05-13 12:13:49.881633 spotON_sdk-0.0.4.1/spotON_sdk/settings/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.1/spotON_sdk/settings/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.1/spotON_sdk/settings/Feedback/Units.py
+-rw-r--r--   0        0        0      132 2023-05-13 12:05:25.975505 spotON_sdk-0.0.4.1/spotON_sdk/settings/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-16 22:28:41.467762 spotON_sdk-0.0.4.1/spotON_sdk/settings/Switchtypes/Switchtypes.py
+-rw-r--r--   0        0        0       91 2023-05-13 12:09:16.378665 spotON_sdk-0.0.4.1/spotON_sdk/settings/Switchtypes/__init__.py
+-rw-r--r--   0        0        0      137 2023-05-13 12:11:13.611869 spotON_sdk-0.0.4.1/spotON_sdk/settings/__init__.py
+-rw-r--r--   0        0        0      342 2023-05-13 12:13:23.297526 spotON_sdk-0.0.4.1/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.1/PKG-INFO
```

### Comparing `spotON_sdk-0.0.4.0/.gitignore` & `spotON_sdk-0.0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.0/LICENSE` & `spotON_sdk-0.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.0/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.4.1/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.0/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.4.1/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.0/spotON_sdk/data_helpers/entsoe_query.py` & `spotON_sdk-0.0.4.1/spotON_sdk/data_helpers/entsoe_query.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.0/spotON_sdk/settings/Config/Config.py` & `spotON_sdk-0.0.4.1/spotON_sdk/settings/Config/Config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,89 @@
-from dataclasses import dataclass,field
+from enum import Flag, auto
 from typing import List
-
+from dataclasses import dataclass, field
 from .markets import Market
 
 
-class PeriodTypes():
-    wholeDay :str = "24h Hour Period"
-    timeFrame :str = "Timeframe"
+
+class Pricefinding_Type(Flag):
+    INTERRUPTED = auto()
+    CONTINUOUS = auto()
+
+
+class TimeFrame_Type(Flag):
+    WHOLE_DAY = auto()
+    TIMEFRAME = auto()
+
+
+
 
 @dataclass
 class TimeFrameValidation():
     passed :bool
     def return_Validation_Result(self):
         if self.passed == False:
             return "<br> 🚨 <mark> Your Timeframe is SHORTER than your desired ON Time</mark> "
         else:
             return ""
 
+@dataclass
+class Resolution():
+    name :str 
+    value: float
+
+
 
 @dataclass
 class Config():
+    #TODO Implement resolution 15Min, 30Min etc....
     nr_of_Hours_On :int
-    uninterrupted :bool
+    pricefinding_Type :Pricefinding_Type
     market : Market 
     timeframe :List[List[int]] 
-    periodType : PeriodTypes| str = field(default="")
-    dayframe: List[int] | None = field(default=None,init=False) 
-    bestHour :str = ""
-    week: int = 100
+    timeframe_Type : TimeFrame_Type = field(init=False)
+    week: int | None = field(init=False,default=None)
+    resolution: Resolution = field(default_factory=lambda: Resolution("One_Hour", 1))
     timeFrameValidation = TimeFrameValidation(False)
 
     def __post_init__(self):
+        def check_Period_type():
+            if len(self.find_Possible_Hours())>=24:
+                self.timeframe_Type = TimeFrame_Type.WHOLE_DAY
+            else:
+                self.timeframe_Type = TimeFrame_Type.TIMEFRAME
+
         def check_nr_of_Hours_not_0():
             if self.nr_of_Hours_On < 1:
                 raise ValueError(f"Hey your Number of Hours On can't be zero")
 
         def check_TimeFrame_is_large_enogh():
             if len(self.find_Possible_Hours()) > self.nr_of_Hours_On:
                 self.timeFrameValidation = TimeFrameValidation(True)
             else:
                 self.timeFrameValidation = TimeFrameValidation(False)
         
-        def checkConfig():
-            if self.uninterrupted:
+        def checkLogic():
+            if self.pricefinding_Type == Pricefinding_Type.CONTINUOUS:
                 if len(self.timeframe) > 1:
-                    raise ValueError(f"Hey your Timeframe has the Attribute of Beeing uninterruped means you can't have multiple timeframes")
+                    raise ValueError(f"Hey your Timeframe has the Attribute of Beeing CONTINUOUS means you can't have multiple timeframes")
 
 
 
         def check_Overlapping_Arrays():
             possible_Hours = self.find_Possible_Hours()
             if(len(set(possible_Hours)) != len(possible_Hours)):
                 raise ValueError(f"Hey your Timeframes {self.timeframe} have overlapping Hours. Reduce it to one")
             
-        
+        check_Period_type()
         check_nr_of_Hours_not_0()
         check_TimeFrame_is_large_enogh()
-        checkConfig()
+        checkLogic()
         #check_Overlapping_Arrays()
-        
+
     def find_Possible_Hours(self):
         possible_Hours = []
         for timeframe in self.timeframe:
             start,end = timeframe[0],timeframe[1]
             def loop_Hours(_start,_end):
                 for hour in range (_start,_end):
                     possible_Hours.append(hour)
@@ -74,8 +95,25 @@
                 loop_Hours(0,end)
 
         if possible_Hours == []:    # If its the same start and end consider the whole day is OK
             possible_Hours = [*range(0,24)]
 
 
         return possible_Hours
+    
+    def return_possible_Starting_Hours(self):
+        if self.timeframe_Type == TimeFrame_Type.WHOLE_DAY:
+            valid_Hours_List = self.find_Possible_Hours()
+
+        elif self.timeframe_Type == TimeFrame_Type.TIMEFRAME:
+            '''Deletes Hours that are outside the timeframe End'''
+            possible_Hours = self.find_Possible_Hours()
+            nr_of_Hours_On = self.nr_of_Hours_On
+            
+            valid_Hours_List = []
+            for hour in possible_Hours:
+                    if hour + nr_of_Hours_On - self.resolution.value in possible_Hours:
+                            valid_Hours_List.append(hour)
+            
+        return valid_Hours_List
+
```

### Comparing `spotON_sdk-0.0.4.0/spotON_sdk/settings/Config/bidding_zones.py` & `spotON_sdk-0.0.4.1/spotON_sdk/settings/Config/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.0/spotON_sdk/settings/Config/countries.py` & `spotON_sdk-0.0.4.1/spotON_sdk/settings/Config/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.0/spotON_sdk/settings/Config/markets.py` & `spotON_sdk-0.0.4.1/spotON_sdk/settings/Config/markets.py`

 * *Files identical despite different names*

