# Comparing `tmp/Geode_Background-7.1.3-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Background-7.1.4-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 3416631 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      195 b- defN 23-May-12 12:22 geode_background/__init__.py
--rw-rw-rw-  2.0 fat      199 b- defN 23-May-12 12:22 geode_background/solid.py
--rw-rw-rw-  2.0 fat      203 b- defN 23-May-12 12:22 geode_background/surface.py
--rw-rw-rw-  2.0 fat  2102784 b- defN 23-May-12 12:23 geode_background/bin/Geode-Background_brep.dll
--rw-rw-rw-  2.0 fat    60928 b- defN 23-May-12 12:23 geode_background/bin/Geode-Background_common.dll
--rw-rw-rw-  2.0 fat  2377728 b- defN 23-May-12 12:23 geode_background/bin/Geode-Background_solid.dll
--rw-rw-rw-  2.0 fat  2170880 b- defN 23-May-12 12:23 geode_background/bin/Geode-Background_surface.dll
--rw-rw-rw-  2.0 fat   125440 b- defN 23-May-12 12:23 geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   124928 b- defN 23-May-12 12:23 geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   125440 b- defN 23-May-12 12:23 geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1103 b- defN 23-May-12 12:23 Geode_Background-7.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-12 12:23 Geode_Background-7.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-12 12:23 Geode_Background-7.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1386 b- defN 23-May-12 12:23 Geode_Background-7.1.3.dist-info/RECORD
-14 files, 7091331 bytes uncompressed, 3414281 bytes compressed:  51.9%
+Zip file size: 4922470 bytes, number of entries: 14
+-rw-r--r--  2.0 unx       90 b- defN 23-May-17 15:35 geode_background/__init__.py
+-rw-r--r--  2.0 unx      192 b- defN 23-May-17 15:35 geode_background/solid.py
+-rw-r--r--  2.0 unx      196 b- defN 23-May-17 15:35 geode_background/surface.py
+-rwxr-xr-x  2.0 unx   122232 b- defN 23-May-17 15:36 geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   122232 b- defN 23-May-17 15:36 geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   122232 b- defN 23-May-17 15:36 geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx  3562624 b- defN 23-May-17 15:36 geode_background/lib64/libGeode-Background_brep.so
+-rwxr-xr-x  2.0 unx   206696 b- defN 23-May-17 15:36 geode_background/lib64/libGeode-Background_common.so
+-rwxr-xr-x  2.0 unx  3983096 b- defN 23-May-17 15:36 geode_background/lib64/libGeode-Background_solid.so
+-rwxr-xr-x  2.0 unx  3651968 b- defN 23-May-17 15:36 geode_background/lib64/libGeode-Background_surface.so
+-rw-r--r--  2.0 unx     1059 b- defN 23-May-17 15:36 Geode_Background-7.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-May-17 15:36 Geode_Background-7.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-17 15:36 Geode_Background-7.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1444 b- defN 23-May-17 15:36 Geode_Background-7.1.4.dist-info/RECORD
+14 files, 11774181 bytes uncompressed, 4920004 bytes compressed:  58.2%
```

## zipnote {}

```diff
@@ -3,41 +3,41 @@
 
 Filename: geode_background/solid.py
 Comment: 
 
 Filename: geode_background/surface.py
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_brep.dll
+Filename: geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_common.dll
+Filename: geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_solid.dll
+Filename: geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_surface.dll
+Filename: geode_background/lib64/libGeode-Background_brep.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_common.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_solid.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_surface.so
 Comment: 
 
-Filename: Geode_Background-7.1.3.dist-info/METADATA
+Filename: Geode_Background-7.1.4.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Background-7.1.3.dist-info/WHEEL
+Filename: Geode_Background-7.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Background-7.1.3.dist-info/top_level.txt
+Filename: Geode_Background-7.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Background-7.1.3.dist-info/RECORD
+Filename: Geode_Background-7.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_background/__init__.py

```diff
@@ -1,7 +1,4 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .surface import *
-from .solid import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+from .surface import *
+from .solid import *
```

## geode_background/solid.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .bin.geode_background_py_solid import *
-BackgroundSolidLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .lib64.geode_background_py_solid import *
+BackgroundSolidLibrary.initialize()
```

## geode_background/surface.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .bin.geode_background_py_surface import *
-BackgroundSurfaceLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .lib64.geode_background_py_surface import *
+BackgroundSurfaceLibrary.initialize()
```

## Comparing `Geode_Background-7.1.3.dist-info/METADATA` & `Geode_Background-7.1.4.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 2.1
-Name: Geode-Background
-Version: 7.1.3
-Summary: Geode-solutions OpenGeode module for building background meshes
-Home-page: https://github.com/Geode-solutions/Geode-Background
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: geode-common (==25.*,>=25.0.7)
-Requires-Dist: opengeode-core (==14.*,>=14.0.17)
-
-<h1 align="center">BackgroundMesh<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Module to generate a background mesh for OpenGeode</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/BackgroundMesh_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/BackgroundMesh_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/BackgroundMesh_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/BackgroundMesh_private.svg" alt="Version">
-</p>
-
-
+Metadata-Version: 2.1
+Name: Geode-Background
+Version: 7.1.4
+Summary: Geode-solutions OpenGeode module for building background meshes
+Home-page: https://github.com/Geode-solutions/Geode-Background
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Description-Content-Type: text/markdown
+Requires-Dist: geode-common (==25.*,>=25.0.7)
+Requires-Dist: opengeode-core (==14.*,>=14.0.17)
+
+<h1 align="center">BackgroundMesh<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Module to generate a background mesh for OpenGeode</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/BackgroundMesh_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/BackgroundMesh_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/BackgroundMesh_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/BackgroundMesh_private.svg" alt="Version">
+</p>
```

