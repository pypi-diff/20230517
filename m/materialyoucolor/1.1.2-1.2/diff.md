# Comparing `tmp/materialyoucolor-1.1.2.tar.gz` & `tmp/materialyoucolor-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "materialyoucolor-1.1.2.tar", last modified: Wed May 17 12:32:46 2023, max compression
+gzip compressed data, was "materialyoucolor-1.2.tar", last modified: Wed May 17 12:03:34 2023, max compression
```

## Comparing `materialyoucolor-1.1.2.tar` & `materialyoucolor-1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:46.792262 materialyoucolor-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-17 12:32:46.792262 materialyoucolor-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:46.788262 materialyoucolor-1.1.2/materialyoucolor/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:46.788262 materialyoucolor-1.1.2/materialyoucolor/blend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/blend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/blend/blend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:46.788262 materialyoucolor-1.1.2/materialyoucolor/hct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/hct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/hct/cam16.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/hct/hct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/hct/viewing_conditions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:46.788262 materialyoucolor-1.1.2/materialyoucolor/palettes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/palettes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/palettes/core_palette.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/palettes/tonal_palette.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:46.788262 materialyoucolor-1.1.2/materialyoucolor/scheme/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/scheme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/scheme/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:46.788262 materialyoucolor-1.1.2/materialyoucolor/score/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/score/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/score/score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:46.788262 materialyoucolor-1.1.2/materialyoucolor/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15411 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/utils/color_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/utils/math_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/materialyoucolor/utils/theme_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:32:46.788262 materialyoucolor-1.1.2/materialyoucolor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-17 12:32:46.000000 materialyoucolor-1.1.2/materialyoucolor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-17 12:32:46.000000 materialyoucolor-1.1.2/materialyoucolor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:32:46.000000 materialyoucolor-1.1.2/materialyoucolor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 12:32:46.000000 materialyoucolor-1.1.2/materialyoucolor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 12:32:46.000000 materialyoucolor-1.1.2/materialyoucolor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:32:46.792262 materialyoucolor-1.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-05-17 12:32:35.000000 materialyoucolor-1.1.2/setup.py
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

### Comparing `materialyoucolor-1.1.2/LICENSE` & `materialyoucolor-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/PKG-INFO` & `materialyoucolor-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: materialyoucolor
-Version: 1.1.2
+Version: 1.2
 Summary: Material You color generation algorithms in pure python!
 Author: Ansh Dadwal
 Author-email: anshdadwal298@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # materialyoucolor-pyhton
```

### Comparing `materialyoucolor-1.1.2/README.md` & `materialyoucolor-1.2/README.md`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/materialyoucolor/blend/blend.py` & `materialyoucolor-1.2/materialyoucolor/blend/blend.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/materialyoucolor/hct/cam16.py` & `materialyoucolor-1.2/materialyoucolor/hct/cam16.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/materialyoucolor/hct/hct.py` & `materialyoucolor-1.2/materialyoucolor/hct/hct.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/materialyoucolor/hct/viewing_conditions.py` & `materialyoucolor-1.2/materialyoucolor/hct/viewing_conditions.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/materialyoucolor/palettes/core_palette.py` & `materialyoucolor-1.2/materialyoucolor/palettes/core_palette.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/materialyoucolor/palettes/tonal_palette.py` & `materialyoucolor-1.2/materialyoucolor/palettes/tonal_palette.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/materialyoucolor/scheme/scheme.py` & `materialyoucolor-1.2/materialyoucolor/scheme/scheme.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
                 "error": core.error.tone(40),
                 "errorContainer": core.error.tone(90),
                 "onError": core.error.tone(100),
                 "onErrorContainer": core.error.tone(10),
                 "outline": core.n2.tone(50),
                 "outlineVariant": core.n2.tone(80),
                 "shadow": core.n1.tone(0),
-                "surfaceTint": core.a1.tone(40),
+                "surfaceTint": core.a1.tone(50),  # This tone was not given
                 "scrim": core.n1.tone(0),
             }
         )
 
     @staticmethod
     def dark(argb):
         core = CorePalette.of(argb)
@@ -170,14 +170,14 @@
                 "error": core.error.tone(80),
                 "errorContainer": core.error.tone(30),
                 "onError": core.error.tone(20),
                 "onErrorContainer": core.error.tone(90),
                 "outline": core.n2.tone(60),
                 "outlineVariant": core.n2.tone(30),
                 "shadow": core.n1.tone(0),
-                "surfaceTint": core.a1.tone(80),
+                "surfaceTint": core.a1.tone(30),  # This tone was not given
                 "scrim": core.n1.tone(0),
             }
         )
 
     def toJSON(self):
         return json.dumps(self.props)
```

### Comparing `materialyoucolor-1.1.2/materialyoucolor/score/score.py` & `materialyoucolor-1.2/materialyoucolor/score/score.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/materialyoucolor/utils/color_utils.py` & `materialyoucolor-1.2/materialyoucolor/utils/color_utils.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/materialyoucolor/utils/math_utils.py` & `materialyoucolor-1.2/materialyoucolor/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/materialyoucolor/utils/string_utils.py` & `materialyoucolor-1.2/materialyoucolor/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/materialyoucolor/utils/theme_utils.py` & `materialyoucolor-1.2/materialyoucolor/utils/theme_utils.py`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/materialyoucolor.egg-info/PKG-INFO` & `materialyoucolor-1.2/materialyoucolor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: materialyoucolor
-Version: 1.1.2
+Version: 1.2
 Summary: Material You color generation algorithms in pure python!
 Author: Ansh Dadwal
 Author-email: anshdadwal298@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # materialyoucolor-pyhton
```

### Comparing `materialyoucolor-1.1.2/materialyoucolor.egg-info/SOURCES.txt` & `materialyoucolor-1.2/materialyoucolor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `materialyoucolor-1.1.2/setup.py` & `materialyoucolor-1.2/setup.py`

 * *Files identical despite different names*

