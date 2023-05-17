# Comparing `tmp/mwxlib-0.83.3-py3-none-any.whl.zip` & `tmp/mwxlib-0.83.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 161815 bytes, number of entries: 22
+Zip file size: 161800 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2520 b- defN 23-May-02 16:40 mwx/__init__.py
 -rw-rw-rw-  2.0 fat    43445 b- defN 23-May-02 17:15 mwx/controls.py
--rw-rw-rw-  2.0 fat    73310 b- defN 23-May-17 11:19 mwx/framework.py
--rw-rw-rw-  2.0 fat    69516 b- defN 23-May-17 11:19 mwx/graphman.py
+-rw-rw-rw-  2.0 fat    73243 b- defN 23-May-17 15:10 mwx/framework.py
+-rw-rw-rw-  2.0 fat    69534 b- defN 23-May-17 15:10 mwx/graphman.py
 -rw-rw-rw-  2.0 fat    46248 b- defN 23-Feb-21 08:49 mwx/images.py
 -rw-rw-rw-  2.0 fat    36017 b- defN 23-May-17 04:56 mwx/matplot2.py
 -rw-rw-rw-  2.0 fat    68253 b- defN 23-May-17 11:19 mwx/matplot2g.py
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
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-17 11:21 mwxlib-0.83.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-May-17 11:21 mwxlib-0.83.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-17 11:21 mwxlib-0.83.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-May-17 11:21 mwxlib-0.83.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-May-17 11:21 mwxlib-0.83.3.dist-info/RECORD
-22 files, 614142 bytes uncompressed, 159313 bytes compressed:  74.1%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-17 15:30 mwxlib-0.83.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-May-17 15:30 mwxlib-0.83.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-17 15:30 mwxlib-0.83.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-May-17 15:30 mwxlib-0.83.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-May-17 15:30 mwxlib-0.83.4.dist-info/RECORD
+22 files, 614093 bytes uncompressed, 159298 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.83.3.dist-info/LICENSE
+Filename: mwxlib-0.83.4.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.83.3.dist-info/METADATA
+Filename: mwxlib-0.83.4.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.83.3.dist-info/WHEEL
+Filename: mwxlib-0.83.4.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.83.3.dist-info/top_level.txt
+Filename: mwxlib-0.83.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.83.3.dist-info/RECORD
+Filename: mwxlib-0.83.4.dist-info/RECORD
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
-__version__ = "0.83.3"
+__version__ = "0.83.4"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
@@ -1406,26 +1406,23 @@
                     nb.Selection = j # the focus is moved
                 break
         else:
             return
         if show is None:
             show = not pane.IsShown() # toggle show
         
-        ## Modify aui pane floating position when it is shown,
-        ## Note: This is a known bug in wxWidgets 3.17--3.20,
-        ##       and will be fixed in wxPython 4.2.1.
-        if show:
-            w, h = wx.DisplaySize()
-            x, y = pane.floating_pos
-            if x > 2*w or y > h:
-                pane.floating_pos = wx.GetMousePosition()
-        
         if wnd and win.IsShown(): # restore focus
             wnd.SetFocus()
         
+        ## Modify the floating position of the pane when displayed.
+        ## Note: This is a known bug in wxWidgets 3.17 -- 3.20,
+        ##       and will be fixed in wxPython 4.2.1.
+        if wx.Display.GetFromWindow(pane.window) == -1:
+            pane.floating_pos = wx.GetMousePosition()
+        
         nb.Show(show)
         pane.Show(show)
         self._mgr.Update()
     
     ## --------------------------------
     ## Actions for handler
     ## --------------------------------
```

## mwx/graphman.py

```diff
@@ -899,27 +899,28 @@
     
     def _show_pane(self, name, show=True):
         """Show named pane window (internal use only)."""
         pane = self.get_pane(name)
         plug = self.get_plug(name)
         if plug:
             nb = plug.__notebook # given when load_plug
-            if nb:
-                if show:
-                    nb.SetSelection(nb.GetPageIndex(plug))
+            if nb and show:
+                nb.SetSelection(nb.GetPageIndex(plug))
             if show:
-                ## Modify aui pane floating position when it is shown,
-                ## to address a known BUG with wxWidgets 3.17 -- 3.20.
-                if wx.Display.GetFromWindow(pane.window) == -1:
-                    pane.floating_pos = wx.GetMousePosition()
                 if not pane.IsShown():
                     plug.handler('page_shown', plug)
             else:
                 if pane.IsShown():
                     plug.handler('page_closed', plug)
+        
+        ## Modify the floating position of the pane when displayed.
+        ## Note: This is a known bug in wxWidgets 3.17 -- 3.20,
+        ##       and will be fixed in wxPython 4.2.1.
+        if wx.Display.GetFromWindow(pane.window) == -1:
+            pane.floating_pos = wx.GetMousePosition()
         pane.Show(show)
     
     def update_pane(self, name, show=False, **kwargs):
         """Update the layout of the pane.
         
         Note:
             This is called automatically from load_plug,
```

## Comparing `mwxlib-0.83.3.dist-info/LICENSE` & `mwxlib-0.83.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.83.3.dist-info/METADATA` & `mwxlib-0.83.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.83.3
+Version: 0.83.4
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mwxlib-0.83.3.dist-info/RECORD` & `mwxlib-0.83.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 mwx/__init__.py,sha256=bSRdncjfSCKycMFQVnagOi9R2vUCC5snGkjea7jqPgU,2520
 mwx/controls.py,sha256=7hnSimA3bKDgTct29l6Hqpq7BCKqCeOjZJ6JQ1xjh7I,43445
-mwx/framework.py,sha256=6fAXOKEmMDHTr1l6aazNpOnQ23xHV1A3rmBCi-FFvJs,73310
-mwx/graphman.py,sha256=ICYNl2qSZ7TetvI4J_r2_e3hWGFoeZghd2MvxMnHP9M,69516
+mwx/framework.py,sha256=_WT2Pod18b2CFYuJTNnglpWph-A4NWdPLFCmyKFzb78,73243
+mwx/graphman.py,sha256=Edw2pZKghWGkbR_AV9PDWQpZz6q8XstTL5Q-xDrAce4,69534
 mwx/images.py,sha256=9e8X7OpJ6Z3fF3ez17P_qk2D1NMO10-lN8TCtulAqT0,46248
 mwx/matplot2.py,sha256=W_FpY0S33crCAh7N9YTXo-jgYzj8uL9gqXkekfQo7Pk,36017
 mwx/matplot2g.py,sha256=cBuLMnQt3XSKQL9io0XJb_v8Lv0pO9hm0IMjVIERtu4,68253
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
-mwxlib-0.83.3.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
-mwxlib-0.83.3.dist-info/METADATA,sha256=qNvQqhKMdvPW0cUvy2vpjh3DOhL5UlY989rH-Fyb_rE,1893
-mwxlib-0.83.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mwxlib-0.83.3.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
-mwxlib-0.83.3.dist-info/RECORD,,
+mwxlib-0.83.4.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
+mwxlib-0.83.4.dist-info/METADATA,sha256=j9WUxZBLCznmBJsIjheewsBQpN15LmpWdnSWP8rWnuI,1893
+mwxlib-0.83.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mwxlib-0.83.4.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
+mwxlib-0.83.4.dist-info/RECORD,,
```

