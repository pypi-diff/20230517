# Comparing `tmp/augratin-23.5.16.1.tar.gz` & `tmp/augratin-23.5.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augratin-23.5.16.1.tar", last modified: Tue May 16 23:38:19 2023, max compression
+gzip compressed data, was "augratin-23.5.17.1.tar", last modified: Wed May 17 18:03:59 2023, max compression
```

## Comparing `augratin-23.5.16.1.tar` & `augratin-23.5.17.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 23:38:19.797559 augratin-23.5.16.1/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.5.16.1/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4646 2023-05-16 23:38:19.797559 augratin-23.5.16.1/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3869 2023-05-16 19:43:59.000000 augratin-23.5.16.1/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 23:38:19.761558 augratin-23.5.16.1/augratin/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39599 2023-05-16 23:24:16.000000 augratin-23.5.16.1/augratin/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 23:38:19.795559 augratin-23.5.16.1/augratin/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25551 2023-05-16 23:31:35.000000 augratin-23.5.16.1/augratin/data/dialog.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/data/k6gte-augratin-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/data/k6gte-augratin-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/data/k6gte-augratin-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/data/k6gte-augratin.desktop
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 23:38:19.796559 augratin-23.5.16.1/augratin/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.16.1/augratin/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-16 19:37:32.000000 augratin-23.5.16.1/augratin/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2071 2023-03-28 14:10:04.000000 augratin-23.5.16.1/augratin/lib/omnirig_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2023-05-16 23:33:39.000000 augratin-23.5.16.1/augratin/lib/version.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 23:38:19.786559 augratin-23.5.16.1/augratin.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4646 2023-05-16 23:38:19.000000 augratin-23.5.16.1/augratin.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      591 2023-05-16 23:38:19.000000 augratin-23.5.16.1/augratin.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-16 23:38:19.000000 augratin-23.5.16.1/augratin.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-16 23:38:19.000000 augratin-23.5.16.1/augratin.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       71 2023-05-16 23:38:19.000000 augratin-23.5.16.1/augratin.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-05-16 23:38:19.000000 augratin-23.5.16.1/augratin.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1144 2023-05-16 23:33:41.000000 augratin-23.5.16.1/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-16 23:38:19.797559 augratin-23.5.16.1/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-17 18:03:59.665894 augratin-23.5.17.1/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.5.17.1/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4789 2023-05-17 18:03:59.664894 augratin-23.5.17.1/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4012 2023-05-17 17:56:34.000000 augratin-23.5.17.1/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-17 18:03:59.640894 augratin-23.5.17.1/augratin/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.17.1/augratin/__init__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    40025 2023-05-17 17:53:49.000000 augratin-23.5.17.1/augratin/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-17 18:03:59.656894 augratin-23.5.17.1/augratin/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.5.17.1/augratin/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27227 2023-05-17 18:02:04.000000 augratin-23.5.17.1/augratin/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.5.17.1/augratin/data/k6gte-augratin-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.5.17.1/augratin/data/k6gte-augratin-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.5.17.1/augratin/data/k6gte-augratin-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.5.17.1/augratin/data/k6gte-augratin.desktop
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-17 18:03:59.663894 augratin-23.5.17.1/augratin/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.17.1/augratin/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-16 19:37:32.000000 augratin-23.5.17.1/augratin/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2071 2023-03-28 14:10:04.000000 augratin-23.5.17.1/augratin/lib/omnirig_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2023-05-17 17:54:59.000000 augratin-23.5.17.1/augratin/lib/version.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-17 18:03:59.647894 augratin-23.5.17.1/augratin.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4789 2023-05-17 18:03:59.000000 augratin-23.5.17.1/augratin.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      591 2023-05-17 18:03:59.000000 augratin-23.5.17.1/augratin.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-17 18:03:59.000000 augratin-23.5.17.1/augratin.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-17 18:03:59.000000 augratin-23.5.17.1/augratin.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       71 2023-05-17 18:03:59.000000 augratin-23.5.17.1/augratin.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-05-17 18:03:59.000000 augratin-23.5.17.1/augratin.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1144 2023-05-17 17:55:01.000000 augratin-23.5.17.1/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-17 18:03:59.666894 augratin-23.5.17.1/setup.cfg
```

### Comparing `augratin-23.5.16.1/LICENSE` & `augratin-23.5.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16.1/PKG-INFO` & `augratin-23.5.17.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.5.16.1
+Version: 23.5.17.1
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -52,14 +52,15 @@
 All contacts are stored in an ADIF file in your home directory,
 which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
+- [23-5-17] Reworked bandmap display. Spots with QRT in comment are now muted. Center bandmap on RX freq when changing vfo or zooming display.
 - [23-5-15] Start big code changes to impliment better bandmap.
 - [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
 
 ## Installing, Updating, Running, Removing
```

### Comparing `augratin-23.5.16.1/README.md` & `augratin-23.5.17.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 All contacts are stored in an ADIF file in your home directory,
 which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
+- [23-5-17] Reworked bandmap display. Spots with QRT in comment are now muted. Center bandmap on RX freq when changing vfo or zooming display.
 - [23-5-15] Start big code changes to impliment better bandmap.
 - [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
 
 ## Installing, Updating, Running, Removing
```

### Comparing `augratin-23.5.16.1/augratin/__main__.py` & `augratin-23.5.17.1/augratin/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     dest="debug",
     help="Debug",
 )
 
 args = parser.parse_args()
 
 PIXELSPERSTEP = 10
+YOFFSET = 10
 
 FORCED_INTERFACE = None
 SERVER_ADDRESS = None
 OMNI_RIGNUMBER = 1
 
 if args.rigctld:
     FORCED_INTERFACE = "rigctld"
@@ -371,14 +372,15 @@
         uic.loadUi(data_path, self)
         self.zoom_in_button.clicked.connect(self.dec_zoom)
         self.zoom_out_button.clicked.connect(self.inc_zoom)
         self.bandmap_scene = QtWidgets.QGraphicsScene()
         self.bandmap_scene.clear()
         self.bandmap_scene.setFocusOnTouch(False)
         self.bandmap_scene.selectionChanged.connect(self.spotclicked)
+        self.bandmap_scene.setFont(QtGui.QFont("JetBrains Mono", pointSize=5))
         self.spotdb = Database()
         self.comboBox_mode.currentTextChanged.connect(self.getspots)
         self.comboBox_band.hide()
         # self.comboBox_band.currentTextChanged.connect(self.getspots)
         self.mycall_field.textEdited.connect(self.save_call_and_grid)
         self.mygrid_field.textEdited.connect(self.save_call_and_grid)
         self.log_button.clicked.connect(self.log_contact)
@@ -411,14 +413,15 @@
             else:
                 newbw = 0
             if self.rx_freq != newfreq:
                 self.rx_freq = newfreq
                 self.set_band(f"{self.getband(str(int(newfreq * 1000)))}m")
                 step, _ = self.determine_step_digits()
                 self.drawTXRXMarks(step)
+                self.center_on_rxfreq()
             if self.bandwidth != newbw:
                 self.bandwidth = newbw
                 step, _ = self.determine_step_digits()
                 self.drawTXRXMarks(step)
 
     def save_call_and_grid(self):
         """Saves users callsign and gridsquare to json file."""
@@ -595,40 +598,44 @@
         self.clear_freq_mark(self.rxMark)
         self.clear_freq_mark(self.txMark)
         self.clear_freq_mark(self.bandwidth_mark)
         self.bandmap_scene.clear()
 
         step, _digits = self.determine_step_digits()
         steps = int(round((self.currentBand.end - self.currentBand.start) / step))
-        self.graphicsView.setFixedSize(330, steps * PIXELSPERSTEP + 30)
         self.graphicsView.setScene(self.bandmap_scene)
         for i in range(steps):  # Draw tickmarks
             length = 10
             if i % 5 == 0:
                 length = 15
             self.bandmap_scene.addLine(
-                10,
+                170,
                 i * PIXELSPERSTEP,
-                length + 10,
+                length + 170,
                 i * PIXELSPERSTEP,
                 QtGui.QPen(QtGui.QColor(192, 192, 192)),
             )
             if i % 5 == 0:  # Add Frequency
                 freq = self.currentBand.start + step * i
                 text = f"{freq:.3f}"
-                self.something = self.bandmap_scene.addText(text)
+                self.something = self.bandmap_scene.addText(
+                    text, QtGui.QFont("JetBrains Mono", pointSize=11)
+                )
                 self.something.setPos(
-                    -(self.something.boundingRect().width()) + 10,
+                    -(self.something.boundingRect().width()) + 170,
                     i * PIXELSPERSTEP - (self.something.boundingRect().height() / 2),
                 )
 
         freq = self.currentBand.end + step * steps
         endFreqDigits = f"{freq:.3f}"
         self.bandmap_scene.setSceneRect(
-            160 - (len(endFreqDigits) * PIXELSPERSTEP), 0, 0, steps * PIXELSPERSTEP + 20
+            160 - (len(endFreqDigits) * PIXELSPERSTEP),
+            -15,
+            0,
+            steps * PIXELSPERSTEP + 20,
         )
 
         self.drawTXRXMarks(step)
         self.update_stations()
 
     def update_stations(self):
         """doc"""
@@ -651,41 +658,44 @@
                 ):
                     freq_y = (
                         (items.get("frequency") - self.currentBand.start) / step
                     ) * PIXELSPERSTEP
                     text_y = max(min_y + 5, freq_y)
                     self.lineitemlist.append(
                         self.bandmap_scene.addLine(
-                            22,
+                            180,
                             freq_y,
-                            55,
+                            210,
                             text_y,
                             QtGui.QPen(QtGui.QColor(192, 192, 192)),
                         )
                     )
                     text = self.bandmap_scene.addText(
                         items.get("activator")
                         + " @ "
                         + items.get("reference")
                         + " "
                         + items.get("mode")
                         + " "
-                        + items.get("spotTime").split("T")[1][:-3]
+                        + items.get("spotTime").split("T")[1][:-3],
+                        QtGui.QFont("JetBrains Mono", pointSize=11),
                     )
                     text.document().setDocumentMargin(0)
-                    text.setPos(60, text_y - (text.boundingRect().height() / 2))
+                    text.setPos(210, text_y - (text.boundingRect().height() / 2))
                     text.setFlags(
                         QtWidgets.QGraphicsItem.ItemIsFocusable
                         | QtWidgets.QGraphicsItem.ItemIsSelectable
                         | text.flags()
                     )
                     text.setProperty("freq", items.get("frequency"))
                     text.setProperty("spotId", items.get("spotId"))
                     text.setProperty("mode", items.get("mode"))
                     text.setToolTip(items.get("comments"))
+                    if "QRT" in items.get("comments", "").upper():
+                        text.setDefaultTextColor(QtGui.QColor(120, 120, 120, 120))
 
                     min_y = text_y + text.boundingRect().height() / 2
 
                     # textColor = Data::statusToColor(lower.value().status,
                     # qApp->palette().color(QPalette::Text));
                     # text->setDefaultTextColor(textColor);
                     self.textItemList.append(text)
@@ -749,15 +759,15 @@
             0, ((freq - self.currentBand.start) / step) * PIXELSPERSTEP
         )
         return ret
 
     def center_on_rxfreq(self):
         """doc"""
         freq_pos = self.Freq2ScenePos(self.rx_freq).y()
-        self.scrollArea.verticalScrollBar().setValue(
+        self.graphicsView.verticalScrollBar().setSliderPosition(
             int(freq_pos - (self.height() / 2) + 80)
         )
 
     def drawfreqmark(self, freq, _step, color, currentPolygon):
         """doc"""
 
         self.clear_freq_mark(currentPolygon)
@@ -765,17 +775,17 @@
         if freq < self.currentBand.start or freq > self.currentBand.end:
             return
 
         Yposition = self.Freq2ScenePos(freq).y()
 
         poly = QtGui.QPolygonF()
 
-        poly.append(QtCore.QPointF(21, Yposition))
-        poly.append(QtCore.QPointF(10, Yposition - 7))
-        poly.append(QtCore.QPointF(10, Yposition + 7))
+        poly.append(QtCore.QPointF(181, Yposition))
+        poly.append(QtCore.QPointF(170, Yposition - 7))
+        poly.append(QtCore.QPointF(170, Yposition + 7))
         pen = QtGui.QPen()
         brush = QtGui.QBrush(color)
         currentPolygon.append(self.bandmap_scene.addPolygon(poly, pen, brush))
 
     def draw_bandwidth(self, freq, _step, color, currentPolygon):
         """bandwidth"""
         logger.debug("%s", f"mark:{currentPolygon} f:{freq} b:{self.bandwidth}")
@@ -786,18 +796,18 @@
             # color = QtGui.QColor(30, 30, 180)
             bw_start = freq - ((self.bandwidth / 2) / 1000000)
             bw_end = freq + ((self.bandwidth / 2) / 1000000)
             logger.debug("%s", f"s:{bw_start} e:{bw_end}")
             Yposition_neg = self.Freq2ScenePos(bw_start).y()
             Yposition_pos = self.Freq2ScenePos(bw_end).y()
             poly = QtGui.QPolygonF()
-            poly.append(QtCore.QPointF(15, Yposition_neg))
-            poly.append(QtCore.QPointF(20, Yposition_neg))
-            poly.append(QtCore.QPointF(20, Yposition_pos))
-            poly.append(QtCore.QPointF(15, Yposition_pos))
+            poly.append(QtCore.QPointF(175, Yposition_neg))
+            poly.append(QtCore.QPointF(180, Yposition_neg))
+            poly.append(QtCore.QPointF(180, Yposition_pos))
+            poly.append(QtCore.QPointF(175, Yposition_pos))
             pen = QtGui.QPen()
             brush = QtGui.QBrush(color)
             currentPolygon.append(self.bandmap_scene.addPolygon(poly, pen, brush))
 
     def determine_step_digits(self):
         """doc"""
         return_zoom = {
```

### Comparing `augratin-23.5.16.1/augratin/data/JetBrainsMono-Regular.ttf` & `augratin-23.5.17.1/augratin/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16.1/augratin/data/dialog.ui` & `augratin-23.5.17.1/augratin/data/dialog.ui`

 * *Files 8% similar despite different names*

#### Comparing `augratin-23.5.16.1/augratin/data/dialog.ui` & `augratin-23.5.17.1/augratin/data/dialog.ui`

```diff
@@ -25,14 +25,15 @@
     <property name="windowTitle">
       <string>K6GTE AuGratin</string>
     </property>
     <widget class="QWidget" name="centralwidget">
       <property name="font">
         <font>
           <family>JetBrains Mono</family>
+          <pointsize>11</pointsize>
         </font>
       </property>
       <layout class="QVBoxLayout" name="verticalLayout_3">
         <item>
           <layout class="QHBoxLayout" name="horizontalLayout" stretch="2,0,3">
             <property name="leftMargin">
               <number>9</number>
@@ -273,16 +274,29 @@
                                 <horstretch>0</horstretch>
                                 <verstretch>0</verstretch>
                               </sizepolicy>
                             </property>
                             <property name="font">
                               <font>
                                 <family>JetBrains Mono</family>
+                                <pointsize>11</pointsize>
                               </font>
                             </property>
+                            <property name="alignment">
+                              <set>Qt::AlignLeading|Qt::AlignLeft|Qt::AlignTop</set>
+                            </property>
+                            <property name="renderHints">
+                              <set>QPainter::TextAntialiasing</set>
+                            </property>
+                            <property name="transformationAnchor">
+                              <enum>QGraphicsView::NoAnchor</enum>
+                            </property>
+                            <property name="resizeAnchor">
+                              <enum>QGraphicsView::AnchorViewCenter</enum>
+                            </property>
                           </widget>
                         </item>
                       </layout>
                     </widget>
                   </widget>
                 </item>
               </layout>
@@ -299,26 +313,28 @@
                 <item>
                   <layout class="QHBoxLayout" name="horizontalLayout_5">
                     <item>
                       <widget class="QLabel" name="label_6">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="text">
                           <string>Your Call:</string>
                         </property>
                       </widget>
                     </item>
                     <item>
                       <widget class="QLineEdit" name="mycall_field">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="placeholderText">
                           <string/>
@@ -326,26 +342,28 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QLabel" name="label_5">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="text">
                           <string>Your Grid:</string>
                         </property>
                       </widget>
                     </item>
                     <item>
                       <widget class="QLineEdit" name="mygrid_field">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="text">
                           <string/>
@@ -373,14 +391,15 @@
                 <item>
                   <layout class="QHBoxLayout" name="horizontalLayout_4" stretch="0,1">
                     <item>
                       <widget class="QLineEdit" name="activator_call">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="autoFillBackground">
                           <bool>false</bool>
@@ -391,14 +410,15 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QLineEdit" name="activator_name">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="placeholderText">
                           <string>Activator Name</string>
@@ -410,14 +430,15 @@
                 <item>
                   <layout class="QHBoxLayout" name="horizontalLayout_8" stretch="0,1">
                     <item>
                       <widget class="QLineEdit" name="park_designator">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="placeholderText">
                           <string>XX-####</string>
@@ -425,14 +446,15 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QLineEdit" name="park_name">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="placeholderText">
                           <string>Park Name</string>
@@ -444,14 +466,15 @@
                 <item>
                   <layout class="QHBoxLayout" name="horizontalLayout_10" stretch="0,1">
                     <item>
                       <widget class="QLineEdit" name="park_section">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="placeholderText">
                           <string>Section</string>
@@ -459,14 +482,15 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QLineEdit" name="park_state">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="placeholderText">
                           <string>State</string>
@@ -478,14 +502,15 @@
                 <item>
                   <layout class="QHBoxLayout" name="horizontalLayout_6">
                     <item>
                       <widget class="QLineEdit" name="park_grid">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="alignment">
                           <set>Qt::AlignCenter</set>
@@ -496,14 +521,15 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QLineEdit" name="park_distance">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="alignment">
                           <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
@@ -514,26 +540,28 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QLabel" name="label">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="text">
                           <string>Km</string>
                         </property>
                       </widget>
                     </item>
                     <item>
                       <widget class="QLineEdit" name="park_direction">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="alignment">
                           <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
@@ -544,14 +572,15 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QLabel" name="label_2">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="text">
                           <string>Deg</string>
                         </property>
                       </widget>
                     </item>
@@ -573,26 +602,28 @@
                 <item>
                   <layout class="QHBoxLayout" name="horizontalLayout_9">
                     <item>
                       <widget class="QLabel" name="label_7">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="text">
                           <string>Time:</string>
                         </property>
                       </widget>
                     </item>
                     <item>
                       <widget class="QLineEdit" name="time_field">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="placeholderText">
                           <string>HHMMSS</string>
@@ -600,26 +631,28 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QLabel" name="label_8">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="text">
                           <string>Date:</string>
                         </property>
                       </widget>
                     </item>
                     <item>
                       <widget class="QLineEdit" name="date_field">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="placeholderText">
                           <string>YYYYMMDD</string>
@@ -638,20 +671,21 @@
                           </size>
                         </property>
                       </spacer>
                     </item>
                   </layout>
                 </item>
                 <item>
-                  <layout class="QHBoxLayout" name="horizontalLayout_3" stretch="1,3,1,1,1,1,1,1">
+                  <layout class="QHBoxLayout" name="horizontalLayout_3" stretch="1,9,1,1,1,1,1,1">
                     <item>
                       <widget class="QLineEdit" name="band_field">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="placeholderText">
                           <string>000M</string>
@@ -659,14 +693,15 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QLineEdit" name="freq_field">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="placeholderText">
                           <string>000000000</string>
@@ -674,14 +709,15 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QLineEdit" name="mode_field">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="placeholderText">
                           <string>Mode</string>
@@ -702,26 +738,28 @@
                       </spacer>
                     </item>
                     <item>
                       <widget class="QLabel" name="label_3">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="text">
                           <string>RST TX:</string>
                         </property>
                       </widget>
                     </item>
                     <item>
                       <widget class="QLineEdit" name="rst_sent">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::StrongFocus</enum>
                         </property>
                         <property name="placeholderText">
                           <string>599</string>
@@ -729,26 +767,28 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QLabel" name="label_4">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="text">
                           <string>RST RX:</string>
                         </property>
                       </widget>
                     </item>
                     <item>
                       <widget class="QLineEdit" name="rst_recieved">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::StrongFocus</enum>
                         </property>
                         <property name="text">
                           <string/>
@@ -769,14 +809,15 @@
                             <horstretch>0</horstretch>
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>11</pointsize>
                           </font>
                         </property>
                         <property name="focusPolicy">
                           <enum>Qt::ClickFocus</enum>
                         </property>
                         <property name="placeholderText">
                           <string>Comments</string>
```

### Comparing `augratin-23.5.16.1/augratin/data/k6gte-augratin-128.png` & `augratin-23.5.17.1/augratin/data/k6gte-augratin-128.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16.1/augratin/data/k6gte-augratin-32.png` & `augratin-23.5.17.1/augratin/data/k6gte-augratin-32.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16.1/augratin/data/k6gte-augratin-64.png` & `augratin-23.5.17.1/augratin/data/k6gte-augratin-64.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16.1/augratin/lib/cat_interface.py` & `augratin-23.5.17.1/augratin/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16.1/augratin/lib/omnirig_interface.py` & `augratin-23.5.17.1/augratin/lib/omnirig_interface.py`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16.1/augratin.egg-info/PKG-INFO` & `augratin-23.5.17.1/augratin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.5.16.1
+Version: 23.5.17.1
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -52,14 +52,15 @@
 All contacts are stored in an ADIF file in your home directory,
 which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
+- [23-5-17] Reworked bandmap display. Spots with QRT in comment are now muted. Center bandmap on RX freq when changing vfo or zooming display.
 - [23-5-15] Start big code changes to impliment better bandmap.
 - [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
 
 ## Installing, Updating, Running, Removing
```

### Comparing `augratin-23.5.16.1/augratin.egg-info/SOURCES.txt` & `augratin-23.5.17.1/augratin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `augratin-23.5.16.1/pyproject.toml` & `augratin-23.5.17.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "augratin" 
-version = "23.5.16.1"
+version = "23.5.17.1"
 description = "An aid for POTA hunters"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
```

