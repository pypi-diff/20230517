# Comparing `tmp/pyfreebody-0.2.1.tar.gz` & `tmp/pyfreebody-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfreebody-0.2.1.tar", last modified: Sat Jan  8 18:38:17 2022, max compression
+gzip compressed data, was "pyfreebody-0.3.0.tar", last modified: Wed May 17 13:48:21 2023, max compression
```

## Comparing `pyfreebody-0.2.1.tar` & `pyfreebody-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,28 @@
-drwxr-xr-x   0 velo      (1000) velo      (1000)        0 2022-01-08 18:38:17.864794 pyfreebody-0.2.1/
--rw-r--r--   0 velo      (1000) velo      (1000)    16725 2022-01-07 18:59:35.000000 pyfreebody-0.2.1/LICENSE
--rw-r--r--   0 velo      (1000) velo      (1000)      344 2022-01-08 18:38:17.864794 pyfreebody-0.2.1/PKG-INFO
--rw-r--r--   0 velo      (1000) velo      (1000)      330 2022-01-08 18:31:03.000000 pyfreebody-0.2.1/README.md
-drwxr-xr-x   0 velo      (1000) velo      (1000)        0 2022-01-08 18:38:17.864794 pyfreebody-0.2.1/pyfreebody/
--rw-r--r--   0 velo      (1000) velo      (1000)        0 2022-01-07 09:20:20.000000 pyfreebody-0.2.1/pyfreebody/__init__.py
--rw-r--r--   0 velo      (1000) velo      (1000)     4743 2022-01-08 18:31:03.000000 pyfreebody-0.2.1/pyfreebody/pyfreebody.py
-drwxr-xr-x   0 velo      (1000) velo      (1000)        0 2022-01-08 18:38:17.864794 pyfreebody-0.2.1/pyfreebody.egg-info/
--rw-r--r--   0 velo      (1000) velo      (1000)      344 2022-01-08 18:38:17.000000 pyfreebody-0.2.1/pyfreebody.egg-info/PKG-INFO
--rw-r--r--   0 velo      (1000) velo      (1000)      243 2022-01-08 18:38:17.000000 pyfreebody-0.2.1/pyfreebody.egg-info/SOURCES.txt
--rw-r--r--   0 velo      (1000) velo      (1000)        1 2022-01-08 18:38:17.000000 pyfreebody-0.2.1/pyfreebody.egg-info/dependency_links.txt
--rw-r--r--   0 velo      (1000) velo      (1000)        7 2022-01-08 18:38:17.000000 pyfreebody-0.2.1/pyfreebody.egg-info/requires.txt
--rw-r--r--   0 velo      (1000) velo      (1000)       11 2022-01-08 18:38:17.000000 pyfreebody-0.2.1/pyfreebody.egg-info/top_level.txt
--rw-r--r--   0 velo      (1000) velo      (1000)       38 2022-01-08 18:38:17.864794 pyfreebody-0.2.1/setup.cfg
--rw-r--r--   0 velo      (1000) velo      (1000)      472 2022-01-08 18:38:09.000000 pyfreebody-0.2.1/setup.py
+drwxr-xr-x   0 velocitatem  (1000) velocitatem  (1000)        0 2023-05-17 13:48:21.972133 pyfreebody-0.3.0/
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)       94 2023-05-17 13:17:54.000000 pyfreebody-0.3.0/.gitignore
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)    16725 2023-05-17 13:17:54.000000 pyfreebody-0.3.0/LICENSE
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)      152 2023-05-17 13:48:21.972133 pyfreebody-0.3.0/PKG-INFO
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)      330 2023-05-17 13:17:54.000000 pyfreebody-0.3.0/README.md
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)   119788 2023-05-17 13:17:54.000000 pyfreebody-0.3.0/SourceCodePro-Regular.ttf
+drwxr-xr-x   0 velocitatem  (1000) velocitatem  (1000)        0 2023-05-17 13:48:21.972133 pyfreebody-0.3.0/demos/
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)       48 2023-05-17 13:17:54.000000 pyfreebody-0.3.0/demos/.gitignore
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)      467 2023-05-17 13:17:54.000000 pyfreebody-0.3.0/demos/demo.org
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)      233 2023-05-17 13:27:20.000000 pyfreebody-0.3.0/demos/demo1.py
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)     2721 2023-05-17 13:17:54.000000 pyfreebody-0.3.0/docs.org
+drwxr-xr-x   0 velocitatem  (1000) velocitatem  (1000)        0 2023-05-17 13:48:21.972133 pyfreebody-0.3.0/examples/
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)    13181 2023-05-17 13:17:54.000000 pyfreebody-0.3.0/examples/simple.out.png
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)   137629 2023-05-17 13:17:54.000000 pyfreebody-0.3.0/examples/simple.png
+drwxr-xr-x   0 velocitatem  (1000) velocitatem  (1000)        0 2023-05-17 13:48:21.972133 pyfreebody-0.3.0/pyfreebody/
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)   119788 2023-05-17 13:17:54.000000 pyfreebody-0.3.0/pyfreebody/SourceCodePro-Regular.ttf
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)        0 2023-05-17 13:22:33.000000 pyfreebody-0.3.0/pyfreebody/__init__.py
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)     4924 2023-05-17 13:38:47.000000 pyfreebody-0.3.0/pyfreebody/pyfreebody.py
+drwxr-xr-x   0 velocitatem  (1000) velocitatem  (1000)        0 2023-05-17 13:48:21.972133 pyfreebody-0.3.0/pyfreebody/tests/
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)      286 2023-05-17 13:17:54.000000 pyfreebody-0.3.0/pyfreebody/tests/test1.py
+drwxr-xr-x   0 velocitatem  (1000) velocitatem  (1000)        0 2023-05-17 13:48:21.972133 pyfreebody-0.3.0/pyfreebody.egg-info/
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)      152 2023-05-17 13:48:21.000000 pyfreebody-0.3.0/pyfreebody.egg-info/PKG-INFO
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)      443 2023-05-17 13:48:21.000000 pyfreebody-0.3.0/pyfreebody.egg-info/SOURCES.txt
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)        1 2023-05-17 13:48:21.000000 pyfreebody-0.3.0/pyfreebody.egg-info/dependency_links.txt
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)        7 2023-05-17 13:48:21.000000 pyfreebody-0.3.0/pyfreebody.egg-info/requires.txt
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)       11 2023-05-17 13:48:21.000000 pyfreebody-0.3.0/pyfreebody.egg-info/top_level.txt
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)       38 2023-05-17 13:48:21.972133 pyfreebody-0.3.0/setup.cfg
+-rw-r--r--   0 velocitatem  (1000) velocitatem  (1000)      315 2023-05-17 13:48:10.000000 pyfreebody-0.3.0/setup.py
```

### Comparing `pyfreebody-0.2.1/LICENSE` & `pyfreebody-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfreebody-0.2.1/pyfreebody/pyfreebody.py` & `pyfreebody-0.3.0/pyfreebody/pyfreebody.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from random import randint
 from PIL import Image, ImageDraw, ImageFont
 import math
 from datetime import datetime
 import enum
 import os
 
+class SystemType(enum.Enum):
+    basic = 0
+    inclinedPlane = 1
 
 class System:
     def __init__(self, sysType=SystemType.basic, incline=0):
         self.sysType = sysType
         self.incline = incline
 
 class Body:
@@ -25,17 +28,14 @@
 
 class Direction(enum.Enum):
     up = math.pi /2
     down = (3 * math.pi) / 2
     left = math.pi
     right = 0
 
-class SystemType(enum.Enum):
-    basic = 0
-    inclinedPlane = 1
 
 class Freebody:
 
     def __init__ (self,name="empty", mass=24, sysType = SystemType.basic, incline=math.pi/6):
         body = Body(name, mass)
         self.system = System(sysType, incline)
         self.body = body
@@ -95,27 +95,33 @@
         canvas.text((center-(mtsw/2), center+(mtsh/2)), masstxt, fill = black, font = font)
 
         canvas.text((10,size-30), str(self.body.name), fill = black, font = font)
         now = datetime.now()
         dtstr = now.strftime("%d-%m-%Y %H:%M:%S")
         path = "pyfreebody-"+self.body.name+".png"
         img.save(path)
+        # try to open the image
+        try:
+            img.show()
+        except:
+            print("Image saved to: "+path)
+
         return path
 
 
 size = 600
 arrowHeadSize = 15
 cw = 400 * 0.1
 center = size / 2;
 rectW = size * 0.4
 
 black = (0,0,0)
 white = (225,225,225)
 
-home = os.path.expanduser("~")
+home = os.path.dirname(os.path.abspath(__file__)) #<-- absolute dir the script is in
 font = ImageFont.truetype(home+"/pyfreebody.ttf", 20)
 fontTag = ImageFont.truetype(home+"/pyfreebody.ttf", 12)
 
 def makeRectangle(l, w, theta, offset=(0,0)):
     c, s = math.cos(theta), math.sin(theta)
     rectCoords = [(l/2.0, w/2.0), (l/2.0, -w/2.0), (-l/2.0, -w/2.0), (-l/2.0, w/2.0)]
     return [(c*x-s*y+offset[0], s*x+c*y+offset[1]) for (x,y) in rectCoords]
@@ -155,8 +161,7 @@
     canvas.text((5,5+i*20), text, fill = color, font = font)
 
 def CreatArrow(canvas, force, color):
     arrowBase = ArrowCordinates(force)
     canvas.line(arrowBase, width=10, fill = color)
     canvas.text(tagCordinates(arrowBase), "F"+(force.name[0:1]).lower(), font=fontTag, fill = black)
     #canvas.polygon(ArrowHeadCordinates(arrowBase), fill = color)
-
```

