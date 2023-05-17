# Comparing `tmp/segmentheepy_test-0.0.5-py3-none-any.whl.zip` & `tmp/segmentheepy_test-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10627 bytes, number of entries: 9
+Zip file size: 10776 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-09 16:01 segmenthee/__init__.py
--rw-rw-r--  2.0 unx    26963 b- defN 23-May-16 09:18 segmenthee/cart_api.py
+-rw-rw-r--  2.0 unx    27783 b- defN 23-May-17 10:24 segmenthee/cart_api.py
 -rw-rw-r--  2.0 unx      766 b- defN 23-May-09 16:01 segmenthee/config.py
 -rw-rw-r--  2.0 unx     2023 b- defN 23-May-09 16:01 segmenthee/parser_api.py
 -rw-rw-r--  2.0 unx     7932 b- defN 23-May-09 16:02 segmenthee/shop.py
--rw-rw-r--  2.0 unx      261 b- defN 23-May-16 09:29 segmentheepy_test-0.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-16 09:29 segmentheepy_test-0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-May-16 09:29 segmentheepy_test-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      725 b- defN 23-May-16 09:29 segmentheepy_test-0.0.5.dist-info/RECORD
-9 files, 38773 bytes uncompressed, 9373 bytes compressed:  75.8%
+-rw-rw-r--  2.0 unx      261 b- defN 23-May-17 10:31 segmentheepy_test-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-17 10:31 segmentheepy_test-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-May-17 10:31 segmentheepy_test-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      725 b- defN 23-May-17 10:31 segmentheepy_test-0.0.6.dist-info/RECORD
+9 files, 39593 bytes uncompressed, 9522 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: segmenthee/parser_api.py
 Comment: 
 
 Filename: segmenthee/shop.py
 Comment: 
 
-Filename: segmentheepy_test-0.0.5.dist-info/METADATA
+Filename: segmentheepy_test-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: segmentheepy_test-0.0.5.dist-info/WHEEL
+Filename: segmentheepy_test-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: segmentheepy_test-0.0.5.dist-info/top_level.txt
+Filename: segmentheepy_test-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: segmentheepy_test-0.0.5.dist-info/RECORD
+Filename: segmentheepy_test-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## segmenthee/cart_api.py

```diff
@@ -24,29 +24,30 @@
     classcount += 1
     return retval
 
 #collect name from classindex
 classnames = dict()
 
 params = {
-    "clickrate": 0.75,
-    "actionseparation": [0.0, 0.25, 0.025],
-    "actionaffinity": [0.0, 0.25, 0.025],
-    "categoryaffinity": [0.0, 0.25, 0.025],
-    "carttotaltrend": [0.0, 0.25, 0.025],
-    "cartcounttrend": [0.0, 0.25, 0.025],
-    "avgpricemanipulation": [0.0, 0.25, 0.025],
-    "lastpriceviewedtrend": [0.0, 0.25, 0.025],
-    "tabcounttrend": [0.0, 0.25, 0.025],
-    "redirectstrend": [0.0, 0.25, 0.025],
-    "tabtypetrend": [0.0, 0.25, 0.025],
-    "navigationtrend": [0.0, 0.25, 0.025],
-    "referrertrend": [0.0, 0.25, 0.025],
-    "pagetrend": [0.0, 0.25, 0.025],
-    "sorttrend": [0.0, 0.25, 0.025]
+    "clickrate": 0.5,
+    "actionseparation": (0.5, 0.005),
+    "actionaffinity": (0.0, 0.025, 0.03),
+    "timeaffinity": (0.0, 0.025, 0.03),
+    "categoryaffinity": (0.025, 0.03),
+    "carttotaltrend": (0.05, 0.025),
+    "cartcounttrend": (0.01, 0.04),
+    "avgpricemanipulation": (0.05, 0.025),
+    "lastpriceviewedtrend": (0.05, 0.025),
+    "tabcounttrend": (0.01, 0.04),
+    "redirectstrend": (0.25, 0.01),
+    "tabtypetrend": (0.25, 0.01),
+    "navigationtrend": (0.25, 0.01),
+    "referrertrend": (0.25, 0.01),
+    "pagetrend": (0.01, 0.04),
+    "sorttrend": (0.25, 0.01)
 }
 
 MAX_CATEGORY = 6
 tabtype_dict = {'New':0, 'Existing':1}
 navigation_dict = {'NAVIGATE':0,'FORWARD':1,'BACK':2,'RELOAD':3}
 origin_dict = {"facebook":0,"google":1,"shop":2}
 sort_dict = {'default':0, 'name':1, 'price':2, 'order':3, 'relevance':4, 'date':5, 'rating':6, 'latest':7, 'discount':8, 'view':9}
@@ -84,14 +85,17 @@
     if 'fbclid' in keys:
         return 'facebook'
     return ''
 
 
 # timeweights = json.load(open("vagyaim/timeweights.json"))
 
+def FeatureNotAvailableWarning(feature_str):
+    print(f"Warning: {feature_str} not in state.")
+
 def LogCategory(retval,coeffs,category):
     if "categoryaffinity" not in retval:
         return None
     arr = retval["categoryaffinity"]
     categoryattfacts = coeffs["categoryaffinity"]
     for attix in range(len(categoryattfacts)):
         attfact = categoryattfacts[attix]
@@ -130,19 +134,23 @@
         values[attix] += (1 - featureattfacts[attix]) * new_value
         
 def UpdateAffinity(retval, coeffs, feature, update_index):
     if feature not in retval:
         return None
     values = retval[feature]
     featureattfacts = coeffs[feature]
+    if (feature == "actionaffinity"):
+        difffeature = "actiondifference"
+        for attix in range(len(featureattfacts)):
+            for act in range(len(values[0])):
+                retval["actiondifference"][attix][act] = -(1 - featureattfacts[attix]) * values[attix][act]
+            retval["actiondifference"][attix][update_index] += (1 - featureattfacts[attix])
     for attix in range(len(featureattfacts)):
         for act in range(len(values[0])):
-            retval["actiondifference"][attix][act] = (featureattfacts[attix] - 1) * values[attix][act]
             values[attix][act] *= featureattfacts[attix]
-        retval["actiondifference"][attix][update_index] += (featureattfacts[attix] - 1)
         values[attix][update_index] += 1 - featureattfacts[attix]
         
 def GetCoefficients(coeffs, params, delta_time):
     ''' exp(-lambda * delta_time) '''
     for key in params:
         if not isinstance(params[key],list):
             continue
@@ -218,28 +226,37 @@
         retval = super().Update(prevstate)
         retval["actioncount"] += 1
         if retval["actioncount"] > 1: #lastactioneventtime is not None
             delta_time = self.time - retval["lastactioneventtime"]
             GetCoefficients(self.coeffs, params, delta_time)
             retval["clickrate"] = delta_time
             UpdateAffinity(retval, self.coeffs, "actionaffinity", self.classindex())
+            UpdateAffinity(retval, self.coeffs, "timeaffinity", retval["lastactioneventindex"])
             UpdateAttribute(retval, self.coeffs, "actionseparation", delta_time)
             #frustration: clickrates
             if retval["actioncount"] == 2: #initialize clickrates
                 UpdateClickrates(retval, self.time, params["clickrate"], initialize=True)
             else: #actioncount >= 3
                 UpdateClickrates(retval, self.time, params["clickrate"], initialize=False)
         else: #first action event
-            GetCoefficients(self.coeffs, params, 0) #timeaffinity stays 0.0
+            GetCoefficients(self.coeffs, params, 0) #time dependent affinity parameter stays 0.0
             UpdateAffinity(retval, self.coeffs, "actionaffinity", self.classindex())
-            #arr = retval["actionaffinity"][0]
-            #for act in range(classcount):
-            #    arr[act] *= params["actionaffinity"][0]
-            #arr[self.classindex()] += 1 - params["actionaffinity"][0]
+            # actionaffinity
+            arr = retval["actionaffinity"][0]
+            for act in range(classcount):
+                arr[act] *= 0.0
+            arr[self.classindex()] += 1.0
+            # actiondifference
+            arr = retval["actiondifference"][0]
+            for act in range(classcount):
+                arr[act] *= 0.0
+            arr[self.classindex()] += 1.0
         retval["lastactioneventtime"] = self.time
+        retval["lastactioneventindex"] = self.classindex()
+        # retval["lastactioneventclass"] = self.eventclass
         if retval["highwatermark"] < 1:
             retval["highwatermark"] = 1
         return retval
 
 class CartModifyEvent(UserActionEvent):
     def __init__(self, time: int, delta_count: int, delta_total):
         super().__init__(time)
@@ -541,26 +558,25 @@
         "origin": origin,
         "device": device,
         "os": os,
         "lang":lang,
         "actioncount": 0,
         "lastbodyeventtime": None,
         "lastactioneventtime": None,
-        # "firsteventclass": firsteventclass,
-        # "lastbodyeventclass": firsteventclass,
-        # "lastactioneventclass": None,
+        "lastactioneventindex": None,
         "clickrate_avg": 0.0,
         "clickrate_squares": 0.0,
         "clickrate_var": 0.0,
         "z_score": 0.0,
         "sessionstatus": "Browsing",
         "clickrate": 0.0,
         "actionseparation": [0.0] * len(params["actionseparation"]),
-        "actionaffinity": [[1/classcount] * classcount for _ in range(len(params["actionaffinity"]))],
-        "actiondifference": [[1 / classcount] * classcount for _ in range(len(params["actionaffinity"]))],
+        "actionaffinity": [[1 / classcount] * classcount for _ in range(len(params["actionaffinity"]))],
+        "actiondifference": [[0.0] * classcount for _ in range(len(params["actionaffinity"]))],
+        "timeaffinity": [[1 / classcount] * classcount for _ in range(len(params["timeaffinity"]))],
         "lastcategory": None,
         "categoryaffinity": [[1/MAX_CATEGORY] * MAX_CATEGORY for _ in range(len(params["categoryaffinity"]))],
         "carttotal":0.0,
         "cartcount":0,
         "cartdeltatotal": 0.0,
         "cartdeltacount": 0,
         "carttotaltrend": [0.0] * len(params["carttotaltrend"]),
@@ -611,14 +627,19 @@
             row["actionaffinity_" + str(i) + "_" + classnames[j]] = arr[i][j]
 
     arr = state["actiondifference"]
     for i in range(len(arr)):
         for j in range(len(arr[0])):
             row["actiondifference_" + str(i) + "_" + classnames[j]] = arr[i][j]
 
+    arr = state["timeaffinity"]
+    for i in range(len(arr)):
+        for j in range(len(arr[0])):
+            row["timeaffinity_" + str(i) + "_" + classnames[j]] = arr[i][j]
+
     arr = state["categoryaffinity"]
     for i in range(len(arr)):
         for j in range(len(arr[0])):
             row["categoryaffinity_" + str(i) + "_" + str(j)] = arr[i][j]
             
     arr = state["carttotaltrend"]
     for i in range(len(arr)):
```

## Comparing `segmentheepy_test-0.0.5.dist-info/RECORD` & `segmentheepy_test-0.0.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 segmenthee/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-segmenthee/cart_api.py,sha256=u5A4u-30q9o3LNQfCxHIpAXHDrxYYl55lKDj8vQ49_8,26963
+segmenthee/cart_api.py,sha256=muy11e0_wzc81AYcbgqTFQjQZmAIIKt-MwWq-3gCiNw,27783
 segmenthee/config.py,sha256=lXea6JINCK44eZP38JaQOlfgVerzFx0e9wDxObuw54c,766
 segmenthee/parser_api.py,sha256=TB-Q8roqNAV_wwYSrdJYchNoC3zTGRKI0die0sN-K-8,2023
 segmenthee/shop.py,sha256=RlKZfL1vebVw6JOxUthPfzgzkcU7MaAYE96Wc4EYDJQ,7932
-segmentheepy_test-0.0.5.dist-info/METADATA,sha256=Ynhs5_g3V8hMWDGN6c_bZUBEMTDZXVO5pom1UY5J8_o,261
-segmentheepy_test-0.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-segmentheepy_test-0.0.5.dist-info/top_level.txt,sha256=ESnfgSm7LAnmWZiJ4HDmTbd5B0AemZ20M9sFA5X59IU,11
-segmentheepy_test-0.0.5.dist-info/RECORD,,
+segmentheepy_test-0.0.6.dist-info/METADATA,sha256=R6FXlLi6Eek2ZZG28okjvCLmeQnSgOB_7VR0UeazLlg,261
+segmentheepy_test-0.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+segmentheepy_test-0.0.6.dist-info/top_level.txt,sha256=ESnfgSm7LAnmWZiJ4HDmTbd5B0AemZ20M9sFA5X59IU,11
+segmentheepy_test-0.0.6.dist-info/RECORD,,
```

