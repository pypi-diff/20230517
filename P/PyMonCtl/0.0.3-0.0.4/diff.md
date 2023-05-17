# Comparing `tmp/PyMonCtl-0.0.3-py3-none-any.whl.zip` & `tmp/PyMonCtl-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 54549 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat    14793 b- defN 23-May-17 11:39 pymonctl/__init__.py
--rw-rw-rw-  2.0 fat    13558 b- defN 23-May-17 10:55 pymonctl/_pymonctl_linux.py
+Zip file size: 54630 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat    14793 b- defN 23-May-17 16:17 pymonctl/__init__.py
+-rw-rw-rw-  2.0 fat    14123 b- defN 23-May-17 16:09 pymonctl/_pymonctl_linux.py
 -rw-rw-rw-  2.0 fat     8617 b- defN 23-May-17 10:55 pymonctl/_pymonctl_macos.py
 -rw-rw-rw-  2.0 fat     8206 b- defN 23-May-17 09:27 pymonctl/_pymonctl_win.py
 -rw-rw-rw-  2.0 fat   165002 b- defN 23-Apr-19 07:41 pymonctl/_xlibcontainer.py
--rw-rw-rw-  2.0 fat       85 b- defN 23-May-17 11:39 PyMonCtl-0.0.3.dist-info/AUTHORS.txt
--rw-rw-rw-  2.0 fat     3202 b- defN 23-May-17 11:39 PyMonCtl-0.0.3.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     7012 b- defN 23-May-17 11:39 PyMonCtl-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-17 11:39 PyMonCtl-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-17 11:39 PyMonCtl-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      899 b- defN 23-May-17 11:39 PyMonCtl-0.0.3.dist-info/RECORD
-11 files, 221475 bytes uncompressed, 53033 bytes compressed:  76.1%
+-rw-rw-rw-  2.0 fat       85 b- defN 23-May-17 16:20 PyMonCtl-0.0.4.dist-info/AUTHORS.txt
+-rw-rw-rw-  2.0 fat     3202 b- defN 23-May-17 16:20 PyMonCtl-0.0.4.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     7012 b- defN 23-May-17 16:20 PyMonCtl-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-17 16:20 PyMonCtl-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-17 16:20 PyMonCtl-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      899 b- defN 23-May-17 16:20 PyMonCtl-0.0.4.dist-info/RECORD
+11 files, 222040 bytes uncompressed, 53114 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: pymonctl/_pymonctl_win.py
 Comment: 
 
 Filename: pymonctl/_xlibcontainer.py
 Comment: 
 
-Filename: PyMonCtl-0.0.3.dist-info/AUTHORS.txt
+Filename: PyMonCtl-0.0.4.dist-info/AUTHORS.txt
 Comment: 
 
-Filename: PyMonCtl-0.0.3.dist-info/LICENSE.txt
+Filename: PyMonCtl-0.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PyMonCtl-0.0.3.dist-info/METADATA
+Filename: PyMonCtl-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: PyMonCtl-0.0.3.dist-info/WHEEL
+Filename: PyMonCtl-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: PyMonCtl-0.0.3.dist-info/top_level.txt
+Filename: PyMonCtl-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: PyMonCtl-0.0.3.dist-info/RECORD
+Filename: PyMonCtl-0.0.4.dist-info/RECORD
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
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 def version(numberOnly: bool = True):
     """Returns the current version of PyMonCtl module, in the form ''x.x.xx'' as string"""
     return ("" if numberOnly else "PyMonCtl-")+__version__
```

## pymonctl/_pymonctl_linux.py

```diff
@@ -14,15 +14,14 @@
 import Xlib.display
 import Xlib.X
 import Xlib.ext.randr
 
 from pymonctl._xlibcontainer import Props, defaultRootWindow, getProperty, getPropertyValue
 from pymonctl import Structs, _pointInBox
 
-
 def __getDisplays() -> List[Xlib.display.Display]:
     displays: List[Xlib.display.Display] = []
     try:
         files = os.listdir("/tmp/.X11-unix")
     except:
         files = []
     for f in files:
@@ -81,51 +80,49 @@
 
 def _getAllScreens():
     # https://stackoverflow.com/questions/8705814/get-display-count-and-resolution-for-each-display-in-python-without-xrandr
     # https://www.x.org/releases/X11R7.7/doc/libX11/libX11/libX11.html#Obtaining_Information_about_the_Display_Image_Formats_or_Screens
     # https://github.com/alexer/python-xlib/blob/master/examples/xrandr.py
     result: dict[str, Structs.ScreenValue] = {}
 
-    for crtc in __getAllCrtcs():
-        display, screen, root, res, output, outputInfo, crtcNumber, crtcInfo = crtc
-
-        if crtcInfo.mode:
-            name = outputInfo.name
-            dId = output
-            x, y, w, h = crtcInfo.x, crtcInfo.y, crtcInfo.width, crtcInfo.height
-            wa: List[int] = getPropertyValue(getProperty(window=root, prop=Props.Root.WORKAREA.value, display=display), display=display)
-            wx, wy, wr, wb = x + wa[0], y + wa[1], x + w - (crtcInfo.width - wa[2] - wa[0]), y + h - (crtcInfo.height - wa[3] - wa[1])
-            try:
-                dpiX, dpiY = round(crtcInfo.width * 25.4 / outputInfo.mm_width), round(crtcInfo.height * 25.4 / outputInfo.mm_height)
-            except:
-                try:
-                    dpiX, dpiY = round(w * 25.4 / screen.width_in_mms), round(h * 25.4 / screen.height_in_mms)
-                except:
-                    dpiX = dpiY = 0
-            scaleX, scaleY = round(dpiX / 96 * 100), round(dpiY / 96 * 100)
-            rot = int(math.log(crtcInfo.rotation, 2))
-            freq = 0.0
-            for mode in res.modes:
-                if crtcInfo.mode == mode.id:
-                    freq = mode.dot_clock / ((mode.h_total * mode.v_total) or 1)
-                    break
-            depth = screen.root_depth
-
-            result[name] = {
-                'id': dId,
-                'is_primary': (x, y) == (0, 0),
-                'pos': Structs.Point(x, y),
-                'size': Structs.Size(w, h),
-                'workarea': Structs.Rect(wx, wy, wr, wb),
-                'scale': (scaleX, scaleY),
-                'dpi': (dpiX, dpiY),
-                'orientation': rot,
-                'frequency': freq,
-                'colordepth': depth
-            }
+    crtcs = __getAllCrtcs()
+    for monitor in __getAllMonitors():
+        display, root, monitor, monitorName = monitor
+        for crtc in crtcs:
+            display, screen, root, res, output, outputInfo, crtc, crtcInfo = crtc
+
+            if outputInfo.name == monitorName and outputInfo.crtc == crtc:
+                is_primary = monitor.primary == 1
+                x, y, w, h = crtcInfo.x, crtcInfo.y, crtcInfo.width, crtcInfo.height
+                # https://askubuntu.com/questions/1124149/how-to-get-taskbar-size-and-position-with-python
+                wa: List[int] = defaultRootWindow.getWorkArea()
+                wx, wy, wr, wb = wa[0], wa[1], wa[2], wa[3]
+                dpiX, dpiY = round((w * 25.4) / outputInfo.mm_width), round((h * 25.4) / outputInfo.mm_height)
+                scaleX, scaleY = round((dpiX / 96) * 100), round((dpiY / 96) * 100)
+                rot = int(math.log(crtcInfo.rotation, 2))
+                freq = 0.0
+                for mode in res.modes:
+                    if crtcInfo.mode == mode.id:
+                        freq = round(mode.dot_clock / ((mode.h_total * mode.v_total) or 1), 2)
+                        break
+                depth = screen.root_depth
+
+                result[outputInfo.name] = {
+                    'id': output,
+                    'is_primary': is_primary,
+                    'pos': Structs.Point(x, y),
+                    'size': Structs.Size(w, h),
+                    'workarea': Structs.Rect(wx, wy, wr, wb),
+                    'scale': (scaleX, scaleY),
+                    'dpi': (dpiX, dpiY),
+                    'orientation': rot,
+                    'frequency': freq,
+                    'colordepth': depth
+                }
+                break
     return result
 
 
 def _getMonitorsCount() -> int:
     monitors = [__getAllMonitors()]
     count = len(monitors)
     if count == 0:
@@ -226,15 +223,15 @@
                     allModes = res.modes
                     break
             if mode: break
 
     if mode and allModes:
         for m in allModes:
             if mode == m.id:
-                outMode = Structs.DisplayMode(m.width, m.height, m.dot_clock / ((m.h_total * m.v_total) or 1))
+                outMode = Structs.DisplayMode(m.width, m.height, round(m.dot_clock / ((m.h_total * m.v_total) or 1), 2))
                 break
     return outMode
 
 
 def __getAllowedModesID(name: str = "") -> List[Tuple[int, Structs.DisplayMode]]:
 
     modes: List[Tuple[int, Structs.DisplayMode]] = []
@@ -247,18 +244,37 @@
             break
     else:
         root = defaultRootWindow.root
         res = root.xrandr_get_screen_resources()
         allModes = res.modes
 
     for mode in allModes:
-        modes.append((mode.id, Structs.DisplayMode(mode.width, mode.height, mode.dot_clock / ((mode.h_total * mode.v_total) or 1))))
+        modes.append((mode.id, Structs.DisplayMode(mode.width, mode.height, round(mode.dot_clock / ((mode.h_total * mode.v_total) or 1), 2))))
     return modes
 
 
+def __getModeID(modeIn: Structs.DisplayMode, name: str = ""):
+
+    allModes = []
+
+    if name:
+        for crtc in __getAllCrtcs(name):
+            res = crtc[3]
+            allModes = res.modes
+            break
+    else:
+        root = defaultRootWindow.root
+        res = root.xrandr_get_screen_resources()
+        allModes = res.modes
+
+    for mode in allModes:
+        freq = round(mode.dot_clock / ((mode.h_total * mode.v_total) or 1), 2)
+        if modeIn.width == mode.width and modeIn.height == mode.height and modeIn.frequency == freq:
+            return mode.id
+
 def _getAllowedModes(name: str = "") -> List[Structs.DisplayMode]:
 
     modes: List[Structs.DisplayMode] = []
     allModes = []
 
     if name:
         for crtc in __getAllCrtcs(name):
@@ -269,15 +285,15 @@
                 break
     else:
         root = defaultRootWindow.root
         res = root.xrandr_get_screen_resources()
         allModes = res.modes
 
     for mode in allModes:
-        modes.append(Structs.DisplayMode(mode.width, mode.height, mode.dot_clock / ((mode.h_total * mode.v_total) or 1)))
+        modes.append(Structs.DisplayMode(mode.width, mode.height, round(mode.dot_clock / ((mode.h_total * mode.v_total) or 1), 2)))
     return modes
 
 
 # def _eventLoop(kill: threading.Event, interval: float):
 #
 #     pp = pprint.PrettyPrinter(indent=4)
 #
@@ -330,18 +346,17 @@
 def _changeMode(mode: Structs.DisplayMode, name: str = ""):
     # https://stackoverflow.com/questions/12706631/x11-change-resolution-and-make-window-fullscreen
     # Xlib.ext.randr.set_screen_size(defaultRootWindow.root, mode.width, mode.height, 0, 0)
     # Xlib.ext.randr.set_screen_config(defaultRootWindow.root, size_id, 0, 0, round(mode.frequency), 0)
     # Xlib.ext.randr.change_output_property()
     allModes = _getAllowedModes(name)
     if mode in allModes:
-        cmd = " -s %sx%s -r %s" % (mode.width, mode.height, round(mode.frequency))
+        cmd = " --mode %sx%s -r %s" % (mode.width, mode.height, round(mode.frequency, 2))
         if name and name in __getMonitorsNames():
             cmd = (" --output %s" % name) + cmd
-            # cmd = (" --screen %s" % 0) + cmd
         cmd = "xrandr" + cmd
         ret = subprocess.check_output(cmd, shell=True).decode(encoding="utf-8").replace("\n", "")
 
 
 def _changeScale(scale: int, name: str = ""):
     pass
```

## Comparing `PyMonCtl-0.0.3.dist-info/LICENSE.txt` & `PyMonCtl-0.0.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PyMonCtl-0.0.3.dist-info/METADATA` & `PyMonCtl-0.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMonCtl
-Version: 0.0.3
+Version: 0.0.4
 Summary: Cross-Platform toolkit to get info on and control monitors connected
 Home-page: https://github.com/Kalmat/PyMonCtl
 Author: Kalmat
 Author-email: palookjones@gmail.com
 License: BSD 3
 Keywords: screen display monitor control geometry size position frequency scale orientation screen-size mouse-position
 Classifier: Development Status :: 4 - Beta
```

## Comparing `PyMonCtl-0.0.3.dist-info/RECORD` & `PyMonCtl-0.0.4.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-pymonctl/__init__.py,sha256=Wk4geaRIdlBIYy8APv0x7u0t1OQKp8w5R6wOfLU3foY,14793
-pymonctl/_pymonctl_linux.py,sha256=N1d2wOvlS0lIryIGakuIpZK1Zxg4w_ejnVFsQTGBRdA,13558
+pymonctl/__init__.py,sha256=QZbDWmVaouVAnaOKffh4ygXWrKbgxtZuTMuhPlHlFQM,14793
+pymonctl/_pymonctl_linux.py,sha256=w15El_5wpXr5ltU8qo0qYDrMiYZrWEgyUtttGkQjLWc,14123
 pymonctl/_pymonctl_macos.py,sha256=-AMkpekoaOZb_J_BPm2pWKv6qaCf0QoMjA_YedXZeOA,8617
 pymonctl/_pymonctl_win.py,sha256=bKZ78UGkPaKeJ1nOWtldGr9tMfZfZRKRrvbUG_1066Q,8206
 pymonctl/_xlibcontainer.py,sha256=dJ2xEkVYtcHfXEd-PUZqd6GSFhRpz7RF4Yuq5ZHCHMk,165002
-PyMonCtl-0.0.3.dist-info/AUTHORS.txt,sha256=hJRXEf80q4Koen2zRkwWtA3uA-A-oFLVVRXvjcAAadc,85
-PyMonCtl-0.0.3.dist-info/LICENSE.txt,sha256=IX3853XOcIGOsZt2TCL9GG5dgJZk2STGmsMNO0RuCrM,3202
-PyMonCtl-0.0.3.dist-info/METADATA,sha256=7cFfpn1AjbnBuQb3i1NBaRE-KEeI3XKeTpqQpSlGBng,7012
-PyMonCtl-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-PyMonCtl-0.0.3.dist-info/top_level.txt,sha256=PwNGH7cWhb_rQ6QJw3fiACSpamugKo_a42DdNhloTaU,9
-PyMonCtl-0.0.3.dist-info/RECORD,,
+PyMonCtl-0.0.4.dist-info/AUTHORS.txt,sha256=hJRXEf80q4Koen2zRkwWtA3uA-A-oFLVVRXvjcAAadc,85
+PyMonCtl-0.0.4.dist-info/LICENSE.txt,sha256=IX3853XOcIGOsZt2TCL9GG5dgJZk2STGmsMNO0RuCrM,3202
+PyMonCtl-0.0.4.dist-info/METADATA,sha256=j6qOigfoCgzwUj24Dnc0NVqg2H_jhf4gd-hBP4GTRM0,7012
+PyMonCtl-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+PyMonCtl-0.0.4.dist-info/top_level.txt,sha256=PwNGH7cWhb_rQ6QJw3fiACSpamugKo_a42DdNhloTaU,9
+PyMonCtl-0.0.4.dist-info/RECORD,,
```

