# Comparing `tmp/onsite-1.0.3.tar.gz` & `tmp/onsite-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onsite-1.0.3.tar", last modified: Thu May  4 05:22:44 2023, max compression
+gzip compressed data, was "onsite-1.0.4.tar", last modified: Wed May 17 08:34:47 2023, max compression
```

## Comparing `onsite-1.0.3.tar` & `onsite-1.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.260293 onsite-1.0.3/
--rw-rw-rw-   0        0        0     1094 2023-04-27 06:03:34.000000 onsite-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1999 2023-05-04 05:22:44.259294 onsite-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1595 2023-05-04 05:10:32.000000 onsite-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.223294 onsite-1.0.3/onsite/
--rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/__init__.py
--rw-rw-rw-   0        0        0    24362 2023-04-27 08:29:11.000000 onsite-1.0.3/onsite/controller.py
--rw-rw-rw-   0        0        0     1833 2023-04-27 06:04:56.000000 onsite-1.0.3/onsite/env.py
--rw-rw-rw-   0        0        0     1329 2023-04-27 06:04:56.000000 onsite-1.0.3/onsite/observation.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.240293 onsite-1.0.3/onsite/opendrive2discretenet/
--rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/__init__.py
--rw-rw-rw-   0        0        0    11497 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/converter.py
--rw-rw-rw-   0        0        0     2782 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/discrete_network.py
--rw-rw-rw-   0        0        0    18735 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/network.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.243294 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/
--rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.255294 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/
--rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/__init__.py
--rw-rw-rw-   0        0        0     2211 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/eulerspiral.py
--rw-rw-rw-   0        0        0     8552 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/geometry.py
--rw-rw-rw-   0        0        0     4115 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/junction.py
--rw-rw-rw-   0        0        0     2391 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/opendrive.py
--rw-rw-rw-   0        0        0     3417 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/road.py
--rw-rw-rw-   0        0        0      604 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadElevationProfile.py
--rw-rw-rw-   0        0        0     8581 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadLanes.py
--rw-rw-rw-   0        0        0     3755 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadLateralProfile.py
--rw-rw-rw-   0        0        0     5397 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadLink.py
--rw-rw-rw-   0        0        0     9660 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadPlanView.py
--rw-rw-rw-   0        0        0     1327 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/road_record.py
--rw-rw-rw-   0        0        0     2163 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadtype.py
--rw-rw-rw-   0        0        0    26573 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.259294 onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/
--rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/__init__.py
--rw-rw-rw-   0        0        0     3896 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/border.py
--rw-rw-rw-   0        0        0     9672 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/plane.py
--rw-rw-rw-   0        0        0    11525 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/plane_group.py
--rw-rw-rw-   0        0        0      835 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/utils.py
--rw-rw-rw-   0        0        0     4373 2023-04-27 06:04:56.000000 onsite-1.0.3/onsite/recorder.py
--rw-rw-rw-   0        0        0     4063 2023-04-27 06:04:56.000000 onsite-1.0.3/onsite/scenarioOrganizer.py
--rw-rw-rw-   0        0        0    11914 2023-04-27 06:04:56.000000 onsite-1.0.3/onsite/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.236294 onsite-1.0.3/onsite.egg-info/
--rw-rw-rw-   0        0        0     1999 2023-05-04 05:22:44.000000 onsite-1.0.3/onsite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1755 2023-05-04 05:22:44.000000 onsite-1.0.3/onsite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 05:22:44.000000 onsite-1.0.3/onsite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-04 05:22:44.000000 onsite-1.0.3/onsite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 05:22:44.000000 onsite-1.0.3/onsite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 05:22:44.260293 onsite-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-05-04 05:10:59.000000 onsite-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:34:47.790248 onsite-1.0.4/
+-rw-rw-rw-   0        0        0     1094 2023-04-27 06:03:34.000000 onsite-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2060 2023-05-17 08:34:47.789250 onsite-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1656 2023-05-17 08:33:18.000000 onsite-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 08:34:47.744250 onsite-1.0.4/onsite/
+-rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/__init__.py
+-rw-rw-rw-   0        0        0    24528 2023-05-15 11:52:29.000000 onsite-1.0.4/onsite/controller.py
+-rw-rw-rw-   0        0        0     1833 2023-04-27 06:04:56.000000 onsite-1.0.4/onsite/env.py
+-rw-rw-rw-   0        0        0     1329 2023-04-27 06:04:56.000000 onsite-1.0.4/onsite/observation.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:34:47.755249 onsite-1.0.4/onsite/opendrive2discretenet/
+-rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/__init__.py
+-rw-rw-rw-   0        0        0    11497 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/converter.py
+-rw-rw-rw-   0        0        0     2782 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/discrete_network.py
+-rw-rw-rw-   0        0        0    18735 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/network.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:34:47.756248 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/
+-rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:34:47.777248 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/
+-rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/__init__.py
+-rw-rw-rw-   0        0        0     2211 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/eulerspiral.py
+-rw-rw-rw-   0        0        0     8552 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/geometry.py
+-rw-rw-rw-   0        0        0     4115 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/junction.py
+-rw-rw-rw-   0        0        0     2391 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/opendrive.py
+-rw-rw-rw-   0        0        0     3417 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/road.py
+-rw-rw-rw-   0        0        0      604 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/roadElevationProfile.py
+-rw-rw-rw-   0        0        0     8581 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/roadLanes.py
+-rw-rw-rw-   0        0        0     3755 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/roadLateralProfile.py
+-rw-rw-rw-   0        0        0     5397 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/roadLink.py
+-rw-rw-rw-   0        0        0     9660 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/roadPlanView.py
+-rw-rw-rw-   0        0        0     1327 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/road_record.py
+-rw-rw-rw-   0        0        0     2163 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/roadtype.py
+-rw-rw-rw-   0        0        0    26573 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:34:47.788250 onsite-1.0.4/onsite/opendrive2discretenet/plane_elements/
+-rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/plane_elements/__init__.py
+-rw-rw-rw-   0        0        0     3896 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/plane_elements/border.py
+-rw-rw-rw-   0        0        0     9672 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/plane_elements/plane.py
+-rw-rw-rw-   0        0        0    11525 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/plane_elements/plane_group.py
+-rw-rw-rw-   0        0        0      835 2023-04-27 06:03:34.000000 onsite-1.0.4/onsite/opendrive2discretenet/utils.py
+-rw-rw-rw-   0        0        0     4373 2023-04-27 06:04:56.000000 onsite-1.0.4/onsite/recorder.py
+-rw-rw-rw-   0        0        0     4063 2023-04-27 06:04:56.000000 onsite-1.0.4/onsite/scenarioOrganizer.py
+-rw-rw-rw-   0        0        0    11914 2023-04-27 06:04:56.000000 onsite-1.0.4/onsite/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:34:47.749250 onsite-1.0.4/onsite.egg-info/
+-rw-rw-rw-   0        0        0     2060 2023-05-17 08:34:47.000000 onsite-1.0.4/onsite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1755 2023-05-17 08:34:47.000000 onsite-1.0.4/onsite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 08:34:47.000000 onsite-1.0.4/onsite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-17 08:34:47.000000 onsite-1.0.4/onsite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 08:34:47.000000 onsite-1.0.4/onsite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 08:34:47.790248 onsite-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-05-17 08:33:35.000000 onsite-1.0.4/setup.py
```

### Comparing `onsite-1.0.3/LICENSE.txt` & `onsite-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/PKG-INFO` & `onsite-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: onsite
-Version: 1.0.3
+Version: 1.0.4
 Summary: A tool package for Onsite
 Home-page: https://gitee.com/huangyansmile/onsite-public
 Author: Huang Yan
 Author-email: huangyan520@tongji.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ## 架构
 
 
 ## 更新说明
+- Version 1.0.4
+
+    比赛正式版，修复若干bug.
+
 - Version 1.0.3
 
     比赛正式版，修复若干bug.
 
 - Version 1.0.2
 
     比赛正式版，修复若干bug.
```

### Comparing `onsite-1.0.3/README.md` & `onsite-1.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 ## 架构
 
 
 ## 更新说明
+- Version 1.0.4
+
+    比赛正式版，修复若干bug.
+
 - Version 1.0.3
 
     比赛正式版，修复若干bug.
 
 - Version 1.0.2
 
     比赛正式版，修复若干bug.
```

### Comparing `onsite-1.0.3/onsite/controller.py` & `onsite-1.0.4/onsite/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,19 +359,21 @@
         new_observation = copy.copy(old_observation)
         new_observation.light_info = self.control_info.light_info[str(np.around(old_observation.test_setting['t'], 3))]
         return new_observation
 
     def _update_ego_and_t(self, action: tuple, old_observation: Observation) -> Observation:
         # 拷贝一份旧观察值
         new_observation = copy.copy(old_observation)
+        # 小数点位数，避免浮点数精度问题
+        decimal_places = len(str(old_observation.test_setting['dt']).split('.')[-1])
         # 首先修改时间，新时间=t+dt
-        new_observation.test_setting['t'] = float(
+        new_observation.test_setting['t'] = round(float(
             old_observation.test_setting['t'] +
             old_observation.test_setting['dt']
-        )
+        ), decimal_places)
         # 修改本车的位置，方式是前向欧拉更新，1.根据旧速度更新位置；2.然后更新速度。
         # 速度和位置的更新基于自行车模型。
         # 首先分别取出加速度和方向盘转角
         a, rot = action
         # 取出步长
         dt = old_observation.test_setting['dt']
         # 取出本车的各类信息
```

### Comparing `onsite-1.0.3/onsite/env.py` & `onsite-1.0.4/onsite/env.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/observation.py` & `onsite-1.0.4/onsite/observation.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/converter.py` & `onsite-1.0.4/onsite/opendrive2discretenet/converter.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/discrete_network.py` & `onsite-1.0.4/onsite/opendrive2discretenet/discrete_network.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/network.py` & `onsite-1.0.4/onsite/opendrive2discretenet/network.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/eulerspiral.py` & `onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/eulerspiral.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/geometry.py` & `onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/geometry.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/junction.py` & `onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/junction.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/opendrive.py` & `onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/opendrive.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/road.py` & `onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/road.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadElevationProfile.py` & `onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/roadElevationProfile.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadLanes.py` & `onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/roadLanes.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadLateralProfile.py` & `onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/roadLateralProfile.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadLink.py` & `onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/roadLink.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadPlanView.py` & `onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/roadPlanView.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/road_record.py` & `onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/road_record.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadtype.py` & `onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/elements/roadtype.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/parser.py` & `onsite-1.0.4/onsite/opendrive2discretenet/opendriveparser/parser.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/border.py` & `onsite-1.0.4/onsite/opendrive2discretenet/plane_elements/border.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/plane.py` & `onsite-1.0.4/onsite/opendrive2discretenet/plane_elements/plane.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/plane_group.py` & `onsite-1.0.4/onsite/opendrive2discretenet/plane_elements/plane_group.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/opendrive2discretenet/utils.py` & `onsite-1.0.4/onsite/opendrive2discretenet/utils.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/recorder.py` & `onsite-1.0.4/onsite/recorder.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/scenarioOrganizer.py` & `onsite-1.0.4/onsite/scenarioOrganizer.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite/visualizer.py` & `onsite-1.0.4/onsite/visualizer.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/onsite.egg-info/PKG-INFO` & `onsite-1.0.4/onsite.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: onsite
-Version: 1.0.3
+Version: 1.0.4
 Summary: A tool package for Onsite
 Home-page: https://gitee.com/huangyansmile/onsite-public
 Author: Huang Yan
 Author-email: huangyan520@tongji.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ## 架构
 
 
 ## 更新说明
+- Version 1.0.4
+
+    比赛正式版，修复若干bug.
+
 - Version 1.0.3
 
     比赛正式版，修复若干bug.
 
 - Version 1.0.2
 
     比赛正式版，修复若干bug.
```

### Comparing `onsite-1.0.3/onsite.egg-info/SOURCES.txt` & `onsite-1.0.4/onsite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onsite-1.0.3/setup.py` & `onsite-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="onsite", 
-    version="1.0.3",
+    version="1.0.4",
     author="Huang Yan",   
     author_email="huangyan520@tongji.edu.cn",   
     description="A tool package for Onsite",
     long_description=long_description,    
     long_description_content_type="text/markdown",
     url="https://gitee.com/huangyansmile/onsite-public", 
     packages=setuptools.find_packages(),
```

