# Comparing `tmp/hagis-0.7.3.tar.gz` & `tmp/hagis-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.7.3.tar", last modified: Fri May 12 11:55:46 2023, max compression
+gzip compressed data, was "hagis-0.7.4.tar", last modified: Wed May 17 20:52:12 2023, max compression
```

## Comparing `hagis-0.7.3.tar` & `hagis-0.7.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 11:55:46.081746 hagis-0.7.3/
--rw-rw-rw-   0        0        0      923 2023-05-12 11:55:46.072140 hagis-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 11:55:46.072140 hagis-0.7.3/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-05-12 11:55:45.000000 hagis-0.7.3/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-12 11:55:45.000000 hagis-0.7.3/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 11:55:45.000000 hagis-0.7.3/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-12 11:55:45.000000 hagis-0.7.3/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    23894 2023-05-12 00:42:32.000000 hagis-0.7.3/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-11 20:03:14.000000 hagis-0.7.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 11:55:46.084694 hagis-0.7.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 20:52:12.241524 hagis-0.7.4/
+-rw-rw-rw-   0        0        0      923 2023-05-17 20:52:12.240349 hagis-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-17 20:49:35.000000 hagis-0.7.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 20:52:12.238382 hagis-0.7.4/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-05-17 20:52:12.000000 hagis-0.7.4/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-17 20:52:12.000000 hagis-0.7.4/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 20:52:12.000000 hagis-0.7.4/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-17 20:52:12.000000 hagis-0.7.4/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    26722 2023-05-17 18:59:21.000000 hagis-0.7.4/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-17 16:36:21.000000 hagis-0.7.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 20:52:12.242391 hagis-0.7.4/setup.cfg
```

### Comparing `hagis-0.7.3/PKG-INFO` & `hagis-0.7.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.7.3
+Version: 0.7.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.7.3/hagis.egg-info/PKG-INFO` & `hagis-0.7.4/hagis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.7.3
+Version: 0.7.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.7.3/hagis.py` & `hagis-0.7.4/hagis.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,16 +74,22 @@
 
                     if property_name.lower() == shape_property_name.lower():
                         self._shape_property_name = property_name
                         self._shape_property_type = property_type
 
                     self._lower_field_to_property_name_type[lower_field] = property_name, property_type
 
-        self._is_arcgis_gemetry = hasattr(self._shape_property_type, "__module__")\
-            and self._shape_property_type.__module__.startswith("arcgis.geometry.")
+        self.geometry_module = GeometryModule.none
+
+        if hasattr(self._shape_property_type, "__module__"):
+            module = self._shape_property_type.__module__
+            if module.startswith("arcgis.geometry."):
+                self.geometry_module = GeometryModule.arcgis
+            elif module.startswith("shapely.geometry."):
+                self.geometry_module = GeometryModule.shapely
 
     _token_cache: Dict[Tuple[str, str], Tuple[str, int]] = {}
 
     def set_token_generator(self, username: str, password: str, referer: str = "",
                             token_url: str = "https://www.arcgis.com/sharing/generateToken", **kwargs: Any) -> None:
         """ Sets the token generation parameters.
 
@@ -299,16 +305,18 @@
         attributes: Dict[str, Any] = {}
 
         dictionary["attributes"] = attributes
 
         for key, value in item.__dict__.items():
             field = self._property_name_to_lower_field[key]
             if key.lower() == self._shape_property_name.lower():
-                if self._is_arcgis_gemetry:
+                if self.geometry_module == GeometryModule.arcgis:
                     dictionary["geometry"] = loads(value.JSON)
+                elif self.geometry_module == GeometryModule.shapely:
+                    dictionary["geometry"] = self._from_shapely(value)
                 else:
                     dictionary["geometry"] = value.__dict__
             elif isinstance(value, datetime):
                 attributes[field] = int((value - datetime.utcfromtimestamp(0)).total_seconds() * 1000)
             else:
                 attributes[field] = value
 
@@ -371,22 +379,81 @@
     def _map(self, row: SimpleNamespace) -> SimpleNamespace:
         if not hasattr(row, "geometry"):
             return row.attributes
 
         if self._shape_property_type is None or self._shape_property_type in self._unknown_shape_types:
             shape = row.geometry
         else:
-            if self._is_arcgis_gemetry:
+            if self.geometry_module == GeometryModule.arcgis:
                 shape = self._shape_property_type(row.geometry.__dict__)
+            elif self.geometry_module == GeometryModule.shapely:
+                shape = self._to_shapely(row.geometry.__dict__, self._shape_property_type)
             else:
                 shape = self._shape_property_type()
                 shape.__dict__ = row.geometry.__dict__
 
         return SimpleNamespace(**row.attributes.__dict__, **{self._shape_property_name: shape})
 
+    @staticmethod
+    def _from_shapely(shape: Any) -> Dict[str, Any]:
+        if shape.type == "Point":
+            if shape.has_z:
+                return {"x": shape.x, "y": shape.y, "z": shape.z}
+            else:
+                return {"x": shape.x, "y": shape.y}
+
+        if shape.type == "MultiPoint":
+            return {"points": [[p.x, p.y, p.z] if p.has_z else [p.x, p.y] for p in shape.geoms]}
+
+        if shape.type == "MultiLineString":
+            return {"paths": [[list(p) for p in path.coords] for path in shape.geoms]}
+
+        if shape.type == "MultiPolygon":
+            rings: List[List[List[float]]] = []
+            for polygon in shape.geoms:
+                for ring in [polygon.exterior] + list(polygon.interiors):
+                    rings.append([list(p) for p in ring.coords])
+            return {"rings": rings}
+
+        raise TypeError("Unsupported shape type.")
+
+    @staticmethod
+    def _to_shapely(d: Dict[str, Any], shape_type: Any) -> Any:
+        if "x" in d and "y" in d:
+            if "z" in d:
+                return shape_type(d["x"], d["y"], d["z"])
+            else:
+                return shape_type(d["x"], d["y"])
+
+        if "points" in d:
+            return shape_type(d["points"])
+
+        if "paths" in d:
+            return shape_type(d["paths"])
+
+        if "rings" in d:
+            polygons: List[Any] = []
+            shell = d["rings"][0]
+            holes: List[Any] = []
+            is_clockwise = Layer._is_clockwise(shell)
+            for ring in d["rings"][1:]:
+                if Layer._is_clockwise(ring) == is_clockwise:
+                    polygons.append([shell, holes])
+                    shell, holes = ring, []
+                else:
+                    holes.append(ring)
+            polygons.append([shell, holes])
+            return shape_type(polygons)
+
+        raise TypeError("Unsupported shape type.")
+
+    @staticmethod
+    def _is_clockwise(ring: List[List[float]]) -> bool:
+        return sum((ring[i + 1][0] - ring[i][0]) * (ring[i + 1][1] + ring[i][1]) for i in range(len(ring) - 1)) > 0
+
     def _query(self, where_clause: str, fields: str, record_count: Optional[int], max_workers: Optional[int],
                **kwargs: Any) -> Iterator[SimpleNamespace]:
         def get_rows(where_clause: str):
             return self._get_rows(where_clause, fields, **kwargs)
 
         rows, exceeded_transfer_limit = get_rows(where_clause)
 
@@ -540,19 +607,26 @@
 
         # Generate a where clause.
         where_clause = LambdaVisitor(expression, freevars, self._property_name_to_lower_field).to_sql().strip()
 
         return where_clause
 
 
+class GeometryModule(Enum):
+    none = 0
+    arcgis = 1
+    shapely = 2
+
+
 class Point:  # pylint: disable=too-few-public-methods
     """ Point class.
     """
     x: float
     y: float
+    z: Optional[float] = None
 
 
 class MultiPoint:  # pylint: disable=too-few-public-methods
     """ MultiPoint class.
     """
     points: List[List[float]]
```

### Comparing `hagis-0.7.3/pyproject.toml` & `hagis-0.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.7.3"
+version = "0.7.4"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

