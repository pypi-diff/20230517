# Comparing `tmp/mwxlib-0.83.2-py3-none-any.whl.zip` & `tmp/mwxlib-0.83.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 161723 bytes, number of entries: 22
+Zip file size: 161815 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2520 b- defN 23-May-02 16:40 mwx/__init__.py
 -rw-rw-rw-  2.0 fat    43445 b- defN 23-May-02 17:15 mwx/controls.py
--rw-rw-rw-  2.0 fat    73310 b- defN 23-May-17 05:03 mwx/framework.py
--rw-rw-rw-  2.0 fat    69631 b- defN 23-May-17 04:15 mwx/graphman.py
+-rw-rw-rw-  2.0 fat    73310 b- defN 23-May-17 11:19 mwx/framework.py
+-rw-rw-rw-  2.0 fat    69516 b- defN 23-May-17 11:19 mwx/graphman.py
 -rw-rw-rw-  2.0 fat    46248 b- defN 23-Feb-21 08:49 mwx/images.py
 -rw-rw-rw-  2.0 fat    36017 b- defN 23-May-17 04:56 mwx/matplot2.py
--rw-rw-rw-  2.0 fat    67638 b- defN 23-May-17 05:03 mwx/matplot2g.py
+-rw-rw-rw-  2.0 fat    68253 b- defN 23-May-17 11:19 mwx/matplot2g.py
 -rw-rw-rw-  2.0 fat    27606 b- defN 23-Apr-27 09:45 mwx/matplot2lg.py
 -rw-rw-rw-  2.0 fat     6878 b- defN 23-Feb-21 08:50 mwx/mgplt.py
 -rw-rw-rw-  2.0 fat   138127 b- defN 23-May-17 04:56 mwx/nutshell.py
 -rw-rw-rw-  2.0 fat    37351 b- defN 23-May-16 17:41 mwx/utilus.py
 -rw-rw-rw-  2.0 fat    11343 b- defN 23-May-16 07:42 mwx/wxmon.py
 -rw-rw-rw-  2.0 fat    19367 b- defN 23-May-16 07:42 mwx/wxpdb.py
 -rw-rw-rw-  2.0 fat     5254 b- defN 23-May-16 07:42 mwx/wxwil.py
 -rw-rw-rw-  2.0 fat     7424 b- defN 23-May-16 07:42 mwx/wxwit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-23 14:06 mwx/py/__init__.py
 -rw-rw-rw-  2.0 fat    16794 b- defN 23-Apr-27 09:45 mwx/py/filling.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-17 05:05 mwxlib-0.83.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-May-17 05:05 mwxlib-0.83.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-17 05:05 mwxlib-0.83.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-May-17 05:05 mwxlib-0.83.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-May-17 05:05 mwxlib-0.83.2.dist-info/RECORD
-22 files, 613642 bytes uncompressed, 159221 bytes compressed:  74.1%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-17 11:21 mwxlib-0.83.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-May-17 11:21 mwxlib-0.83.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-17 11:21 mwxlib-0.83.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-May-17 11:21 mwxlib-0.83.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-May-17 11:21 mwxlib-0.83.3.dist-info/RECORD
+22 files, 614142 bytes uncompressed, 159313 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.83.2.dist-info/LICENSE
+Filename: mwxlib-0.83.3.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.83.2.dist-info/METADATA
+Filename: mwxlib-0.83.3.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.83.2.dist-info/WHEEL
+Filename: mwxlib-0.83.3.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.83.2.dist-info/top_level.txt
+Filename: mwxlib-0.83.3.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.83.2.dist-info/RECORD
+Filename: mwxlib-0.83.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mwx/framework.py

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 """mwxlib framework
 
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 """
-__version__ = "0.83.2"
+__version__ = "0.83.3"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
@@ -1484,15 +1484,15 @@
         self.inspector.highlight(obj, *args, **kwargs)
     
     ## Note: history 変数に余計な文字列が入らないようにする
     @postcall
     def debug(self, obj, *args, **kwargs):
         if isinstance(obj, wx.Object) or obj is None:
             if args or kwargs:
-                self.message("- args:{} and kwargs:{} were given,"
+                self.message("- Args:{} and kwargs:{} were given,"
                              " but ignored for object monitoring.")
             self.monitor.watch(obj)
             if obj:
                 self.popup_window(self.monitor, focus=0)
                 self.linfo.watch(obj.__dict__)
                 self.ginfo.watch({})
         elif isinstance(obj, type(print)):
```

## mwx/graphman.py

```diff
@@ -905,19 +905,16 @@
             nb = plug.__notebook # given when load_plug
             if nb:
                 if show:
                     nb.SetSelection(nb.GetPageIndex(plug))
             if show:
                 ## Modify aui pane floating position when it is shown,
                 ## to address a known BUG with wxWidgets 3.17 -- 3.20.
-                if wx.VERSION <= (4,2,0):
-                    w, h = wx.DisplaySize()
-                    x, y = pane.floating_pos
-                    if x > 2*w or y > h:
-                        pane.floating_pos = wx.GetMousePosition()
+                if wx.Display.GetFromWindow(pane.window) == -1:
+                    pane.floating_pos = wx.GetMousePosition()
                 if not pane.IsShown():
                     plug.handler('page_shown', plug)
             else:
                 if pane.IsShown():
                     plug.handler('page_closed', plug)
         pane.Show(show)
```

## mwx/matplot2g.py

```diff
@@ -1038,34 +1038,47 @@
             else:
                 self.message("Read image from clipboard")
                 self.load(Clipboard.imread())
         except Exception as e:
             self.message("- No data in clipboard: {}".format(e))
             traceback.print_exc()
     
+    def destroy_colorbar(self):
+        if self.cbar:
+            self.cbar = None
+            cax = self.figure.axes[1]
+            self.figure.delaxes(cax)
+            self.canvas.draw_idle()
+            self.handler.unbind('frame_cmapped', self.update_colorbar)
+            self.handler.unbind('frame_shown', self.update_colorbar)
+    
+    def update_colorbar(self, frame):
+        if self.cbar:
+            self.cbar.update_normal(frame)
+            self.canvas.draw_idle()
+            self.figure.draw_without_rendering()
+    
     def create_colorbar(self):
         """Make a colorbar.
         The colorbar is plotted in self.figure.axes[1] (second axes)
         """
         from mpl_toolkits.axes_grid1 import make_axes_locatable
         if self.frame:
             divider = make_axes_locatable(self.axes)
             cax = divider.append_axes('right', size=0.1, pad=0.1)
-            cbar = self.figure.colorbar(self.frame, cax=cax)
-            @self.handler.bind('frame_cmapped')
-            @self.handler.bind('frame_shown')
-            def update_cmap(frame):
-                cbar.update_normal(frame)
-                cbar.draw_all()
-                self.canvas.draw_idle()
-            update_cmap(self.frame)
+            self.cbar = self.figure.colorbar(self.frame, cax=cax)
+            self.update_colorbar(self.frame)
+            self.handler.bind('frame_cmapped', self.update_colorbar)
+            self.handler.bind('frame_shown', self.update_colorbar)
         else:
-            self['*dummy*'] = np.random.rand(2,2) # dummy
-            self.create_colorbar()
-            del self['*dummy*']
+            self.message("- A frame must exist to create a colorbar.")
+            ## self['*dummy*'] = np.random.rand(2,2) # dummy
+            ## self.create_colorbar()
+            ## del self['*dummy*']
+            pass
     
     ## --------------------------------
     ## matplotlib interfaces
     ## --------------------------------
     
     def on_pick(self, evt): #<matplotlib.backend_bases.PickEvent>
         """Pickup image and other arts.
@@ -1575,15 +1588,15 @@
         xm, ym = self.marked.get_data(orig=0)
         return np.array((xm, ym))
     
     @Markers.setter
     def Markers(self, v):
         x, y = v
         if len(x) > self.maxnum_markers:
-            self.message("- got too many markers ({}) to plot".format(len(x)))
+            self.message("- Got too many markers ({}) to plot".format(len(x)))
             return
         self.marked.set_data(x, y)
         self.__marksel = []
         self.update_art_of_mark()
         self.handler('mark_drawn', self.frame)
     
     @Markers.deleter
@@ -1755,15 +1768,16 @@
     def _imread(path):
         return Image.open(path)
     
     frm.graph.load(_imread(u"C:/usr/home/workspace/images/sample.bmp"), "sample")
     frm.graph.load(_imread(u"C:/usr/home/workspace/images/サンプル.bmp"), "サンプル")
     frm.graph.load(_imread(u"C:/usr/home/workspace/images/sample_circ.bmp"), "sample data")
     
-    frm.graph.newbuffer = np.uint8(255 * np.random.randn(512,512,3))
+    ## frm.graph.newbuffer = np.uint8(255 * np.random.randn(512,512,3))
+    frm.graph.newbuffer = np.float32(np.random.randn(512,512))
     frm.graph.frame.unit = 0.5
     frm.graph.create_colorbar()
     
     def _plot(graph, r=10):
         ux = uy = graph.unit
         t = np.arange(0,4,0.01) * pi
         x = r * ux * np.cos(t)
```

## Comparing `mwxlib-0.83.2.dist-info/LICENSE` & `mwxlib-0.83.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.83.2.dist-info/METADATA` & `mwxlib-0.83.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.83.2
+Version: 0.83.3
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mwxlib-0.83.2.dist-info/RECORD` & `mwxlib-0.83.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 mwx/__init__.py,sha256=bSRdncjfSCKycMFQVnagOi9R2vUCC5snGkjea7jqPgU,2520
 mwx/controls.py,sha256=7hnSimA3bKDgTct29l6Hqpq7BCKqCeOjZJ6JQ1xjh7I,43445
-mwx/framework.py,sha256=5fJ7vFf5VxwUiTDO4ynEMZmVKumkmpxELgq9iWJpMrk,73310
-mwx/graphman.py,sha256=AY5uDOwuguJdCi_7CHBHxuuO8p3AuXtdY-meIY-caIU,69631
+mwx/framework.py,sha256=6fAXOKEmMDHTr1l6aazNpOnQ23xHV1A3rmBCi-FFvJs,73310
+mwx/graphman.py,sha256=ICYNl2qSZ7TetvI4J_r2_e3hWGFoeZghd2MvxMnHP9M,69516
 mwx/images.py,sha256=9e8X7OpJ6Z3fF3ez17P_qk2D1NMO10-lN8TCtulAqT0,46248
 mwx/matplot2.py,sha256=W_FpY0S33crCAh7N9YTXo-jgYzj8uL9gqXkekfQo7Pk,36017
-mwx/matplot2g.py,sha256=STQlY5GZ7uGb0SLqkUldpZm4B3PpgEtFW_wqc--qMUg,67638
+mwx/matplot2g.py,sha256=cBuLMnQt3XSKQL9io0XJb_v8Lv0pO9hm0IMjVIERtu4,68253
 mwx/matplot2lg.py,sha256=h_aFij_7ksG2DXuYCaGmjtlcl122vZnwbMTv21Mprcg,27606
 mwx/mgplt.py,sha256=49_wpFZUEKErQmtobqrlNKDjWlAsdLft-izlqSyGPD0,6878
 mwx/nutshell.py,sha256=gKIDIFEji9x8ypPUdWmroUvPs0dTyoPg-zMnrvdJArA,138127
 mwx/utilus.py,sha256=q1DZGRNvtzk6Yavlc9XuLWMWgLS236khbiG4wa-hDj0,37351
 mwx/wxmon.py,sha256=hEXto7dD5JunPf-iv2hhcwTIILLkNPlcl6wRt20_Wqc,11343
 mwx/wxpdb.py,sha256=M_xxXzIYhAwO1IHXVkjIC4Y2JCCCGLdgPL5R4bRtp04,19367
 mwx/wxwil.py,sha256=DPXXx4OdEzvHr-_jxz9J29Ozufmb6Vr7rXVkG_LKQd0,5254
 mwx/wxwit.py,sha256=UG361QTUheO_hlSIRgkprrGUYh0IzHB8ZqOoJeeMzUs,7424
 mwx/py/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mwx/py/filling.py,sha256=f6KMBcBv7gwrl6qmJYLTL-O0Z47bWNAdTCZtUZIo8vM,16794
-mwxlib-0.83.2.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
-mwxlib-0.83.2.dist-info/METADATA,sha256=PVB3-t4dP77yT3Jt3DEb2EwVI0iFtPDeZ2LP1lIq0M8,1893
-mwxlib-0.83.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mwxlib-0.83.2.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
-mwxlib-0.83.2.dist-info/RECORD,,
+mwxlib-0.83.3.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
+mwxlib-0.83.3.dist-info/METADATA,sha256=qNvQqhKMdvPW0cUvy2vpjh3DOhL5UlY989rH-Fyb_rE,1893
+mwxlib-0.83.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mwxlib-0.83.3.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
+mwxlib-0.83.3.dist-info/RECORD,,
```

