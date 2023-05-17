# Comparing `tmp/PyMonCtl-0.0.4-py3-none-any.whl.zip` & `tmp/PyMonCtl-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 54630 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat    14793 b- defN 23-May-17 16:17 pymonctl/__init__.py
+Zip file size: 54631 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat    14793 b- defN 23-May-17 19:07 pymonctl/__init__.py
 -rw-rw-rw-  2.0 fat    14123 b- defN 23-May-17 16:09 pymonctl/_pymonctl_linux.py
--rw-rw-rw-  2.0 fat     8617 b- defN 23-May-17 10:55 pymonctl/_pymonctl_macos.py
+-rw-rw-rw-  2.0 fat     8589 b- defN 23-May-17 19:06 pymonctl/_pymonctl_macos.py
 -rw-rw-rw-  2.0 fat     8206 b- defN 23-May-17 09:27 pymonctl/_pymonctl_win.py
 -rw-rw-rw-  2.0 fat   165002 b- defN 23-Apr-19 07:41 pymonctl/_xlibcontainer.py
--rw-rw-rw-  2.0 fat       85 b- defN 23-May-17 16:20 PyMonCtl-0.0.4.dist-info/AUTHORS.txt
--rw-rw-rw-  2.0 fat     3202 b- defN 23-May-17 16:20 PyMonCtl-0.0.4.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     7012 b- defN 23-May-17 16:20 PyMonCtl-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-17 16:20 PyMonCtl-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-17 16:20 PyMonCtl-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      899 b- defN 23-May-17 16:20 PyMonCtl-0.0.4.dist-info/RECORD
-11 files, 222040 bytes uncompressed, 53114 bytes compressed:  76.1%
+-rw-rw-rw-  2.0 fat       85 b- defN 23-May-17 19:07 PyMonCtl-0.0.5.dist-info/AUTHORS.txt
+-rw-rw-rw-  2.0 fat     3202 b- defN 23-May-17 19:07 PyMonCtl-0.0.5.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     7012 b- defN 23-May-17 19:07 PyMonCtl-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-17 19:07 PyMonCtl-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-17 19:07 PyMonCtl-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      899 b- defN 23-May-17 19:07 PyMonCtl-0.0.5.dist-info/RECORD
+11 files, 222012 bytes uncompressed, 53115 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: pymonctl/_pymonctl_win.py
 Comment: 
 
 Filename: pymonctl/_xlibcontainer.py
 Comment: 
 
-Filename: PyMonCtl-0.0.4.dist-info/AUTHORS.txt
+Filename: PyMonCtl-0.0.5.dist-info/AUTHORS.txt
 Comment: 
 
-Filename: PyMonCtl-0.0.4.dist-info/LICENSE.txt
+Filename: PyMonCtl-0.0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PyMonCtl-0.0.4.dist-info/METADATA
+Filename: PyMonCtl-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: PyMonCtl-0.0.4.dist-info/WHEEL
+Filename: PyMonCtl-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: PyMonCtl-0.0.4.dist-info/top_level.txt
+Filename: PyMonCtl-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: PyMonCtl-0.0.4.dist-info/RECORD
+Filename: PyMonCtl-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymonctl/__init__.py

```diff
@@ -11,15 +11,15 @@
 __all__ = [
     "enableUpdate", "disableUpdate", "isUpdateEnabled", "updateInterval",
     "getMonitors", "getMonitorsCount", "findMonitorName", "findMonitorInfo",
     "getSize", "getWorkArea", "getMousePos", "Structs",
     "getCurrentMode", "getAllowedModes", "changeMode",
 ]
 # Mac only
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 
 def version(numberOnly: bool = True):
     """Returns the current version of PyMonCtl module, in the form ''x.x.xx'' as string"""
     return ("" if numberOnly else "PyMonCtl-")+__version__
```

## pymonctl/_pymonctl_macos.py

```diff
@@ -18,17 +18,17 @@
 
 def __getAllMonitors(name: str = ""):
     screens = AppKit.NSScreen.screens()
     for screen in screens:
         desc = screen.deviceDescription()
         displayId = desc['NSScreenNumber']  # Quartz.NSScreenNumber seems to be wrong
         try:
-            scrName = screen.localizedName() + "_" + str(displayId)  # In older macOS, screen doesn't have localizedName() method
+            scrName = screen.localizedName()  # In older macOS, screen doesn't have localizedName() method
         except:
-            scrName = "Display" + "_" + str(displayId)
+            scrName = "Display"
 
         if not name or (name and scrName == name):
             yield [screen, desc, displayId, scrName]
             if name:
                 break
 
 
@@ -57,16 +57,16 @@
         scale = int(screen.backingScaleFactor() * 100)
         dpi = desc[Quartz.NSDeviceResolution].sizeValue()
         dpiX, dpiY = int(dpi.width), int(dpi.height)
         rot = int(Quartz.CGDisplayRotation(display))
         freq = Quartz.CGDisplayModeGetRefreshRate(Quartz.CGDisplayCopyDisplayMode(display))
         depth = Quartz.CGDisplayBitsPerPixel(display)
 
-        result[scrName + "_" + str(display)] = {
-            'id': display,
+        result[scrName] = {
+            'id': display + "_" + str(displayId),
             'is_primary': is_primary,
             'pos': Structs.Point(x, y),
             'size': Structs.Size(w, h),
             'workarea': Structs.Rect(wx, wy, wr, wb),
             'scale': (scale, scale),
             'dpi': (dpiX, dpiY),
             'orientation': rot,
@@ -145,16 +145,17 @@
     screens = AppKit.NSScreen.screens()
     for screen in screens:
         frame = screen.frame()
         if _pointInBox(x, y, int(frame.origin.x), int(frame.origin.y), int(frame.size.width), int(frame.size.height)):
             desc = screen.deviceDescription()
             displayId = desc['NSScreenNumber']  # Quartz.NSScreenNumber seems to be wrong
             try:
-                name = screen.localizedName() + "_" + str(displayId)  # In older macOS, screen doesn't have localizedName() method
+                name = screen.localizedName() + "_" + str(displayId)
             except:
+                # In older macOS, screen doesn't have localizedName() method
                 name = "Display" + "_" + str(displayId)
     return name
 
 
 def _getCurrentMode(name: str = "") -> Optional[Structs.DisplayMode]:
     res: Optional[Structs.DisplayMode] = None
     displayId = __getDisplayId(name)
```

## Comparing `PyMonCtl-0.0.4.dist-info/LICENSE.txt` & `PyMonCtl-0.0.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PyMonCtl-0.0.4.dist-info/METADATA` & `PyMonCtl-0.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMonCtl
-Version: 0.0.4
+Version: 0.0.5
 Summary: Cross-Platform toolkit to get info on and control monitors connected
 Home-page: https://github.com/Kalmat/PyMonCtl
 Author: Kalmat
 Author-email: palookjones@gmail.com
 License: BSD 3
 Keywords: screen display monitor control geometry size position frequency scale orientation screen-size mouse-position
 Classifier: Development Status :: 4 - Beta
```

## Comparing `PyMonCtl-0.0.4.dist-info/RECORD` & `PyMonCtl-0.0.5.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-pymonctl/__init__.py,sha256=QZbDWmVaouVAnaOKffh4ygXWrKbgxtZuTMuhPlHlFQM,14793
+pymonctl/__init__.py,sha256=ws1D2Oa23TPOgi0nvU8-F0su6H6qkduzZt7JVPz-ndw,14793
 pymonctl/_pymonctl_linux.py,sha256=w15El_5wpXr5ltU8qo0qYDrMiYZrWEgyUtttGkQjLWc,14123
-pymonctl/_pymonctl_macos.py,sha256=-AMkpekoaOZb_J_BPm2pWKv6qaCf0QoMjA_YedXZeOA,8617
+pymonctl/_pymonctl_macos.py,sha256=5Si0B8-P8VQyd1OWZigbnF9ChlkDRhtS7AEG6xPTXMw,8589
 pymonctl/_pymonctl_win.py,sha256=bKZ78UGkPaKeJ1nOWtldGr9tMfZfZRKRrvbUG_1066Q,8206
 pymonctl/_xlibcontainer.py,sha256=dJ2xEkVYtcHfXEd-PUZqd6GSFhRpz7RF4Yuq5ZHCHMk,165002
-PyMonCtl-0.0.4.dist-info/AUTHORS.txt,sha256=hJRXEf80q4Koen2zRkwWtA3uA-A-oFLVVRXvjcAAadc,85
-PyMonCtl-0.0.4.dist-info/LICENSE.txt,sha256=IX3853XOcIGOsZt2TCL9GG5dgJZk2STGmsMNO0RuCrM,3202
-PyMonCtl-0.0.4.dist-info/METADATA,sha256=j6qOigfoCgzwUj24Dnc0NVqg2H_jhf4gd-hBP4GTRM0,7012
-PyMonCtl-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-PyMonCtl-0.0.4.dist-info/top_level.txt,sha256=PwNGH7cWhb_rQ6QJw3fiACSpamugKo_a42DdNhloTaU,9
-PyMonCtl-0.0.4.dist-info/RECORD,,
+PyMonCtl-0.0.5.dist-info/AUTHORS.txt,sha256=hJRXEf80q4Koen2zRkwWtA3uA-A-oFLVVRXvjcAAadc,85
+PyMonCtl-0.0.5.dist-info/LICENSE.txt,sha256=IX3853XOcIGOsZt2TCL9GG5dgJZk2STGmsMNO0RuCrM,3202
+PyMonCtl-0.0.5.dist-info/METADATA,sha256=2MuKF75Zze6pvRKVthfMApVUZKQT7bWIbGXfydCV4eM,7012
+PyMonCtl-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+PyMonCtl-0.0.5.dist-info/top_level.txt,sha256=PwNGH7cWhb_rQ6QJw3fiACSpamugKo_a42DdNhloTaU,9
+PyMonCtl-0.0.5.dist-info/RECORD,,
```

