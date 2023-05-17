# Comparing `tmp/geoserver-pyadm-1.0.0.tar.gz` & `tmp/geoserver-pyadm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoserver-pyadm-1.0.0.tar", last modified: Fri May 12 03:12:49 2023, max compression
+gzip compressed data, was "geoserver-pyadm-1.0.1.tar", last modified: Wed May 17 03:13:59 2023, max compression
```

## Comparing `geoserver-pyadm-1.0.0.tar` & `geoserver-pyadm-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 mchin      (501) staff       (20)        0 2023-05-12 03:12:49.602741 geoserver-pyadm-1.0.0/
--rw-r--r--   0 mchin      (501) staff       (20)     1068 2023-04-27 01:58:37.000000 geoserver-pyadm-1.0.0/LICENSE
--rw-r--r--   0 mchin      (501) staff       (20)       34 2023-04-27 03:03:07.000000 geoserver-pyadm-1.0.0/MANIFEST.in
--rw-r--r--   0 mchin      (501) staff       (20)     1810 2023-05-12 03:12:49.602247 geoserver-pyadm-1.0.0/PKG-INFO
--rw-r--r--   0 mchin      (501) staff       (20)       65 2023-05-12 03:08:50.000000 geoserver-pyadm-1.0.0/README.md
--rw-r--r--   0 mchin      (501) staff       (20)      833 2023-04-27 03:41:41.000000 geoserver-pyadm-1.0.0/pyproject.toml
--rw-r--r--   0 mchin      (501) staff       (20)       38 2023-05-12 03:12:49.602894 geoserver-pyadm-1.0.0/setup.cfg
-drwxr-xr-x   0 mchin      (501) staff       (20)        0 2023-05-12 03:12:49.586796 geoserver-pyadm-1.0.0/src/
-drwxr-xr-x   0 mchin      (501) staff       (20)        0 2023-05-12 03:12:49.593141 geoserver-pyadm-1.0.0/src/geoserver_pyadm/
--rw-r--r--   0 mchin      (501) staff       (20)      655 2023-05-12 00:42:21.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/__init__.py
--rw-r--r--   0 mchin      (501) staff       (20)      190 2023-04-27 02:09:35.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/__main__.py
--rw-r--r--   0 mchin      (501) staff       (20)     1915 2023-05-11 10:36:28.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/_auth.py
--rw-r--r--   0 mchin      (501) staff       (20)     1456 2023-05-12 01:32:31.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/_exceptions.py
--rw-r--r--   0 mchin      (501) staff       (20)     3917 2023-05-12 00:38:34.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/datastore.py
--rw-r--r--   0 mchin      (501) staff       (20)      661 2023-05-12 00:43:09.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/geoserver.py
--rw-r--r--   0 mchin      (501) staff       (20)      915 2023-05-12 00:28:22.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/info.py
--rw-r--r--   0 mchin      (501) staff       (20)     5550 2023-05-12 00:37:42.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/layer.py
--rw-r--r--   0 mchin      (501) staff       (20)     5819 2023-05-12 00:37:45.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/style.py
-drwxr-xr-x   0 mchin      (501) staff       (20)        0 2023-05-12 03:12:49.601276 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/
--rw-r--r--   0 mchin      (501) staff       (20)      701 2023-05-12 01:49:11.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/importer.py
--rw-r--r--   0 mchin      (501) staff       (20)      359 2023-05-04 03:16:18.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-add-and-upload-style.py
--rw-r--r--   0 mchin      (501) staff       (20)      611 2023-05-04 03:16:28.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-create-store.py
--rw-r--r--   0 mchin      (501) staff       (20)      107 2023-05-12 01:37:02.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-create-workspace.py
--rw-r--r--   0 mchin      (501) staff       (20)     1155 2023-05-09 02:18:45.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-delete-layer.py
--rw-r--r--   0 mchin      (501) staff       (20)      144 2023-05-04 03:16:40.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-delete-store.py
--rw-r--r--   0 mchin      (501) staff       (20)      186 2023-05-04 03:16:46.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-delete-style.py
--rw-r--r--   0 mchin      (501) staff       (20)      111 2023-05-12 01:54:29.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-delete-workspace.py
--rw-r--r--   0 mchin      (501) staff       (20)     1224 2023-05-05 05:26:00.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-get-functions.py
--rw-r--r--   0 mchin      (501) staff       (20)      144 2023-05-08 02:18:34.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-get-settings.py
--rw-r--r--   0 mchin      (501) staff       (20)      348 2023-05-04 03:14:36.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-modify-style.py
--rw-r--r--   0 mchin      (501) staff       (20)      340 2023-05-04 03:17:18.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-publish-raster-layer-on-server.py
--rw-r--r--   0 mchin      (501) staff       (20)      495 2023-05-04 03:17:26.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-publish-shapefiles-on-server.py
--rw-r--r--   0 mchin      (501) staff       (20)      447 2023-05-04 03:22:42.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-set-styles.py
--rw-r--r--   0 mchin      (501) staff       (20)     1205 2023-05-12 02:33:29.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-upload-local-raster.py
--rw-r--r--   0 mchin      (501) staff       (20)     1118 2023-05-09 01:42:15.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-upload-local-shapefiles.py
--rw-r--r--   0 mchin      (501) staff       (20)    10322 2023-05-12 02:49:06.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/upload.py
--rw-r--r--   0 mchin      (501) staff       (20)     2854 2023-05-12 01:35:28.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm/workspace.py
-drwxr-xr-x   0 mchin      (501) staff       (20)        0 2023-05-12 03:12:49.595050 geoserver-pyadm-1.0.0/src/geoserver_pyadm.egg-info/
--rw-r--r--   0 mchin      (501) staff       (20)     1810 2023-05-12 03:12:49.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm.egg-info/PKG-INFO
--rw-r--r--   0 mchin      (501) staff       (20)     1441 2023-05-12 03:12:49.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm.egg-info/SOURCES.txt
--rw-r--r--   0 mchin      (501) staff       (20)        1 2023-05-12 03:12:49.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm.egg-info/dependency_links.txt
--rw-r--r--   0 mchin      (501) staff       (20)       68 2023-05-12 03:12:49.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm.egg-info/entry_points.txt
--rw-r--r--   0 mchin      (501) staff       (20)       67 2023-05-12 03:12:49.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm.egg-info/requires.txt
--rw-r--r--   0 mchin      (501) staff       (20)       16 2023-05-12 03:12:49.000000 geoserver-pyadm-1.0.0/src/geoserver_pyadm.egg-info/top_level.txt
+drwxr-xr-x   0 mchin      (501) staff       (20)        0 2023-05-17 03:13:59.040167 geoserver-pyadm-1.0.1/
+-rw-r--r--   0 mchin      (501) staff       (20)     1068 2023-04-27 01:58:37.000000 geoserver-pyadm-1.0.1/LICENSE
+-rw-r--r--   0 mchin      (501) staff       (20)       34 2023-04-27 03:03:07.000000 geoserver-pyadm-1.0.1/MANIFEST.in
+-rw-r--r--   0 mchin      (501) staff       (20)     1810 2023-05-17 03:13:59.039874 geoserver-pyadm-1.0.1/PKG-INFO
+-rw-r--r--   0 mchin      (501) staff       (20)       65 2023-05-12 03:08:50.000000 geoserver-pyadm-1.0.1/README.md
+-rw-r--r--   0 mchin      (501) staff       (20)      833 2023-05-17 03:13:43.000000 geoserver-pyadm-1.0.1/pyproject.toml
+-rw-r--r--   0 mchin      (501) staff       (20)       38 2023-05-17 03:13:59.040255 geoserver-pyadm-1.0.1/setup.cfg
+drwxr-xr-x   0 mchin      (501) staff       (20)        0 2023-05-17 03:13:59.024604 geoserver-pyadm-1.0.1/src/
+drwxr-xr-x   0 mchin      (501) staff       (20)        0 2023-05-17 03:13:59.029331 geoserver-pyadm-1.0.1/src/geoserver_pyadm/
+-rw-r--r--   0 mchin      (501) staff       (20)      655 2023-05-12 00:42:21.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/__init__.py
+-rw-r--r--   0 mchin      (501) staff       (20)      190 2023-04-27 02:09:35.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/__main__.py
+-rw-r--r--   0 mchin      (501) staff       (20)     1915 2023-05-11 10:36:28.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/_auth.py
+-rw-r--r--   0 mchin      (501) staff       (20)     2942 2023-05-16 06:16:38.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/_exceptions.py
+-rw-r--r--   0 mchin      (501) staff       (20)     6032 2023-05-17 02:08:02.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/datastore.py
+-rw-r--r--   0 mchin      (501) staff       (20)      871 2023-05-17 02:04:04.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/geoserver.py
+-rw-r--r--   0 mchin      (501) staff       (20)      915 2023-05-12 00:28:22.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/info.py
+-rw-r--r--   0 mchin      (501) staff       (20)     6629 2023-05-17 00:56:24.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/layer.py
+-rw-r--r--   0 mchin      (501) staff       (20)     5832 2023-05-16 05:29:53.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/style.py
+drwxr-xr-x   0 mchin      (501) staff       (20)        0 2023-05-17 03:13:59.039437 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/
+-rw-r--r--   0 mchin      (501) staff       (20)      701 2023-05-12 01:49:11.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/importer.py
+-rw-r--r--   0 mchin      (501) staff       (20)      359 2023-05-04 03:16:18.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-add-and-upload-style.py
+-rw-r--r--   0 mchin      (501) staff       (20)      624 2023-05-17 02:06:34.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-create-store.py
+-rw-r--r--   0 mchin      (501) staff       (20)      107 2023-05-12 01:37:02.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-create-workspace.py
+-rw-r--r--   0 mchin      (501) staff       (20)     1155 2023-05-09 02:18:45.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-delete-layer.py
+-rw-r--r--   0 mchin      (501) staff       (20)      144 2023-05-04 03:16:40.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-delete-store.py
+-rw-r--r--   0 mchin      (501) staff       (20)      186 2023-05-04 03:16:46.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-delete-style.py
+-rw-r--r--   0 mchin      (501) staff       (20)      111 2023-05-12 01:54:29.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-delete-workspace.py
+-rw-r--r--   0 mchin      (501) staff       (20)     1224 2023-05-05 05:26:00.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-get-functions.py
+-rw-r--r--   0 mchin      (501) staff       (20)      144 2023-05-08 02:18:34.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-get-settings.py
+-rw-r--r--   0 mchin      (501) staff       (20)      348 2023-05-04 03:14:36.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-modify-style.py
+-rw-r--r--   0 mchin      (501) staff       (20)      340 2023-05-04 03:17:18.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-publish-raster-layer-on-server.py
+-rw-r--r--   0 mchin      (501) staff       (20)     1104 2023-05-16 05:55:08.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-publish-shapefiles-on-server.py
+-rw-r--r--   0 mchin      (501) staff       (20)      447 2023-05-04 03:22:42.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-set-styles.py
+-rw-r--r--   0 mchin      (501) staff       (20)     2204 2023-05-17 02:53:27.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-upload-geopackage.py
+-rw-r--r--   0 mchin      (501) staff       (20)     1374 2023-05-17 02:57:11.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-upload-local-raster.py
+-rw-r--r--   0 mchin      (501) staff       (20)     1118 2023-05-09 01:42:15.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-upload-local-shapefiles.py
+-rw-r--r--   0 mchin      (501) staff       (20)    15285 2023-05-17 02:45:20.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/upload.py
+-rw-r--r--   0 mchin      (501) staff       (20)     2854 2023-05-12 01:35:28.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm/workspace.py
+drwxr-xr-x   0 mchin      (501) staff       (20)        0 2023-05-17 03:13:59.031553 geoserver-pyadm-1.0.1/src/geoserver_pyadm.egg-info/
+-rw-r--r--   0 mchin      (501) staff       (20)     1810 2023-05-17 03:13:59.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm.egg-info/PKG-INFO
+-rw-r--r--   0 mchin      (501) staff       (20)     1492 2023-05-17 03:13:59.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm.egg-info/SOURCES.txt
+-rw-r--r--   0 mchin      (501) staff       (20)        1 2023-05-17 03:13:59.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm.egg-info/dependency_links.txt
+-rw-r--r--   0 mchin      (501) staff       (20)       68 2023-05-17 03:13:59.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm.egg-info/entry_points.txt
+-rw-r--r--   0 mchin      (501) staff       (20)       67 2023-05-17 03:13:59.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm.egg-info/requires.txt
+-rw-r--r--   0 mchin      (501) staff       (20)       16 2023-05-17 03:13:59.000000 geoserver-pyadm-1.0.1/src/geoserver_pyadm.egg-info/top_level.txt
```

### Comparing `geoserver-pyadm-1.0.0/LICENSE` & `geoserver-pyadm-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geoserver-pyadm-1.0.0/PKG-INFO` & `geoserver-pyadm-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoserver-pyadm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Geoserver Python client
 Author-email: Michael Chin <michael.chin@sydney.edu.au>
 License: MIT License
         
         Copyright (c) 2023 michaelchin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geoserver-pyadm-1.0.0/pyproject.toml` & `geoserver-pyadm-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geoserver-pyadm"
-version = "1.0.0"
+version = "1.0.1"
 description = "Geoserver Python client"
 readme = "README.md"
 authors = [{ name = "Michael Chin", email = "michael.chin@sydney.edu.au" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/__init__.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/__init__.py`

 * *Files identical despite different names*

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/_auth.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/_auth.py`

 * *Files identical despite different names*

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/geoserver.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/geoserver.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,21 +11,37 @@
 from .upload import (
     upload_raster,
     upload_raster_folder,
     upload_shapefile,
     upload_shapefile_folder,
     upload_shapefile_zip,
     upload_style,
+    upload_geopackage,
+    upload_geopackage_zip,
 )
 
 from .info import get_global_settings, get_status, get_version
 
-from .layer import get_layer, get_layer_styles, get_layers
+from .layer import (
+    get_layer,
+    get_layer_styles,
+    get_layers,
+    publish_layer,
+    publish_raster_layer,
+    delete_layer,
+    publish_geopackage_layer,
+)
 
-from .datastore import get_datastores, create_coveragestore, create_store, delete_store
+from .datastore import (
+    get_datastores,
+    create_coveragestore,
+    create_store,
+    delete_store,
+    create_geopackage_store,
+)
 
 from .style import (
     get_styles,
     modify_style,
     add_additional_style,
     add_style,
     delete_style,
```

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/info.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/info.py`

 * *Files identical despite different names*

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/layer.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import requests
+import requests, json
 
 from . import _auth as a
 from ._auth import auth
 
 
 @auth
 def publish_layer(workspace_name, store_name, layer_name):
@@ -117,15 +117,15 @@
     """Delete a layer/layers by name
 
     :param layer_name: the name of the layer which you would like to delete
     :param workspace:  (Default value = None) If the workspace name is not given,
         delete all layers with the given name.
 
     """
-    payload = {"recurse": "true", "quietOnNotFound": "true"}
+    payload = {"recurse": "True", "quietOnNotFound": "True"}
 
     if workspace:
         url = f"{a.server_url}/rest/workspaces/{workspace}/layers/{layer_name}"
         r = requests.delete(
             url=url,
             params=payload,
             auth=(a.username, a.passwd),
@@ -172,7 +172,40 @@
         ret = []
         data = r.json()
         if "style" in data["styles"]:
             ret = [d["name"] for d in data["styles"]["style"]]
         return ret
     else:
         return None
+
+
+@auth
+def publish_geopackage_layer(
+    workspace_name, store_name, layer_name, geom_type="polygon"
+):
+    """Publish a geopackage layer in the data store
+
+    :param workspace_name: the name of the workspace in which the data store is
+    :param store_name: the name of the data store in which the layer you would like to publish is
+    :param layer_name: the name of geopackage layer which you would like to publish.
+
+    """
+    url = f"{a.server_url}/rest/workspaces/{workspace_name}/datastores/{store_name}/featuretypes/"
+
+    layer_cfg = {
+        "featureType": {
+            "name": f"{layer_name}_{geom_type}",
+            "nativeName": f"{layer_name}_{geom_type}",
+            "title": f"{layer_name}_{geom_type}",
+        }
+    }
+    headers = {"content-type": "application/json"}
+
+    r = requests.post(
+        url,
+        data=json.dumps(layer_cfg),
+        auth=(a.username, a.passwd),
+        headers=headers,
+    )
+    if r.status_code not in [200, 201]:
+        print(f"Unable to publish layer {layer_name}. {r.status_code}, {r.content}")
+    return r
```

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/style.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/style.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 import requests
 
 from . import _auth as a
 from ._auth import auth
 
 
 @auth
```

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/importer.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/importer.py`

 * *Files identical despite different names*

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-create-store.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-create-store.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 store_name_2 = "a-test-store-2"
 
 r = geoserver.create_workspace(ws_name)
 print(r)
 
 # create a store from a folder on geoserver(relative path to "data_dir")
 # you can publish the layers in the folder later via web page or api
-r = geoserver.create_store(ws_name, store_name_1, "data/nyc")
+r = geoserver.create_store(ws_name, store_name_1, "data/nyc", is_dir=True)
 print(r)
 
 # create a store from a shapefile on geoserver(relative path to "data_dir")
 # you can publish the shapefile layer later via web page or api
 r = geoserver.create_store(ws_name, store_name_2, "data/shapefiles/states.shp")
 print(r)
```

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-delete-layer.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-delete-layer.py`

 * *Files identical despite different names*

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-get-functions.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-get-functions.py`

 * *Files identical despite different names*

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-upload-local-raster.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-upload-local-raster.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,7 +41,13 @@
 print(r)
 
 os.system(
     "zip -oj rasters/EarthByte_AREPS_Muller_etal_2016_AgeGrid-0.tiff.zip rasters/EarthByte_AREPS_Muller_etal_2016_AgeGrid-0.tiff"
 )
 
 os.system("rm -f rasters/EarthByte_AREPS_Muller_etal_2016_AgeGrid-0.tiff")
+
+if len(sys.argv) > 1:
+    print(sys.argv[1])
+    if sys.argv[1] == "clean":
+        geoserver.delete_workspace(ws_name_1)
+        geoserver.delete_workspace(ws_name_2)
```

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/test/test-upload-local-shapefiles.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/test/test-upload-local-shapefiles.py`

 * *Files identical despite different names*

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/upload.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/upload.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import glob
+import json
 import os
 import tempfile
 import zipfile
 from pathlib import Path
 
 import requests
 
@@ -157,52 +158,119 @@
         )
         if r.status_code not in [200, 201]:
             print(f"Unable to upload style {file_path}. {r.content}")
         return r
 
 
 @auth
-def upload_shapefile_zip(workspace_name, store_name, file_path, configure="none"):
+def upload_zip(workspace_name, store_name, file_path, format="shp", configure="none"):
     """Upload a local .zip file which contains shapefile.
         warning: when use configure="all", all the shapefiles in the datastore will
         be published(not only the one you just uploaded)
 
     :param workspace_name: the name of destine workspace in which you would like to
         upload the shapefile
     :param store_name: the name of datastore in which you would like to upload the shapefile
     :param file_path: the local file path to your shapefile(.zip)
+    :param format: support 'shp' and 'gpkg'
     :param configure: this parameter takes three possible values
         "first" —- (Default) Only setup the first feature type available in the data store.
         "none"  —- Do not configure any feature types.
         "all"   —- Configure all feature types.
 
     """
-    # a.username, a.passwd, a.server_url = get_cfg()
-
     headers = {
         "Content-type": "application/zip",
         "Accept": "application/xml",
     }
 
     file_name = Path(file_path).stem
     url = (
         f"{a.server_url}/rest/workspaces/{workspace_name}/datastores"
-        + f"/{store_name}/file.shp?filename={file_name}&update=overwrite&configure={configure}"
+        + f"/{store_name}/file.{format}?filename={file_name}&update=overwrite&configure={configure}"
     )
 
     with open(file_path, "rb") as f:
         r = requests.put(
             url,
             data=f.read(),
             auth=(a.username, a.passwd),
             headers=headers,
         )
     return r
 
 
+def upload_geopackage_zip(workspace_name, store_name, file_path, configure="none"):
+    """Upload a local .zip file which contains geopackage file.
+        warning: when use configure="all", all the shapefiles in the datastore will
+        be published(not only the one you just uploaded)
+
+    :param workspace_name: the name of destine workspace in which you would like to
+        upload the shapefile
+    :param store_name: the name of datastore in which you would like to upload the shapefile
+    :param file_path: the local file path to your geopackage(.zip)
+    :param configure: this parameter takes three possible values
+        "first" —- (Default) Only setup the first feature type available in the data store.
+        "none"  —- Do not configure any feature types.
+        "all"   —- Configure all feature types.
+
+    """
+    r = upload_zip(workspace_name, store_name, file_path, "gpkg", configure)
+
+    # it seems there is bug in geoserver 2.21
+    # I have to update the "database" path to make the store valid
+    headers = {
+        "Content-type": "application/json",
+    }
+
+    cfg = {
+        "dataStore": {
+            "name": store_name,
+            "type": "GeoPackage",
+            "connectionParameters": {
+                "entry": [
+                    {
+                        "@key": "database",
+                        "$": f"file:data/{workspace_name}/{store_name}/{os.path.basename(file_path)[:-4]}",
+                    },
+                    {"@key": "dbtype", "$": "geopkg"},
+                ]
+            },
+        }
+    }
+
+    url = f"{a.server_url}/rest/workspaces/{workspace_name}/datastores/{store_name}/"
+
+    requests.put(
+        url,
+        data=json.dumps(cfg),
+        auth=(a.username, a.passwd),
+        headers=headers,
+    )
+    return r
+
+
+def upload_shapefile_zip(workspace_name, store_name, file_path, configure="none"):
+    """Upload a local .zip file which contains shapefile.
+        warning: when use configure="all", all the shapefiles in the datastore will
+        be published(not only the one you just uploaded)
+
+    :param workspace_name: the name of destine workspace in which you would like to
+        upload the shapefile
+    :param store_name: the name of datastore in which you would like to upload the shapefile
+    :param file_path: the local file path to your shapefile(.zip)
+    :param configure: this parameter takes three possible values
+        "first" —- (Default) Only setup the first feature type available in the data store.
+        "none"  —- Do not configure any feature types.
+        "all"   —- Configure all feature types.
+
+    """
+    return upload_zip(workspace_name, store_name, file_path, "shp", configure)
+
+
 def upload_shapefile(workspace_name, store_name, file_path, configure="none"):
     """Upload a local shapefile. A shapefile may contain several files.
         You need to specify the path of the .shp file.
 
         warning: when use configure="all", all the shapefiles in the datastore will
         be published(not only the one you just uploaded)
 
@@ -229,22 +297,84 @@
                 f"{tmp_dir}/{file_name}.zip",
                 mode="w",
                 compression=zipfile.ZIP_DEFLATED,
                 compresslevel=9,
             ) as tmp_zip:
                 for f in files:
                     tmp_zip.write(f, os.path.basename(f))
-            t = f"{tmp_dir}/{file_name}.zip"
+
             return upload_shapefile_zip(
                 workspace_name, store_name, f"{tmp_dir}/{file_name}.zip", configure
             )
     else:
         raise Exception(f"Unsupported file extension: {file_path}")
 
 
+def upload_geopackage(workspace_name, store_name, file_path, configure="none"):
+    """Upload a local geopackage file.
+
+        warning: when use configure="all", all the shapefiles in the datastore will
+        be published(not only the one you just uploaded)
+
+    :param workspace_name: the name of destine workspace in which you would like to
+        upload the shapefile
+    :param store_name: the name of datastore in which you would like to upload the shapefile
+    :param file_path: the local path to your geopackge file
+    :param configure: this parameter takes three possible values
+        first—(Default) Only setup the first feature type available in the data store.
+        none—Do not configure any feature types.
+        all—Configure all feature types.
+
+    """
+    p = Path(file_path)
+    file_name = p.stem
+    ext = p.suffix
+
+    if ext == ".zip":
+        return upload_zip(workspace_name, store_name, file_path, "gpkg", configure)
+    elif ext == ".gpkg":
+        """
+        # upload geopackage file without compression
+        headers = {
+            "Content-type": "application/x-sqlite3",
+            "Accept": "application/xml",
+        }
+
+        url = (
+            f"{a.server_url}/rest/workspaces/{workspace_name}/datastores"
+            + f"/{store_name}/file.gpkg?filename={file_name}{ext}&update=overwrite&configure={configure}"
+        )
+
+        with open(file_path, "rb") as f:
+            r = requests.put(
+                url,
+                data=f.read(),
+                auth=(a.username, a.passwd),
+                headers=headers,
+            )"""
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            files = glob.glob(f"{file_path[:-5]}.*")
+            with zipfile.ZipFile(
+                f"{tmp_dir}/{file_name}{ext}.zip",
+                mode="w",
+                compression=zipfile.ZIP_DEFLATED,
+                compresslevel=9,
+            ) as tmp_zip:
+                for f in files:
+                    tmp_zip.write(f, os.path.basename(f))
+            return upload_geopackage_zip(
+                workspace_name,
+                store_name,
+                f"{tmp_dir}/{file_name}{ext}.zip",
+                configure,
+            )
+    else:
+        raise Exception(f"Unsupported file extension: {file_path}")
+
+
 def upload_shapefile_folder(workspace_name, store_name, folder_path, configure="none"):
     """Upload all the shapefiles within a local folder. The shapefiles can be .zip files or separate files.
         Make sure your .zip is valid. If there is a folder in your .zip file, the upload will fail.
         For example, if, inside you .zip file, your files looks like shapefile/xxxxxxx.shp, the .zip file cannot be uploaded.
         Inside your .zip file, it must looks like this xxxxxxxx.shp, xxxxxxxx.dbf, etc.
 
         warning: when use configure="all", all the shapefiles in the datastore will
```

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm/workspace.py` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm/workspace.py`

 * *Files identical despite different names*

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm.egg-info/PKG-INFO` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoserver-pyadm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Geoserver Python client
 Author-email: Michael Chin <michael.chin@sydney.edu.au>
 License: MIT License
         
         Copyright (c) 2023 michaelchin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geoserver-pyadm-1.0.0/src/geoserver_pyadm.egg-info/SOURCES.txt` & `geoserver-pyadm-1.0.1/src/geoserver_pyadm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,9 +29,10 @@
 src/geoserver_pyadm/test/test-delete-workspace.py
 src/geoserver_pyadm/test/test-get-functions.py
 src/geoserver_pyadm/test/test-get-settings.py
 src/geoserver_pyadm/test/test-modify-style.py
 src/geoserver_pyadm/test/test-publish-raster-layer-on-server.py
 src/geoserver_pyadm/test/test-publish-shapefiles-on-server.py
 src/geoserver_pyadm/test/test-set-styles.py
+src/geoserver_pyadm/test/test-upload-geopackage.py
 src/geoserver_pyadm/test/test-upload-local-raster.py
 src/geoserver_pyadm/test/test-upload-local-shapefiles.py
```

