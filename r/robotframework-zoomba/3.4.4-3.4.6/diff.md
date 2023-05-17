# Comparing `tmp/robotframework-zoomba-3.4.4.tar.gz` & `tmp/robotframework-zoomba-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-zoomba-3.4.4.tar", last modified: Mon Mar 13 18:25:01 2023, max compression
+gzip compressed data, was "robotframework-zoomba-3.4.6.tar", last modified: Wed May 17 19:38:05 2023, max compression
```

## Comparing `robotframework-zoomba-3.4.4.tar` & `robotframework-zoomba-3.4.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:25:01.431602 robotframework-zoomba-3.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-03-13 18:25:01.431602 robotframework-zoomba-3.4.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:25:01.431602 robotframework-zoomba-3.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-13 18:25:01.431602 robotframework-zoomba-3.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:25:01.431602 robotframework-zoomba-3.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:25:01.431602 robotframework-zoomba-3.4.4/src/Zoomba/
--rw-r--r--   0 runner    (1001) docker     (123)    32068 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/src/Zoomba/APILibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/src/Zoomba/DesktopLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)    22070 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/src/Zoomba/GUILibrary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:25:01.431602 robotframework-zoomba-3.4.4/src/Zoomba/Helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/src/Zoomba/Helpers/ReactSelect.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/src/Zoomba/Helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/src/Zoomba/MobileLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/src/Zoomba/SOAPLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/src/Zoomba/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:25:01.431602 robotframework-zoomba-3.4.4/src/robotframework_zoomba.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-03-13 18:25:01.000000 robotframework-zoomba-3.4.4/src/robotframework_zoomba.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-13 18:25:01.000000 robotframework-zoomba-3.4.4/src/robotframework_zoomba.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 18:25:01.000000 robotframework-zoomba-3.4.4/src/robotframework_zoomba.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-13 18:25:01.000000 robotframework-zoomba-3.4.4/src/robotframework_zoomba.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-13 18:25:01.000000 robotframework-zoomba-3.4.4/src/robotframework_zoomba.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-13 18:24:52.000000 robotframework-zoomba-3.4.4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:05.411110 robotframework-zoomba-3.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-05-17 19:38:05.411110 robotframework-zoomba-3.4.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:05.407110 robotframework-zoomba-3.4.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 19:38:05.411110 robotframework-zoomba-3.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:05.407110 robotframework-zoomba-3.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:05.411110 robotframework-zoomba-3.4.6/src/Zoomba/
+-rw-r--r--   0 runner    (1001) docker     (123)    32068 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/src/Zoomba/APILibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/src/Zoomba/DesktopLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22070 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/src/Zoomba/GUILibrary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:05.411110 robotframework-zoomba-3.4.6/src/Zoomba/Helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/src/Zoomba/Helpers/ReactSelect.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/src/Zoomba/Helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/src/Zoomba/MobileLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/src/Zoomba/SOAPLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/src/Zoomba/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:05.411110 robotframework-zoomba-3.4.6/src/robotframework_zoomba.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-05-17 19:38:05.000000 robotframework-zoomba-3.4.6/src/robotframework_zoomba.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-17 19:38:05.000000 robotframework-zoomba-3.4.6/src/robotframework_zoomba.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:38:05.000000 robotframework-zoomba-3.4.6/src/robotframework_zoomba.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-17 19:38:05.000000 robotframework-zoomba-3.4.6/src/robotframework_zoomba.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 19:38:05.000000 robotframework-zoomba-3.4.6/src/robotframework_zoomba.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 19:37:50.000000 robotframework-zoomba-3.4.6/version.py
```

### Comparing `robotframework-zoomba-3.4.4/LICENSE` & `robotframework-zoomba-3.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-3.4.4/PKG-INFO` & `robotframework-zoomba-3.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-zoomba
-Version: 3.4.4
+Version: 3.4.6
 Summary: Robot Framework mini-framework.
 Home-page: https://github.com/Accruent/zoomba
 Maintainer: Alex Calandra, Michael Hintz, Keith Smoland, Matthew Giardina, Brandon Wolfe, Neil Howell, Tommy Hoang
 Maintainer-email: robosquad@accruent.com
 License: GPL-3.0
 Keywords: Robot Framework robot-framework selenium requests appium soap winappdriver appium robotframeworkdesktop windows zoomba python robotframework-library appium-windows appiumlibrary api-rest api soap-api appium-mobile mobile
 Platform: any
```

### Comparing `robotframework-zoomba-3.4.4/docs/README.md` & `robotframework-zoomba-3.4.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-3.4.4/setup.py` & `robotframework-zoomba-3.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-3.4.4/src/Zoomba/APILibrary.py` & `robotframework-zoomba-3.4.6/src/Zoomba/APILibrary.py`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-3.4.4/src/Zoomba/GUILibrary.py` & `robotframework-zoomba-3.4.6/src/Zoomba/GUILibrary.py`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-3.4.4/src/Zoomba/Helpers/ReactSelect.py` & `robotframework-zoomba-3.4.6/src/Zoomba/Helpers/ReactSelect.py`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-3.4.4/src/Zoomba/SOAPLibrary.py` & `robotframework-zoomba-3.4.6/src/Zoomba/SOAPLibrary.py`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-3.4.4/src/robotframework_zoomba.egg-info/PKG-INFO` & `robotframework-zoomba-3.4.6/src/robotframework_zoomba.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-zoomba
-Version: 3.4.4
+Version: 3.4.6
 Summary: Robot Framework mini-framework.
 Home-page: https://github.com/Accruent/zoomba
 Maintainer: Alex Calandra, Michael Hintz, Keith Smoland, Matthew Giardina, Brandon Wolfe, Neil Howell, Tommy Hoang
 Maintainer-email: robosquad@accruent.com
 License: GPL-3.0
 Keywords: Robot Framework robot-framework selenium requests appium soap winappdriver appium robotframeworkdesktop windows zoomba python robotframework-library appium-windows appiumlibrary api-rest api soap-api appium-mobile mobile
 Platform: any
```

### Comparing `robotframework-zoomba-3.4.4/src/robotframework_zoomba.egg-info/SOURCES.txt` & `robotframework-zoomba-3.4.6/src/robotframework_zoomba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

