# Comparing `tmp/fudgeo-0.5.0-py3-none-any.whl.zip` & `tmp/fudgeo-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 28058 bytes, number of entries: 17
--rw-r--r--  2.0 unx      117 b- defN 23-May-12 16:27 fudgeo/__init__.py
+Zip file size: 28084 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      117 b- defN 23-May-17 18:29 fudgeo/__init__.py
 -rw-r--r--  2.0 unx     2538 b- defN 23-May-11 16:25 fudgeo/constant.py
 -rw-r--r--  2.0 unx     1157 b- defN 23-Jan-04 21:53 fudgeo/enumeration.py
 -rw-r--r--  2.0 unx    20081 b- defN 23-May-12 12:57 fudgeo/geopkg.py
 -rw-r--r--  2.0 unx     2673 b- defN 23-May-06 22:48 fudgeo/geopkg.sql
 -rw-r--r--  2.0 unx     7768 b- defN 23-May-06 22:48 fudgeo/sql.py
 -rw-r--r--  2.0 unx      974 b- defN 23-May-06 22:48 fudgeo/geometry/__init__.py
--rw-r--r--  2.0 unx     2012 b- defN 23-May-11 23:19 fudgeo/geometry/base.py
--rw-r--r--  2.0 unx    18786 b- defN 23-May-12 01:46 fudgeo/geometry/linestring.py
--rw-r--r--  2.0 unx    20019 b- defN 23-May-12 12:56 fudgeo/geometry/point.py
--rw-r--r--  2.0 unx    26589 b- defN 23-May-12 01:46 fudgeo/geometry/polygon.py
--rw-r--r--  2.0 unx    16275 b- defN 23-May-12 13:03 fudgeo/geometry/util.py
--rw-r--r--  2.0 unx     1088 b- defN 23-May-12 18:48 fudgeo-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    12609 b- defN 23-May-12 18:48 fudgeo-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-12 18:48 fudgeo-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-12 18:48 fudgeo-0.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1323 b- defN 23-May-12 18:48 fudgeo-0.5.0.dist-info/RECORD
-17 files, 134108 bytes uncompressed, 25926 bytes compressed:  80.7%
+-rw-r--r--  2.0 unx     1983 b- defN 23-May-17 18:29 fudgeo/geometry/base.py
+-rw-r--r--  2.0 unx    18746 b- defN 23-May-17 18:29 fudgeo/geometry/linestring.py
+-rw-r--r--  2.0 unx    19883 b- defN 23-May-17 18:29 fudgeo/geometry/point.py
+-rw-r--r--  2.0 unx    26514 b- defN 23-May-17 18:29 fudgeo/geometry/polygon.py
+-rw-r--r--  2.0 unx    16219 b- defN 23-May-17 18:29 fudgeo/geometry/util.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-17 18:30 fudgeo-0.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12716 b- defN 23-May-17 18:30 fudgeo-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 18:30 fudgeo-0.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-17 18:30 fudgeo-0.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1323 b- defN 23-May-17 18:30 fudgeo-0.5.1.dist-info/RECORD
+17 files, 133879 bytes uncompressed, 25952 bytes compressed:  80.6%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: fudgeo/geometry/polygon.py
 Comment: 
 
 Filename: fudgeo/geometry/util.py
 Comment: 
 
-Filename: fudgeo-0.5.0.dist-info/LICENSE
+Filename: fudgeo-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: fudgeo-0.5.0.dist-info/METADATA
+Filename: fudgeo-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: fudgeo-0.5.0.dist-info/WHEEL
+Filename: fudgeo-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: fudgeo-0.5.0.dist-info/top_level.txt
+Filename: fudgeo-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: fudgeo-0.5.0.dist-info/RECORD
+Filename: fudgeo-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fudgeo/__init__.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 Package Initialization
 """
 
 
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 
 
 if __name__ == '__main__':
     pass
```

## fudgeo/geometry/base.py

```diff
@@ -23,30 +23,29 @@
         super().__init__()
         self.srs_id: int = srs_id
         self._env: Envelope = EMPTY_ENVELOPE
         self._args: Optional[Tuple[memoryview, int]] = None
     # End init built-in
 
     @abstractmethod
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:  # pragma: nocover
+    def _to_wkb(self, ary: bytearray) -> bytearray:  # pragma: nocover
         """
         To WKB
         """
         pass
     # End _to_wkb method
 
     @staticmethod
-    def _join_geometries(prefix: bytes,
+    def _join_geometries(ary: bytearray,
                          geoms: List['AbstractGeometry']) -> bytearray:
         """
         Join Geometries
         """
-        ary = bytearray(prefix)
         for geom in geoms:
-            ary.extend(geom._to_wkb())
+            geom._to_wkb(ary)
         return ary
     # End _join_geometries method
 
     @property
     @abstractmethod
     def is_empty(self) -> bool:
         """
@@ -65,16 +64,17 @@
     # End envelope property
 
     def to_gpkg(self) -> bytes:
         """
         To Geopackage
         """
         env_code, env_wkb = self.envelope.to_wkb()
-        return (make_header(srs_id=self.srs_id, is_empty=self.is_empty,
-                            envelope_code=env_code) + env_wkb + self._to_wkb())
+        ary = bytearray(make_header(srs_id=self.srs_id, is_empty=self.is_empty,
+                        envelope_code=env_code) + env_wkb)
+        return self._to_wkb(ary)
     # End to_gpkg method
 
     @classmethod
     @abstractmethod
     def from_gpkg(cls, value: bytes) -> 'AbstractGeometry':  # pragma: nocover
         """
         From Geopackage
```

## fudgeo/geometry/linestring.py

```diff
@@ -89,19 +89,19 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
-        return pack_coordinates(WKB_LINESTRING_PRE, self.coordinates)
+        return pack_coordinates(ary, WKB_LINESTRING_PRE, self.coordinates)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LineString':
         """
         From Geopackage
         """
@@ -173,20 +173,20 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_z(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         return pack_coordinates(
-            WKB_LINESTRING_Z_PRE, self.coordinates, has_z=True)
+            ary, WKB_LINESTRING_Z_PRE, self.coordinates, has_z=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LineStringZ':
         """
         From Geopackage
         """
@@ -258,20 +258,20 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_m(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         return pack_coordinates(
-            WKB_LINESTRING_M_PRE, self.coordinates, has_m=True)
+            ary, WKB_LINESTRING_M_PRE, self.coordinates, has_m=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LineStringM':
         """
         From Geopackage
         """
@@ -343,20 +343,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_zm(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         return pack_coordinates(
-            WKB_LINESTRING_ZM_PRE, self.coordinates, has_z=True, has_m=True)
+            ary, WKB_LINESTRING_ZM_PRE, self.coordinates,
+            has_z=True, has_m=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LineStringZM':
         """
         From Geopackage
         """
@@ -414,21 +415,21 @@
     def is_empty(self) -> bool:
         """
         Is Empty
         """
         return not (bool(self._args) or bool(self.lines))
     # End is_empty property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.lines
-        prefix = WKB_MULTI_LINESTRING_PRE + pack(COUNT_CODE, len(geoms))
-        return self._join_geometries(prefix, geoms)
+        ary.extend(WKB_MULTI_LINESTRING_PRE + pack(COUNT_CODE, len(geoms)))
+        return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
@@ -510,21 +511,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_z(self.lines)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.lines
-        prefix = WKB_MULTI_LINESTRING_Z_PRE + pack(COUNT_CODE, len(geoms))
-        return self._join_geometries(prefix, geoms)
+        ary.extend(WKB_MULTI_LINESTRING_Z_PRE + pack(COUNT_CODE, len(geoms)))
+        return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiLineStringZ':
         """
         From Geopackage
         """
@@ -594,21 +595,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_m(self.lines)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.lines
-        prefix = WKB_MULTI_LINESTRING_M_PRE + pack(COUNT_CODE, len(geoms))
-        return self._join_geometries(prefix, geoms)
+        ary.extend(WKB_MULTI_LINESTRING_M_PRE + pack(COUNT_CODE, len(geoms)))
+        return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiLineStringM':
         """
         From Geopackage
         """
@@ -679,21 +680,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_zm(self.lines)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.lines
-        prefix = WKB_MULTI_LINESTRING_ZM_PRE + pack(COUNT_CODE, len(geoms))
-        return self._join_geometries(prefix, geoms)
+        ary.extend(WKB_MULTI_LINESTRING_ZM_PRE + pack(COUNT_CODE, len(geoms)))
+        return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiLineStringZM':
         """
         From Geopackage
         """
```

## fudgeo/geometry/point.py

```diff
@@ -2,18 +2,18 @@
 """
 Points
 """
 
 
 from math import isnan, nan
 from struct import pack, unpack
-from typing import List, TYPE_CHECKING
+from typing import List, Optional, TYPE_CHECKING
 
 from fudgeo.constant import (
-    DOUBLE, EMPTY, FOUR_D, FOUR_D_PACK_CODE, FOUR_D_UNPACK_CODE, HEADER_OFFSET,
+    DOUBLE, FOUR_D, FOUR_D_PACK_CODE, FOUR_D_UNPACK_CODE, HEADER_OFFSET,
     QUADRUPLE, THREE_D, THREE_D_PACK_CODE, THREE_D_UNPACK_CODE, TRIPLE, TWO_D,
     TWO_D_PACK_CODE, TWO_D_UNPACK_CODE, WKB_MULTI_POINT_M_PRE,
     WKB_MULTI_POINT_PRE, WKB_MULTI_POINT_ZM_PRE, WKB_MULTI_POINT_Z_PRE,
     WKB_POINT_M_PRE, WKB_POINT_PRE, WKB_POINT_ZM_PRE, WKB_POINT_Z_PRE)
 from fudgeo.geometry.base import AbstractGeometry
 from fudgeo.geometry.util import (
     EMPTY_ENVELOPE, Envelope, as_array, envelope_from_coordinates,
@@ -65,20 +65,19 @@
         """
         Unpack Values
         """
         *_, x, y = unpack(TWO_D_UNPACK_CODE, view)
         return x, y
     # End _unpack method
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, ary: Optional[bytearray] = None) -> bytes:
         """
         To WKB
         """
-        pre = WKB_POINT_PRE if use_prefix else EMPTY
-        return pre + pack(TWO_D_PACK_CODE, self.x, self.y)
+        return WKB_POINT_PRE + pack(TWO_D_PACK_CODE, self.x, self.y)
     # End _to_wkb method
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
@@ -165,20 +164,19 @@
         """
         Unpack Values
         """
         *_, x, y, z = unpack(THREE_D_UNPACK_CODE, view)
         return x, y, z
     # End _unpack method
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, ary: Optional[bytearray] = None) -> bytes:
         """
         To WKB
         """
-        pre = WKB_POINT_Z_PRE if use_prefix else EMPTY
-        return pre + pack(THREE_D_PACK_CODE, self.x, self.y, self.z)
+        return WKB_POINT_Z_PRE + pack(THREE_D_PACK_CODE, self.x, self.y, self.z)
     # End _to_wkb method
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
@@ -265,20 +263,19 @@
         """
         Unpack Values
         """
         *_, x, y, m = unpack(THREE_D_UNPACK_CODE, view)
         return x, y, m
     # End _unpack method
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, ary: Optional[bytearray] = None) -> bytes:
         """
         To WKB
         """
-        pre = WKB_POINT_M_PRE if use_prefix else EMPTY
-        return pre + pack(THREE_D_PACK_CODE, self.x, self.y, self.m)
+        return WKB_POINT_M_PRE + pack(THREE_D_PACK_CODE, self.x, self.y, self.m)
     # End _to_wkb method
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
@@ -369,20 +366,20 @@
         """
         Unpack Values
         """
         *_, x, y, z, m = unpack(FOUR_D_UNPACK_CODE, view)
         return x, y, z, m
     # End _unpack method
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, ary: Optional[bytearray] = None) -> bytes:
         """
         To WKB
         """
-        pre = WKB_POINT_ZM_PRE if use_prefix else EMPTY
-        return pre + pack(FOUR_D_PACK_CODE, self.x, self.y, self.z, self.m)
+        return WKB_POINT_ZM_PRE + pack(
+            FOUR_D_PACK_CODE, self.x, self.y, self.z, self.m)
     # End _to_wkb method
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
@@ -390,15 +387,15 @@
     # End envelope property
 
     def to_gpkg(self) -> bytes:
         """
         To Geopackage
         """
         return (make_header(srs_id=self.srs_id,
-                            is_empty=self.is_empty) + self._to_wkb())
+                            is_empty=self.is_empty) + self._to_wkb(None))
     # End to_gpkg method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PointZM':
         """
         From Geopackage
         """
@@ -491,20 +488,20 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         return pack_coordinates(
-            WKB_MULTI_POINT_PRE, self.coordinates, use_point_prefix=True)
+            ary, WKB_MULTI_POINT_PRE, self.coordinates, use_point_prefix=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPoint':
         """
         From Geopackage
         """
@@ -576,20 +573,20 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_z(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         return pack_coordinates(
-            WKB_MULTI_POINT_Z_PRE, self.coordinates,
+            ary, WKB_MULTI_POINT_Z_PRE, self.coordinates,
             has_z=True, use_point_prefix=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPointZ':
         """
         From Geopackage
@@ -662,20 +659,20 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_m(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         return pack_coordinates(
-            WKB_MULTI_POINT_M_PRE, self.coordinates,
+            ary, WKB_MULTI_POINT_M_PRE, self.coordinates,
             has_m=True, use_point_prefix=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPointM':
         """
         From Geopackage
@@ -748,20 +745,20 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_zm(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         return pack_coordinates(
-            WKB_MULTI_POINT_ZM_PRE, self.coordinates,
+            ary, WKB_MULTI_POINT_ZM_PRE, self.coordinates,
             has_z=True, has_m=True, use_point_prefix=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPointZM':
         """
         From Geopackage
```

## fudgeo/geometry/polygon.py

```diff
@@ -77,19 +77,19 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
-        return pack_coordinates(EMPTY, self.coordinates)
+        return pack_coordinates(ary, EMPTY, self.coordinates)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LinearRing':  # pragma: nocover
         """
         From Geopackage, no-op for Linear Ring
         """
@@ -137,19 +137,19 @@
         Points
         """
         srs_id = self.srs_id
         return [PointZ(x=x, y=y, z=z, srs_id=srs_id)
                 for x, y, z in self.coordinates]
     # End points property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
-        return pack_coordinates(EMPTY, self.coordinates, has_z=True)
+        return pack_coordinates(ary, EMPTY, self.coordinates, has_z=True)
     # End _to_wkb method
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
@@ -221,19 +221,19 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_m(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
-        return pack_coordinates(EMPTY, self.coordinates, has_m=True)
+        return pack_coordinates(ary, EMPTY, self.coordinates, has_m=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LinearRingM':  # pragma: nocover
         """
         From Geopackage, no-op for Linear Ring
         """
@@ -291,19 +291,20 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_zm(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
-        return pack_coordinates(EMPTY, self.coordinates, has_z=True, has_m=True)
+        return pack_coordinates(
+            ary, EMPTY, self.coordinates, has_z=True, has_m=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LinearRingZM':  # pragma: nocover
         """
         From Geopackage, no-op for Linear Ring
         """
@@ -374,21 +375,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries(self.rings)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.rings
-        prefix = WKB_POLYGON_PRE + pack(COUNT_CODE, len(geoms))
-        return self._join_geometries(prefix, geoms)
+        ary.extend(WKB_POLYGON_PRE + pack(COUNT_CODE, len(geoms)))
+        return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'Polygon':
         """
         From Geopackage
         """
@@ -459,21 +460,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_z(self.rings)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.rings
-        prefix = WKB_POLYGON_Z_PRE + pack(COUNT_CODE, len(geoms))
-        return self._join_geometries(prefix, geoms)
+        ary.extend(WKB_POLYGON_Z_PRE + pack(COUNT_CODE, len(geoms)))
+        return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PolygonZ':
         """
         From Geopackage
         """
@@ -544,21 +545,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_m(self.rings)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.rings
-        prefix = WKB_POLYGON_M_PRE + pack(COUNT_CODE, len(geoms))
-        return self._join_geometries(prefix, geoms)
+        ary.extend(WKB_POLYGON_M_PRE + pack(COUNT_CODE, len(geoms)))
+        return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PolygonM':
         """
         From Geopackage
         """
@@ -630,21 +631,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_zm(self.rings)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.rings
-        prefix = WKB_POLYGON_ZM_PRE + pack(COUNT_CODE, len(geoms))
-        return self._join_geometries(prefix, geoms)
+        ary.extend(WKB_POLYGON_ZM_PRE + pack(COUNT_CODE, len(geoms)))
+        return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PolygonZM':
         """
         From Geopackage
         """
@@ -716,21 +717,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries(self.polygons)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.polygons
-        prefix = WKB_MULTI_POLYGON_PRE + pack(COUNT_CODE, len(geoms))
-        return self._join_geometries(prefix, geoms)
+        ary.extend(WKB_MULTI_POLYGON_PRE + pack(COUNT_CODE, len(geoms)))
+        return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPolygon':
         """
         From Geopackage
         """
@@ -802,21 +803,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_z(self.polygons)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.polygons
-        prefix = WKB_MULTI_POLYGON_Z_PRE + pack(COUNT_CODE, len(geoms))
-        return self._join_geometries(prefix, geoms)
+        ary.extend(WKB_MULTI_POLYGON_Z_PRE + pack(COUNT_CODE, len(geoms)))
+        return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPolygonZ':
         """
         From Geopackage
         """
@@ -888,21 +889,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_m(self.polygons)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.polygons
-        prefix = WKB_MULTI_POLYGON_M_PRE + pack(COUNT_CODE, len(geoms))
-        return self._join_geometries(prefix, geoms)
+        ary.extend(WKB_MULTI_POLYGON_M_PRE + pack(COUNT_CODE, len(geoms)))
+        return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPolygonM':
         """
         From Geopackage
         """
@@ -974,21 +975,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_zm(self.polygons)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
+    def _to_wkb(self, ary: bytearray) -> bytearray:
         """
         To WKB
         """
         geoms = self.polygons
-        prefix = WKB_MULTI_POLYGON_ZM_PRE + pack(COUNT_CODE, len(geoms))
-        return self._join_geometries(prefix, geoms)
+        ary.extend(WKB_MULTI_POLYGON_ZM_PRE + pack(COUNT_CODE, len(geoms)))
+        return self._join_geometries(ary, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPolygonZM':
         """
         From Geopackage
         """
```

## fudgeo/geometry/util.py

```diff
@@ -198,31 +198,32 @@
     # End max_m property
 # End Envelope class
 
 
 EMPTY_ENVELOPE = Envelope(code=0, min_x=nan, max_x=nan, min_y=nan, max_y=nan)
 
 
-def lazy_unpack(cls: Any, value: bytes, dimension: int) -> Any:
+def lazy_unpack(cls: Any, value: Union[bytes, bytearray],
+                dimension: int) -> Any:
     """
     Unpack just the header and envelope, adding data to class for later use.
     """
-    view = memoryview(value)
-    srs_id, env_code, offset, is_empty = unpack_header(view[:HEADER_OFFSET])
+    srs_id, env_code, offset, is_empty = unpack_header(bytes(value[:HEADER_OFFSET]))
     obj = cls([], srs_id=srs_id)
     if is_empty:
         return obj
+    view = memoryview(value)
     obj._env = unpack_envelope(code=env_code, view=view[:offset])
     obj._args = view[offset:], dimension
     return obj
 # End lazy_unpack function
 
 
 def unpack_line(view: memoryview, dimension: int,
-                is_ring: bool = False) -> List[Tuple[float, ...]]:
+                is_ring: bool = False) -> ndarray:
     """
     Unpack Values for LineString
     """
     count, data = get_count_and_data(view, is_ring=is_ring)
     return frombuffer(
         data, dtype=float, count=dimension * count).reshape(-1, dimension)
 # End unpack_line function
@@ -241,22 +242,22 @@
     for i in range(0, len(data), size):
         ary.extend(data[i + offset:i + size])
     return frombuffer(
         ary, dtype=float, count=dimension * count).reshape(-1, dimension)
 # End unpack_points function
 
 
-def pack_coordinates(prefix: bytes, coordinates: ndarray,
+def pack_coordinates(ary: bytearray, prefix: bytes, coordinates: ndarray,
                      has_z: bool = False, has_m: bool = False,
                      use_point_prefix: bool = False) -> bytearray:
     """
     Pack Coordinates
     """
     count = len(coordinates)
-    ary = bytearray(prefix + pack(COUNT_CODE, count))
+    ary.extend(prefix + pack(COUNT_CODE, count))
     data = coordinates.tobytes()
     if not use_point_prefix:
         ary.extend(data)
         return ary
     length = len(data)
     view = memoryview(data)
     step = length // count
@@ -265,36 +266,34 @@
         ary.extend(prefix)
         ary.extend(view[i:i + step])
     return ary
 # End pack_coordinates function
 
 
 def unpack_lines(view: memoryview, dimension: int, is_ring: bool = False) \
-        -> List[List[Tuple[float, ...]]]:
+        -> List[ndarray]:
     """
     Unpack Values for Multi LineString and Polygons
     """
     size, last_end = 8 * dimension, 0
     offset, unit = (4, COUNT_CODE) if is_ring else (9, '<BII')
     count, data = get_count_and_data(view)
     lines = []
     for _ in range(count):
         *_, length = unpack(unit, data[last_end:last_end + offset])
         end = last_end + offset + (size * length)
-        # noinspection PyTypeChecker
-        points: List[Tuple[float, ...]] = unpack_line(
-            data[last_end:end], dimension, is_ring=is_ring)
+        points = unpack_line(data[last_end:end], dimension, is_ring=is_ring)
         last_end = end
         lines.append(points)
     return lines
 # End unpack_lines function
 
 
 def unpack_polygons(view: memoryview, dimension: int) \
-        -> List[List[List[Tuple[float, ...]]]]:
+        -> List[List[ndarray]]:
     """
     Unpack Values for Multi Polygon Type Containing Polygons
     """
     size, last_end = 8 * dimension, 0
     count, data = get_count_and_data(view)
     polygons = []
     for _ in range(0, count):
@@ -328,15 +327,15 @@
         envelope_code = 0
     flags |= (envelope_code << 1)
     return pack(HEADER_CODE, GP_MAGIC, 0, flags, srs_id)
 # End make_header function
 
 
 @lru_cache(maxsize=None)
-def unpack_header(view: memoryview) -> Tuple[int, int, int, bool]:
+def unpack_header(view: Union[bytes, memoryview]) -> Tuple[int, int, int, bool]:
     """
     Cached Unpacking of a GeoPackage Geometry Header
     """
     _, _, flags, srs_id = unpack(HEADER_CODE, view)
     envelope_code = (flags & (0x07 << 1)) >> 1
     is_empty = bool((flags & (0x01 << 4)) >> 4)
     return srs_id, envelope_code, ENVELOPE_OFFSET[envelope_code], is_empty
```

## Comparing `fudgeo-0.5.0.dist-info/LICENSE` & `fudgeo-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fudgeo-0.5.0.dist-info/METADATA` & `fudgeo-0.5.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fudgeo
-Version: 0.5.0
+Version: 0.5.1
 Summary: GeoPackage support from Python.  fudgeo is a simple package for creating OGC GeoPackages, Feature Classes, Tables, and geometries (read and write).
 Author-email: "Integrated Informatics Inc." <contact@integrated-informatics.com>
 License: MIT License
         
         Copyright (c) 2021-2023 Integrated Informatics Inc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -256,14 +256,17 @@
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Release History
 
+### v0.5.1
+* small performance improvements by reducing `bytes` concatenation and building up `bytearray`
+
 ### v0.5.0
 * performance improvements for geometry reading (especially for geometries with large numbers of points / parts)
 * performance improvements for geometry writing
 * incorporated `numpy` and `bottleneck` as dependencies
 
 ### v0.4.2
 * only unpack header and delay unpacking coordinates until needed
```

## Comparing `fudgeo-0.5.0.dist-info/RECORD` & `fudgeo-0.5.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-fudgeo/__init__.py,sha256=KozCNcZLFxSNF54wJ5akYLIN25MjKT2XuCIb6-JwA-Q,117
+fudgeo/__init__.py,sha256=cV2PjqAwCsMP7XXF7T8rT1-eBg0VMQ_AyJZcqwtYiqo,117
 fudgeo/constant.py,sha256=-fE2Lyobm43rnDNzxsLUhaCfMMlaO5cCUmOFEL05LCQ,2538
 fudgeo/enumeration.py,sha256=NvgtVBYxfULGVIks-J0rFLRxvGrtU2DM1bjZB0HxZRU,1157
 fudgeo/geopkg.py,sha256=LL5uO82kL5CgTlIdxbr_2hiUf-kqDVXdtz8vDASXj_g,20081
 fudgeo/geopkg.sql,sha256=Tt0Fi4w-ySR7tDUJsPt-5mA_Sw2oUs8co5rFGEleS24,2673
 fudgeo/sql.py,sha256=AJcNZAjvGHvmc88NCU1TTsfjJ0tVZ6muTyNzA8yZcW0,7768
 fudgeo/geometry/__init__.py,sha256=N4sf5FJB13JoNxB_GyyO9ohXbtKoSoVvbKTnltMXq-0,974
-fudgeo/geometry/base.py,sha256=MF2b9lCrsbufB-IQrS8aE4p1PcRtyV8n0bxcuN_68jU,2012
-fudgeo/geometry/linestring.py,sha256=3Y0giqvXjjbHeOmSZKEgnivzxq0L8Xiazd8ggcpsXME,18786
-fudgeo/geometry/point.py,sha256=vGryK_D-04JIyLa4vDerLmPhOCUG4iJ1JzQJoxIzX9o,20019
-fudgeo/geometry/polygon.py,sha256=JkR0nHKv21Sjnxs1F7PB3qoTHwWbszPhA4nMkuuyKDs,26589
-fudgeo/geometry/util.py,sha256=9rjxRx4rS_e97N2vibO3l2x_QzT07DKgpmH6X93SEko,16275
-fudgeo-0.5.0.dist-info/LICENSE,sha256=kg8K68wjqhzaDoPNP6FWgXT2UuLmZbswzv72syix3Gw,1088
-fudgeo-0.5.0.dist-info/METADATA,sha256=balGUiS7dG9E1OjRJ74dj6BVYbgtipddDeH1h2n1PCM,12609
-fudgeo-0.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fudgeo-0.5.0.dist-info/top_level.txt,sha256=RlcnukuWGTUINTexweATRDqQgM1d0q2iaOd6B6tBWWI,7
-fudgeo-0.5.0.dist-info/RECORD,,
+fudgeo/geometry/base.py,sha256=vBsJeaE6zio9ag4suupYxd3UizbobUoG6yzVrCqxwm4,1983
+fudgeo/geometry/linestring.py,sha256=IY0xKsbe4VCB4uYUXkVPmgTLCiv216t2wgBeUAqzCqM,18746
+fudgeo/geometry/point.py,sha256=uH5Kyl4PnCQM2PagzrbHsHGv6LMxBLkVoKjCK05LPQw,19883
+fudgeo/geometry/polygon.py,sha256=q3GAB-_1AMWXSHqJNEOzwh2X5N8OcglTzQM41koAKfI,26514
+fudgeo/geometry/util.py,sha256=h-xxOR2rETbjCUfPqi9_PwvnhBE2pdpnS66qxGoj9xI,16219
+fudgeo-0.5.1.dist-info/LICENSE,sha256=kg8K68wjqhzaDoPNP6FWgXT2UuLmZbswzv72syix3Gw,1088
+fudgeo-0.5.1.dist-info/METADATA,sha256=VDJaB9PHzZxPZcNxu7SQVcJdk1OqXHBtv21KXPrrAbs,12716
+fudgeo-0.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fudgeo-0.5.1.dist-info/top_level.txt,sha256=RlcnukuWGTUINTexweATRDqQgM1d0q2iaOd6B6tBWWI,7
+fudgeo-0.5.1.dist-info/RECORD,,
```

