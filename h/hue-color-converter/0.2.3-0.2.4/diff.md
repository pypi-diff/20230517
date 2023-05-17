# Comparing `tmp/hue-color-converter-0.2.3.tar.gz` & `tmp/hue_color_converter-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hue-color-converter-0.2.3.tar", max compression
+gzip compressed data, was "hue_color_converter-0.2.4.tar", max compression
```

## Comparing `hue-color-converter-0.2.3.tar` & `hue_color_converter-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1070 2022-09-07 04:20:09.807259 hue-color-converter-0.2.3/LICENSE.txt
--rw-r--r--   0        0        0      644 2022-09-07 04:20:09.807259 hue-color-converter-0.2.3/README.md
--rw-r--r--   0        0        0       77 2022-09-07 04:20:09.807259 hue-color-converter-0.2.3/hue_color_converter/__init__.py
--rw-r--r--   0        0        0     4377 2022-09-07 04:20:09.807259 hue-color-converter-0.2.3/hue_color_converter/converter.py
--rw-r--r--   0        0        0      898 2022-09-07 04:20:09.807259 hue-color-converter-0.2.3/hue_color_converter/gamuts.py
--rw-r--r--   0        0        0      564 2022-09-07 04:20:09.807259 hue-color-converter-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 hue-color-converter-0.2.3/setup.py
--rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 hue-color-converter-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-17 03:53:33.847210 hue_color_converter-0.2.4/LICENSE.txt
+-rw-r--r--   0        0        0      644 2023-05-17 03:53:33.847210 hue_color_converter-0.2.4/README.md
+-rw-r--r--   0        0        0       77 2023-05-17 03:53:33.847210 hue_color_converter-0.2.4/hue_color_converter/__init__.py
+-rw-r--r--   0        0        0     4377 2023-05-17 03:53:33.847210 hue_color_converter-0.2.4/hue_color_converter/converter.py
+-rw-r--r--   0        0        0      898 2023-05-17 03:53:33.847210 hue_color_converter-0.2.4/hue_color_converter/gamuts.py
+-rw-r--r--   0        0        0      564 2023-05-17 03:53:33.847210 hue_color_converter-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 hue_color_converter-0.2.4/PKG-INFO
```

### Comparing `hue-color-converter-0.2.3/LICENSE.txt` & `hue_color_converter-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hue-color-converter-0.2.3/README.md` & `hue_color_converter-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `hue-color-converter-0.2.3/hue_color_converter/converter.py` & `hue_color_converter-0.2.4/hue_color_converter/converter.py`

 * *Files identical despite different names*

### Comparing `hue-color-converter-0.2.3/hue_color_converter/gamuts.py` & `hue_color_converter-0.2.4/hue_color_converter/gamuts.py`

 * *Files identical despite different names*

### Comparing `hue-color-converter-0.2.3/pyproject.toml` & `hue_color_converter-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "hue-color-converter"
-version = "0.2.3"
+version = "0.2.4"
 description = "color converter for philips hue"
 authors = ["Zachary Juang <zachary822@me.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "hue_color_converter"}]
 
 [tool.poetry.urls]
 repository = "https://github.com/zachary822/hue_color_converter"
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.12"
-Shapely = "^1.8.4"
+Shapely = "^2.0.1"
 numpy = "^1.23.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hue-color-converter-0.2.3/PKG-INFO` & `hue_color_converter-0.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: hue-color-converter
-Version: 0.2.3
+Version: 0.2.4
 Summary: color converter for philips hue
 License: MIT
 Author: Zachary Juang
 Author-email: zachary822@me.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Shapely (>=1.8.4,<2.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Shapely (>=2.0.1,<3.0.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Project-URL: repository, https://github.com/zachary822/hue_color_converter
 Description-Content-Type: text/markdown
 
 # Philips Hue Color Converter  (CIE xyY)
 
 Converts RGB to CIE xyY for Philips Hue
```

