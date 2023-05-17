# Comparing `tmp/morecantile-4.0.0a0.tar.gz` & `tmp/morecantile-4.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morecantile-4.0.0a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "morecantile-4.0.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `morecantile-4.0.0a0.tar` & `morecantile-4.0.0a1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      217 2023-05-15 15:52:57.079291 morecantile-4.0.0a0/.bumpversion.cfg
--rw-r--r--   0        0        0     1817 2023-05-15 15:52:57.079291 morecantile-4.0.0a0/.gitignore
--rw-r--r--   0        0        0      822 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/LICENSE
--rw-r--r--   0        0        0     5305 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/README.md
--rw-r--r--   0        0        0      438 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/__init__.py
--rw-r--r--   0        0        0     1015 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/commons.py
--rw-r--r--   0        0        0     7267 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/CanadianNAD83_LCC.json
--rw-r--r--   0        0        0     4679 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/EuropeanETRS89_LAEAQuad.json
--rw-r--r--   0        0        0     5176 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/LINZAntarticaMapTilegrid.json
--rw-r--r--   0        0        0     8457 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/NZTM2000Quad.json
--rw-r--r--   0        0        0      242 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/README.md
--rw-r--r--   0        0        0     7374 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/UPSAntarcticWGS84Quad.json
--rw-r--r--   0        0        0     7365 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/UPSArcticWGS84Quad.json
--rw-r--r--   0        0        0     7367 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/UTM31WGS84Quad.json
--rw-r--r--   0        0        0     6932 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/WGS1984Quad.json
--rw-r--r--   0        0        0     7843 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/WebMercatorQuad.json
--rw-r--r--   0        0        0     7072 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/WorldCRS84Quad.json
--rw-r--r--   0        0        0     7001 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/data/WorldMercatorWGS84Quad.json
--rw-r--r--   0        0        0     1748 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/defaults.py
--rw-r--r--   0        0        0      907 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/errors.py
--rw-r--r--   0        0        0    39247 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/models.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/py.typed
--rw-r--r--   0        0        0       23 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/scripts/__init__.py
--rw-r--r--   0        0        0    16657 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/scripts/cli.py
--rw-r--r--   0        0        0     3364 2023-05-15 15:52:57.083291 morecantile-4.0.0a0/morecantile/utils.py
--rw-r--r--   0        0        0     2295 2023-05-15 15:52:57.087291 morecantile-4.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     6734 1970-01-01 00:00:00.000000 morecantile-4.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0      217 2023-05-17 07:36:10.367266 morecantile-4.0.0a1/.bumpversion.cfg
+-rw-r--r--   0        0        0     1817 2023-05-17 07:36:10.367266 morecantile-4.0.0a1/.gitignore
+-rw-r--r--   0        0        0      822 2023-05-17 07:36:10.367266 morecantile-4.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/LICENSE
+-rw-r--r--   0        0        0     5305 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/README.md
+-rw-r--r--   0        0        0      438 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/__init__.py
+-rw-r--r--   0        0        0     1015 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/commons.py
+-rw-r--r--   0        0        0     7267 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/data/CanadianNAD83_LCC.json
+-rw-r--r--   0        0        0     4679 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/data/EuropeanETRS89_LAEAQuad.json
+-rw-r--r--   0        0        0     5176 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/data/LINZAntarticaMapTilegrid.json
+-rw-r--r--   0        0        0     8457 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/data/NZTM2000Quad.json
+-rw-r--r--   0        0        0      242 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/data/README.md
+-rw-r--r--   0        0        0     7374 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/data/UPSAntarcticWGS84Quad.json
+-rw-r--r--   0        0        0     7365 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/data/UPSArcticWGS84Quad.json
+-rw-r--r--   0        0        0     7367 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/data/UTM31WGS84Quad.json
+-rw-r--r--   0        0        0     6932 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/data/WGS1984Quad.json
+-rw-r--r--   0        0        0     7843 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/data/WebMercatorQuad.json
+-rw-r--r--   0        0        0     7072 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/data/WorldCRS84Quad.json
+-rw-r--r--   0        0        0     7001 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/data/WorldMercatorWGS84Quad.json
+-rw-r--r--   0        0        0     1748 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/defaults.py
+-rw-r--r--   0        0        0      907 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/errors.py
+-rw-r--r--   0        0        0    39392 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/models.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/py.typed
+-rw-r--r--   0        0        0       23 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/scripts/__init__.py
+-rw-r--r--   0        0        0    16657 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/scripts/cli.py
+-rw-r--r--   0        0        0     3364 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/morecantile/utils.py
+-rw-r--r--   0        0        0     2295 2023-05-17 07:36:10.371266 morecantile-4.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     6734 1970-01-01 00:00:00.000000 morecantile-4.0.0a1/PKG-INFO
```

### Comparing `morecantile-4.0.0a0/.gitignore` & `morecantile-4.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/.pre-commit-config.yaml` & `morecantile-4.0.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/LICENSE` & `morecantile-4.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/README.md` & `morecantile-4.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/commons.py` & `morecantile-4.0.0a1/morecantile/commons.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/data/CanadianNAD83_LCC.json` & `morecantile-4.0.0a1/morecantile/data/CanadianNAD83_LCC.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/data/EuropeanETRS89_LAEAQuad.json` & `morecantile-4.0.0a1/morecantile/data/EuropeanETRS89_LAEAQuad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/data/LINZAntarticaMapTilegrid.json` & `morecantile-4.0.0a1/morecantile/data/LINZAntarticaMapTilegrid.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/data/NZTM2000Quad.json` & `morecantile-4.0.0a1/morecantile/data/NZTM2000Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/data/UPSAntarcticWGS84Quad.json` & `morecantile-4.0.0a1/morecantile/data/UPSAntarcticWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/data/UPSArcticWGS84Quad.json` & `morecantile-4.0.0a1/morecantile/data/UPSArcticWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/data/UTM31WGS84Quad.json` & `morecantile-4.0.0a1/morecantile/data/UTM31WGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/data/WGS1984Quad.json` & `morecantile-4.0.0a1/morecantile/data/WGS1984Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/data/WebMercatorQuad.json` & `morecantile-4.0.0a1/morecantile/data/WebMercatorQuad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/data/WorldCRS84Quad.json` & `morecantile-4.0.0a1/morecantile/data/WorldCRS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/data/WorldMercatorWGS84Quad.json` & `morecantile-4.0.0a1/morecantile/data/WorldMercatorWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/defaults.py` & `morecantile-4.0.0a1/morecantile/defaults.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/errors.py` & `morecantile-4.0.0a1/morecantile/errors.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/models.py` & `morecantile-4.0.0a1/morecantile/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
     def __iter__(self):
         """Iterate over matrices"""
         for matrix in self.tileMatrices:
             yield matrix
 
     def __repr__(self):
         """Simplify default pydantic model repr."""
-        return f"<TileMatrixSet title='{self.title}' id='{self.id}'>"
+        return f"<TileMatrixSet title='{self.title}' id='{self.id}' crs='{self.crs}>"
 
     @property
     def geographic_crs(self) -> CRSType:
         """Return the TMS's geographic CRS."""
         return self._geographic_crs
 
     @property
@@ -800,15 +800,20 @@
         right, bottom = self._ul(Tile(matrix.matrixWidth, matrix.matrixHeight, zoom))
 
         return BoundingBox(left, bottom, right, top)
 
     @property
     @cached(  # type: ignore
         LRUCache(maxsize=512),
-        key=lambda self: hashkey(self.id, self.tileMatrices[0].pointOfOrigin),
+        key=lambda self: hashkey(
+            self.crs,
+            self.tileMatrices[0].pointOfOrigin,
+            self.tileMatrices[0].matrixWidth,
+            self.tileMatrices[0].matrixHeight,
+        ),
     )
     def bbox(self):
         """Return TMS bounding box in geographic coordinate reference system."""
         left, bottom, right, top = self.xy_bbox
         return BoundingBox(
             *self._to_geographic.transform_bounds(
                 left,
```

### Comparing `morecantile-4.0.0a0/morecantile/scripts/cli.py` & `morecantile-4.0.0a1/morecantile/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/morecantile/utils.py` & `morecantile-4.0.0a1/morecantile/utils.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/pyproject.toml` & `morecantile-4.0.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.0a0/PKG-INFO` & `morecantile-4.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morecantile
-Version: 4.0.0a0
+Version: 4.0.0a1
 Summary: Construct and use map tile grids (a.k.a TileMatrixSet / TMS).
 Keywords: GIS,TMS,TileMatrixSet,Map Tile
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: morecantile Version: 4.0.0a0 Summary: Construct and
+Metadata-Version: 2.1 Name: morecantile Version: 4.0.0a1 Summary: Construct and
 use map tile grids (a.k.a TileMatrixSet / TMS). Keywords:
 GIS,TMS,TileMatrixSet,Map Tile Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

