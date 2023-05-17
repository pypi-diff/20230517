# Comparing `tmp/picframe-2022.6.3.tar.gz` & `tmp/picframe-2023.5.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picframe-2022.6.3.tar", last modified: Fri Jun  3 11:29:58 2022, max compression
+gzip compressed data, was "picframe-2023.5.17.tar", last modified: Wed May 17 08:43:42 2023, max compression
```

## Comparing `picframe-2022.6.3.tar` & `picframe-2023.5.17.tar`

### file list

```diff
@@ -1,31 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 11:29:58.723932 picframe-2022.6.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-06-03 11:29:47.000000 picframe-2022.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-06-03 11:29:58.723932 picframe-2022.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-06-03 11:29:47.000000 picframe-2022.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 11:29:58.723932 picframe-2022.6.3/picframe/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-06-03 11:29:58.723932 picframe-2022.6.3/picframe/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    12097 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/geo_reverse.py
--rw-r--r--   0 runner    (1001) docker     (121)     7254 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/get_image_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)    24078 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     6922 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/interface_http.py
--rw-r--r--   0 runner    (1001) docker     (121)    23748 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/interface_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (121)    14392 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/interface_peripherals.py
--rw-r--r--   0 runner    (1001) docker     (121)    21060 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/mat_image.py
--rw-r--r--   0 runner    (1001) docker     (121)    18252 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/start.py
--rw-r--r--   0 runner    (1001) docker     (121)    27258 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/viewer_display.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 11:29:58.723932 picframe-2022.6.3/picframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-06-03 11:29:58.723932 picframe-2022.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-06-03 11:29:47.000000 picframe-2022.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 11:29:58.723932 picframe-2022.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 11:29:47.000000 picframe-2022.6.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4341 2022-06-03 11:29:47.000000 picframe-2022.6.3/test/test_get_image_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.030278 picframe-2023.5.17/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 08:43:19.000000 picframe-2023.5.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-17 08:43:42.030278 picframe-2023.5.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-17 08:43:19.000000 picframe-2023.5.17/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-17 08:43:19.000000 picframe-2023.5.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-17 08:43:42.030278 picframe-2023.5.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-17 08:43:19.000000 picframe-2023.5.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.018278 picframe-2023.5.17/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.030278 picframe-2023.5.17/src/picframe/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-17 08:43:42.030278 picframe-2023.5.17/src/picframe/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.026278 picframe-2023.5.17/src/picframe/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/config/configuration_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.026278 picframe-2023.5.17/src/picframe/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.026278 picframe-2023.5.17/src/picframe/data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/fonts/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   455164 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/fonts/NotoSans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   471004 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/fonts/NotoSans-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   470472 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/fonts/NotoSans-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   455188 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/fonts/NotoSans-Regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.030278 picframe-2023.5.17/src/picframe/data/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/mat/9_patch_bevel.png
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/mat/9_patch_drop_shadow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/mat/9_patch_highlight.png
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/mat/9_patch_inner_shadow.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2081776 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/mat/mat_texture.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   160442 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/no_pictures.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.030278 picframe-2023.5.17/src/picframe/data/shaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/shaders/blend_new.fs
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/shaders/blend_new.vs
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/geo_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/get_image_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.030278 picframe-2023.5.17/src/picframe/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/html/pf_functions.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24184 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/interface_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23963 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/interface_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/interface_peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/mat_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27228 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/viewer_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.026278 picframe-2023.5.17/src/picframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-17 08:43:42.000000 picframe-2023.5.17/src/picframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-17 08:43:42.000000 picframe-2023.5.17/src/picframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 08:43:42.000000 picframe-2023.5.17/src/picframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 08:43:42.000000 picframe-2023.5.17/src/picframe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 08:43:42.000000 picframe-2023.5.17/src/picframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 08:43:42.000000 picframe-2023.5.17/src/picframe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.030278 picframe-2023.5.17/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-17 08:43:19.000000 picframe-2023.5.17/test/test_get_image_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-17 08:43:19.000000 picframe-2023.5.17/versioneer.py
```

### Comparing `picframe-2022.6.3/LICENSE` & `picframe-2023.5.17/LICENSE`

 * *Files identical despite different names*

### Comparing `picframe-2022.6.3/PKG-INFO` & `picframe-2023.5.17/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: picframe
-Version: 2022.6.3
+Version: 2023.5.17
 Summary: Picture frame viewer powered by raspberry with homeassistant integration
-Home-page: https://github.com/helgeerbe/picframe
-Author: Paddy Gaunt, Jeff Godfrey, Helge Erbe
-Author-email: helge@erbehome.de
+Author: Paddy Gaunt, Jeff Godfrey
+Author-email: Helge Erbe <helge@erbehome.de>
+Maintainer-email: Helge Erbe <helge@erbehome.de>
 License: MIT
-Keywords: picframe viewer raspberry raspi homeassistant hass
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/helgeerbe/picframe
+Keywords: picframe,viewer,raspberry,raspi,homeassistant,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PictureFrame powered by pi3d
 
 ![picframe logo](https://github.com/helgeerbe/picframe/wiki/images/Picframe_Logo.png)
 
+- [![PyPI version](https://badge.fury.io/py/picframe.svg)](https://badge.fury.io/py/picframe)
 - [PictureFrame powered by pi3d](#pictureframe-powered-by-pi3d)
 - [What Is PictureFrame?](#what-is-pictureframe)
 - [History of PictureFrame](#history-of-pictureframe)
 - [Highlights of PictureFrame](#highlights-of-pictureframe)
 - [Documentation](#documentation)
 - [Acknowledgement](#acknowledgement)
 
@@ -77,9 +84,7 @@
 [glenvorel](https://github.com/glenvorel) Thanks for the new keyboard, mouse and touch screen support.
 
 Many Thanks to Wolfgang [www.thedigitalpictureframe.com](https://www.thedigitalpictureframe.com/) for your inspiring work. 
 
 A special Thank to Paddy Gaunt one of the authors of the [pi3d](https://github.com/pi3d/pi3d_demos) project. You are doing a great job!
 
 Last but no least a big Thank You to Jeff Godfrey. Your auto mat feature and database driven cache is an outstanding piece of code.
-
-
```

### Comparing `picframe-2022.6.3/README.md` & `picframe-2023.5.17/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ## PictureFrame powered by pi3d
 
 ![picframe logo](https://github.com/helgeerbe/picframe/wiki/images/Picframe_Logo.png)
 
+- [![PyPI version](https://badge.fury.io/py/picframe.svg)](https://badge.fury.io/py/picframe)
 - [PictureFrame powered by pi3d](#pictureframe-powered-by-pi3d)
 - [What Is PictureFrame?](#what-is-pictureframe)
 - [History of PictureFrame](#history-of-pictureframe)
 - [Highlights of PictureFrame](#highlights-of-pictureframe)
 - [Documentation](#documentation)
 - [Acknowledgement](#acknowledgement)
```

### Comparing `picframe-2022.6.3/picframe/controller.py` & `picframe-2023.5.17/src/picframe/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """Controller of picframe."""
 
 import logging
 import time
-import json
-import os
 import signal
 import sys
-from picframe.interface_peripherals import InterfacePeripherals
+import ssl
+
 
 def make_date(txt):
-    dt = txt.replace('/',':').replace('-',':').replace(',',':').replace('.',':').split(':')
-    dt_tuple = tuple(int(i) for i in dt) #TODO catch badly formed dates?
+    dt = (txt.replace('/', ':')
+          .replace('-', ':')
+          .replace(',', ':')
+          .replace('.', ':')
+          .split(':'))
+    dt_tuple = tuple(int(i) for i in dt)  # TODO catch badly formed dates?
     return time.mktime(dt_tuple + (0, 0, 0, 0, 0, 0))
 
+
 class Controller:
     """Controller of picframe.
 
-    This controller interacts via mqtt with the user to steer the image display.
+    This controller interacts via mqtt with the user to steer the image
+    display.
 
     Attributes
     ----------
     model : Model
         model of picframe containing config and business logic
     viewer : ViewerDisplay
         viewer of picframe representing the display
@@ -38,61 +43,66 @@
     """
 
     def __init__(self, model, viewer):
         self.__logger = logging.getLogger("controller.Controller")
         self.__logger.info('creating an instance of Controller')
         self.__model = model
         self.__viewer = viewer
+        self.__http_config = self.__model.get_http_config()
+        self.__mqtt_config = self.__model.get_mqtt_config()
         self.__paused = False
         self.__force_navigate = False
         self.__next_tm = 0
-        self.__date_from = make_date('1901/12/15') # TODO This seems to be the minimum date to be handled by date functions
+        self.__date_from = make_date('1901/12/15')  # TODO This seems to be the minimum date to be handled by date functions  # noqa: E501
         self.__date_to = make_date('2038/1/1')
         self.__location_filter = ""
         self.__where_clauses = {}
         self.__sort_clause = "exif_datetime ASC"
         self.publish_state = lambda x, y: None
         self.keep_looping = True
         self.__location_filter = ''
         self.__tags_filter = ''
         self.__interface_peripherals = None
-        self.__shutdown_complete = False
+        self.__interface_mqtt = None
+        self.__interface_http = None
 
     @property
     def paused(self):
-        """Get or set the current state for pausing image display. Setting paused to true
-        will show the actual image as long paused is not set to false.
+        """Get or set the current state for pausing image display.
+        Setting paused to true will show the actual image as long
+        paused is not set to false.
         """
         return self.__paused
 
     @paused.setter
-    def paused(self, val:bool):
+    def paused(self, val: bool):
         self.__paused = val
-        pic = self.__model.get_current_pics()[0] # only refresh left text
+        pic = self.__model.get_current_pics()[0]  # only refresh left text
         self.__viewer.reset_name_tm(pic, val, side=0, pair=self.__model.get_current_pics()[1] is not None)
-        self.publish_state()
+        if self.__mqtt_config['use_mqtt']:
+            self.publish_state()
 
     def next(self):
         self.__next_tm = 0
         self.__viewer.reset_name_tm()
         self.__force_navigate = True
 
     def back(self):
         self.__model.set_next_file_to_previous_file()
         self.__next_tm = 0
         self.__viewer.reset_name_tm()
         self.__force_navigate = True
 
     def delete(self):
         self.__model.delete_file()
-        self.next() # TODO check needed to avoid skipping one as record has been deleted from model.__file_list
+        self.next()  # TODO check needed to avoid skipping one as record has been deleted from model.__file_list
         self.__next_tm = 0
 
     def set_show_text(self, txt_key=None, val="ON"):
-        if val is True: # allow to be called with boolean from httpserver
+        if val is True:  # allow to be called with boolean from httpserver
             val = "ON"
         self.__viewer.set_show_text(txt_key, val)
         for (side, pic) in enumerate(self.__model.get_current_pics()):
             if pic is not None:
                 self.__viewer.reset_name_tm(pic, self.paused, side, self.__model.get_current_pics()[1] is not None)
 
     def refresh_show_text(self):
@@ -122,15 +132,16 @@
         try:
             self.__date_from = float(val)
         except ValueError:
             self.__date_from = make_date(val if len(val) > 0 else '1901/12/15')
         if len(val) > 0:
             self.__model.set_where_clause('date_from', "exif_datetime > {:.0f}".format(self.__date_from))
         else:
-            self.__model.set_where_clause('date_from') # remove from where_clause
+            # remove from where_clause
+            self.__model.set_where_clause('date_from')
         self.__model.force_reload()
         self.__next_tm = 0
 
     @property
     def date_to(self):
         return self.__date_to
 
@@ -139,46 +150,48 @@
         try:
             self.__date_to = float(val)
         except ValueError:
             self.__date_to = make_date(val if len(val) > 0 else '2038/1/1')
         if len(val) > 0:
             self.__model.set_where_clause('date_to', "exif_datetime < {:.0f}".format(self.__date_to))
         else:
-            self.__model.set_where_clause('date_to') # remove from where_clause
+            self.__model.set_where_clause('date_to')  # remove from where_clause
         self.__model.force_reload()
         self.__next_tm = 0
 
     @property
     def display_is_on(self):
         return self.__viewer.display_is_on
 
     @display_is_on.setter
     def display_is_on(self, on_off):
         self.paused = not on_off
         self.__viewer.display_is_on = on_off
-        self.publish_state()
+        if self.__mqtt_config['use_mqtt']:
+            self.publish_state()
 
     @property
     def clock_is_on(self):
         return self.__viewer.clock_is_on
 
     @clock_is_on.setter
     def clock_is_on(self, on_off):
         self.__viewer.clock_is_on = on_off
 
     @property
     def shuffle(self):
         return self.__model.shuffle
 
     @shuffle.setter
-    def shuffle(self, val:bool):
+    def shuffle(self, val: bool):
         self.__model.shuffle = val
         self.__model.force_reload()
         self.__next_tm = 0
-        self.publish_state()
+        if self.__mqtt_config['use_mqtt']:
+            self.publish_state()
 
     @property
     def fade_time(self):
         return self.__model.fade_time
 
     @fade_time.setter
     def fade_time(self, time):
@@ -187,29 +200,30 @@
 
     @property
     def time_delay(self):
         return self.__model.time_delay
 
     @time_delay.setter
     def time_delay(self, time):
-        time = float(time) # convert string before comparison
+        time = float(time)  # convert string before comparison
         # might break it if too quick
         if time < 5.0:
             time = 5.0
         self.__model.time_delay = time
         self.__next_tm = 0
 
     @property
     def brightness(self):
         return self.__viewer.get_brightness()
 
     @brightness.setter
     def brightness(self, val):
         self.__viewer.set_brightness(float(val))
-        self.publish_state()
+        if self.__mqtt_config['use_mqtt']:
+            self.publish_state()
 
     @property
     def matting_images(self):
         return self.__viewer.get_matting_images()
 
     @matting_images.setter
     def matting_images(self, val):
@@ -222,55 +236,55 @@
 
     @location_filter.setter
     def location_filter(self, val):
         self.__location_filter = val
         if len(val) > 0:
             self.__model.set_where_clause("location_filter", self.__build_filter(val, "location"))
         else:
-            self.__model.set_where_clause("location_filter") # remove from where_clause
+            self.__model.set_where_clause("location_filter")  # remove from where_clause
         self.__model.force_reload()
         self.__next_tm = 0
 
     @property
     def tags_filter(self):
         return self.__tags_filter
 
     @tags_filter.setter
     def tags_filter(self, val):
         self.__tags_filter = val
         if len(val) > 0:
             self.__model.set_where_clause("tags_filter", self.__build_filter(val, "tags"))
         else:
-            self.__model.set_where_clause("tags_filter") # remove from where_clause
+            self.__model.set_where_clause("tags_filter")  # remove from where_clause
         self.__model.force_reload()
         self.__next_tm = 0
 
     def __build_filter(self, val, field):
         if val.count("(") != val.count(")"):
-            return None # this should clear the filter and not raise an error
-        val = val.replace(";", "").replace("'", "").replace("%", "").replace('"', '') # SQL scrambling
-        tokens = ("(", ")", "AND", "OR", "NOT") # now copes with NOT
-        val_split = val.replace("(", " ( ").replace(")", " ) ").split() # so brackets not joined to words
+            return None  # this should clear the filter and not raise an error
+        val = val.replace(";", "").replace("'", "").replace("%", "").replace('"', '')  # SQL scrambling
+        tokens = ("(", ")", "AND", "OR", "NOT")  # now copes with NOT
+        val_split = val.replace("(", " ( ").replace(")", " ) ").split()  # so brackets not joined to words
         filter = []
         last_token = ""
         for s in val_split:
             s_upper = s.upper()
             if s_upper in tokens:
                 if s_upper in ("AND", "OR"):
                     if last_token in ("AND", "OR"):
-                        return None # must have a non-token between
+                        return None  # must have a non-token between
                     last_token = s_upper
                 filter.append(s)
             else:
                 if last_token is not None:
                     filter.append("{} LIKE '%{}%'".format(field, s))
                 else:
                     filter[-1] = filter[-1].replace("%'", " {}%'".format(s))
                 last_token = None
-        return "({})".format(" ".join(filter)) # if OR outside brackets will modify the logic of rest of where clauses
+        return "({})".format(" ".join(filter))  # if OR outside brackets will modify the logic of rest of where clauses
 
     def text_is_on(self, txt_key):
         return self.__viewer.text_is_on(txt_key)
 
     def get_number_of_files(self):
         return self.__model.get_number_of_files()
 
@@ -278,67 +292,89 @@
         actual_dir, dir_list = self.__model.get_directory_list()
         return actual_dir, dir_list
 
     def get_current_path(self):
         (pic, _) = self.__model.get_current_pics()
         return pic.fname
 
-    def loop(self): #TODO exit loop gracefully and call image_cache.stop()
+    def loop(self):  # TODO exit loop gracefully and call image_cache.stop()
         # catch ctrl-c
         signal.signal(signal.SIGINT, self.__signal_handler)
 
-        #next_check_tm = time.time() + self.__model.get_model_config()['check_dir_tm']
         while self.keep_looping:
-
-            #if self.__next_tm == 0: #TODO double check why these were set when next_tm == 0
-            #    time_delay = 1 # must not be 0
-            #    fade_time = 1 # must not be 0
-            #else:
             time_delay = self.__model.time_delay
             fade_time = self.__model.fade_time
 
             tm = time.time()
-            pics = None #get_next_file returns a tuple of two in case paired portraits have been specified
+            pics = None  # get_next_file returns a tuple of two in case paired portraits have been specified
             if not self.paused and tm > self.__next_tm or self.__force_navigate:
                 self.__next_tm = tm + self.__model.time_delay
                 self.__force_navigate = False
                 pics = self.__model.get_next_file()
                 if pics[0] is None:
-                    self.__next_tm = 0 # skip this image file moved or otherwise not on db
-                    pics = None # signal slideshow_is_running not to load new image
+                    self.__next_tm = 0  # skip this image file moved or otherwise not on db
+                    pics = None  # signal slideshow_is_running not to load new image
                 else:
                     image_attr = {}
                     for key in self.__model.get_model_config()['image_attr']:
                         if key == 'PICFRAME GPS':
                             image_attr['latitude'] = pics[0].latitude
                             image_attr['longitude'] = pics[0].longitude
                         elif key == 'PICFRAME LOCATION':
                             image_attr['location'] = pics[0].location
                         else:
                             field_name = self.__model.EXIF_TO_FIELD[key]
-                            image_attr[key] = pics[0].__dict__[field_name] #TODO nicer using namedtuple for Pic
-                    self.publish_state(pics[0].fname, image_attr)
+                            image_attr[key] = pics[0].__dict__[field_name]  # TODO nicer using namedtuple for Pic
+                    if self.__mqtt_config['use_mqtt']:
+                        self.publish_state(pics[0].fname, image_attr)
             self.__model.pause_looping = self.__viewer.is_in_transition()
             (loop_running, skip_image) = self.__viewer.slideshow_is_running(pics, time_delay, fade_time, self.__paused)
             if not loop_running:
                 break
             if skip_image:
                 self.__next_tm = 0
             self.__interface_peripherals.check_input()
-        self.__shutdown_complete = True
 
     def start(self):
         self.__viewer.slideshow_start()
+        from picframe.interface_peripherals import InterfacePeripherals
         self.__interface_peripherals = InterfacePeripherals(self.__model, self.__viewer, self)
 
+        # start mqtt
+        if self.__mqtt_config['use_mqtt']:
+            from picframe import interface_mqtt
+            try:
+                self.__interface_mqtt = interface_mqtt.InterfaceMQTT(self, self.__mqtt_config)
+                self.__interface_mqtt.start()
+            except Exception:
+                self.__logger.error("Can't initialize mqtt. Stopping picframe")
+                sys.exit(1)
+
+        # start http server
+        if self.__http_config['use_http']:
+            from picframe import interface_http
+            model_config = self.__model.get_model_config()
+            self.__interface_http = interface_http.InterfaceHttp(self,
+                                                                 self.__http_config['path'],
+                                                                 model_config['pic_dir'],
+                                                                 model_config['no_files_img'],
+                                                                 self.__http_config['port'])  # TODO: Implement TLS
+            if self.__http_config['use_ssl']:
+                self.__interface_http.socket = ssl.wrap_socket(
+                                                self.__interface_http.socket,
+                                                keyfile=self.__http_config['keyfile'],
+                                                certfile=self.__http_config['certfile'],
+                                                server_side=True)
+
     def stop(self):
         self.keep_looping = False
         self.__interface_peripherals.stop()
-        while not self.__shutdown_complete:
-            time.sleep(0.05) # block until main loop has stopped
-        self.__model.stop_image_chache() # close db tidily (blocks till closed)
-        self.__viewer.slideshow_stop() # do this last
+        if self.__interface_mqtt:
+            self.__interface_mqtt.stop()
+        if self.__interface_http:
+            self.__interface_http.stop()
+        self.__model.stop_image_chache()  # close db tidily (blocks till closed)
+        self.__viewer.slideshow_stop()  # do this last
 
     def __signal_handler(self, sig, frame):
         print('You pressed Ctrl-c!')
-        self.__shutdown_complete = True
-        self.stop()
+        self.keep_looping = False
```

### Comparing `picframe-2022.6.3/picframe/geo_reverse.py` & `picframe-2023.5.17/src/picframe/geo_reverse.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,37 @@
-import os
 import json
 import urllib.request
 import locale
 import logging
-import time
 
 URL = "https://nominatim.openstreetmap.org/reverse?format=geojson&lat={}&lon={}&zoom={}&email={}&accept-language={}"
 
+
 class GeoReverse:
     def __init__(self, geo_key, zoom=18, key_list=None):
         self.__logger = logging.getLogger("geo_reverse.GeoReverse")
         self.__geo_key = geo_key
         self.__zoom = zoom
         self.__key_list = key_list
-        #self.__file_path = os.path.expanduser(file_path)
         self.__geo_locations = {}
-        #if os.path.isfile(file_path):
-        #    with open(file_path) as f:
-        #        for line in f:
-        #            if line == '\n':
-        #                continue
-        #            (name, var) = line.partition('=')[::2]
-        #            self.__geo_locations[name] = var.rstrip('\n')
         self.__language = locale.getlocale()[0][:2]
 
     def get_address(self, lat, lon):
         try:
             with urllib.request.urlopen(URL.format(lat, lon, self.__zoom, self.__geo_key, self.__language),
                                         timeout=3.0) as req:
-                    data = json.loads(req.read().decode())
+                data = json.loads(req.read().decode())
             adr = data['features'][0]['properties']['address']
             # some experimentation might be needed to get a good set of alternatives in key_list
             adr_list = []
             if self.__key_list is not None:
                 for part in self.__key_list:
                     for option in part:
                         if option in adr:
                             adr_list.append(adr[option])
-                            break # add just the first one from the options
+                            break  # add just the first one from the options
             else:
                 adr_list = adr.values()
             return ", ".join(adr_list)
-        except Exception as e: #TODO return different thing for different exceptions
+        except Exception as e:  # TODO return different thing for different exceptions
             self.__logger.error("lat=%f, lon=%f -> %s", lat, lon, e)
             return ""
```

### Comparing `picframe-2022.6.3/picframe/image_cache.py` & `picframe-2023.5.17/src/picframe/image_cache.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,92 +1,86 @@
 import sqlite3
 import os
 import time
 import logging
 import threading
 from picframe import get_image_meta
 
+
 class ImageCache:
 
-    EXTENSIONS = ['.png','.jpg','.jpeg','.heif','.heic']
+    EXTENSIONS = ['.png', '.jpg', '.jpeg', '.heif', '.heic']
     EXIF_TO_FIELD = {'EXIF FNumber': 'f_number',
                      'Image Make': 'make',
                      'Image Model': 'model',
                      'EXIF ExposureTime': 'exposure_time',
                      'EXIF ISOSpeedRatings': 'iso',
                      'EXIF FocalLength': 'focal_length',
                      'EXIF Rating': 'rating',
                      'EXIF LensModel': 'lens',
                      'EXIF DateTimeOriginal': 'exif_datetime',
                      'IPTC Keywords': 'tags',
                      'IPTC Caption/Abstract': 'caption',
                      'IPTC Object Name': 'title'}
 
-
     def __init__(self, picture_dir, follow_links, db_file, geo_reverse, portrait_pairs=False):
         # TODO these class methods will crash if Model attempts to instantiate this using a
         # different version from the latest one - should this argument be taken out?
         self.__modified_folders = []
         self.__modified_files = []
-        self.__cached_file_stats = [] # collection shared between threads
-        self.__cached_file_stats_lock = threading.Lock() # lock to manage shared collection
+        self.__cached_file_stats = []  # collection shared between threads
         self.__logger = logging.getLogger("image_cache.ImageCache")
         self.__logger.debug('Creating an instance of ImageCache')
         self.__picture_dir = picture_dir
         self.__follow_links = follow_links
         self.__db_file = db_file
         self.__geo_reverse = geo_reverse
-        self.__portrait_pairs = portrait_pairs #TODO have a function to turn this on and off?
+        self.__portrait_pairs = portrait_pairs  # TODO have a function to turn this on and off?
         self.__db = self.__create_open_db(self.__db_file)
+        self.__db_write_lock = threading.Lock()  # lock to serialize db writes between threads
         # NB this is where the required schema is set
         self.__update_schema(3)
 
         self.__keep_looping = True
         self.__pause_looping = False
         self.__shutdown_completed = False
         self.__purge_files = False
 
         t = threading.Thread(target=self.__loop)
         t.start()
 
-
     def __loop(self):
         while self.__keep_looping:
             if not self.__pause_looping:
                 self.update_cache()
                 time.sleep(2.0)
             time.sleep(0.01)
-        self.__update_file_stats() # write any unsaved file stats before closing
-        self.__db.commit() # close after update_cache finished for last time
+        self.__db_write_lock.acquire()
+        self.__db.commit()  # close after update_cache finished for last time
+        self.__db_write_lock.release()
         self.__db.close()
         self.__shutdown_completed = True
 
-
     def pause_looping(self, value):
         self.__pause_looping = value
 
-
     def stop(self):
         self.__keep_looping = False
         while not self.__shutdown_completed:
-            time.sleep(0.05) # make function blocking to ensure staged shutdown
+            time.sleep(0.05)  # make function blocking to ensure staged shutdown
 
     def purge_files(self):
         self.__purge_files = True
 
     def update_cache(self):
         """Update the cache database with new and/or modified files
         """
 
         self.__logger.debug('Updating cache')
 
-        # Update any cached file stats. This should be really light-weight
-        # so just process any new stats in every pass...
-        self.__update_file_stats()
-
         # If the current collection of updated files is empty, check for disk-based changes
         if not self.__modified_files:
             self.__logger.debug('No unprocessed files in memory, checking disk')
             self.__modified_folders = self.__get_modified_folders()
             self.__modified_files = self.__get_modified_files(self.__modified_folders)
             self.__logger.debug('Found %d new files on disk', len(self.__modified_files))
 
@@ -102,26 +96,27 @@
             self.__modified_folders.clear()
 
         # If looping is still not paused, remove any files or folders from the db that are no longer on disk
         if not self.__pause_looping:
             self.__purge_missing_files_and_folders()
 
         # Commit the current set of changes
+        self.__db_write_lock.acquire()
         self.__db.commit()
+        self.__db_write_lock.release()
 
-
-    def query_cache(self, where_clause, sort_clause = 'fname ASC'):
+    def query_cache(self, where_clause, sort_clause='fname ASC'):
         cursor = self.__db.cursor()
-        cursor.row_factory = None # we don't want the "sqlite3.Row" setting from the db here...
+        cursor.row_factory = None  # we don't want the "sqlite3.Row" setting from the db here...
         try:
-            if not self.__portrait_pairs: # TODO SQL insertion? Does it matter in this app?
+            if not self.__portrait_pairs:  # TODO SQL insertion? Does it matter in this app?
                 sql = """SELECT file_id FROM all_data WHERE {0} ORDER BY {1}
                     """.format(where_clause, sort_clause)
                 return cursor.execute(sql).fetchall()
-            else: # make two SELECTS
+            else:  # make two SELECTS
                 sql = """SELECT
                             CASE
                                 WHEN is_portrait = 0 THEN file_id
                                 ELSE -1
                             END
                             FROM all_data WHERE {0} ORDER BY {1}
                                         """.format(where_clause, sort_clause)
@@ -143,67 +138,66 @@
                         if pair_list:
                             elem += pair_list.pop(0)
                             # Here, we just doubled-up a set of portrait images.
                             # Skip the next available "portrait slot" as it's unneeded.
                             skip_portrait_slot = True
                         newlist.append(elem)
                 return newlist
-        except:
+        except Exception:
             return []
 
-
     def get_file_info(self, file_id):
-        if not file_id: return None
+        if not file_id:
+            return None
         sql = "SELECT * FROM all_data where file_id = {0}".format(file_id)
         row = self.__db.execute(sql).fetchone()
         try:
-            if row is not None and row['last_modified']  != os.path.getmtime(row['fname']):
+            if row is not None and row['last_modified'] != os.path.getmtime(row['fname']):
                 self.__logger.debug('Cache miss: File %s changed on disk', row['fname'])
                 self.__insert_file(row['fname'], file_id)
-                row = self.__db.execute(sql).fetchone() # description inserted in table
+                row = self.__db.execute(sql).fetchone()  # description inserted in table
         except OSError:
-            self.__logger.warning("Image '%s' does not exists or is inaccessible" %row['fname'])
+            self.__logger.warning("Image '%s' does not exists or is inaccessible", row['fname'])
         if row is not None and row['latitude'] is not None and row['longitude'] is not None and row['location'] is None:
             if self.__get_geo_location(row['latitude'], row['longitude']):
-                row = self.__db.execute(sql).fetchone() # description inserted in table
-        self.__add_file_to_stats_cache(file_id) # Add a record to the file stats cache collection
-        return row # NB if select fails (i.e. moved file) will return None
+                row = self.__db.execute(sql).fetchone()  # description inserted in table
+        sql = "UPDATE file SET displayed_count = displayed_count + 1, last_displayed = ? WHERE file_id = ?"
+        starttime = round(time.time() * 1000)
+        self.__db_write_lock.acquire()
+        waittime = round(time.time() * 1000)
+        self.__db.execute(sql, (time.time(), file_id))  # Add file stats
+        self.__db_write_lock.release()
+        now = round(time.time() * 1000)
+        self.__logger.debug(
+            'Update file stats: Wait for %d ms and need %d ms for update ',
+            waittime - starttime, now - waittime)
+        return row  # NB if select fails (i.e. moved file) will return None
 
     def get_column_names(self):
         sql = "PRAGMA table_info(all_data)"
         rows = self.__db.execute(sql).fetchall()
         return [row['name'] for row in rows]
 
-    def __add_file_to_stats_cache(self, file_id):
-        # This collection is shared between threads, so lock it to update
-        self.__cached_file_stats_lock.acquire()
-        self.__cached_file_stats.append([file_id, time.time()])
-        self.__cached_file_stats_lock.release()
-
-    def __update_file_stats(self):
-        # Process (and drain) the entire collection of cached file stats by storing them in the db
-        # Note, this is likely an empty or very small collection
-        if self.__cached_file_stats:
-            sql = "UPDATE file SET displayed_count = displayed_count + 1, last_displayed = ? WHERE file_id = ?"
-            self.__cached_file_stats_lock.acquire()
-            while self.__cached_file_stats:
-                file_id, timestamp = self.__cached_file_stats.pop()
-                self.__db.execute(sql, (timestamp, file_id))
-            self.__cached_file_stats_lock.release()
-
-    def __get_geo_location(self, lat, lon): # TODO periodically check all lat/lon in meta with no location and try again
+    def __get_geo_location(self, lat, lon):  # TODO periodically check all lat/lon in meta with no location and try again # noqa: E501
         location = self.__geo_reverse.get_address(lat, lon)
         if len(location) == 0:
-            return False #TODO this will continue to try even if there is some permanant cause
+            return False  # TODO this will continue to try even if there is some permanant cause
         else:
             sql = "INSERT OR REPLACE INTO location (latitude, longitude, description) VALUES (?, ?, ?)"
+            starttime = round(time.time() * 1000)
+            self.__db_write_lock.acquire()
+            waittime = round(time.time() * 1000)
             self.__db.execute(sql, (lat, lon, location))
+            self.__db_write_lock.release()
+            now = round(time.time() * 1000)
+            self.__logger.debug(
+                'Update location: Wait for db %d ms and need %d ms for update ',
+                waittime - starttime, now - waittime)
             return True
 
-
     def __create_open_db(self, db_file):
         sql_folder_table = """
             CREATE TABLE IF NOT EXISTS folder (
                 folder_id INTEGER NOT NULL PRIMARY KEY,
                 name TEXT UNIQUE NOT NULL,
                 last_modified REAL DEFAULT 0 NOT NULL
             )"""
@@ -292,23 +286,22 @@
             CREATE TRIGGER IF NOT EXISTS Clean_Meta_Trigger
             AFTER DELETE ON file
             FOR EACH ROW
             BEGIN
                 DELETE FROM meta WHERE file_id = OLD.file_id;
             END"""
 
-        db = sqlite3.connect(db_file, check_same_thread=False) # writing only done in loop thread, reading in this so should be safe
-        db.row_factory = sqlite3.Row # make results accessible by field name
+        db = sqlite3.connect(db_file, check_same_thread=False)
+        db.row_factory = sqlite3.Row  # make results accessible by field name
         for item in (sql_folder_table, sql_file_table, sql_meta_table, sql_location_table, sql_meta_index,
-                    sql_all_data_view, sql_db_info_table, sql_clean_file_trigger, sql_clean_meta_trigger):
+                     sql_all_data_view, sql_db_info_table, sql_clean_file_trigger, sql_clean_meta_trigger):
             db.execute(item)
 
         return db
 
-
     def __update_schema(self, required_db_schema_version):
         sql_select = "SELECT schema_version from db_info"
         schema_version = self.__db.execute(sql_select).fetchone()
         schema_version = 1 if not schema_version else schema_version[0]
 
         # DB is newer than the application. The User needs to upgrade...
         if schema_version > required_db_schema_version:
@@ -359,167 +352,167 @@
     #     - Found on disk, but newer than the associated record in the 'folder' table
     #     - Found on disk, but flagged as 'missing' in the 'folder' table
     # --- Note that all folders returned currently exist on disk
     def __get_modified_folders(self):
         out_of_date_folders = []
         sql_select = "SELECT * FROM folder WHERE name = ?"
         for dir in [d[0] for d in os.walk(self.__picture_dir, followlinks=self.__follow_links)]:
-            if os.path.basename(dir)[0] == '.': continue # ignore hidden folders
+            if os.path.basename(dir)[0] == '.':
+                continue  # ignore hidden folders
             mod_tm = int(os.stat(dir).st_mtime)
             found = self.__db.execute(sql_select, (dir,)).fetchone()
             if not found or found['last_modified'] < mod_tm or found['missing'] == 1:
                 out_of_date_folders.append((dir, mod_tm))
         return out_of_date_folders
 
-
     def __get_modified_files(self, modified_folders):
         out_of_date_files = []
-        #sql_select = "SELECT fname, last_modified FROM all_data WHERE fname = ? and last_modified >= ?"
+        # sql_select = "SELECT fname, last_modified FROM all_data WHERE fname = ? and last_modified >= ?"
         sql_select = """
         SELECT file.basename, file.last_modified
             FROM file
                 INNER JOIN folder
                     ON folder.folder_id = file.folder_id
             WHERE file.basename = ? AND file.extension = ? AND folder.name = ? AND file.last_modified >= ?
         """
-        for dir,_date in modified_folders:
+        for dir, _date in modified_folders:
             for file in os.listdir(dir):
                 base, extension = os.path.splitext(file)
                 if (extension.lower() in ImageCache.EXTENSIONS
-                        and not '.AppleDouble' in dir and not file.startswith('.')): # have to filter out all the Apple junk
+                        # have to filter out all the Apple junk
+                        and '.AppleDouble' not in dir and not file.startswith('.')):
                     full_file = os.path.join(dir, file)
-                    mod_tm =  os.path.getmtime(full_file)
+                    mod_tm = os.path.getmtime(full_file)
                     found = self.__db.execute(sql_select, (base, extension.lstrip("."), dir, mod_tm)).fetchone()
                     if not found:
                         out_of_date_files.append(full_file)
         return out_of_date_files
 
-
-    def __insert_file(self, file, file_id = None):
-        file_insert = "INSERT OR REPLACE INTO file(folder_id, basename, extension, last_modified) VALUES((SELECT folder_id from folder where name = ?), ?, ?, ?)"
-        file_update = "UPDATE file SET folder_id = (SELECT folder_id from folder where name = ?), basename = ?, extension = ?, last_modified = ? WHERE file_id = ?"
+    def __insert_file(self, file, file_id=None):
+        file_insert = "INSERT OR REPLACE INTO file(folder_id, basename, extension, last_modified) VALUES((SELECT folder_id from folder where name = ?), ?, ?, ?)"  # noqa: E501
+        file_update = "UPDATE file SET folder_id = (SELECT folder_id from folder where name = ?), basename = ?, extension = ?, last_modified = ? WHERE file_id = ?"  # noqa: E501
         # Insert the new folder if it's not already in the table. Update the missing field separately.
         folder_insert = "INSERT OR IGNORE INTO folder(name) VALUES(?)"
         folder_update = "UPDATE folder SET missing = 0 where name = ?"
 
-        mod_tm =  os.path.getmtime(file)
+        mod_tm = os.path.getmtime(file)
         dir, file_only = os.path.split(file)
         base, extension = os.path.splitext(file_only)
 
         # Get the file's meta info and build the INSERT statement dynamically
         meta = self.__get_exif_info(file)
         meta_insert = self.__get_meta_sql_from_dict(meta)
         vals = list(meta.values())
         vals.insert(0, file)
 
         # Insert this file's info into the folder, file, and meta tables
+        self.__db_write_lock.acquire()
         self.__db.execute(folder_insert, (dir,))
         self.__db.execute(folder_update, (dir,))
         if file_id is None:
             self.__db.execute(file_insert, (dir, base, extension.lstrip("."), mod_tm))
         else:
             self.__db.execute(file_update, (dir, base, extension.lstrip("."), mod_tm, file_id))
         self.__db.execute(meta_insert, vals)
-
+        self.__db_write_lock.release()
 
     def __update_folder_info(self, folder_collection):
         update_data = []
         sql = "UPDATE folder SET last_modified = ?, missing = 0 WHERE name = ?"
         for folder, modtime in folder_collection:
             update_data.append((modtime, folder))
+        self.__db_write_lock.acquire()
         self.__db.executemany(sql, update_data)
-
+        self.__db_write_lock.release()
 
     def __get_meta_sql_from_dict(self, dict):
         columns = ', '.join(dict.keys())
         ques = ', '.join('?' * len(dict.keys()))
-        return 'INSERT OR REPLACE INTO meta(file_id, {0}) VALUES((SELECT file_id from all_data where fname = ?), {1})'.format(columns, ques)
-
+        return 'INSERT OR REPLACE INTO meta(file_id, {0}) VALUES((SELECT file_id from all_data where fname = ?), {1})'.format(columns, ques)  # noqa: E501
 
     def __purge_missing_files_and_folders(self):
         # Find folders in the db that are no longer on disk
         folder_id_list = []
         for row in self.__db.execute('SELECT folder_id, name from folder'):
             if not os.path.exists(row['name']):
                 folder_id_list.append([row['folder_id']])
 
         # Flag or delete any non-existent folders from the db. Note, deleting will automatically
         # remove orphaned records from the 'file' and 'meta' tables
         if len(folder_id_list):
+            self.__db_write_lock.acquire()
             if self.__purge_files:
                 self.__db.executemany('DELETE FROM folder WHERE folder_id = ?', folder_id_list)
             else:
                 self.__db.executemany('UPDATE folder SET missing = 1 WHERE folder_id = ?', folder_id_list)
+            self.__db_write_lock.release()
 
         # Find files in the db that are no longer on disk
         if self.__purge_files:
             file_id_list = []
             for row in self.__db.execute('SELECT file_id, fname from all_data'):
                 if not os.path.exists(row['fname']):
                     file_id_list.append([row['file_id']])
 
             # Delete any non-existent files from the db. Note, this will automatically
             # remove matching records from the 'meta' table as well.
             if len(file_id_list):
+                self.__db_write_lock.acquire()
                 self.__db.executemany('DELETE FROM file WHERE file_id = ?', file_id_list)
+                self.__db_write_lock.release()
             self.__purge_files = False
 
     def __get_exif_info(self, file_path_name):
         exifs = get_image_meta.GetImageMeta(file_path_name)
         # Dict to store interesting EXIF data
         # Note, the 'key' must match a field in the 'meta' table
         e = {}
 
         e['orientation'] = exifs.get_orientation()
 
         width, height = exifs.get_size()
         ext = os.path.splitext(file_path_name)[1].lower()
-        if ext not in ('.heif','.heic') and e['orientation'] in (5, 6, 7, 8):
-            width, height = height, width # swap values
+        if ext not in ('.heif', '.heic') and e['orientation'] in (5, 6, 7, 8):
+            width, height = height, width  # swap values
         e['width'] = width
         e['height'] = height
 
-
         e['f_number'] = exifs.get_exif('EXIF FNumber')
         e['make'] = exifs.get_exif('Image Make')
         e['model'] = exifs.get_exif('Image Model')
         e['exposure_time'] = exifs.get_exif('EXIF ExposureTime')
-        e['iso'] =  exifs.get_exif('EXIF ISOSpeedRatings')
-        e['focal_length'] =  exifs.get_exif('EXIF FocalLength')
+        e['iso'] = exifs.get_exif('EXIF ISOSpeedRatings')
+        e['focal_length'] = exifs.get_exif('EXIF FocalLength')
         e['rating'] = exifs.get_exif('Image Rating')
         e['lens'] = exifs.get_exif('EXIF LensModel')
         e['exif_datetime'] = None
         val = exifs.get_exif('EXIF DateTimeOriginal')
-        if val != None:
+        if val is not None:
             # Remove any subsecond portion of the DateTimeOriginal value. According to the spec, it's
             # not valid here anyway (should be in SubSecTimeOriginal), but it does exist sometimes.
             val = val.split('.', 1)[0]
             try:
                 e['exif_datetime'] = time.mktime(time.strptime(val, '%Y:%m:%d %H:%M:%S'))
-            except:
+            except Exception:
                 pass
 
         # If we still don't have a date/time, just use the file's modificaiton time
-        if e['exif_datetime'] == None:
+        if e['exif_datetime'] is None:
             e['exif_datetime'] = os.path.getmtime(file_path_name)
 
         gps = exifs.get_location()
         lat = gps['latitude']
         lon = gps['longitude']
-        e['latitude'] = round(lat, 4) if lat is not None else lat #TODO sqlite requires (None,) to insert NULL
+        e['latitude'] = round(lat, 4) if lat is not None else lat  # TODO sqlite requires (None,) to insert NULL
         e['longitude'] = round(lon, 4) if lon is not None else lon
 
-        #IPTC
+        # IPTC
         e['tags'] = exifs.get_exif('IPTC Keywords')
         e['title'] = exifs.get_exif('IPTC Object Name')
         e['caption'] = exifs.get_exif('IPTC Caption/Abstract')
 
-
         return e
 
 
 # If being executed (instead of imported), kick it off...
 if __name__ == "__main__":
     cache = ImageCache(picture_dir='/home/pi/Pictures', follow_links=False, db_file='/home/pi/db.db3', geo_reverse=None)
-    #cache.update_cache()
-    # items = cache.query_cache("make like '%google%'", "exif_datetime asc")
-    #info = cache.get_file_info(12)
```

### Comparing `picframe-2022.6.3/picframe/interface_http.py` & `picframe-2023.5.17/src/picframe/interface_http.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,134 +1,130 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import time
 import os
 import logging
 import json
 import threading
-from functools import partial
 
 try:
-    from http.server import BaseHTTPRequestHandler, HTTPServer #py3
+    from http.server import BaseHTTPRequestHandler, HTTPServer  # py3
     import urllib.parse as urlparse
 except ImportError:
-    from BaseHTTPServer import BaseHTTPRequestHandler, HTTPServer #py2
+    from BaseHTTPServer import BaseHTTPRequestHandler, HTTPServer  # py2
     import urlparse
 
 EXTENSIONS = [".jpg", ".jpeg", ".png", ".heif", ".heic"]
 
+
 def heif_to_jpg(fname):
     try:
-        import pyheif
         from PIL import Image
+        from pi_heif import register_heif_opener
 
-        heif_file = pyheif.read(fname)
-        image = Image.frombytes(heif_file.mode, heif_file.size, heif_file.data,
-                                "raw", heif_file.mode, heif_file.stride)
+        register_heif_opener()
+        image = Image.open(fname)
         if image.mode not in ("RGB", "RGBA"):
             image = image.convert("RGB")
-        image.save("/dev/shm/temp.jpg") # default 75% quality
+        image.save("/dev/shm/temp.jpg")  # default 75% quality
         return "/dev/shm/temp.jpg"
-    except:
+    except Exception:
         logger = logging.getLogger("interface_http.heif_to_jpg")
-        logger.warning("Failed attempt to convert %s \n** Have you installed pyheif? **", fname)
-        return "" # this will not render as a page and will generate error TODO serve specific page with explicit error
+        logger.warning("Failed attempt to convert %s \n** Have you installed pi_heif? **", fname)
+        return ""  # this will not render as a page and will generate error TODO serve specific page with explicit error
+
 
 class RequestHandler(BaseHTTPRequestHandler):
 
-    def do_GET(self):
+    def do_GET(self):  # noqa: C901
         try:
             path_split = self.path.split("?")
             page_ok = False
-            if len(path_split) == 1: # i.e. no ? - just serve index.html or image
-                if path_split[0] != "/": # serve static page from html_path...
+            if len(path_split) == 1:  # i.e. no ? - just serve index.html or image
+                if path_split[0] != "/":  # serve static page from html_path...
                     html_page = path_split[0].strip("/")
                 else:
                     html_page = "index.html"
                 _, extension = os.path.splitext(html_page)
                 if html_page == "current_image" or extension.lower() in EXTENSIONS:
                     # NB homeassistant needs to pass url ending in an image extension
                     # in order to trigger streaming whatever is the currently showing image
                     content_type = "image"
                     page = self.server._controller.get_current_path()
-                    _, extension = os.path.splitext(page) # as current_image may be heic
+                    _, extension = os.path.splitext(page)  # as current_image may be heic
                     if extension.lower() in ('.heic', '.heif'):
                         page = heif_to_jpg(page)
                 else:
                     page = os.path.join(self.server._html_path, html_page)
                     content_type = "text/html"
                 page = urlparse.unquote(page)
                 if os.path.isfile(page):
                     self.send_response(200)
                     self.send_header('Content-type', content_type)
-                    #TODO check if html or js - in which case application/javascript
+                    # TODO check if html or js - in which case application/javascript
                     # really should filter out attempts to render all other file types (jpg etc?)
                     self.end_headers()
                     with open(page, "rb") as f:
                         page_bytes = f.read()
                         self.wfile.write(page_bytes)
                     self.connection.close()
                     page_ok = True
-            else: # server type request - get or set info
+            else:  # server type request - get or set info
                 start_time = time.time()
                 message = {}
                 self.send_response(200)
                 self.server._logger.debug('http request from: ' + self.client_address[0])
 
                 for key, value in dict(urlparse.parse_qsl(path_split[1], True)).items():
                     self.send_header('Content-type', 'text')
                     self.end_headers()
                     if key == "all":
                         for subkey in self.server._setters:
                             message[subkey] = getattr(self.server._controller, subkey)
                     elif key in dir(self.server._controller):
-                        if value != "": # parse_qsl can return empty string for value when just querying
+                        if value != "":  # parse_qsl can return empty string for value when just querying
                             lwr_val = value.lower()
-                            if lwr_val in ("true", "on", "yes"): # this only works for simple values *not* json style kwargs
+                            if lwr_val in ("true", "on", "yes"):  # this only works for simple values *not* json style kwargs # noqa: E501
                                 value = True
                             elif lwr_val in ("false", "off", "no"):
                                 value = False
                             try:
                                 if key in self.server._setters:
                                     setattr(self.server._controller, key, value)
                                 else:
-                                    value = value.replace("\'", "\"") # only " permitted in json
+                                    value = value.replace("\'", "\"")  # only " permitted in json
                                     # value must be json kwargs
                                     getattr(self.server._controller, key)(**json.loads(value))
                             except Exception as e:
                                 message['ERROR'] = 'Excepton:{}>{};'.format(key, e)
-                        if key in self.server._setters: # can get info back from controller TODO 
+                        if key in self.server._setters:  # can get info back from controller TODO
                             message[key] = getattr(self.server._controller, key)
 
                     self.wfile.write(bytes(json.dumps(message), "utf8"))
                     self.connection.close()
                     page_ok = True
 
                 self.server._logger.info(message)
-                self.server._logger.debug("request finished in:  %s seconds" %
-                              (time.time() - start_time))
+                self.server._logger.debug("request finished in:  %s seconds" % (time.time() - start_time))
             if not page_ok:
                 self.send_response(404)
                 self.connection.close()
         except Exception as e:
             self.server._logger.warning(e)
             self.send_response(400)
             self.connection.close()
 
         return
 
-
     def log_request(self, code):
         pass
 
-
     def do_POST(self):
         self.do_GET()
 
-
     def end_headers(self):
         try:
             super().end_headers()
         except BrokenPipeError as e:
             self.connection.close()
             self.server._logger.error('httpserver error: {}'.format(e))
 
@@ -143,13 +139,13 @@
         self._controller = controller
         self._pic_dir = os.path.expanduser(pic_dir)
         self._no_files_img = os.path.expanduser(no_files_img)
         self._html_path = os.path.expanduser(html_path)
         # TODO check below works with all decorated methods.. seems to work
         controller_class = controller.__class__
         self._setters = [method for method in dir(controller_class)
-                            if 'setter' in dir(getattr(controller_class, method))]
+                         if 'setter' in dir(getattr(controller_class, method))]
         t = threading.Thread(target=self.serve_forever)
         t.start()
 
     def stop(self):
         self.shutdown()
```

### Comparing `picframe-2022.6.3/picframe/interface_mqtt.py` & `picframe-2023.5.17/src/picframe/interface_mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """MQTT interface of picframe."""
 
 import logging
-import time
 import paho.mqtt.client as mqtt
 import json
 import os
 from picframe import __version__
 
 
 class InterfaceMQTT:
@@ -26,25 +25,28 @@
 
     def __init__(self, controller, mqtt_config):
         self.__logger = logging.getLogger("interface_mqtt.InterfaceMQTT")
         self.__logger.info('creating an instance of InterfaceMQTT')
         self.__controller = controller
         try:
             device_id = mqtt_config['device_id']
-            self.__client = mqtt.Client(client_id = device_id, clean_session=True)
+            self.__client = mqtt.Client(client_id=device_id, clean_session=True)
             login = mqtt_config['login']
             password = mqtt_config['password']
             self.__client.username_pw_set(login, password)
             tls = mqtt_config['tls']
             if tls:
                 self.__client.tls_set(tls)
             server = mqtt_config['server']
             port = mqtt_config['port']
             self.__client.connect(server, port, 60)
-            self.__client.will_set("homeassistant/switch/" + mqtt_config['device_id'] + "/available", "offline", qos=0, retain=True)
+            self.__client.will_set("homeassistant/switch/"
+                                   + mqtt_config['device_id']
+                                   + "/available",
+                                   "offline", qos=0, retain=True)
             self.__client.on_connect = self.on_connect
             self.__client.on_message = self.on_message
             self.__device_id = mqtt_config['device_id']
             self.__device_url = mqtt_config['device_url']
         except Exception as e:
             self.__logger.error("MQTT not set up because of: {}".format(e))
             raise
@@ -60,138 +62,139 @@
     def stop(self):
         try:
             self.__controller.publish_state = None
             self.__client.loop_stop()
         except Exception as e:
             self.__logger.error("MQTT stopping failed because of: {}".format(e))
 
-
     def on_connect(self, client, userdata, flags, rc):
         if rc != 0:
             self.__logger.warning("Can't connect with mqtt broker. Reason = {0}".format(rc))
             return
         self.__logger.info('Connected with mqtt broker')
 
         # send last will and testament
         available_topic = "homeassistant/switch/" + self.__device_id + "/available"
         client.publish(available_topic, "online", qos=0, retain=True)
 
-        ## sensors
+        # sensors
         self.__setup_sensor(client, "date_from", "mdi:calendar-arrow-left", available_topic, entity_category="config")
         self.__setup_sensor(client, "date_to", "mdi:calendar-arrow-right", available_topic, entity_category="config")
         self.__setup_sensor(client, "location_filter", "mdi:map-search", available_topic, entity_category="config")
         self.__setup_sensor(client, "tags_filter", "mdi:image-search", available_topic, entity_category="config")
         self.__setup_sensor(client, "image_counter", "mdi:camera-burst", available_topic, entity_category="diagnostic")
-        self.__setup_sensor(client, "image", "mdi:file-image", available_topic, has_attributes=True, entity_category="diagnostic")
+        self.__setup_sensor(client, "image", "mdi:file-image",
+                            available_topic, has_attributes=True, entity_category="diagnostic")
 
-        ## numbers
+        # numbers
         self.__setup_number(client, "brightness", 0.0, 1.0, 0.1, "mdi:brightness-6", available_topic)
         self.__setup_number(client, "time_delay", 1, 400, 1, "mdi:image-plus", available_topic)
-        self.__setup_number(client, "fade_time", 1, 50, 1,"mdi:image-size-select-large", available_topic)
+        self.__setup_number(client, "fade_time", 1, 50, 1, "mdi:image-size-select-large", available_topic)
         self.__setup_number(client, "matting_images", 0.0, 1.0, 0.01, "mdi:image-frame", available_topic)
 
-        ## selects
+        # selects
         _, dir_list = self.__controller.get_directory_list()
         dir_list.sort()
         self.__setup_select(client, "directory", dir_list, "mdi:folder-multiple-image", available_topic, init=True)
         command_topic = self.__device_id + "/directory"
         client.subscribe(command_topic, qos=0)
 
-        ## switches
+        # switches
         self.__setup_switch(client, "_text_refresh", "mdi:refresh", available_topic, entity_category="config")
         self.__setup_switch(client, "_name_toggle", "mdi:subtitles", available_topic,
                             self.__controller.text_is_on("name"), entity_category="config")
         self.__setup_switch(client, "_title_toggle", "mdi:subtitles", available_topic,
                             self.__controller.text_is_on("title"), entity_category="config")
         self.__setup_switch(client, "_caption_toggle", "mdi:subtitles", available_topic,
                             self.__controller.text_is_on("caption"), entity_category="config")
         self.__setup_switch(client, "_date_toggle", "mdi:calendar-today", available_topic,
                             self.__controller.text_is_on("date"), entity_category="config")
         self.__setup_switch(client, "_location_toggle", "mdi:crosshairs-gps", available_topic,
                             self.__controller.text_is_on("location"), entity_category="config")
         self.__setup_switch(client, "_directory_toggle", "mdi:folder", available_topic,
                             self.__controller.text_is_on("directory"), entity_category="config")
-        self.__setup_switch(client, "_text_off", "mdi:badge-account-horizontal-outline", available_topic, entity_category="config")
+        self.__setup_switch(client, "_text_off", "mdi:badge-account-horizontal-outline",
+                            available_topic, entity_category="config")
         self.__setup_switch(client, "_display", "mdi:panorama", available_topic,
                             self.__controller.display_is_on)
         self.__setup_switch(client, "_clock", "mdi:clock-outline", available_topic,
                             self.__controller.clock_is_on, entity_category="config")
         self.__setup_switch(client, "_shuffle", "mdi:shuffle-variant", available_topic,
                             self.__controller.shuffle)
         self.__setup_switch(client, "_paused", "mdi:pause", available_topic,
                             self.__controller.paused)
 
         # buttons
         self.__setup_button(client, "_delete", "mdi:delete", available_topic)
         self.__setup_button(client, "_back", "mdi:skip-previous", available_topic)
         self.__setup_button(client, "_next", "mdi:skip-next", available_topic)
 
-        client.subscribe(self.__device_id + "/purge_files", qos=0) # close down without killing!
-        client.subscribe(self.__device_id + "/stop", qos=0) # close down without killing!
+        client.subscribe(self.__device_id + "/purge_files", qos=0)  # close down without killing!
+        client.subscribe(self.__device_id + "/stop", qos=0)  # close down without killing!
 
     def __setup_sensor(self, client, topic, icon, available_topic, has_attributes=False, entity_category=None):
         sensor_topic_head = "homeassistant/sensor/" + self.__device_id
         config_topic = sensor_topic_head + "_" + topic + "/config"
         name = self.__device_id + "_" + topic
         dict = {"name": name,
                 "icon": icon,
                 "value_template": "{{ value_json." + topic + "}}",
                 "avty_t": available_topic,
                 "uniq_id": name,
-                "dev":{"ids":[self.__device_id]}}
-        if has_attributes == True:
+                "dev": {"ids": [self.__device_id]}}
+        if has_attributes is True:
             dict["state_topic"] = sensor_topic_head + "_" + topic + "/state"
             dict["json_attributes_topic"] = sensor_topic_head + "_" + topic + "/attributes"
         else:
             dict["state_topic"] = sensor_topic_head + "/state"
         if entity_category:
             dict["entity_category"] = entity_category
-                                     
+
         config_payload = json.dumps(dict)
         client.publish(config_topic, config_payload, qos=0, retain=True)
         client.subscribe(self.__device_id + "/" + topic, qos=0)
 
     def __setup_number(self, client, topic, min, max, step, icon, available_topic):
         number_topic_head = "homeassistant/number/" + self.__device_id
         config_topic = number_topic_head + "_" + topic + "/config"
         command_topic = self.__device_id + "/" + topic
         state_topic = "homeassistant/sensor/" + self.__device_id + "/state"
         name = self.__device_id + "_" + topic
         config_payload = json.dumps({"name": name,
-                                    "min": min,
-                                    "max": max,
-                                    "step": step,
-                                    "icon": icon,
-                                    "entity_category": "config",
-                                    "state_topic": state_topic,
-                                    "command_topic": command_topic,
-                                    "value_template": "{{ value_json." + topic + "}}",
-                                    "avty_t": available_topic,
-                                    "uniq_id": name,
-                                    "dev":{"ids":[self.__device_id]}})
+                                     "min": min,
+                                     "max": max,
+                                     "step": step,
+                                     "icon": icon,
+                                     "entity_category": "config",
+                                     "state_topic": state_topic,
+                                     "command_topic": command_topic,
+                                     "value_template": "{{ value_json." + topic + "}}",
+                                     "avty_t": available_topic,
+                                     "uniq_id": name,
+                                     "dev": {"ids": [self.__device_id]}})
         client.publish(config_topic, config_payload, qos=0, retain=True)
         client.subscribe(command_topic, qos=0)
 
     def __setup_select(self, client, topic, options, icon, available_topic, init=False):
         select_topic_head = "homeassistant/select/" + self.__device_id
         config_topic = select_topic_head + "_" + topic + "/config"
         command_topic = self.__device_id + "/" + topic
         state_topic = "homeassistant/sensor/" + self.__device_id + "/state"
         name = self.__device_id + "_" + topic
 
         config_payload = json.dumps({"name": name,
-                                    "entity_category": "config",
-                                    "icon": icon,
-                                    "options": options,
-                                    "state_topic": state_topic,
-                                    "command_topic": command_topic,
-                                    "value_template": "{{ value_json." + topic + "}}",
-                                    "avty_t": available_topic,
-                                    "uniq_id": name,
-                                    "dev":{"ids":[self.__device_id]}})
+                                     "entity_category": "config",
+                                     "icon": icon,
+                                     "options": options,
+                                     "state_topic": state_topic,
+                                     "command_topic": command_topic,
+                                     "value_template": "{{ value_json." + topic + "}}",
+                                     "avty_t": available_topic,
+                                     "uniq_id": name,
+                                     "dev": {"ids": [self.__device_id]}})
         client.publish(config_topic, config_payload, qos=0, retain=True)
         if init:
             client.subscribe(command_topic, qos=0)
 
     def __setup_switch(self, client, topic, icon,
                        available_topic, is_on=False, entity_category=None):
         switch_topic_head = "homeassistant/switch/" + self.__device_id
@@ -200,62 +203,60 @@
         state_topic = switch_topic_head + topic + "/state"
         dict = {"name": self.__device_id + topic,
                 "icon": icon,
                 "command_topic": command_topic,
                 "state_topic": state_topic,
                 "avty_t": available_topic,
                 "uniq_id": self.__device_id + topic,
-                "dev": {
-                "ids": [self.__device_id],
-                "name": self.__device_id,
-                "mdl": "PictureFrame",
-                "sw": __version__,
-                "mf": "pi3d PictureFrame project"}}
-        if self.__device_url :
+                "dev": {"ids": [self.__device_id],
+                        "name": self.__device_id,
+                        "mdl": "PictureFrame",
+                        "sw": __version__,
+                        "mf": "pi3d PictureFrame project"}}
+        if self.__device_url:
             dict["dev"]["cu"] = self.__device_url
         if entity_category:
             dict["entity_category"] = entity_category
         config_payload = json.dumps(dict)
 
-        client.subscribe(command_topic , qos=0)
+        client.subscribe(command_topic, qos=0)
         client.publish(config_topic, config_payload, qos=0, retain=True)
         client.publish(state_topic, "ON" if is_on else "OFF", qos=0, retain=True)
 
     def __setup_button(self, client, topic, icon,
                        available_topic, entity_category=None):
         button_topic_head = "homeassistant/button/" + self.__device_id
         config_topic = button_topic_head + topic + "/config"
         command_topic = button_topic_head + topic + "/set"
         dict = {"name": self.__device_id + topic,
                 "icon": icon,
                 "command_topic": command_topic,
                 "payload_press": "ON",
                 "avty_t": available_topic,
                 "uniq_id": self.__device_id + topic,
-                "dev": {
-                "ids": [self.__device_id],
-                "name": self.__device_id,
-                "mdl": "PictureFrame",
-                "sw": __version__,
-                "mf": "pi3d PictureFrame project"}}
-        if self.__device_url :
+                "dev": {"ids": [self.__device_id],
+                        "name": self.__device_id,
+                        "mdl": "PictureFrame",
+                        "sw": __version__,
+                        "mf": "pi3d PictureFrame project"}}
+        if self.__device_url:
             dict["dev"]["cu"] = self.__device_url
         if entity_category:
             dict["entity_category"] = entity_category
         config_payload = json.dumps(dict)
 
-        client.subscribe(command_topic , qos=0)
+        client.subscribe(command_topic, qos=0)
         client.publish(config_topic, config_payload, qos=0, retain=True)
 
-    def on_message(self, client, userdata, message):
+    def on_message(self, client, userdata, message):  # noqa: C901
         msg = message.payload.decode("utf-8")
         switch_topic_head = "homeassistant/switch/" + self.__device_id
         button_topic_head = "homeassistant/button/" + self.__device_id
 
-        ###### switches ######
+        # ##### switches ######
         # display
         if message.topic == switch_topic_head + "_display/set":
             state_topic = switch_topic_head + "_display/state"
             if msg == "ON":
                 self.__controller.display_is_on = True
                 client.publish(state_topic, "ON", retain=True)
             elif msg == "OFF":
@@ -357,15 +358,15 @@
         # text_refresh
         elif message.topic == switch_topic_head + "_text_refresh/set":
             state_topic = switch_topic_head + "_text_refresh/state"
             if msg == "ON":
                 client.publish(state_topic, "OFF", retain=True)
                 self.__controller.refresh_show_text()
 
-        ##### values ########
+        # #### values ########
         # change subdirectory
         elif message.topic == self.__device_id + "/directory":
             self.__logger.info("Recieved subdirectory: %s", msg)
             self.__controller.subdirectory = msg
         # date_from
         elif message.topic == self.__device_id + "/date_from":
             self.__logger.info("Recieved date_from: %s", msg)
@@ -401,65 +402,66 @@
 
         # set the flag to purge files from database
         elif message.topic == self.__device_id + "/purge_files":
             self.__controller.purge_files()
 
         # stop loops and end program
         elif message.topic == self.__device_id + "/stop":
-            self.__controller.stop()
+            self.__controller.keep_looping = False
 
     def publish_state(self, image=None, image_attr=None):
         sensor_topic_head = "homeassistant/sensor/" + self.__device_id
         switch_topic_head = "homeassistant/switch/" + self.__device_id
         available_topic = switch_topic_head + "/available"
 
         sensor_state_payload = {}
         image_state_payload = {}
 
-        ## image
+        # image
         # image attributes
         if image_attr is not None:
             attributes_topic = sensor_topic_head + "_image/attributes"
             self.__logger.debug("Send image attributes: %s", image_attr)
             self.__client.publish(attributes_topic, json.dumps(image_attr), qos=0, retain=False)
         # image sensor
         if image is not None:
             _, tail = os.path.split(image)
             image_state_payload["image"] = tail
             image_state_topic = sensor_topic_head + "_image/state"
             self.__logger.info("Send image state: %s", image_state_payload)
             self.__client.publish(image_state_topic, json.dumps(image_state_payload), qos=0, retain=False)
 
-        ## sensor
+        # sensor
         # directory sensor
         actual_dir, dir_list = self.__controller.get_directory_list()
         sensor_state_payload["directory"] = actual_dir
         # image counter sensor
         sensor_state_payload["image_counter"] = str(self.__controller.get_number_of_files())
         # date_from
         sensor_state_payload["date_from"] = int(self.__controller.date_from)
         # date_to
         sensor_state_payload["date_to"] = int(self.__controller.date_to)
         # location_filter
         sensor_state_payload["location_filter"] = self.__controller.location_filter
         # tags_filter
         sensor_state_payload["tags_filter"] = self.__controller.tags_filter
-        ## number state
+        # number state
         # time_delay
         sensor_state_payload["time_delay"] = self.__controller.time_delay
         # fade_time
         sensor_state_payload["fade_time"] = self.__controller.fade_time
         # brightness
         sensor_state_payload["brightness"] = self.__controller.brightness
         # matting_images
         sensor_state_payload["matting_images"] = self.__controller.matting_images
 
-        #pulish sensors
+        # pulish sensors
         dir_list.sort()
-        self.__setup_select(self.__client, "directory", dir_list, "mdi:folder-multiple-image", available_topic, init=False)
+        self.__setup_select(self.__client, "directory", dir_list,
+                            "mdi:folder-multiple-image", available_topic, init=False)
 
         self.__logger.info("Send sensor state: %s", sensor_state_payload)
         sensor_state_topic = sensor_topic_head + "/state"
         self.__client.publish(sensor_state_topic, json.dumps(sensor_state_payload), qos=0, retain=False)
 
         # publish state of switches
         # pause
@@ -473,8 +475,7 @@
         # display
         state_topic = switch_topic_head + "_display/state"
         payload = "ON" if self.__controller.display_is_on else "OFF"
         self.__client.publish(state_topic, payload, retain=True)
 
         # send last will and testament
         self.__client.publish(available_topic, "online", qos=0, retain=True)
-
```

### Comparing `picframe-2022.6.3/picframe/interface_peripherals.py` & `picframe-2023.5.17/src/picframe/interface_peripherals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import inspect
 import logging
 import subprocess
 import sys
 import time
 import typing
-
 import numpy as np
 import pi3d
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -20,17 +19,17 @@
         model: Model of picframe containing config and business logic.
         viewer: Viewer of picframe representing the display.
         controller: Controller of picframe steering image display.
     """
 
     def __init__(
         self,
-        model: "picframe.model.Model",
-        viewer: "picframe.viewer_display.ViewerDisplay",
-        controller: "picframe.controller.Controller",
+        model,
+        viewer,
+        controller,
     ) -> None:
         logger.info("creating an instance of InterfacePeripherals")
 
         self.__model = model
         self.__viewer = viewer
         self.controller = controller
```

### Comparing `picframe-2022.6.3/picframe/mat_image.py` & `picframe-2023.5.17/src/picframe/mat_image.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from PIL import Image, ImageOps, ImageDraw
 from ninepatch import Ninepatch
 import numpy as np
 import random
 import logging
-import time
+
 
 class MatImage:
 
     # region Constructor
 
-    def __init__(self, display_size, mat_type = None, outer_mat_color = None,
-                resource_folder='.', inner_mat_color = None, outer_mat_border = 75,
-                inner_mat_border = 40, outer_mat_use_texture = True,
-                inner_mat_use_texture = False, auto_inner_mat_color = True):
-
-        self.__mat_types = ['float', 'float_polaroid', 'float_color_wrap', 'single_bevel', 'double_bevel', 'double_flat']
+    def __init__(self, display_size, mat_type=None, outer_mat_color=None,
+                 resource_folder='.', inner_mat_color=None, outer_mat_border=75,
+                 inner_mat_border=40, outer_mat_use_texture=True,
+                 inner_mat_use_texture=False, auto_inner_mat_color=True):
+
+        self.__mat_types = ['float',
+                            'float_polaroid',
+                            'float_color_wrap',
+                            'single_bevel',
+                            'double_bevel',
+                            'double_flat']
 
         self.__logger = logging.getLogger("mat_image.MatImage")
 
         self.auto_inner_mat_color = auto_inner_mat_color
         self.display_size = display_size
         self.inner_mat_border = inner_mat_border
         self.inner_mat_color = inner_mat_color
@@ -139,15 +144,16 @@
             image = self.__style_float_color_wrap(images)
         elif mat_type == 'single_bevel':
             image = self.__style_single_mat_bevel(images)
         elif mat_type == 'double_bevel':
             image = self.__style_double_mat_bevel(images)
         elif mat_type == 'double_flat':
             image = self.__style_double_mat_flat(images)
-        else: image = None
+        else:
+            image = None
 
         return image
 
     # endregion Public Methods
 
     # region Matting Styles
 
@@ -164,87 +170,96 @@
             final_images.append(image)
 
         return self.__layout_images(final_images)
 
     def __style_float_polaroid(self, images):
         border_width = 18
         pic_count = len(images)
-        pic_wid = (self.display_width / pic_count) - (((pic_count + 1) / pic_count) * self.outer_mat_border) - (border_width * 2)
+        pic_wid = ((self.display_width / pic_count)
+                   - (((pic_count + 1) / pic_count) * self.outer_mat_border)
+                   - (border_width * 2))
         pic_height = self.display_height - (self.outer_mat_border * 2) - (border_width * 2)
 
         final_images = []
         for image in images:
             image = self.__scale_image(image, (pic_wid, pic_height))
             self.__add_image_outline(image, self.__outer_mat_color_save)
             image = ImageOps.expand(image, border_width)
-            self.__add_image_outline(image, (210,210,210), outline_width=border_width)
+            self.__add_image_outline(image, (210, 210, 210), outline_width=border_width)
             image = self.__add_drop_shadow(image)
             final_images.append(image)
 
         return self.__layout_images(final_images)
 
     def __style_float_color_wrap(self, images):
         border_width = 18
         pic_count = len(images)
-        pic_wid = (self.display_width / pic_count) - (((pic_count + 1) / pic_count) * self.outer_mat_border) - (border_width * 2)
+        pic_wid = ((self.display_width / pic_count)
+                   - (((pic_count + 1) / pic_count) * self.outer_mat_border)
+                   - (border_width * 2))
         pic_height = self.display_height - (self.outer_mat_border * 2) - (border_width * 2)
 
         final_images = []
         for image in images:
             color = self.__get_darker_shade(self.__outer_mat_color_save, 0.35)
             color2 = self.__get_darker_shade(self.__outer_mat_color_save, 0.2)
             image = self.__scale_image(image, (pic_wid, pic_height))
             self.__add_image_outline(image, color2)
             image = ImageOps.expand(image, border_width)
             self.__add_image_outline(image, color, outline_width=border_width)
             highlight = self.__9patch_highlight.render(image.width, image.height)
-            image.paste(highlight, (0,0), highlight)
+            image.paste(highlight, (0, 0), highlight)
             image = self.__add_drop_shadow(image)
             final_images.append(image)
 
         return self.__layout_images(final_images)
 
-
     def __style_single_mat_bevel(self, images):
         bevel_wid = 5
         pic_count = len(images)
-        pic_wid = (self.display_width / pic_count) - (((pic_count + 1) / pic_count) * self.outer_mat_border) - (bevel_wid * 2)
+        pic_wid = ((self.display_width / pic_count)
+                   - (((pic_count + 1) / pic_count) * self.outer_mat_border)
+                   - (bevel_wid * 2))
         pic_height = self.display_height - (self.outer_mat_border * 2) - (bevel_wid * 2)
 
         final_images = []
         for image in images:
             image = self.__scale_image(image, (pic_wid, pic_height))
             image = self.__add_outer_bevel(image)
             final_images.append(image)
 
         return self.__layout_images(final_images)
 
-
     def __style_double_mat_bevel(self, images):
         bevel_wid = 5
         pic_count = len(images)
-        pic_wid = (self.display_width / pic_count) - (((pic_count + 1) / pic_count) * self.outer_mat_border) - (self.inner_mat_border * 2) - (bevel_wid * 4)
+        pic_wid = ((self.display_width / pic_count)
+                   - (((pic_count + 1) / pic_count) * self.outer_mat_border)
+                   - (self.inner_mat_border * 2)
+                   - (bevel_wid * 4))
         pic_height = self.display_height - (self.outer_mat_border * 2) - (self.inner_mat_border * 2) - (bevel_wid * 4)
 
         final_images = []
         for image in images:
             image = self.__scale_image(image, (pic_wid, pic_height))
-            mat_size = (image.width + (self.inner_mat_border * 2) + (bevel_wid * 2), image.height + (self.inner_mat_border * 2) + (bevel_wid * 2))
+            mat_size = (image.width + (self.inner_mat_border * 2) + (bevel_wid * 2),
+                        image.height + (self.inner_mat_border * 2) + (bevel_wid * 2))
             mat_image = self.__get_inner_mat(mat_size)
             mat_image = self.__add_outer_bevel(mat_image)
             image = self.__add_outer_bevel(image)
             mat_image.paste(image, (self.inner_mat_border + bevel_wid, self.inner_mat_border + bevel_wid))
             final_images.append(mat_image)
 
         return self.__layout_images(final_images)
 
-
     def __style_double_mat_flat(self, images):
         pic_count = len(images)
-        pic_wid = (self.display_width / pic_count) - (((pic_count + 1) / pic_count) * self.outer_mat_border) - (self.inner_mat_border * 2)
+        pic_wid = ((self.display_width / pic_count)
+                   - (((pic_count + 1) / pic_count) * self.outer_mat_border)
+                   - (self.inner_mat_border * 2))
         pic_height = self.display_height - (self.outer_mat_border * 2) - (self.inner_mat_border * 2)
 
         final_images = []
         for image in images:
             image = self.__scale_image(image, (pic_wid, pic_height))
             self.__add_image_outline(image, self.__outer_mat_color_save)
             mat_size = (image.width + (self.inner_mat_border * 2), image.height + (self.inner_mat_border * 2))
@@ -256,310 +271,180 @@
         return self.__layout_images(final_images)
 
     # endregion Matting styles
 
     # region Helper Methods
 
     def __get_mat_type_from_user_string(self, mat_type_string):
-        if mat_type_string == None: mat_type_string = ''
+        if mat_type_string is None:
+            mat_type_string = ''
 
         final = []
-        mat_type_string = mat_type_string.replace(',', "") # remove commas from the string
+        mat_type_string = mat_type_string.replace(',', "")  # remove commas from the string
         for type in mat_type_string.split():
             if type in self.mat_types:
                 final.append(type)
             else:
                 self.__logger.debug('Skipping invalid mat type: %s', type)
 
         if not final:
             self.__logger.debug('No valid mat types defined - using: %s', self.mat_types)
             final = self.mat_types
 
         return final
 
     def __scale_image(self, image, size=None):
-        if size == None:
+        if size is None:
             width, height = self.display_size
         else:
             width, height = size
 
         scale = min(width/image.width, height/image.height)
         image = image.resize((int(image.width * scale), int(image.height * scale)), resample=Image.BICUBIC)
         return image
 
-
     def __get_outer_mat_color(self, image):
         k = KmeansNp(k=3, max_iterations=10, size=100)
         colors = k.run(image)
         return tuple(colors[0])
 
-
-    """def __get_least_gray_color(self, colors):
-        dist = -1
-        color = colors[0]
-        for this_color in colors:
-            this_dist =  max(this_color) - min(this_color)
-            if this_dist > dist:
-                dist = this_dist
-                color = this_color
-        return tuple(map(int, color))"""
-
-
-    def __get_darker_shade(self, rgb_color, fractional_percent = 0.5):
+    def __get_darker_shade(self, rgb_color, fractional_percent=0.5):
         return tuple(map(lambda c: int(c * fractional_percent), rgb_color))
 
-
     def __get_colorized_mat(self, color, use_texture):
         if use_texture:
             mat_img = self.__mat_texture.copy()
             mat_img = mat_img.resize(self.display_size, resample=Image.BICUBIC)
             mat_img = ImageOps.colorize(mat_img, black="black", white=color)
         else:
             mat_img = Image.new('RGB', self.display_size, color)
 
         return mat_img
 
-
     def __get_inner_mat(self, size):
-        w,h = size
+        w, h = size
 
         # If the color wasn't specified, get one
         if not self.inner_mat_color:
             color = self.__get_darker_shade(self.__outer_mat_color_save, 0.50)
         else:
             color = tuple(self.inner_mat_color)
 
         mat = self.__get_colorized_mat(color, self.inner_mat_use_texture)
         mat = mat.crop((0, 0, w, h))
 
         return mat
 
-
-    def __add_outer_bevel(self, image, expand = True):
+    def __add_outer_bevel(self, image, expand=True):
         if expand:
             image = ImageOps.expand(image, 5)
         outer_bevel_image = self.__9patch_bevel.render(image.width, image.height)
-        image.paste(outer_bevel_image, (0,0), outer_bevel_image)
+        image.paste(outer_bevel_image, (0, 0), outer_bevel_image)
         return image
 
-
     def __add_inner_shadow(self, image):
         inner_shadow_image = self.__9patch_inner_shadow.render(image.width, image.height)
-        image.paste(inner_shadow_image, (0,0), inner_shadow_image)
+        image.paste(inner_shadow_image, (0, 0), inner_shadow_image)
         return image
 
-
-    def __add_image_outline(self, img, mat_base_color, outline_width=1, auto_adjust = False):
+    def __add_image_outline(self, img, mat_base_color, outline_width=1, auto_adjust=False):
         if auto_adjust:
             # Calculate the outline color from the mat_color
             brightness = sum(mat_base_color[0:3]) / 3
             outline_color_offset = 30 if brightness < 127 else -30
             outline_color = tuple(map(lambda x: x + outline_color_offset, mat_base_color))
         else:
             outline_color = mat_base_color
 
         rect = ImageDraw.Draw(img)
         shape = [0, 0, img.width-1, img.height-1]
         rect.rectangle(shape, outline=outline_color, width=outline_width)
 
-
     def __add_drop_shadow(self, image):
         shadow_offset = 15
-        mod_image = Image.new('RGBA', (image.width + shadow_offset, image.height + shadow_offset), (0,0,0,0))
+        mod_image = Image.new('RGBA', (image.width + shadow_offset, image.height + shadow_offset), (0, 0, 0, 0))
         shadow_image = self.__9patch_drop_shadow.render(mod_image.width, mod_image.height)
-        mod_image.paste(shadow_image, (0,0), shadow_image)
-        mod_image.paste(image, (0,0))
+        mod_image.paste(shadow_image, (0, 0), shadow_image)
+        mod_image.paste(image, (0, 0))
         return mod_image
 
-
     def __layout_images(self, images):
         mat_image = self.__get_colorized_mat(self.__outer_mat_color_save, self.outer_mat_use_texture)
         total_wid = self.outer_mat_border * (len(images) + 1)
         for image in images:
             total_wid += image.width
 
         xloc = int((mat_image.width - total_wid) / 2)
         for image in images:
             xloc += self.outer_mat_border
-            yloc =  int((mat_image.height -  image.height) / 2)
+            yloc = int((mat_image.height - image.height) / 2)
             if image.mode == 'RGBA':
                 mat_image.paste(image, (xloc, yloc), image)
             else:
                 mat_image.paste(image, (xloc, yloc))
             xloc += image.width
 
         return mat_image
 
-    # endregion Helper functions
-
-# region Automatic Color Selection ----
-
-"""class Cluster(object):
-
-    def __init__(self):
-        self.pixels = []
-        self.centroid = None
-
-    def addPoint(self, pixel):
-        self.pixels.append(pixel)
-
-    def setNewCentroid(self):
-        R = [colour[0] for colour in self.pixels]
-        G = [colour[1] for colour in self.pixels]
-        B = [colour[2] for colour in self.pixels]
-
-        R = sum(R) / len(R)
-        G = sum(G) / len(G)
-        B = sum(B) / len(B)
-
-        self.centroid = (R, G, B)
-        self.pixels = []
-
-        return self.centroid
-
-
-class Kmeans(object):
-
-    def __init__(self, k=3, max_iterations=5, min_distance=5.0, size=200):
-        self.k = k
-        self.max_iterations = max_iterations
-        self.min_distance = min_distance
-        self.size = (size, size)
-
-    def run(self, image):
-        image = image.copy()
-        image.thumbnail(self.size)
-        if image.mode != 'RGB':
-            image = image.convert('RGB') # JAG, some numpy manipulations here don't expect an Alpha channel
-        self.image = image
-
-        self.pixels = np.array(image.getdata(), dtype=np.float)
-
-        self.clusters = [None for i in range(self.k)]
-        self.oldClusters = None
-
-        randomPixels = random.sample(list(self.pixels), self.k)
-
-        for idx in range(self.k):
-            self.clusters[idx] = Cluster()
-            self.clusters[idx].centroid = randomPixels[idx]
-
-        iterations = 0
-        self.start_clusters = [c.centroid for c in self.clusters] # make copy
-
-        while self.shouldExit(iterations) is False:
-
-            self.oldClusters = [cluster.centroid for cluster in self.clusters]
-
-            for pixel in self.pixels:
-                self.assignClusters(pixel)
-
-            for cluster in self.clusters:
-                if not cluster.pixels: continue
-                cluster.setNewCentroid()
-
-            iterations += 1
-
-        return [cluster.centroid for cluster in self.clusters]
-
-    def assignClusters(self, pixel):
-        shortest = float('Inf')
-        for cluster in self.clusters:
-            distance = self.calcDistance(cluster.centroid, pixel)
-            if distance < shortest:
-                shortest = distance
-                nearest = cluster
-
-        nearest.addPoint(pixel)
-
-    def calcDistance(self, a, b):
-        result = np.sqrt(sum((a - b) ** 2))
-        return result
-
-    def shouldExit(self, iterations):
-
-        if self.oldClusters is None:
-            return False
-
-        for idx in range(self.k):
-            dist = self.calcDistance(
-                np.array(self.clusters[idx].centroid),
-                np.array(self.oldClusters[idx])
-            )
-            if dist < self.min_distance:
-                return True
-
-        if iterations <= self.max_iterations:
-            return False
-
-        return True"""
 
 class KmeansNp:
     def __init__(self, k=3, max_iterations=5, min_distance=5.0, size=200):
         self.k = k
         self.max_iterations = max_iterations
         self.min_distance = min_distance
         self.size = (size, size)
 
     def run(self, image, start_clusters=None):
         image = image.copy()
         image.thumbnail(self.size)
-        im = np.array(image, dtype=float)[:,:,:3]
-        # following section can be used to give the clusters location as well as colour proximity
-        #(ix0, ix1) = np.indices(im.shape[:2]) # vert,horiz pixel locations
-        #ix0.shape = ix0.shape + (1,) # make same dim as im
-        #ix1.shape = ix1.shape + (1,) # make same dim as im
-        #im = np.append(im, ix0, axis=2) # TODO multiply by scale rel to rgb scale
-        #im = np.append(im, ix1, axis=2) # im now r,g,b,u,v
-        d = im.shape[-1] # 3 or 5 if u,v added
-        im = im.reshape(-1, d) #NB need to use floats to avoid coercing to uint8 scrambling subtractions
+        im = np.array(image, dtype=float)[:, :, :3]
+        d = im.shape[-1]  # 3 or 5 if u,v added
+        im = im.reshape(-1, d)  # NB need to use floats to avoid coercing to uint8 scrambling subtractions
         n = len(im)
         if start_clusters is None:
             centroids = im[np.random.choice(np.arange(n), self.k)]
         else:
             centroids = np.array(start_clusters, dtype=float)
         old_centroids = centroids.copy()
         for i in range(self.max_iterations):
-            im.shape = (1, n, d) # add dimension to allow broadcasting
-            centroids.shape = (self.k, 1, d) # ditto
-            dists = (((im - centroids) ** 2).sum(axis=2)) ** 0.5 # euclidean distance - manhattan might be fine and faster
-            ix = np.argmin(dists, axis=0) # indices of nearest centroid for each pixel
-            im.shape = (n, d) # reduce dimensions for mean
-            centroids.shape = (self.k, d) # ditto
-            counts = np.unique(ix, return_counts=True)[1] # count the number of each index
-            to_keep = [] # discard any centroids with no pixels nearest to them
-            for j in range(self.k): # write back average location of all nearest pixels
-                j_pixels = im[ix == j] # view into im where ix points to centroid j
-                if len(j_pixels) > 0: # error if try to get mean zero length array TODO remove groups with few pixels?
+            im.shape = (1, n, d)  # add dimension to allow broadcasting
+            centroids.shape = (self.k, 1, d)  # ditto
+            dists = (((im - centroids) ** 2).sum(axis=2)) ** 0.5  # euclidean distance - manhattan might be fine and faster # noqa: E501
+            ix = np.argmin(dists, axis=0)  # indices of nearest centroid for each pixel
+            im.shape = (n, d)  # reduce dimensions for mean
+            centroids.shape = (self.k, d)  # ditto
+            to_keep = []  # discard any centroids with no pixels nearest to them
+            for j in range(self.k):  # write back average location of all nearest pixels
+                j_pixels = im[ix == j]  # view into im where ix points to centroid j
+                if len(j_pixels) > 0:  # error if try to get mean zero length array TODO remove groups with few pixels?
                     centroids[j] = j_pixels.mean(axis=0)
                     to_keep.append(j)
-            if len(to_keep) < len(centroids): # this will be relatively rare
-                for j in to_keep[::-1]: # delete in reverse order of index
+            if len(to_keep) < len(centroids):  # this will be relatively rare
+                for j in to_keep[::-1]:  # delete in reverse order of index
                     centroids = np.delete(centroids, j, axis=0)
                     old_centroids = np.delete(old_centroids, j, axis=0)
             movement = ((((centroids - old_centroids) ** 2).sum(axis=1)) ** 0.5).max()
             if movement < self.min_distance:
                 break
             old_centroids = centroids.copy()
 
-        c_max, c_min = centroids[:,:3].max(axis=1), centroids[:,:3].min(axis=1) # max, min for each centroid
-        #c_lum = 0.5 * (c_max + c_min)
-        #c_sat = (c_max - c_min) / (255.0 - np.abs(c_lum * 2.0 - 255.0)) # should check for lum == 255
-        c_sat = c_max - c_min # value used previously includes element of lum TODO bias more to lighter using (1.5 * c_max - c_min)
-        ix_order = np.argsort(c_sat)[::-1] # indices to sorted values - reversed
+        c_max, c_min = centroids[:, :3].max(axis=1), centroids[:, :3].min(axis=1)  # max, min for each centroid
+        c_sat = c_max - c_min  # value used previously includes element of lum TODO bias more to lighter using (1.5 * c_max - c_min) # noqa: E501
+        ix_order = np.argsort(c_sat)[::-1]  # indices to sorted values - reversed
         return centroids[ix_order, :3].astype(np.uint8)
 
+
 if __name__ == "__main__":
 
     save_folder = '/home/pi/pic_save'
     file1 = '/home/pi/Pictures/Sagelight/2011-01-22_12-05-18-10_edited.jpg'
     file2 = '/home/pi/Pictures/Sagelight/2011-01-22_12-06-07-10_edited.jpg'
     image1 = Image.open(file1)
     image2 = Image.open(file2)
     images = (image1, image2)
 
     matter = MatImage((1920, 1080))
 
     for mat_type in matter.mat_types:
         matter.mat_type = mat_type
         img = matter.mat_image(images)
-        img.save('{0}/{1}_texture.jpg'.format(save_folder, mat_type))
+        img.save('{0}/{1}_texture.jpg'.format(save_folder, mat_type))
```

### Comparing `picframe-2022.6.3/picframe/model.py` & `picframe-2023.5.17/src/picframe/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 import yaml
 import os
 import time
 import logging
-import random
-import json
 import locale
 from picframe import geo_reverse, image_cache
 
 DEFAULT_CONFIGFILE = "~/picframe_data/config/configuration.yaml"
 DEFAULT_CONFIG = {
     'viewer': {
         'blur_amount': 12,
         'blur_zoom': 1.0,
         'blur_edges': False,
         'edge_alpha': 0.5,
         'fps': 20.0,
         'background': [0.2, 0.2, 0.3, 1.0],
-        'blend_type': "blend", # {"blend":0.0, "burn":1.0, "bump":2.0}
-
+        'blend_type': "blend",  # {"blend":0.0, "burn":1.0, "bump":2.0}
         'font_file': '~/picframe_data/data/fonts/NotoSans-Regular.ttf',
         'shader': '~/picframe_data/data/shaders/blend_new',
         'show_text_fm': '%b %d, %Y',
         'show_text_tm': 20.0,
         'show_text_sz': 40,
         'show_text': "name location",
         'text_justify': 'L',
         'text_bkg_hgt': 0.25,
         'text_opacity': 1.0,
         'fit': False,
-        #'auto_resize': True,
         'kenburns': False,
         'display_x': 0,
         'display_y': 0,
         'display_w': None,
         'display_h': None,
+        'display_power': 0,
         'use_glx': False,                          # default=False. Set to True on linux with xserver running
         'test_key': 'test_value',
         'mat_images': True,
         'mat_type': None,
         'outer_mat_color': None,
         'inner_mat_color': None,
         'outer_mat_border': 75,
@@ -46,15 +43,14 @@
         'outer_mat_use_texture': True,
         'mat_resource_folder': '~/picframe_data/data/mat',
         'show_clock': False,
         'clock_justify': "R",
         'clock_text_sz': 120,
         'clock_format': "%I:%M",
         'clock_opacity': 1.0,
-        #'codepoints': "1234567890AÄÀÆÅÃBCÇDÈÉÊEËFGHIÏÍJKLMNÑOÓÖÔŌØPQRSTUÚÙÜVWXYZaáàãæåäbcçdeéèêëfghiíïjklmnñoóôōøöpqrsßtuúüvwxyz., _-+*()&/`´'•" # limit to 121 ie 11x11 grid_size
         'menu_text_sz': 40,
         'menu_autohide_tm': 10.0,
         'geo_suppress_list': [],
     },
     'model': {
 
         'pic_dir': '~/Pictures',
@@ -63,57 +59,61 @@
         'subdirectory': '',
         'recent_n': 3,
         'reshuffle_num': 1,
         'time_delay': 200.0,
         'fade_time': 10.0,
         'shuffle': True,
         'sort_cols': 'fname ASC',
-        'image_attr': ['PICFRAME GPS'],                          # image attributes send by MQTT, Keys are taken from exifread library, 'PICFRAME GPS' is special to retrieve GPS lon/lat
+        'image_attr': ['PICFRAME GPS'],  # image attributes send by MQTT, Keys are taken from exifread library, 'PICFRAME GPS' is special to retrieve GPS lon/lat # noqa: E501
         'load_geoloc': True,
         'locale': 'en_US.utf8',
-        'key_list': [['tourism','amenity','isolated_dwelling'],['suburb','village'],['city','county'],['region','state','province'],['country']],
+        'key_list': [['tourism', 'amenity', 'isolated_dwelling'],
+                     ['suburb', 'village'],
+                     ['city', 'county'],
+                     ['region', 'state', 'province'],
+                     ['country']],
         'geo_key': 'this_needs_to@be_changed',  # use your email address
         'db_file': '~/picframe_data/data/pictureframe.db3',
         'portrait_pairs': False,
         'deleted_pictures': '~/DeletedPictures',
         'log_level': 'WARNING',
         'log_file': '',
     },
     'mqtt': {
-        'use_mqtt': False,                          # Set tue true, to enable mqtt
+        'use_mqtt': False,  # Set tue true, to enable mqtt
         'server': '',
         'port': 8883,
         'login': '',
         'password': '',
         'tls': '',
-        'device_id': 'picframe',                                 # unique id of device. change if there is more than one picture frame
+        'device_id': 'picframe',  # unique id of device. change if there is more than one picture frame
         'device_url': '',
     },
     'http': {
         'use_http': False,
         'path': '~/picframe_data/html',
         'port': 9000,
         'use_ssl': False,
         'keyfile': "/path/to/key.pem",
         'certfile': "/path/to/fullchain.pem"
     },
     'peripherals': {
-        'input_type': None,                                      # valid options: {None, "keyboard", "touch", "mouse"}
+        'input_type': None,  # valid options: {None, "keyboard", "touch", "mouse"}
         'buttons': {
             'pause': {'enable': True, 'label': 'Pause', 'shortcut': ' '},
             'display_off': {'enable': True, 'label': 'Display off', 'shortcut': 'o'},
             'location': {'enable': False, 'label': 'Location', 'shortcut': 'l'},
             'exit': {'enable': False, 'label': 'Exit', 'shortcut': 'e'},
             'power_down': {'enable': False, 'label': 'Power down', 'shortcut': 'p'}
         },
     },
 }
 
 
-class Pic: #TODO could this be done more elegantly with namedtuple
+class Pic:  # TODO could this be done more elegantly with namedtuple
 
     def __init__(self, fname, last_modified, file_id, orientation=1, exif_datetime=0,
                  f_number=0, exposure_time=None, iso=0, focal_length=None,
                  make=None, model=None, lens=None, rating=None, latitude=None,
                  longitude=None, width=0, height=0, is_portrait=0, location=None, title=None,
                  caption=None, tags=None):
         self.fname = fname
@@ -131,75 +131,76 @@
         self.rating = rating
         self.latitude = latitude
         self.longitude = longitude
         self.width = width
         self.height = height
         self.is_portrait = is_portrait
         self.location = location
-        self.tags=tags
-        self.caption=caption
-        self.title=title
+        self.tags = tags
+        self.caption = caption
+        self.title = title
 
 
 class Model:
 
-    def __init__(self, configfile = DEFAULT_CONFIGFILE):
+    def __init__(self, configfile=DEFAULT_CONFIGFILE):
         self.__logger = logging.getLogger("model.Model")
         self.__logger.debug('creating an instance of Model')
         self.__config = DEFAULT_CONFIG
         self.__last_file_change = 0.0
         configfile = os.path.expanduser(configfile)
-        self.__logger.info("Open config file: %s:",configfile)
+        self.__logger.info("Open config file: %s:", configfile)
         with open(configfile, 'r') as stream:
             try:
                 conf = yaml.safe_load(stream)
                 for section in ['viewer', 'model', 'mqtt', 'http', 'peripherals']:
                     self.__config[section] = {**DEFAULT_CONFIG[section], **conf[section]}
 
                 self.__logger.debug('config data = %s', self.__config)
             except yaml.YAMLError as exc:
                 self.__logger.error("Can't parse yaml config file: %s: %s", configfile, exc)
         root_logger = logging.getLogger()
-        root_logger.setLevel(self.get_model_config()['log_level']) # set root logger
+        root_logger.setLevel(self.get_model_config()['log_level'])  # set root logger
         log_file = self.get_model_config()['log_file']
         if log_file != '':
-            filehandler = logging.FileHandler(log_file) #NB default appending so needs monitoring
+            filehandler = logging.FileHandler(log_file)  # NB default appending so needs monitoring
             formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
             filehandler.setFormatter(formatter)
             for hdlr in root_logger.handlers[:]:  # remove the existing file handlers
                 if isinstance(hdlr, logging.FileHandler):
                     root_logger.removeHandler(hdlr)
             root_logger.addHandler(filehandler)      # set the new handler
 
-        self.__file_list = [] # this is now a list of tuples i.e (file_id1,) or (file_id1, file_id2)
-        self.__number_of_files = 0 # this is shortcut for len(__file_list)
+        self.__file_list = []  # this is now a list of tuples i.e (file_id1,) or (file_id1, file_id2)
+        self.__number_of_files = 0  # this is shortcut for len(__file_list)
         self.__reload_files = True
-        self.__file_index = 0 # pointer to next position in __file_list
-        self.__current_pics = (None, None) # this hold a tuple of (pic, None) or two pic objects if portrait pairs
+        self.__file_index = 0  # pointer to next position in __file_list
+        self.__current_pics = (None, None)  # this hold a tuple of (pic, None) or two pic objects if portrait pairs
         self.__num_run_through = 0
 
-        model_config = self.get_model_config() # alias for brevity as used several times below
+        model_config = self.get_model_config()  # alias for brevity as used several times below
         try:
             locale.setlocale(locale.LC_TIME, model_config['locale'])
-        except:
+        except Exception:
             self.__logger.error("error trying to set locale to {}".format(model_config['locale']))
         self.__pic_dir = os.path.expanduser(model_config['pic_dir'])
         self.__subdirectory = os.path.expanduser(model_config['subdirectory'])
         self.__load_geoloc = model_config['load_geoloc']
-        self.__geo_reverse = geo_reverse.GeoReverse(model_config['geo_key'], key_list=self.get_model_config()['key_list'])
+        self.__geo_reverse = geo_reverse.GeoReverse(model_config['geo_key'],
+                                                    key_list=self.get_model_config()['key_list'])
         self.__image_cache = image_cache.ImageCache(self.__pic_dir,
                                                     model_config['follow_links'],
                                                     os.path.expanduser(model_config['db_file']),
                                                     self.__geo_reverse,
                                                     model_config['portrait_pairs'])
         self.__deleted_pictures = model_config['deleted_pictures']
         self.__no_files_img = os.path.expanduser(model_config['no_files_img'])
         self.__sort_cols = model_config['sort_cols']
         self.__col_names = None
-        self.__where_clauses = {} # these will be modified by controller
+        self.__where_clauses = {}  # these will be modified by controller
 
     def get_viewer_config(self):
         return self.__config['viewer']
 
     def get_model_config(self):
         return self.__config['model']
 
@@ -243,28 +244,24 @@
                 self.__subdirectory = ''
             else:
                 self.__subdirectory = dir
             self.__logger.info("Set subdirectory to: %s", self.__subdirectory)
             self.__reload_files = True
 
     @property
-    def EXIF_TO_FIELD(self): # bit convoluted TODO hold in config? not really configurable
+    def EXIF_TO_FIELD(self):  # bit convoluted TODO hold in config? not really configurable
         return self.__image_cache.EXIF_TO_FIELD
 
     @property
     def shuffle(self):
         return self.__config['model']['shuffle']
 
     @shuffle.setter
-    def shuffle(self, val:bool):
-        self.__config['model']['shuffle'] = val #TODO should this be altered in config?
-        #if val == True:
-        #    self.__shuffle_files()
-        #else:
-        #    self.__sort_files()
+    def shuffle(self, val: bool):
+        self.__config['model']['shuffle'] = val  # TODO should this be altered in config?
         self.__reload_files = True
 
     def set_where_clause(self, key, value=None):
         # value must be a string for later join()
         if (value is None or len(value) == 0):
             if key in self.__where_clauses:
                 self.__where_clauses.pop(key)
@@ -286,34 +283,34 @@
         if self.subdirectory != '':
             actual_dir = self.subdirectory
         follow_links = self.get_model_config()['follow_links']
         subdir_list = next(os.walk(self.__pic_dir, followlinks=follow_links))[1]
         subdir_list[:] = [d for d in subdir_list if not d[0] == '.']
         if not follow_links:
             subdir_list[:] = [d for d in subdir_list if not os.path.islink(self.__pic_dir + '/' + d)]
-        subdir_list.insert(0,root)
+        subdir_list.insert(0, root)
         return actual_dir, subdir_list
 
     def force_reload(self):
         self.__reload_files = True
 
     def set_next_file_to_previous_file(self):
-        self.__file_index = (self.__file_index - 2) % self.__number_of_files # TODO deleting last image results in ZeroDivisionError
+        self.__file_index = (self.__file_index - 2) % self.__number_of_files  # TODO deleting last image results in ZeroDivisionError # noqa: E501
 
     def get_next_file(self):
         missing_images = 0
 
         # loop until we acquire a valid image set
         while True:
             pic1 = None
             pic2 = None
 
             # Reload the playlist if requested
             if self.__reload_files:
-                for _i in range(5): # give image_cache chance on first load if a large directory
+                for _i in range(5):  # give image_cache chance on first load if a large directory
                     self.__get_files()
                     missing_images = 0
                     if self.__number_of_files > 0:
                         break
                     time.sleep(0.5)
 
             # If we don't have any files to show, prepare the "no images" image
@@ -340,17 +337,20 @@
             if len(file_ids) == 2:
                 pic_row = self.__image_cache.get_file_info(file_ids[1])
                 pic2 = Pic(**pic_row) if pic_row is not None else None
 
             # Verify the images in the selected image set actually exist on disk
             # Blank out missing references and swap positions if necessary to try and get
             # a valid image in the first slot.
-            if pic1 and not os.path.isfile(pic1.fname): pic1 = None
-            if pic2 and not os.path.isfile(pic2.fname): pic2 = None
-            if (not pic1 and pic2): pic1, pic2 = pic2, pic1
+            if pic1 and not os.path.isfile(pic1.fname):
+                pic1 = None
+            if pic2 and not os.path.isfile(pic2.fname):
+                pic2 = None
+            if (not pic1 and pic2):
+                pic1, pic2 = pic2, pic1
 
             # Increment the image index for next time
             self.__file_index += 1
 
             # If pic1 is valid here, everything is OK. Break out of the loop and return the set
             if pic1:
                 break
@@ -359,84 +359,69 @@
             # Track the number of times we've looped back so we can abort if we don't have *any* images to display
             missing_images += 1
 
         self.__current_pics = (pic1, pic2)
         return self.__current_pics
 
     def get_number_of_files(self):
-        #return self.__number_of_files
-        #return sum(1 for pics in self.__file_list for pic in pics if pic is not None)
-        # or
         return sum(
                     sum(1 for pic in pics if pic is not None)
-                        for pics in self.__file_list
+                    for pics in self.__file_list
                 )
 
     def get_current_pics(self):
         return self.__current_pics
 
     def delete_file(self):
         # delete the current pic. If it's a portrait pair then only the left one will be deleted
         pic = self.__current_pics[0]
         if pic is None:
             return None
         f_to_delete = pic.fname
         move_to_dir = os.path.expanduser(self.__deleted_pictures)
-        # TODO should these os system calls be inside a try block in case the file has been deleted after it started to show?
+        # TODO should these os system calls be inside a try block
+        # in case the file has been deleted after it started to show?
         if not os.path.exists(move_to_dir):
-          os.system("mkdir {}".format(move_to_dir)) # problems with ownership using python func
-        os.system("mv '{}' '{}'".format(f_to_delete, move_to_dir)) # and with SMB drives
+            os.system("mkdir {}".format(move_to_dir))  # problems with ownership using python func
+        os.system("mv '{}' '{}'".format(f_to_delete, move_to_dir))  # and with SMB drives
         # find and delete record from __file_list
         for i, file_rec in enumerate(self.__file_list):
-            if file_rec[0] == pic.file_id: # database id TODO check that db tidies itself up
+            if file_rec[0] == pic.file_id:  # database id TODO check that db tidies itself up
                 self.__file_list.pop(i)
                 self.__number_of_files -= 1
                 break
 
     def __get_files(self):
         if self.subdirectory != "":
-            picture_dir = os.path.join(self.__pic_dir, self.subdirectory) # TODO catch, if subdirecotry does not exist
+            picture_dir = os.path.join(self.__pic_dir, self.subdirectory)  # TODO catch, if subdirecotry does not exist
         else:
             picture_dir = self.__pic_dir
-        where_list = ["fname LIKE '{}/%'".format(picture_dir)] # TODO / on end to stop 'test' also selecting test1 test2 etc
+        where_list = ["fname LIKE '{}/%'".format(picture_dir)]  # TODO / on end to stop 'test' also selecting test1 test2 etc  # noqa: E501
         where_list.extend(self.__where_clauses.values())
 
         if len(where_list) > 0:
-            where_clause = " AND ".join(where_list) # TODO now always true - remove unreachable code
+            where_clause = " AND ".join(where_list)  # TODO now always true - remove unreachable code
         else:
             where_clause = "1"
 
         sort_list = []
         recent_n = self.get_model_config()["recent_n"]
         if recent_n > 0:
             sort_list.append("last_modified < {:.0f}".format(time.time() - 3600 * 24 * recent_n))
 
         if self.shuffle:
             sort_list.append("RANDOM()")
         else:
             if self.__col_names is None:
-                self.__col_names = self.__image_cache.get_column_names() # do this once
+                self.__col_names = self.__image_cache.get_column_names()  # do this once
             for col in self.__sort_cols.split(","):
                 colsplit = col.split()
                 if colsplit[0] in self.__col_names and (len(colsplit) == 1 or colsplit[1].upper() in ("ASC", "DESC")):
                     sort_list.append(col)
-            sort_list.append("fname ASC") # always finally sort on this in case nothing else to sort on or sort_cols is ""
+            sort_list.append("fname ASC")  # always finally sort on this in case nothing else to sort on or sort_cols is "" # noqa: E501
         sort_clause = ",".join(sort_list)
 
         self.__file_list = self.__image_cache.query_cache(where_clause, sort_clause)
         self.__number_of_files = len(self.__file_list)
         self.__file_index = 0
         self.__num_run_through = 0
         self.__reload_files = False
-
-    """def __shuffle_files(self):
-        #self.__file_list.sort(key=lambda x: x[1]) # will be later files last
-        recent_n = self.get_model_config()['recent_n']
-        temp_list_first = self.__file_list[-recent_n:]
-        temp_list_last = self.__file_list[:-recent_n]
-        random.seed()
-        random.shuffle(temp_list_first)
-        random.shuffle(temp_list_last)
-        self.__file_list = temp_list_first + temp_list_last
-
-    def __sort_files(self):
-        self.__file_list.sort() # if not shuffled; sort by name"""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `picframe-2022.6.3/picframe/start.py` & `picframe-2023.5.17/src/picframe/start.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,169 +1,141 @@
 import logging
-import sys
 import argparse
 import os
-import ssl
 import locale
+import sys
 from distutils.dir_util import copy_tree
 
-from picframe import model, viewer_display, controller, interface_http, __version__
+from picframe import model, viewer_display, controller, __version__
 
 PICFRAME_DATA_DIR = 'picframe_data'
 
+
 def copy_files(pkgdir, dest, target):
     try:
         fullpath = os.path.join(pkgdir,  target)
         destination = os.path.join(dest,  PICFRAME_DATA_DIR)
         destination = os.path.join(destination,  target)
         copy_tree(fullpath,  destination)
-    except:
+    except Exception:
         raise
 
+
 def create_config(root):
     fullpath_root = os.path.join(root,  PICFRAME_DATA_DIR)
     fullpath = os.path.join(fullpath_root, 'config')
     source = os.path.join(fullpath, 'configuration_example.yaml')
     destination = os.path.join(fullpath, 'configuration.yaml')
-    run_start = os.path.join(fullpath_root, 'run_start.py') # TODO for work-around on RPi4
+    run_start = os.path.join(fullpath_root, 'run_start.py')  # TODO for work-around on RPi4
 
     try:
-        with open (source, "r") as file:
+        with open(source, "r") as file:
             filedata = file.read()
 
         print("This will configure ", destination)
         print("To keep default, just hit enter")
 
         # replace all paths with selected picframe_data path
         filedata = filedata.replace("~/picframe_data", fullpath_root)
 
-        #pic_dir
-        pic_dir= input("Enter picture directory [~/Pictures]: ")
+        # pic_dir
+        pic_dir = input("Enter picture directory [~/Pictures]: ")
         if pic_dir == "":
-            pic_dir = "~/Pictures" # convert to absolute path too for work-around on RPi4 running as root
+            pic_dir = "~/Pictures"  # convert to absolute path too for work-around on RPi4 running as root
         pic_dir = os.path.expanduser(pic_dir)
         filedata = filedata.replace("~/Pictures", pic_dir)
 
-        #deleted_pictures
+        # deleted_pictures
         deleted_pictures = input("Enter picture directory [~/DeletedPictures]: ")
         if deleted_pictures == "":
             deleted_pictures = "~/DeletedPictures"
         deleted_pictures = os.path.expanduser(deleted_pictures)
         filedata = filedata.replace("~/DeletedPictures", deleted_pictures)
 
-        #locale
+        # locale
         lan, enc = locale.getlocale()
         if not lan:
             (lan, enc) = ("en_US", "utf8")
         param = input("Enter locale [" + lan + "." + enc + "]: ") or (lan + "." + enc)
         filedata = filedata.replace("en_US.utf8", param)
 
-        with open (destination, "w") as file:
+        with open(destination, "w") as file:
             file.write(filedata)
 
-        with open (run_start, "w") as file: # TODO work-around for RPi4
+        with open(run_start, "w") as file:  # TODO work-around for RPi4
             file.write("from picframe import start\nstart.main()\n")
-    except:
+    except Exception:
         raise
 
 
-def check_packages (packages):
+def check_packages(packages):
     for package in packages:
         try:
             if package == 'paho.mqtt':
                 import paho.mqtt
-                print(package, ': ',paho.mqtt.__version__)
+                print(package, ': ', paho.mqtt.__version__)
             elif package == 'ninepatch':
-                import ninepatch
+                import ninepatch  # noqa: F401
                 print(package, ': installed, but no version info')
             else:
-                print(package, ': ',__import__(package).__version__)
+                print(package, ': ', __import__(package).__version__)
         except ImportError:
             print(package, ': Not found!')
 
+
 def main():
     logging.basicConfig(stream=sys.stdout, level=logging.INFO)
     logger = logging.getLogger("start.py")
     logger.info('starting %s', sys.argv)
 
     parser = argparse.ArgumentParser()
     group = parser.add_mutually_exclusive_group()
     group.add_argument("-i", "--initialize",
-                        help="creates standard file structure for picframe in destination directory",
-                        metavar=('DESTINATION_DIRECTORY'))
+                       help="creates standard file structure for picframe in destination directory",
+                       metavar=('DESTINATION_DIRECTORY'))
     group.add_argument("-v", "--version", help="print version information",
-                        action="store_true")
+                       action="store_true")
     group.add_argument("configfile", nargs='?', help="/path/to/configuration.yaml")
     args = parser.parse_args()
     if args.initialize:
         if os.geteuid() == 0:
             print("Don't run the initialize step with sudo. It might put the files in the wrong place!")
             return
         pkgdir = sys.modules['picframe'].__path__[0]
-        try: 
+        try:
             dest = os.path.abspath(os.path.expanduser(args.initialize))
             copy_files(pkgdir, dest, 'html')
             copy_files(pkgdir, dest, 'config')
             copy_files(pkgdir, dest, 'data')
             create_config(dest)
             print('created {}/picframe_data'.format(dest))
         except Exception as e:
             print("Can't copy files to: ", args.initialize, ". Reason: ", e)
         return
     elif args.version:
         print("picframe version: ", __version__)
         print("\nChecking required packages......")
-        required_packages=[
-            'PIL',
-            'exifread',
-            'pi3d',
-            'yaml',
-            'paho.mqtt',
-            'iptcinfo3',
-            'numpy',
-            'ninepatch'
-        ]
+        required_packages = ['PIL',
+                             'pi3d',
+                             'yaml',
+                             'paho.mqtt',
+                             'iptcinfo3',
+                             'numpy',
+                             'ninepatch',
+                             'pi_heif',
+                             'defusedxml']
         check_packages(required_packages)
-        print("\nChecking optional packages......")
-        check_packages(['pyheif'])
         return
     elif args.configfile:
         m = model.Model(args.configfile)
     else:
         m = model.Model()
 
     v = viewer_display.ViewerDisplay(m.get_viewer_config())
     c = controller.Controller(m, v)
     c.start()
-
-    mqtt_config = m.get_mqtt_config()
-    if mqtt_config['use_mqtt']:
-        from picframe import interface_mqtt
-        try:
-            mqtt = interface_mqtt.InterfaceMQTT(c, mqtt_config)
-            mqtt.start()
-        except:
-            logger.error("Can't initialize mqtt. Stopping picframe")
-            sys.exit(1) 
-
-
-
-    http_config = m.get_http_config()
-    model_config = m.get_model_config()
-    if http_config['use_http']:
-        server = interface_http.InterfaceHttp(c, http_config['path'], model_config['pic_dir'], model_config['no_files_img'], http_config['port'])
-        if http_config['use_ssl']:
-            server.socket = ssl.wrap_socket(
-                server.socket,
-                keyfile = http_config['keyfile'],
-                certfile = http_config['certfile'],
-                server_side=True)
     c.loop()
-    if mqtt_config['use_mqtt']:
-        mqtt.stop()
-    if http_config['use_http']: #TODO objects living in multiple threads issue at shutdown!
-        server.stop()
     c.stop()
 
 
-if __name__=="__main__": 
-    main() 
+if __name__ == "__main__":
+    main()
```

### Comparing `picframe-2022.6.3/picframe/viewer_display.py` & `picframe-2023.5.17/src/picframe/viewer_display.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import sys
 import pi3d
-#from pi3d.Texture import MAX_SIZE
-import math
 import time
 import subprocess
 import logging
 import os
 import numpy as np
 from PIL import Image, ImageFilter, ImageFile
 from picframe import mat_image, get_image_meta
 from datetime import datetime
 
 # supported display modes for display switch
 dpms_mode = ("unsupported", "pi", "x_dpms")
 
+
 # utility functions with no dependency on ViewerDisplay properties
 def txt_to_bit(txt):
-    txt_map = {"title":1, "caption":2, "name":4, "date":8, "location":16, "folder":32}
+    txt_map = {"title": 1, "caption": 2, "name": 4, "date": 8, "location": 16, "folder": 32}
     if txt in txt_map:
         return txt_map[txt]
     return 0
 
+
 def parse_show_text(txt):
     show_text = 0
     txt = txt.lower()
     for txt_key in ("title", "caption", "name", "date", "location", "folder"):
         if txt_key in txt:
             show_text |= txt_to_bit(txt_key)
     return show_text
 
+
 class ViewerDisplay:
 
     def __init__(self, config):
         self.__logger = logging.getLogger("viewer_display.ViewerDisplay")
         self.__blur_amount = config['blur_amount']
         self.__blur_zoom = config['blur_zoom']
         self.__blur_edges = config['blur_edges']
@@ -46,142 +46,149 @@
         self.__inner_mat_border = config['inner_mat_border']
         self.__outer_mat_use_texture = config['outer_mat_use_texture']
         self.__inner_mat_use_texture = config['inner_mat_use_texture']
         self.__mat_resource_folder = os.path.expanduser(config['mat_resource_folder'])
 
         self.__fps = config['fps']
         self.__background = config['background']
-        self.__blend_type = {"blend":0.0, "burn":1.0, "bump":2.0}[config['blend_type']]
+        self.__blend_type = {"blend": 0.0, "burn": 1.0, "bump": 2.0}[config['blend_type']]
         self.__font_file = os.path.expanduser(config['font_file'])
         self.__shader = os.path.expanduser(config['shader'])
         self.__show_text_tm = float(config['show_text_tm'])
         self.__show_text_fm = config['show_text_fm']
         self.__show_text_sz = config['show_text_sz']
         self.__show_text = parse_show_text(config['show_text'])
         self.__text_justify = config['text_justify'].upper()
         self.__text_bkg_hgt = config['text_bkg_hgt'] if 0 <= config['text_bkg_hgt'] <= 1 else 0.25
         self.__text_opacity = config['text_opacity']
         self.__fit = config['fit']
         self.__geo_suppress_list = config['geo_suppress_list']
-        #self.__auto_resize = config['auto_resize']
         self.__kenburns = config['kenburns']
         if self.__kenburns:
             self.__kb_up = True
             self.__fit = False
             self.__blur_edges = False
         if self.__blur_zoom < 1.0:
             self.__blur_zoom = 1.0
         self.__display_x = int(config['display_x'])
         self.__display_y = int(config['display_y'])
         self.__display_w = None if config['display_w'] is None else int(config['display_w'])
         self.__display_h = None if config['display_h'] is None else int(config['display_h'])
+        self.__display_power = int(config['display_power'])
         self.__use_glx = config['use_glx']
-        #self.__codepoints = config['codepoints']
-        self.__alpha = 0.0 # alpha - proportion front image to back
+        self.__alpha = 0.0  # alpha - proportion front image to back
         self.__delta_alpha = 1.0
         self.__display = None
         self.__slide = None
         self.__flat_shader = None
         self.__xstep = None
         self.__ystep = None
-        #self.__text = None
         self.__textblocks = None
         self.__text_bkg = None
-        self.__sfg = None # slide for background
-        self.__sbg = None # slide for foreground
+        self.__sfg = None  # slide for background
+        self.__sbg = None  # slide for foreground
         self.__next_tm = 0.0
         self.__name_tm = 0.0
         self.__in_transition = False
         self.__matter = None
         self.__prev_clock_time = None
         self.__clock_overlay = None
         self.__show_clock = config['show_clock']
         self.__clock_justify = config['clock_justify']
         self.__clock_text_sz = config['clock_text_sz']
         self.__clock_format = config['clock_format']
         self.__clock_opacity = config['clock_opacity']
-        ImageFile.LOAD_TRUNCATED_IMAGES = True # occasional damaged file hangs app
+        ImageFile.LOAD_TRUNCATED_IMAGES = True  # occasional damaged file hangs app
 
     @property
     def display_is_on(self):
-        try: # vcgencmd only applies to raspberry pi
-            state = str(subprocess.check_output(["vcgencmd", "display_power"]))
-            if (state.find("display_power=1") != -1):
-                return True
-            else:
-                return False
-        except Exception as e:
-            self.__logger.debug("Display ON/OFF is vcgencmd, but an error occurred")
-            self.__logger.debug("Cause: %s", e)
-            try: # try xset on linux, DPMS has to be enabled
-                output = subprocess.check_output(["xset" , "-display", ":0", "-q"])
+        if self.__display_power == 0:
+            try:  # vcgencmd only applies to raspberry pi
+                state = str(subprocess.check_output(["vcgencmd", "display_power"]))
+                if (state.find("display_power=1") != -1):
+                    return True
+                else:
+                    return False
+            except Exception as e:
+                self.__logger.debug("Display ON/OFF is vcgencmd, but an error occurred")
+                self.__logger.debug("Cause: %s", e)
+            return True
+        elif self.__display_power == 1:
+            try:  # try xset on linux, DPMS has to be enabled
+                output = subprocess.check_output(["xset", "-display", ":0", "-q"])
                 if output.find(b'Monitor is On') != -1:
                     return True
                 else:
                     return False
             except Exception as e:
                 self.__logger.debug("Display ON/OFF is X with dpms enabled, but an error occurred")
                 self.__logger.debug("Cause: %s", e)
-                self.__logger.warning("Display ON/OFF is not supported for this platform.")
-        return True
+            return True
+        else:
+            self.__logger.warning("Unsupported setting for display_power=%d.", self.__display_power)
+            return True
 
     @display_is_on.setter
     def display_is_on(self, on_off):
-        try: # vcgencmd only applies to raspberry pi
-            if on_off == True:
-                subprocess.call(["vcgencmd", "display_power", "1"])
-            else:
-                subprocess.call(["vcgencmd", "display_power", "0"])
-        except Exception as e:
-            self.__logger.debug("Display ON/OFF is vcgencmd, but an error occured")
-            self.__logger.debug("Cause: %s", e)
-            try: # try xset on linux, DPMS has to be enabled
-                if on_off == True:
-                    subprocess.call(["xset" , "-display", ":0", "dpms", "force", "on"])
+        self.__logger.debug("Switch display (display_power=%d).", self.__display_power)
+        if self.__display_power == 0:
+            try:  # vcgencmd only applies to raspberry pi
+                if on_off is True:
+                    subprocess.call(["vcgencmd", "display_power", "1"])
+                else:
+                    subprocess.call(["vcgencmd", "display_power", "0"])
+            except Exception as e:
+                self.__logger.debug("Display ON/OFF is vcgencmd, but an error occured")
+                self.__logger.debug("Cause: %s", e)
+        elif self.__display_power == 1:
+            try:  # try xset on linux, DPMS has to be enabled
+                if on_off is True:
+                    subprocess.call(["xset", "-display", ":0", "dpms", "force", "on"])
                 else:
-                    subprocess.call(["xset" , "-display", ":0", "dpms", "force", "off"])
+                    subprocess.call(["xset", "-display", ":0", "dpms", "force", "off"])
             except Exception as e:
                 self.__logger.debug("Display ON/OFF is xset via dpms, but an error occured")
                 self.__logger.debug("Cause: %s", e)
-                self.__logger.warning("Display ON/OFF is not supported for this platform.")
+        else:
+            self.__logger.warning("Unsupported setting for display_power=%d.", self.__display_power)
 
     def set_show_text(self, txt_key=None, val="ON"):
         if txt_key is None:
-            self.__show_text = 0 # no arguments signals turning all off
+            self.__show_text = 0  # no arguments signals turning all off
         else:
-            bit = txt_to_bit(txt_key) # convert field name to relevant bit 1,2,4,8,16 etc
+            bit = txt_to_bit(txt_key)  # convert field name to relevant bit 1,2,4,8,16 etc
             if val == "ON":
-                self.__show_text |= bit # turn it on
-            else: #TODO anything else ok to turn it off?
+                self.__show_text |= bit  # turn it on
+            else:  # TODO anything else ok to turn it off?
                 bits = 65535 ^ bit
-                self.__show_text &= bits # turn it off
+                self.__show_text &= bits  # turn it off
 
     def text_is_on(self, txt_key):
         return self.__show_text & txt_to_bit(txt_key)
 
     def reset_name_tm(self, pic=None, paused=None, side=0, pair=False):
         # only extend i.e. if after initial fade in
-        if pic is not None and paused is not None: # text needs to be refreshed
+        if pic is not None and paused is not None:  # text needs to be refreshed
             self.__make_text(pic, paused, side, pair)
         self.__name_tm = max(self.__name_tm, time.time() + self.__show_text_tm)
 
     def set_brightness(self, val):
-        self.__slide.unif[55] = val # take immediate effect
+        self.__slide.unif[55] = val  # take immediate effect
 
     def get_brightness(self):
-        return round(self.__slide.unif[55], 2) # this will still give 32/64 bit differences sometimes, as will the float(format()) system
+        return round(self.__slide.unif[55], 2)  # this will still give 32/64 bit differences sometimes, as will the float(format()) system # noqa: E501
 
-    def set_matting_images(self, val): # needs to cope with "true", "ON", 0, "0.2" etc.
+    def set_matting_images(self, val):  # needs to cope with "true", "ON", 0, "0.2" etc.
         try:
             float_val = float(val)
-            if round(float_val, 4) == 0.0: # pixellish over a 4k monitor
+            if round(float_val, 4) == 0.0:  # pixellish over a 4k monitor
                 val = "true"
             if round(float_val, 4) == 1.0:
                 val = "false"
-        except: # ignore exceptions, error handling is done in following function
+        except Exception:  # ignore exceptions, error handling is done in following function
             pass
         self.__mat_images, self.__mat_images_tol = self.__get_mat_image_control_values(val)
 
     def get_matting_images(self):
         if self.__mat_images and self.__mat_images_tol > 0:
             return self.__mat_images_tol
         elif self.__mat_images and self.__mat_images_tol == -1:
@@ -196,134 +203,119 @@
     @clock_is_on.setter
     def clock_is_on(self, val):
         self.__show_clock = val
 
     # Concatenate the specified images horizontally. Clip the taller
     # image to the height of the shorter image.
     def __create_image_pair(self, im1, im2):
-        sep = 8 # separation between the images
+        sep = 8  # separation between the images
         # scale widest image to same width as narrower to avoid drastic cropping on mismatched images
         if im1.width > im2.width:
             im1 = im1.resize((im2.width, int(im1.height * im2.width / im1.width)), resample=Image.BICUBIC)
         else:
             im2 = im2.resize((im1.width, int(im2.height * im1.width / im2.width)), resample=Image.BICUBIC)
         dst = Image.new('RGB', (im1.width + im2.width + sep, min(im1.height, im2.height)))
         dst.paste(im1, (0, 0))
         dst.paste(im2, (im1.width + sep, 0))
         return dst
 
     def __orientate_image(self, im, pic):
         ext = os.path.splitext(pic.fname)[1].lower()
-        if ext  in ('.heif','.heic'): # heif and heic images are converted to PIL.Image obects and are alway in correct orienation
+        if ext in ('.heif', '.heic'):  # heif and heic images are converted to PIL.Image obects and are alway in correct orienation # noqa: E501
             return im
         orientation = pic.orientation
         if orientation == 2:
             im = im.transpose(Image.FLIP_LEFT_RIGHT)
         elif orientation == 3:
-            im = im.transpose(Image.ROTATE_180) # rotations are clockwise
+            im = im.transpose(Image.ROTATE_180)  # rotations are clockwise
         elif orientation == 4:
             im = im.transpose(Image.FLIP_TOP_BOTTOM)
         elif orientation == 5:
             im = im.transpose(Image.FLIP_LEFT_RIGHT).transpose(Image.ROTATE_90)
         elif orientation == 6:
             im = im.transpose(Image.ROTATE_270)
         elif orientation == 7:
             im = im.transpose(Image.FLIP_LEFT_RIGHT).transpose(Image.ROTATE_270)
         elif orientation == 8:
             im = im.transpose(Image.ROTATE_90)
         return im
 
-
     def __get_mat_image_control_values(self, mat_images_value):
         on = True
         val = 0.01
         org_val = str(mat_images_value).lower()
         if org_val in ('true', 'yes', 'on'):
             val = -1
         elif org_val in ('false', 'no', 'off'):
             on = False
         else:
             try:
                 val = float(org_val)
-            except:
+            except Exception:
                 self.__logger.warning("Invalid value for config option 'mat_images'. Using default.")
-        return(on, val)
-
+        return (on, val)
 
     def __get_aspect_diff(self, screen_size, image_size):
         screen_aspect = screen_size[0] / screen_size[1]
         image_aspect = image_size[0] / image_size[1]
 
         if screen_aspect > image_aspect:
             diff_aspect = 1 - (image_aspect / screen_aspect)
         else:
             diff_aspect = 1 - (screen_aspect / image_aspect)
         return (screen_aspect, image_aspect, diff_aspect)
 
-
-    def __tex_load(self, pics, size=None):
+    def __tex_load(self, pics, size=None):  # noqa: C901
         try:
-            if self.__mat_images and self.__matter == None:
-                self.__matter = mat_image.MatImage(
-                    display_size = (self.__display.width , self.__display.height),
-                    resource_folder=self.__mat_resource_folder,
-                    mat_type = self.__mat_type,
-                    outer_mat_color = self.__outer_mat_color,
-                    inner_mat_color = self.__inner_mat_color,
-                    outer_mat_border = self.__outer_mat_border,
-                    inner_mat_border = self.__inner_mat_border,
-                    outer_mat_use_texture = self.__outer_mat_use_texture,
-                    inner_mat_use_texture = self.__inner_mat_use_texture)
+            if self.__mat_images and self.__matter is None:
+                self.__matter = mat_image.MatImage(display_size=(self.__display.width, self.__display.height),
+                                                   resource_folder=self.__mat_resource_folder,
+                                                   mat_type=self.__mat_type,
+                                                   outer_mat_color=self.__outer_mat_color,
+                                                   inner_mat_color=self.__inner_mat_color,
+                                                   outer_mat_border=self.__outer_mat_border,
+                                                   inner_mat_border=self.__inner_mat_border,
+                                                   outer_mat_use_texture=self.__outer_mat_use_texture,
+                                                   inner_mat_use_texture=self.__inner_mat_use_texture)
 
             # Load the image(s) and correct their orientation as necessary
             if pics[0]:
                 im = get_image_meta.GetImageMeta.get_image_object(pics[0].fname)
                 if im is None:
                     return None
                 if pics[0].orientation != 1:
                     im = self.__orientate_image(im, pics[0])
 
             if pics[1]:
                 im2 = get_image_meta.GetImageMeta.get_image_object(pics[1].fname)
                 if im2 is None:
                     return None
                 if pics[1].orientation != 1:
-                     im2 = self.__orientate_image(im2, pics[1])
+                    im2 = self.__orientate_image(im2, pics[1])
 
             screen_aspect, image_aspect, diff_aspect = self.__get_aspect_diff(size, im.size)
 
             if self.__mat_images and diff_aspect > self.__mat_images_tol:
                 if not pics[1]:
                     im = self.__matter.mat_image((im,))
                 else:
                     im = self.__matter.mat_image((im, im2))
             else:
-                if pics[1]: #i.e portrait pair
+                if pics[1]:  # i.e portrait pair
                     im = self.__create_image_pair(im, im2)
 
-
-
             (w, h) = im.size
-            # no longer allow automatic resize to be turned off - but GL_MAX_TEXTURE_SIZE used by Texture
-            #max_dimension = MAX_SIZE # TODO changing MAX_SIZE causes serious crash on linux laptop!
-            #if not self.__auto_resize: # turned off for 4K display - will cause issues on RPi before v4
-            #    max_dimension = 3840 # TODO check if mipmapping should be turned off with this setting.
-            #if w > max_dimension:
-            #    im = im.resize((max_dimension, int(h * max_dimension / w)), resample=Image.BICUBIC)
-            #elif h > max_dimension:
-            #    im = im.resize((int(w * max_dimension / h), max_dimension), resample=Image.BICUBIC)
-
             screen_aspect, image_aspect, diff_aspect = self.__get_aspect_diff(size, im.size)
 
             if self.__blur_edges and size:
                 if diff_aspect > 0.01:
                     (sc_b, sc_f) = (size[1] / im.size[1], size[0] / im.size[0])
                     if screen_aspect > image_aspect:
-                        (sc_b, sc_f) = (sc_f, sc_b) # swap round
-                    (w, h) =  (round(size[0] / sc_b / self.__blur_zoom), round(size[1] / sc_b / self.__blur_zoom))
+                        (sc_b, sc_f) = (sc_f, sc_b)  # swap round
+                    (w, h) = (round(size[0] / sc_b / self.__blur_zoom), round(size[1] / sc_b / self.__blur_zoom))
                     (x, y) = (round(0.5 * (im.size[0] - w)), round(0.5 * (im.size[1] - h)))
                     box = (x, y, x + w, y + h)
                     blr_sz = (int(x * 512 / size[0]) for x in size)
                     im_b = im.resize(size, resample=0, box=box).resize(blr_sz)
                     im_b = im_b.filter(ImageFilter.GaussianBlur(self.__blur_amount))
                     im_b = im_b.resize(size, resample=Image.BICUBIC)
                     im_b.putalpha(round(255 * self.__edge_alpha))  # to apply the same EDGE_ALPHA as the no blur method.
@@ -331,71 +323,69 @@
                     """resize can use Image.LANCZOS (alias for Image.ANTIALIAS) for resampling
                     for better rendering of high-contranst diagonal lines. NB downscaled large
                     images are rescaled near the start of this try block if w or h > max_dimension
                     so those lines might need changing too.
                     """
                     im_b.paste(im, box=(round(0.5 * (im_b.size[0] - im.size[0])),
                                         round(0.5 * (im_b.size[1] - im.size[1]))))
-                    im = im_b # have to do this as paste applies in place
+                    im = im_b  # have to do this as paste applies in place
             tex = pi3d.Texture(im, blend=True, m_repeat=True, free_after_load=True)
-            #tex = pi3d.Texture(im, blend=True, m_repeat=True, automatic_resize=config.AUTO_RESIZE,
-            #                    mipmap=config.AUTO_RESIZE, free_after_load=True) # poss try this if still some artifacts with full resolution
         except Exception as e:
             self.__logger.warning("Can't create tex from file: \"%s\" or \"%s\"", pics[0].fname, pics[1])
             self.__logger.warning("Cause: %s", e)
             tex = None
-            #raise # only re-raise errors here while debugging
+            # raise # only re-raise errors here while debugging
         return tex
 
-    def __make_text(self, pic, paused, side=0, pair=False):
+    def __make_text(self, pic, paused, side=0, pair=False):  # noqa: C901
         # if side 0 and pair False then this is a full width text and put into
         # __textblocks[0] otherwise it is half width and put into __textblocks[position]
         info_strings = []
-        if pic is not None and (self.__show_text > 0 or paused): #was SHOW_TEXT_TM > 0.0
-            if (self.__show_text & 1) == 1 and pic.title is not None: # title
+        if pic is not None and (self.__show_text > 0 or paused):  # was SHOW_TEXT_TM > 0.0
+            if (self.__show_text & 1) == 1 and pic.title is not None:  # title
                 info_strings.append(pic.title)
-            if (self.__show_text & 2) == 2 and pic.caption is not None: # caption
+            if (self.__show_text & 2) == 2 and pic.caption is not None:  # caption
                 info_strings.append(pic.caption)
-            if (self.__show_text & 4) == 4: # name
+            if (self.__show_text & 4) == 4:  # name
                 info_strings.append(os.path.basename(pic.fname))
-            if (self.__show_text & 8) == 8 and pic.exif_datetime > 0: # date
+            if (self.__show_text & 8) == 8 and pic.exif_datetime > 0:  # date
                 fdt = time.strftime(self.__show_text_fm, time.localtime(pic.exif_datetime))
                 info_strings.append(fdt)
-            if (self.__show_text & 16) == 16 and pic.location is not None: # location
+            if (self.__show_text & 16) == 16 and pic.location is not None:  # location
                 location = pic.location
                 # search for and remove substrings from the location text
                 if self.__geo_suppress_list is not None:
                     for part in self.__geo_suppress_list:
                         location = location.replace(part, "")
                     # remove any redundant concatination strings once the substrings have been removed
                     location = location.replace(" ,", "")
                     # remove any trailing commas or spaces from the location
                     location = location.strip(", ")
-                info_strings.append(location) #TODO need to sanitize and check longer than 0 for real
-            if (self.__show_text & 32) == 32: # folder
+                info_strings.append(location)  # TODO need to sanitize and check longer than 0 for real
+            if (self.__show_text & 32) == 32:  # folder
                 info_strings.append(os.path.basename(os.path.dirname(pic.fname)))
             if paused:
                 info_strings.append("PAUSED")
         final_string = " • ".join(info_strings)
 
         block = None
         if len(final_string) > 0:
             if side == 0 and not pair:
-                c_rng = self.__display.width - 100 # range for x loc from L to R justified
+                c_rng = self.__display.width - 100  # range for x loc from L to R justified
             else:
-                c_rng = self.__display.width * 0.5 - 100 # range for x loc from L to R justified
+                c_rng = self.__display.width * 0.5 - 100  # range for x loc from L to R justified
             block = pi3d.FixedString(self.__font_file, final_string, shadow_radius=3, font_size=self.__show_text_sz,
-                                    shader=self.__flat_shader, justify=self.__text_justify, width=c_rng,
-                                    color=(255, 255, 255, int(255 * float(self.__text_opacity))))
-            adj_x = (c_rng - block.sprite.width) // 2 # half amount of space outside sprite
+                                     shader=self.__flat_shader, justify=self.__text_justify, width=c_rng,
+                                     color=(255, 255, 255, int(255 * float(self.__text_opacity))))
+            adj_x = (c_rng - block.sprite.width) // 2  # half amount of space outside sprite
             if self.__text_justify == "L":
                 adj_x *= -1
             elif self.__text_justify == "C":
                 adj_x = 0
-            if side == 0 and not pair: # i.e. full width
+            if side == 0 and not pair:  # i.e. full width
                 x = adj_x
             else:
                 x = adj_x + int(self.__display.width * 0.25 * (-1.0 if side == 0 else 1.0))
             y = (block.sprite.height - self.__display.height + self.__show_text_sz) // 2
             block.sprite.position(x, y, 0.1)
             block.sprite.set_alpha(0.0)
         if side == 0:
@@ -407,16 +397,16 @@
 
         # --- Only rebuild the FixedString containing the time valud if the time string has changed.
         #     With the default H:M display, this will only rebuild once each minute. Note however,
         #     time strings containing a "seconds" component will rebuild once per second.
         if current_time != self.__prev_clock_time:
             width = self.__display.width - 50
             self.__clock_overlay = pi3d.FixedString(self.__font_file, current_time, font_size=self.__clock_text_sz,
-                shader=self.__flat_shader, width=width, shadow_radius=3,
-                color=(255, 255, 255, int(255 * float(self.__clock_opacity))))
+                                                    shader=self.__flat_shader, width=width, shadow_radius=3,
+                                                    color=(255, 255, 255, int(255 * float(self.__clock_opacity))))
             x = (width - self.__clock_overlay.sprite.width) // 2
             if self.__clock_justify == "L":
                 x *= -1
             elif self.__clock_justify == "C":
                 x = 0
             y = (self.__display.height - self.__clock_text_sz - 20) // 2
             self.__clock_overlay.sprite.position(x, y, 0.1)
@@ -434,69 +424,70 @@
         return self.__display.height
 
     def is_in_transition(self):
         return self.__in_transition
 
     def slideshow_start(self):
         self.__display = pi3d.Display.create(x=self.__display_x, y=self.__display_y,
-              w=self.__display_w, h=self.__display_h, frames_per_second=self.__fps,
-              display_config=pi3d.DISPLAY_CONFIG_HIDE_CURSOR, background=self.__background, use_glx=self.__use_glx)
+                                             w=self.__display_w, h=self.__display_h, frames_per_second=self.__fps,
+                                             display_config=pi3d.DISPLAY_CONFIG_HIDE_CURSOR,
+                                             background=self.__background, use_glx=self.__use_glx)
         camera = pi3d.Camera(is_3d=False)
         shader = pi3d.Shader(self.__shader)
         self.__slide = pi3d.Sprite(camera=camera, w=self.__display.width, h=self.__display.height, z=5.0)
         self.__slide.set_shader(shader)
         self.__slide.unif[47] = self.__edge_alpha
         self.__slide.unif[54] = float(self.__blend_type)
-        self.__slide.unif[55] = 1.0 #brightness
+        self.__slide.unif[55] = 1.0  # brightness
         self.__textblocks = [None, None]
         self.__flat_shader = pi3d.Shader("uv_flat")
 
         if self.__text_bkg_hgt:
             bkg_hgt = int(min(self.__display.width, self.__display.height) * self.__text_bkg_hgt)
             text_bkg_array = np.zeros((bkg_hgt, 1, 4), dtype=np.uint8)
             text_bkg_array[:, :, 3] = np.linspace(0, 120, bkg_hgt).reshape(-1, 1)
             text_bkg_tex = pi3d.Texture(text_bkg_array, blend=True, mipmap=False, free_after_load=True)
-            self.__text_bkg = pi3d.Sprite(w=self.__display.width, h=bkg_hgt, y=-int(self.__display.height) // 2 + bkg_hgt // 2, z=4.0)
+            self.__text_bkg = pi3d.Sprite(w=self.__display.width,
+                                          h=bkg_hgt, y=-int(self.__display.height) // 2 + bkg_hgt // 2, z=4.0)
             self.__text_bkg.set_draw_details(self.__flat_shader, [text_bkg_tex])
 
-
-    def slideshow_is_running(self, pics=None, time_delay = 200.0, fade_time = 10.0, paused=False):
+    def slideshow_is_running(self, pics=None, time_delay=200.0, fade_time=10.0, paused=False):  # noqa: C901
         if self.clock_is_on:
             self.__draw_clock()
 
         loop_running = self.__display.loop_running()
         tm = time.time()
         if pics is not None:
             new_sfg = self.__tex_load(pics, (self.__display.width, self.__display.height))
             tm = time.time()
             self.__next_tm = tm + time_delay
-            self.__name_tm = tm + fade_time + self.__show_text_tm # text starts after slide transition
-            if new_sfg is not None: # this is a possible return value which needs to be caught
+            self.__name_tm = tm + fade_time + self.__show_text_tm  # text starts after slide transition
+            if new_sfg is not None:  # this is a possible return value which needs to be caught
                 self.__sbg = self.__sfg
                 self.__sfg = new_sfg
             else:
-                (self.__sbg, self.__sfg) = (self.__sfg, self.__sbg) # swap existing images over
+                (self.__sbg, self.__sfg) = (self.__sfg, self.__sbg)  # swap existing images over
             self.__alpha = 0.0
             if fade_time > 0.5:
-                self.__delta_alpha = 1.0 / (self.__fps * fade_time) # delta alpha
+                self.__delta_alpha = 1.0 / (self.__fps * fade_time)  # delta alpha
             else:
-                self.__delta_alpha = 1.0 # else jump alpha from 0 to 1 in one frame
+                self.__delta_alpha = 1.0  # else jump alpha from 0 to 1 in one frame
             # set the file name as the description
             if self.__show_text_tm > 0.0:
                 for i, pic in enumerate(pics):
-                    self.__make_text(pic, paused, i, pics[1] is not None) # send even if pic is None to clear previous text
-            else: # could have a NO IMAGES selected and being drawn
+                    self.__make_text(pic, paused, i, pics[1] is not None)  # send even if pic is None to clear previous text # noqa: E501
+            else:  # could have a NO IMAGES selected and being drawn
                 for block in range(2):
                     self.__textblocks[block] = None
 
-            if self.__sbg is None: # first time through
+            if self.__sbg is None:  # first time through
                 self.__sbg = self.__sfg
             self.__slide.set_textures([self.__sfg, self.__sbg])
-            self.__slide.unif[45:47] = self.__slide.unif[42:44] # transfer front width and height factors to back
-            self.__slide.unif[51:53] = self.__slide.unif[48:50] # transfer front width and height offsets
+            self.__slide.unif[45:47] = self.__slide.unif[42:44]  # transfer front width and height factors to back
+            self.__slide.unif[51:53] = self.__slide.unif[48:50]  # transfer front width and height offsets
             wh_rat = (self.__display.width * self.__sfg.iy) / (self.__display.height * self.__sfg.ix)
             if (wh_rat > 1.0 and self.__fit) or (wh_rat <= 1.0 and not self.__fit):
                 sz1, sz2, os1, os2 = 42, 43, 48, 49
             else:
                 sz1, sz2, os1, os2 = 43, 42, 49, 48
                 wh_rat = 1.0 / wh_rat
             self.__slide.unif[sz1] = wh_rat
@@ -510,47 +501,48 @@
 
         if self.__kenburns and self.__alpha >= 1.0:
             t_factor = time_delay - fade_time - self.__next_tm + tm
             # add exponentially smoothed tweening in case of timing delays etc. to avoid 'jumps'
             self.__slide.unif[48] = self.__slide.unif[48] * 0.95 + self.__xstep * t_factor * 0.05
             self.__slide.unif[49] = self.__slide.unif[49] * 0.95 + self.__ystep * t_factor * 0.05
 
-        if self.__alpha < 1.0: # transition is happening
+        if self.__alpha < 1.0:  # transition is happening
             self.__alpha += self.__delta_alpha
             if self.__alpha > 1.0:
                 self.__alpha = 1.0
             self.__slide.unif[44] = self.__alpha * self.__alpha * (3.0 - 2.0 * self.__alpha)
 
         if (self.__next_tm - tm) < 5.0 or self.__alpha < 1.0:
-            self.__in_transition = True # set __in_transition True a few seconds *before* end of previous slide
-        else: # no transition effect safe to update database, resuffle etc
+            self.__in_transition = True  # set __in_transition True a few seconds *before* end of previous slide
+        else:  # no transition effect safe to update database, resuffle etc
             self.__in_transition = False
 
         self.__slide.draw()
 
         if self.__alpha >= 1.0 and tm < self.__name_tm:
             # this sets alpha for the TextBlock from 0 to 1 then back to 0
             dt = 1.0 - (self.__name_tm - tm) / self.__show_text_tm
-            if dt > 0.995: dt = 1 # ensure that calculated alpha value fully reaches 0 (TODO: Improve!)
-            ramp_pt = max(4.0, self.__show_text_tm / 4.0) # always > 4 so text fade will always < 4s
+            if dt > 0.995:
+                dt = 1  # ensure that calculated alpha value fully reaches 0 (TODO: Improve!)
+            ramp_pt = max(4.0, self.__show_text_tm / 4.0)  # always > 4 so text fade will always < 4s
 
             # create single saw tooth over 0 to __show_text_tm
-            alpha = max(0.0, min(1.0, ramp_pt * (1.0 - abs(1.0 - 2.0 * dt)))) # function only run if image alpha is 1.0 so can use 1.0 - abs...
+            alpha = max(0.0, min(1.0, ramp_pt * (1.0 - abs(1.0 - 2.0 * dt))))  # function only run if image alpha is 1.0 so can use 1.0 - abs... # noqa: E501
 
             # if we have text, set it's current alpha value to fade in/out
             for block in self.__textblocks:
                 if block is not None:
                     block.sprite.set_alpha(alpha)
 
             # if we have a text background to render (and we currently have text), set its alpha and draw it
-            if self.__text_bkg_hgt and any(block is not None for block in self.__textblocks): #txt_len > 0: #only draw background if text there
+            if self.__text_bkg_hgt and any(block is not None for block in self.__textblocks):  # only draw background if text there # noqa: E501
                 self.__text_bkg.set_alpha(alpha)
                 self.__text_bkg.draw()
 
         for block in self.__textblocks:
             if block is not None:
                 block.sprite.draw()
 
-        return (loop_running, False) # now returns tuple with skip image flag added
+        return (loop_running, False)  # now returns tuple with skip image flag added
 
     def slideshow_stop(self):
         self.__display.destroy()
```

### Comparing `picframe-2022.6.3/picframe.egg-info/PKG-INFO` & `picframe-2023.5.17/src/picframe.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: picframe
-Version: 2022.6.3
+Version: 2023.5.17
 Summary: Picture frame viewer powered by raspberry with homeassistant integration
-Home-page: https://github.com/helgeerbe/picframe
-Author: Paddy Gaunt, Jeff Godfrey, Helge Erbe
-Author-email: helge@erbehome.de
+Author: Paddy Gaunt, Jeff Godfrey
+Author-email: Helge Erbe <helge@erbehome.de>
+Maintainer-email: Helge Erbe <helge@erbehome.de>
 License: MIT
-Keywords: picframe viewer raspberry raspi homeassistant hass
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/helgeerbe/picframe
+Keywords: picframe,viewer,raspberry,raspi,homeassistant,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PictureFrame powered by pi3d
 
 ![picframe logo](https://github.com/helgeerbe/picframe/wiki/images/Picframe_Logo.png)
 
+- [![PyPI version](https://badge.fury.io/py/picframe.svg)](https://badge.fury.io/py/picframe)
 - [PictureFrame powered by pi3d](#pictureframe-powered-by-pi3d)
 - [What Is PictureFrame?](#what-is-pictureframe)
 - [History of PictureFrame](#history-of-pictureframe)
 - [Highlights of PictureFrame](#highlights-of-pictureframe)
 - [Documentation](#documentation)
 - [Acknowledgement](#acknowledgement)
 
@@ -77,9 +84,7 @@
 [glenvorel](https://github.com/glenvorel) Thanks for the new keyboard, mouse and touch screen support.
 
 Many Thanks to Wolfgang [www.thedigitalpictureframe.com](https://www.thedigitalpictureframe.com/) for your inspiring work. 
 
 A special Thank to Paddy Gaunt one of the authors of the [pi3d](https://github.com/pi3d/pi3d_demos) project. You are doing a great job!
 
 Last but no least a big Thank You to Jeff Godfrey. Your auto mat feature and database driven cache is an outstanding piece of code.
-
-
```

### Comparing `picframe-2022.6.3/test/test_get_image_meta.py` & `picframe-2023.5.17/test/test_get_image_meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,150 +1,157 @@
 import pytest
 import logging
 
 
-from  picframe.get_image_meta import GetImageMeta
+from src.picframe.get_image_meta import GetImageMeta
 
 logger = logging.getLogger("test_get_image_data")
 logger.setLevel(logging.DEBUG)
 
+
 def test_file_not_found():
     try:
         exifs = GetImageMeta("nonsense")
-        assert exifs.has_exif() == False
-    except:
+        assert exifs.has_exif() is False
+    except Exception:
         pytest.fail("Unexpected exception")
 
+
 def test_open_file():
     try:
         GetImageMeta("test/images/AlleExif.JPG")
-    except:
+    except Exception:
         pytest.fail("Unexpected exception")
 
+
 def test_has_exif():
     try:
         exifs = GetImageMeta("test/images/AlleExif.JPG")
-        assert exifs.has_exif() == True
-    except:
+        assert exifs.has_exif() is True
+    except Exception:
         pytest.fail("Unexpected exception")
 
+
 def images_has_no_exif():
     try:
         exifs = GetImageMeta("test/images/noimage.jpg")
-        assert exifs.has_exif() == False
-    except:
+        assert exifs.has_exif() is False
+    except Exception:
         pytest.fail("Unexpected exception")
 
+
 def test_get_location():
     try:
         exifs = GetImageMeta("test/images/AlleExif.JPG")
         gps = exifs.get_location()
-        assert  gps == {"latitude": 25.197269, "longitude": 55.274359}
-    except:
+        assert gps == {"latitude": 25.197269, "longitude": 55.274359}
+    except Exception:
         pytest.fail("Unexpected exception")
 
+
 def test_get_no_location():
     try:
         exifs = GetImageMeta("test/images/noimage.jpg")
         gps = exifs.get_location()
-        assert  gps == {"latitude": None, "longitude": None}
-    except:
+        assert gps == {"latitude": None, "longitude": None}
+    except Exception:
         pytest.fail("Unexpected exception")
 
+
 def test_exifs_jpg():
     try:
         exifs = GetImageMeta("test/images/AlleExif.JPG")
         val = exifs.get_exif('EXIF FNumber')
-        assert  val == 2.8
+        assert val == 2.8
         val = exifs.get_exif('EXIF ExposureTime')
-        assert  val == "1/30"
+        assert val == "1/30"
         val = exifs.get_exif('EXIF ISOSpeedRatings')
-        assert  val == "6400"
+        assert val == 6400
         val = exifs.get_exif('EXIF FocalLength')
-        assert  val == "17"
+        assert val == "17.0"
         val = exifs.get_exif('EXIF DateTimeOriginal')
-        assert  val == "2020:01:30 20:01:28"
+        assert val == "2020:01:30 20:01:28"
         val = exifs.get_exif('Image Model')
-        assert  val == "ILCE-7RM3"
+        assert val == "ILCE-7RM3"
         width, height = exifs.get_size()
         assert width == 1920
         assert height == 1200
         val = exifs.get_exif('Image Make')
-        assert  val == "SONY"
-        val = exifs.get_exif('EXIF Make') # This should work as well
-        assert  val == "SONY"
-    except:
+        assert val == "SONY"
+        val = exifs.get_exif('EXIF Make')  # This should work as well
+        assert val == "SONY"
+    except Exception:
         pytest.fail("Unexpected exception")
 
+
 def test_get_orientation():
     try:
         # no image
         exifs = GetImageMeta("test/images/noimage.jpg")
         orientation = exifs.get_orientation()
-        assert  orientation == 1
+        assert orientation == 1
 
         # jpg
         exifs = GetImageMeta("test/images/AlleExif.JPG")
         orientation = exifs.get_orientation()
-        assert  orientation == 1
+        assert orientation == 1
 
         exifs = GetImageMeta("test/images/test3.HEIC")
         orientation = exifs.get_orientation()
-        assert  orientation == 6 
-    except:
+        assert orientation == 1
+    except Exception:
         pytest.fail("Unexpected exception")
 
+
 def test_exifs_heic():
     try:
         exifs = GetImageMeta("test/images/test3.HEIC")
         orientation = exifs.get_orientation()
-        assert  orientation == 6
+        assert orientation == 1
 
         width, height = exifs.get_size()
         assert height == 4032
         assert width == 3024
 
-
         f_number = exifs.get_exif('EXIF FNumber')
         assert f_number == 1.8
 
-        make =  exifs.get_exif('Image Make')
+        make = exifs.get_exif('Image Make')
         assert make == "Apple"
 
         model = exifs.get_exif('Image Model')
         assert model == "iPhone 8"
 
         exposure_time = exifs.get_exif('EXIF ExposureTime')
         assert exposure_time == "1/5"
 
-        iso =  exifs.get_exif('EXIF ISOSpeedRatings')
-        assert iso == "100"
+        iso = exifs.get_exif('EXIF ISOSpeedRatings')
+        assert iso == 100
 
-        focal_length =  exifs.get_exif('EXIF FocalLength')
-        assert focal_length == "399/100"
+        focal_length = exifs.get_exif('EXIF FocalLength')
+        assert focal_length == "3.99"
 
         rating = exifs.get_exif('EXIF Rating')
-        assert rating == None
+        assert rating is None
 
         lens = exifs.get_exif('EXIF LensModel')
-        assert lens ==  "iPhone 8 back camera 3.99mm f/1.8"
+        assert lens == "iPhone 8 back camera 3.99mm f/1.8"
 
         exif_datetime = exifs.get_exif('EXIF DateTimeOriginal')
         assert exif_datetime == "2021:05:14 20:27:14"
 
         gps = exifs.get_location()
         assert gps['latitude'] == 38.71365
         gps['longitude'] == -78.15960555555556
-        
 
-        #IPTC
+        # IPTC
         tags = exifs.get_exif('IPTC Keywords')
-        assert tags == None
+        assert tags == 'Stichwort1,Stichwort2,'
 
         title = exifs.get_exif('IPTC Object Name')
-        assert title == None
+        assert title == 'Das ist die Überschrift'
 
         caption = exifs.get_exif('IPTC Caption/Abstract')
-        assert caption == None
+        assert caption == 'Hier ist die Beschreibung'
 
-    except:
-        pytest.fail("Unexpected exception")
+    except Exception:
+        pytest.fail("Unexpected exception")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

