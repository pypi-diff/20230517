# Comparing `tmp/materialyoucolor-1.1.tar.gz` & `tmp/materialyoucolor-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "materialyoucolor-1.1.tar", last modified: Thu Apr 27 16:45:47 2023, max compression
+gzip compressed data, was "materialyoucolor-1.2.tar", last modified: Wed May 17 12:03:34 2023, max compression
```

## Comparing `materialyoucolor-1.1.tar` & `materialyoucolor-1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.593905 materialyoucolor-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-27 16:45:26.000000 materialyoucolor-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-27 16:45:47.593905 materialyoucolor-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-27 16:45:26.000000 materialyoucolor-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.585905 materialyoucolor-1.1/materialyoucolor/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/blend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/blend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/blend/blend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/hct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/hct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/hct/cam16.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/hct/hct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/hct/viewing_conditions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/palettes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/palettes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/palettes/core_palette.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/palettes/tonal_palette.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/scheme/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/scheme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/scheme/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor/score/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/score/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/score/score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.593905 materialyoucolor-1.1/materialyoucolor/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15411 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/color_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/math_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-27 16:45:26.000000 materialyoucolor-1.1/materialyoucolor/utils/theme_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:47.589905 materialyoucolor-1.1/materialyoucolor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 16:45:47.000000 materialyoucolor-1.1/materialyoucolor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:45:47.593905 materialyoucolor-1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      750 2023-04-27 16:45:26.000000 materialyoucolor-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:34.617168 materialyoucolor-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 12:03:23.000000 materialyoucolor-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-17 12:03:34.617168 materialyoucolor-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-17 12:03:23.000000 materialyoucolor-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:34.613168 materialyoucolor-1.2/materialyoucolor/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:34.617168 materialyoucolor-1.2/materialyoucolor/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/blend/blend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:34.617168 materialyoucolor-1.2/materialyoucolor/hct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/hct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/hct/cam16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/hct/hct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/hct/viewing_conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:34.617168 materialyoucolor-1.2/materialyoucolor/palettes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/palettes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/palettes/core_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/palettes/tonal_palette.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:34.617168 materialyoucolor-1.2/materialyoucolor/scheme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/scheme/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:34.617168 materialyoucolor-1.2/materialyoucolor/score/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/score/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/score/score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:34.617168 materialyoucolor-1.2/materialyoucolor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15411 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/utils/color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/utils/math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-17 12:03:23.000000 materialyoucolor-1.2/materialyoucolor/utils/theme_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:03:34.617168 materialyoucolor-1.2/materialyoucolor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-17 12:03:34.000000 materialyoucolor-1.2/materialyoucolor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-17 12:03:34.000000 materialyoucolor-1.2/materialyoucolor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:03:34.000000 materialyoucolor-1.2/materialyoucolor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 12:03:34.000000 materialyoucolor-1.2/materialyoucolor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 12:03:34.000000 materialyoucolor-1.2/materialyoucolor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:03:34.617168 materialyoucolor-1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-05-17 12:03:23.000000 materialyoucolor-1.2/setup.py
```

### Comparing `materialyoucolor-1.1/LICENSE` & `materialyoucolor-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1/PKG-INFO` & `materialyoucolor-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: materialyoucolor
-Version: 1.1
+Version: 1.2
 Summary: Material You color generation algorithms in pure python!
 Author: Ansh Dadwal
 Author-email: anshdadwal298@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # materialyoucolor-pyhton
```

### Comparing `materialyoucolor-1.1/README.md` & `materialyoucolor-1.2/README.md`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1/materialyoucolor/blend/blend.py` & `materialyoucolor-1.2/materialyoucolor/blend/blend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from materialyoucolor.hct.cam16 import Cam16
 from materialyoucolor.hct.hct import Hct
 from materialyoucolor.utils.math_utils import sanitizeDegreesDouble, differenceDegrees
+from materialyoucolor.utils.color_utils import lstarFromArgb
 
 
 class Blend:
     @staticmethod
     def harmonize(designColor, sourceColor):
         fromHct = Hct.fromInt(designColor)
         toHct = Hct.fromInt(sourceColor)
```

### Comparing `materialyoucolor-1.1/materialyoucolor/hct/cam16.py` & `materialyoucolor-1.2/materialyoucolor/hct/cam16.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,9 @@
-from materialyoucolor.utils.color_utils import (
-    redFromArgb,
-    greenFromArgb,
-    blueFromArgb,
-    lstarFromArgb,
-    linearized,
-    argbFromXyz,
-)
-from materialyoucolor.utils.math_utils import signum, sanitizeDegreesDouble, clampDouble
+from materialyoucolor.utils.color_utils import linearized, argbFromXyz
+from materialyoucolor.utils.math_utils import signum
 from materialyoucolor.hct.viewing_conditions import ViewingConditions
 import math
 
 
 class Cam16:
     def __init__(self, hue, chroma, j, q, m, s, jstar, astar, bstar):
         self.hue = hue
```

### Comparing `materialyoucolor-1.1/materialyoucolor/hct/hct.py` & `materialyoucolor-1.2/materialyoucolor/hct/hct.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1/materialyoucolor/hct/viewing_conditions.py` & `materialyoucolor-1.2/materialyoucolor/hct/viewing_conditions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from materialyoucolor.utils.color_utils import whitePointD65, yFromLstar
-from materialyoucolor.utils.math_utils import clampInt, lerp
+from materialyoucolor.utils.math_utils import lerp
 import math
 
 
 class ViewingConditions:
+    
+    DEFAULT = None
+
     def __init__(self, n, aw, nbb, ncb, c, nc, rgbD, fl, fLRoot, z):
         self.n = n
         self.aw = aw
         self.nbb = nbb
         self.ncb = ncb
         self.c = c
         self.nc = nc
         self.rgbD = rgbD
         self.fl = fl
         self.fLRoot = fLRoot
         self.z = z
-
+    
     @staticmethod
     def make(
         whitePoint=whitePointD65(),
         adaptingLuminance=(200.0 / math.pi) * yFromLstar(50.0) / 100.0,
         backgroundLstar=50.0,
         surround=2.0,
         discountingIlluminant=False,
@@ -65,9 +68,8 @@
             (400.0 * rgbAFactors[0]) / (rgbAFactors[0] + 27.13),
             (400.0 * rgbAFactors[1]) / (rgbAFactors[1] + 27.13),
             (400.0 * rgbAFactors[2]) / (rgbAFactors[2] + 27.13),
         ]
         aw = (2.0 * rgbA[0] + rgbA[1] + 0.05 * rgbA[2]) * nbb
         return ViewingConditions(n, aw, nbb, ncb, c, nc, rgbD, fl, pow(fl, 0.25), z)
 
-
 ViewingConditions.DEFAULT = ViewingConditions.make()
```

### Comparing `materialyoucolor-1.1/materialyoucolor/palettes/core_palette.py` & `materialyoucolor-1.2/materialyoucolor/palettes/core_palette.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 class CorePalette:
     def __init__(self, argb):
         hct = Hct.fromInt(argb)
         hue = hct.hue
         self.a1 = TonalPalette.fromHueAndChroma(hue, max(48, hct.chroma))
         self.a2 = TonalPalette.fromHueAndChroma(hue, 16)
         self.a3 = TonalPalette.fromHueAndChroma(hue + 60, 24)
-        self.n1 = TonalPalette.fromHueAndChroma(hue, 4)
+        self.n1 = TonalPalette.fromHueAndChroma(hue, 6)
         self.n2 = TonalPalette.fromHueAndChroma(hue, 8)
         self.error = TonalPalette.fromHueAndChroma(25, 84)
 
     @staticmethod
     def of(argb):
         return CorePalette(argb)
```

### Comparing `materialyoucolor-1.1/materialyoucolor/palettes/tonal_palette.py` & `materialyoucolor-1.2/materialyoucolor/palettes/tonal_palette.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1/materialyoucolor/scheme/scheme.py` & `materialyoucolor-1.2/materialyoucolor/scheme/scheme.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1/materialyoucolor/score/score.py` & `materialyoucolor-1.2/materialyoucolor/score/score.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from materialyoucolor.hct.cam16 import Cam16
 from materialyoucolor.utils.color_utils import lstarFromArgb
 from materialyoucolor.utils.math_utils import sanitizeDegreesInt, differenceDegrees
-from typing import List, Tuple, Dict
+from typing import List, Dict
 from collections import defaultdict
-import math
 
 TARGET_CHROMA = 48.0
 WEIGHT_PROPORTION = 0.7
 WEIGHT_CHROMA_ABOVE = 0.3
 WEIGHT_CHROMA_BELOW = 0.1
 CUTOFF_CHROMA = 15.0
 CUTOFF_TONE = 10.0
@@ -36,15 +35,15 @@
 def Score(
     colors_to_population: Dict[int, int], content_color: bool = False
 ) -> List[int]:
 
     population_sum = sum(colors_to_population.values())
     colors_to_proportion = {}
     colors_to_cam = {}
-    hue_proportions = defaultdict(int)
+    hue_proportions = defaultdict(float)
 
     for color, population in colors_to_population.items():
         proportion = population / population_sum
         colors_to_proportion[color] = proportion
         cam = Cam16.fromInt(color)
         colors_to_cam[color] = cam
         hue = round(cam.hue)
```

### Comparing `materialyoucolor-1.1/materialyoucolor/utils/color_utils.py` & `materialyoucolor-1.2/materialyoucolor/utils/color_utils.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1/materialyoucolor/utils/math_utils.py` & `materialyoucolor-1.2/materialyoucolor/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1/materialyoucolor/utils/string_utils.py` & `materialyoucolor-1.2/materialyoucolor/utils/string_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from materialyoucolor.utils.color_utils import redFromArgb, greenFromArgb, blueFromArgb
+from materialyoucolor.utils.color_utils import redFromArgb, greenFromArgb, blueFromArgb, rshift
 
 def hexFromArgb(argb):
     r = redFromArgb(argb)
     g = greenFromArgb(argb)
     b = blueFromArgb(argb)
     outParts = [f"{r:x}", f"{g:x}", f"{b:x}"]
     for i, part in enumerate(outParts):
@@ -40,15 +40,15 @@
 def parseIntHex(value):
     return int(value, 16)
 
 def argbFromRgb(r, g, b, a=255) -> int:
     return (a << 24) | (r << 16) | (g << 8) | b
 
 
-def rgbFromArgb(self, argb):
+def rgbFromArgb(argb):
     return (
         ((argb >> 16) & 0xFF) / 255,
         ((argb >> 8) & 0xFF) / 255,
         (argb & 0xFF) / 255,
         1,
     )
```

### Comparing `materialyoucolor-1.1/materialyoucolor/utils/theme_utils.py` & `materialyoucolor-1.2/materialyoucolor/utils/theme_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,11 +91,7 @@
             "neutral": palette.n1,
             "neutralVariant": palette.n2,
             "error": palette.error,
         },
         "customColors": [customColor(c, blend=True, source_color=source) for c in customColors],
     }
 
-
-def themeFromImage(image, customColors=[]):
-    source = sourceColorFromImage(image)
-    return themeFromSourceColor(source, customColors)
```

### Comparing `materialyoucolor-1.1/materialyoucolor.egg-info/PKG-INFO` & `materialyoucolor-1.2/materialyoucolor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: materialyoucolor
-Version: 1.1
+Version: 1.2
 Summary: Material You color generation algorithms in pure python!
 Author: Ansh Dadwal
 Author-email: anshdadwal298@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # materialyoucolor-pyhton
```

### Comparing `materialyoucolor-1.1/materialyoucolor.egg-info/SOURCES.txt` & `materialyoucolor-1.2/materialyoucolor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1/setup.py` & `materialyoucolor-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from setuptools import find_packages, setup
 
 assert sys.version_info >= (3, 7, 0), "Materialyoucolor requires Python 3.7+"
 
 with open("README.md", "r") as f:
     long_description = f.read()
     f.close()
+
 with open("materialyoucolor/__init__.py","r") as file:
     VERSION = file.read().split("=")[-1].strip()
     file.close()
     
 setup(
     name="materialyoucolor",
     version=VERSION,
```

