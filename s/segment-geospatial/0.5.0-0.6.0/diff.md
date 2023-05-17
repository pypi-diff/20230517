# Comparing `tmp/segment-geospatial-0.5.0.tar.gz` & `tmp/segment-geospatial-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.5.0.tar", last modified: Wed May 10 20:59:47 2023, max compression
+gzip compressed data, was "segment-geospatial-0.6.0.tar", last modified: Wed May 17 02:18:45 2023, max compression
```

## Comparing `segment-geospatial-0.5.0.tar` & `segment-geospatial-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:59:47.082303 segment-geospatial-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-10 20:59:47.082303 segment-geospatial-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:59:47.078302 segment-geospatial-0.5.0/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/samgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    26344 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/samgeo/samgeo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:59:47.082303 segment-geospatial-0.5.0/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-10 20:59:46.000000 segment-geospatial-0.5.0/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-10 20:59:47.000000 segment-geospatial-0.5.0/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-10 20:59:46.000000 segment-geospatial-0.5.0/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:59:46.000000 segment-geospatial-0.5.0/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-10 20:59:46.000000 segment-geospatial-0.5.0/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 20:59:46.000000 segment-geospatial-0.5.0/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-10 20:59:47.082303 segment-geospatial-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:18:45.848643 segment-geospatial-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-17 02:18:45.848643 segment-geospatial-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:18:45.848643 segment-geospatial-0.6.0/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68522 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26605 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/samgeo/samgeo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:18:45.848643 segment-geospatial-0.6.0/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-17 02:18:45.000000 segment-geospatial-0.6.0/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-17 02:18:45.000000 segment-geospatial-0.6.0/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-17 02:18:45.000000 segment-geospatial-0.6.0/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 02:18:45.000000 segment-geospatial-0.6.0/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-17 02:18:45.000000 segment-geospatial-0.6.0/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 02:18:45.000000 segment-geospatial-0.6.0/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-17 02:18:45.848643 segment-geospatial-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-17 02:18:36.000000 segment-geospatial-0.6.0/setup.py
```

### Comparing `segment-geospatial-0.5.0/LICENSE` & `segment-geospatial-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.5.0/PKG-INFO` & `segment-geospatial-0.6.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: segment-geospatial
-Version: 0.5.0
-Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
-Home-page: https://github.com/opengeos/segment-geospatial
-Author: Qiusheng Wu
-Author-email: giswqs@gmail.com
-License: MIT license
-Keywords: samgeo
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: all
-License-File: LICENSE
-
 # segment-geospatial
 
 [![image](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/badge/Open-Planetary%20Computer-black?style=flat&logo=microsoft)](https://pccompute.westeurope.cloudapp.azure.com/compute/hub/user-redirect/git-pull?repo=https://github.com/opengeos/segment-geospatial&urlpath=lab/tree/segment-geospatial/docs/examples/satellite.ipynb&branch=main)
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/pypi/v/segment-geospatial.svg)](https://pypi.python.org/pypi/segment-geospatial)
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
@@ -35,15 +13,18 @@
 -   Free software: MIT license
 -   Documentation: <https://samgeo.gishub.org>
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
+-   Create foreground and background markers interactively
+-   Load existing markers from vector datasets
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
+-   Save input prompts as GeoJSON files
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
 -   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
@@ -52,22 +33,35 @@
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
 
 -   Interactive segmentation with input prompts
 
-![](https://i.imgur.com/GV7Rzxt.gif)
+![](https://i.imgur.com/2Nyg9uW.gif)
+
+-   Input prompts from existing files
+
+![](https://i.imgur.com/Cb4ZaKY.gif)
 
 ## Tutorials
 
 Video tutorials are available on my [YouTube Channel](https://youtube.com/@giswqs).
 
 [![Alt text](https://img.youtube.com/vi/YHA_-QMB8_U/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
 
+## Using SAM with Desktop GIS
+
+-   **QGIS**: Check out the [Geometric Attributes plugin for QGIS](https://github.com/BjornNyberg/Geometric-Attributes-Toolbox/wiki/User-Guide#segment-anything-model). Credit goes to [Bjorn Nyberg](https://github.com/BjornNyberg).
+-   **ArcGIS**: Check out the [Segment Anything Model (SAM) Toolbox for ArcGIS](https://www.arcgis.com/home/item.html?id=9b67b441f29f4ce6810979f5f0667ebe). Credit goes to [Esri](https://www.esri.com).
+
+## Computing Resources
+
+The Segment Anything Model is computationally intensive, and a powerful GPU is recommended to process large datasets. It is recommended to have a GPU with at least 8 GB of GPU memory. You can utilize the free GPU resources provided by Google Colab. Alternatively, you can apply for [AWS Cloud Credit for Research](https://aws.amazon.com/government-education/research-and-technical-computing/cloud-credit-for-research), which offers cloud credits to support academic research. If you are in the Greater China region, apply for the AWS Cloud Credit [here](https://aws.amazon.com/cn/events/educate_cloud/research-credits).
+
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
```

### Comparing `segment-geospatial-0.5.0/samgeo/common.py` & `segment-geospatial-0.6.0/samgeo/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 import shapely
 import pyproj
 import rasterio
 import geopandas as gpd
 import matplotlib.pyplot as plt
 
 
+def is_colab():
+    """Tests if the code is being executed within Google Colab."""
+    import sys
+
+    if "google.colab" in sys.modules:
+        return True
+    else:
+        return False
+
+
 def check_file_path(file_path, make_dirs=True):
     """Gets the absolute file path.
 
     Args:
         file_path (str): The path to the file.
         make_dirs (bool, optional): Whether to create the directory if it does not exist. Defaults to True.
 
@@ -521,15 +531,17 @@
                 )
             bbox = (math.floor(x0), math.floor(y0), math.ceil(x1), math.ceil(y1))
             bigim = None
             base_size = [256, 256]
             for k, (fut, corner_xy) in enumerate(zip(futures, corners), 1):
                 bigim = paste_tile(bigim, base_size, fut.result(), corner_xy, bbox)
                 if not quiet:
-                    print("Downloaded image %d/%d" % (k, totalnum))
+                    print(
+                        f"Downloaded image {str(k).zfill(len(str(totalnum)))}/{totalnum}"
+                    )
 
         if not quiet:
             print("Saving GeoTIFF. Please wait...")
         img = finish_picture(bigim, base_size, bbox, x0, y0, x1, y1)
         imgbands = len(img.getbands())
         driver = gdal.GetDriverByName("GTiff")
 
@@ -588,14 +600,15 @@
 def get_crs(src_fp):
     with rasterio.open(src_fp) as src:
         return src.crs
 
 
 def get_features(src_fp, bidx=1):
     from rasterio import features
+
     with rasterio.open(src_fp) as src:
         features = features.dataset_features(
             src,
             bidx=bidx,
             sampling=1,
             band=True,
             as_mask=False,
@@ -732,14 +745,101 @@
         print("No valid pixel coordinates found.")
     elif len(result) < len(coords):
         print("Some coordinates are out of the image boundary.")
 
     return result
 
 
+def bbox_to_xy(
+    src_fp: str, coords: list, coord_crs: str = "epsg:4326", **kwargs
+) -> list:
+    """Converts a list of coordinates to pixel coordinates, i.e., (col, row) coordinates.
+
+    Args:
+        src_fp (str): The source raster file path.
+        coords (list): A list of coordinates in the format of [[minx, miny, maxx, maxy], [minx, miny, maxx, maxy], ...]
+        coord_crs (str, optional): The coordinate CRS of the input coordinates. Defaults to "epsg:4326".
+
+    Returns:
+        list: A list of pixel coordinates in the format of [[minx, miny, maxx, maxy], ...]
+    """
+
+    if isinstance(coords, str):
+        gdf = gpd.read_file(coords)
+        coords = gdf.geometry.bounds.values.tolist()
+        if gdf.crs is not None:
+            coord_crs = f"epsg:{gdf.crs.to_epsg()}"
+    elif isinstance(coords, np.ndarray):
+        coords = coords.tolist()
+    if isinstance(coords, dict):
+        import json
+
+        geojson = json.dumps(coords)
+        gdf = gpd.read_file(geojson, driver="GeoJSON")
+        coords = gdf.geometry.bounds.values.tolist()
+
+    elif not isinstance(coords, list):
+        raise ValueError("coords must be a list of coordinates.")
+
+    if not isinstance(coords[0], list):
+        coords = [coords]
+
+    new_coords = []
+
+    with rasterio.open(src_fp) as src:
+        width = src.width
+        height = src.height
+
+        for coord in coords:
+            minx, miny, maxx, maxy = coord
+
+            if coord_crs != src.crs:
+                minx, miny = transform_coords(minx, miny, coord_crs, src.crs, **kwargs)
+                maxx, maxy = transform_coords(maxx, maxy, coord_crs, src.crs, **kwargs)
+
+                rows1, cols1 = rasterio.transform.rowcol(
+                    src.transform, minx, miny, **kwargs
+                )
+                rows2, cols2 = rasterio.transform.rowcol(
+                    src.transform, maxx, maxy, **kwargs
+                )
+
+                new_coords.append([cols1, rows1, cols2, rows2])
+
+            else:
+                new_coords.append([minx, miny, maxx, maxy])
+
+    result = []
+
+    for coord in new_coords:
+        minx, miny, maxx, maxy = coord
+
+        if (
+            minx >= 0
+            and miny >= 0
+            and maxx >= 0
+            and maxy >= 0
+            and minx < width
+            and miny < height
+            and maxx < width
+            and maxy < height
+        ):
+            result.append(coord)
+
+    if len(result) == 0:
+        print("No valid pixel coordinates found.")
+        return None
+    elif len(result) == 1:
+        return result[0]
+    elif len(result) < len(coords):
+        print("Some coordinates are out of the image boundary.")
+
+    return result
+
+
 def geojson_to_xy(
     src_fp: str, geojson: str, coord_crs: str = "epsg:4326", **kwargs
 ) -> list:
     """Converts a geojson file or a dictionary of feature collection to a list of pixel coordinates.
 
     Args:
         src_fp: The source raster file path.
@@ -1463,94 +1563,270 @@
 
         print("Package updated successfully.")
 
     except Exception as e:
         raise Exception(e)
 
 
-def sam_map_gui(sam, basemap="SATELLITE", repeat_mode=True, **kwargs):
+def sam_map_gui(sam, basemap="SATELLITE", repeat_mode=True, out_dir=None, **kwargs):
+    """Display the SAM Map GUI.
+
+    Args:
+        sam (SamGeo):
+        basemap (str, optional): The basemap to use. Defaults to "SATELLITE".
+        repeat_mode (bool, optional): Whether to use the repeat mode for the draw control. Defaults to True.
+        out_dir (str, optional): The output directory. Defaults to None.
+
+    """
     try:
+        import shutil
+        import tempfile
         import leafmap
         import ipyleaflet
         import ipyevents
         import ipywidgets as widgets
+        from ipyfilechooser import FileChooser
     except ImportError:
         raise ImportError(
             "The sam_map function requires the leafmap package. Please install it first."
         )
 
+    if out_dir is None:
+        out_dir = tempfile.gettempdir()
+
     m = leafmap.Map(repeat_mode=repeat_mode, **kwargs)
+    m.default_style = {"cursor": "crosshair"}
     m.add_basemap(basemap, show=False)
-    m.add_raster(sam.image, layer_name="Image")
 
-    widget_width = "100px"
-    padding = "0px 0px 0px 5px"  # upper, right, bottom, left
+    # Skip the image layer if localtileserver is not available
+    try:
+        m.add_raster(sam.image, layer_name="Image")
+    except:
+        pass
+
+    m.fg_markers = []
+    m.bg_markers = []
+
+    fg_layer = ipyleaflet.LayerGroup(layers=m.fg_markers, name="Foreground")
+    bg_layer = ipyleaflet.LayerGroup(layers=m.bg_markers, name="Background")
+    m.add(fg_layer)
+    m.add(bg_layer)
+    m.fg_layer = fg_layer
+    m.bg_layer = bg_layer
+
+    widget_width = "280px"
+    button_width = "90px"
+    padding = "0px 0px 0px 4px"  # upper, right, bottom, left
     style = {"description_width": "initial"}
 
     toolbar_button = widgets.ToggleButton(
         value=True,
         tooltip="Toolbar",
         icon="gear",
-        layout=widgets.Layout(width="28px", height="28px", padding="0px 0px 0px 4px"),
+        layout=widgets.Layout(width="28px", height="28px", padding=padding),
     )
 
     close_button = widgets.ToggleButton(
         value=False,
         tooltip="Close the tool",
         icon="times",
         button_style="primary",
-        layout=widgets.Layout(height="28px", width="28px", padding="0px 0px 0px 4px"),
+        layout=widgets.Layout(height="28px", width="28px", padding=padding),
+    )
+
+    plus_button = widgets.ToggleButton(
+        value=False,
+        tooltip="Load foreground points",
+        icon="plus-circle",
+        button_style="primary",
+        layout=widgets.Layout(height="28px", width="28px", padding=padding),
+    )
+
+    minus_button = widgets.ToggleButton(
+        value=False,
+        tooltip="Load background points",
+        icon="minus-circle",
+        button_style="primary",
+        layout=widgets.Layout(height="28px", width="28px", padding=padding),
+    )
+
+    radio_buttons = widgets.RadioButtons(
+        options=["Foreground", "Background"],
+        description="Class Type:",
+        disabled=False,
+        style=style,
+        layout=widgets.Layout(width=widget_width, padding=padding),
+    )
+
+    fg_count = widgets.IntText(
+        value=0,
+        description="Foreground #:",
+        disabled=True,
+        style=style,
+        layout=widgets.Layout(width="135px", padding=padding),
+    )
+    bg_count = widgets.IntText(
+        value=0,
+        description="Background #:",
+        disabled=True,
+        style=style,
+        layout=widgets.Layout(width="135px", padding=padding),
     )
 
     segment_button = widgets.ToggleButton(
-        description="Segment", value=False, button_style="primary"
+        description="Segment",
+        value=False,
+        button_style="primary",
+        layout=widgets.Layout(padding=padding),
+    )
+
+    save_button = widgets.ToggleButton(
+        description="Save", value=False, button_style="primary"
     )
+
     reset_button = widgets.ToggleButton(
         description="Reset", value=False, button_style="primary"
     )
-    segment_button.layout.width = widget_width
-    reset_button.layout.width = widget_width
-
-    buttons = widgets.VBox([segment_button, reset_button])
+    segment_button.layout.width = button_width
+    save_button.layout.width = button_width
+    reset_button.layout.width = button_width
 
     opacity_slider = widgets.FloatSlider(
+        description="Mask opacity:",
         min=0,
         max=1,
         value=0.5,
-        readout=False,
+        readout=True,
         continuous_update=True,
-        layout=widgets.Layout(width="95px"),
+        layout=widgets.Layout(width=widget_width, padding=padding),
         style=style,
     )
+    buttons = widgets.VBox(
+        [
+            radio_buttons,
+            widgets.HBox([fg_count, bg_count]),
+            opacity_slider,
+            widgets.HBox(
+                [segment_button, save_button, reset_button],
+                layout=widgets.Layout(padding="0px 4px 0px 4px"),
+            ),
+        ]
+    )
 
     def opacity_changed(change):
         if change["new"]:
             mask_layer = m.find_layer("Masks")
             if mask_layer is not None:
                 mask_layer.interact(opacity=opacity_slider.value)
 
     opacity_slider.observe(opacity_changed, "value")
 
-    output = widgets.Output(layout=widgets.Layout(width=widget_width, padding=padding))
+    output = widgets.Output(
+        layout=widgets.Layout(
+            width=widget_width, padding=padding, max_width=widget_width
+        )
+    )
 
     toolbar_header = widgets.HBox()
-    toolbar_header.children = [close_button, toolbar_button]
+    toolbar_header.children = [close_button, plus_button, minus_button, toolbar_button]
     toolbar_footer = widgets.VBox()
     toolbar_footer.children = [
         buttons,
-        opacity_slider,
         output,
     ]
     toolbar_widget = widgets.VBox()
     toolbar_widget.children = [toolbar_header, toolbar_footer]
 
     toolbar_event = ipyevents.Event(
         source=toolbar_widget, watched_events=["mouseenter", "mouseleave"]
     )
 
+    def marker_callback(chooser):
+        with output:
+            if chooser.selected is not None:
+                try:
+                    gdf = gpd.read_file(chooser.selected)
+                    centroids = gdf.centroid
+                    coords = [[point.x, point.y] for point in centroids]
+                    for coord in coords:
+                        if plus_button.value:
+                            if is_colab():  # Colab does not support AwesomeIcon
+                                marker = ipyleaflet.CircleMarker(
+                                    location=(coord[1], coord[0]),
+                                    radius=2,
+                                    color="green",
+                                    fill_color="green",
+                                )
+                            else:
+                                marker = ipyleaflet.Marker(
+                                    location=[coord[1], coord[0]],
+                                    icon=ipyleaflet.AwesomeIcon(
+                                        name="plus-circle",
+                                        marker_color="green",
+                                        icon_color="darkred",
+                                    ),
+                                )
+                            m.fg_layer.add(marker)
+                            m.fg_markers.append(marker)
+                            fg_count.value = len(m.fg_markers)
+                        elif minus_button.value:
+                            if is_colab():
+                                marker = ipyleaflet.CircleMarker(
+                                    location=(coord[1], coord[0]),
+                                    radius=2,
+                                    color="red",
+                                    fill_color="red",
+                                )
+                            else:
+                                marker = ipyleaflet.Marker(
+                                    location=[coord[1], coord[0]],
+                                    icon=ipyleaflet.AwesomeIcon(
+                                        name="minus-circle",
+                                        marker_color="red",
+                                        icon_color="darkred",
+                                    ),
+                                )
+                            m.bg_layer.add(marker)
+                            m.bg_markers.append(marker)
+                            bg_count.value = len(m.bg_markers)
+
+                except Exception as e:
+                    print(e)
+
+            if m.marker_control in m.controls:
+                m.remove_control(m.marker_control)
+                delattr(m, "marker_control")
+
+            plus_button.value = False
+            minus_button.value = False
+
+    def marker_button_click(change):
+        if change["new"]:
+            sandbox_path = os.environ.get("SANDBOX_PATH")
+            filechooser = FileChooser(
+                path=os.getcwd(),
+                sandbox_path=sandbox_path,
+                layout=widgets.Layout(width="454px"),
+            )
+            filechooser.use_dir_icons = True
+            filechooser.filter_pattern = ["*.shp", "*.geojson", "*.gpkg"]
+            filechooser.register_callback(marker_callback)
+            marker_control = ipyleaflet.WidgetControl(
+                widget=filechooser, position="topright"
+            )
+            m.add_control(marker_control)
+            m.marker_control = marker_control
+        else:
+            if hasattr(m, "marker_control") and m.marker_control in m.controls:
+                m.remove_control(m.marker_control)
+                m.marker_control.close()
+
+    plus_button.observe(marker_button_click, "value")
+    minus_button.observe(marker_button_click, "value")
+
     def handle_toolbar_event(event):
         if event["type"] == "mouseenter":
             toolbar_widget.children = [toolbar_header, toolbar_footer]
         elif event["type"] == "mouseleave":
             if not toolbar_button.value:
                 toolbar_widget.children = [toolbar_button]
                 toolbar_button.value = False
@@ -1573,44 +1849,202 @@
             toolbar_button.value = False
             if m.toolbar_control in m.controls:
                 m.remove_control(m.toolbar_control)
             toolbar_widget.close()
 
     close_button.observe(close_btn_click, "value")
 
+    def handle_map_interaction(**kwargs):
+        try:
+            if kwargs.get("type") == "click":
+                latlon = kwargs.get("coordinates")
+                if radio_buttons.value == "Foreground":
+                    if is_colab():
+                        marker = ipyleaflet.CircleMarker(
+                            location=tuple(latlon),
+                            radius=2,
+                            color="green",
+                            fill_color="green",
+                        )
+                    else:
+                        marker = ipyleaflet.Marker(
+                            location=latlon,
+                            icon=ipyleaflet.AwesomeIcon(
+                                name="plus-circle",
+                                marker_color="green",
+                                icon_color="darkred",
+                            ),
+                        )
+                    fg_layer.add(marker)
+                    m.fg_markers.append(marker)
+                    fg_count.value = len(m.fg_markers)
+                elif radio_buttons.value == "Background":
+                    if is_colab():
+                        marker = ipyleaflet.CircleMarker(
+                            location=tuple(latlon),
+                            radius=2,
+                            color="red",
+                            fill_color="red",
+                        )
+                    else:
+                        marker = ipyleaflet.Marker(
+                            location=latlon,
+                            icon=ipyleaflet.AwesomeIcon(
+                                name="minus-circle",
+                                marker_color="red",
+                                icon_color="darkred",
+                            ),
+                        )
+                    bg_layer.add(marker)
+                    m.bg_markers.append(marker)
+                    bg_count.value = len(m.bg_markers)
+
+        except (TypeError, KeyError) as e:
+            print(f"Error handling map interaction: {e}")
+
+    m.on_interaction(handle_map_interaction)
+
     def segment_button_click(change):
         if change["new"]:
             reset_button.value = False
             with output:
                 output.clear_output()
-                print("Segmenting...")
-                try:
-                    if m.user_rois is not None:
+                if len(m.fg_markers) == 0:
+                    print("Please add some foreground markers.")
+                    segment_button.value = False
+                    return
+
+                else:
+                    try:
+                        fg_points = [
+                            [marker.location[1], marker.location[0]]
+                            for marker in m.fg_markers
+                        ]
+                        bg_points = [
+                            [marker.location[1], marker.location[0]]
+                            for marker in m.bg_markers
+                        ]
+                        point_coords = fg_points + bg_points
+                        point_labels = [1] * len(fg_points) + [0] * len(bg_points)
+
                         filename = f"masks_{random_string()}.tif"
-                        sam.predict(point_coords=m.user_rois,  point_crs='EPSG:4326', output=filename)
+                        filename = os.path.join(out_dir, filename)
+                        sam.predict(
+                            point_coords=point_coords,
+                            point_labels=point_labels,
+                            point_crs="EPSG:4326",
+                            output=filename,
+                        )
                         if m.find_layer("Masks") is not None:
                             m.remove_layer(m.find_layer("Masks"))
-                        m.add_raster(filename, nodata=0, cmap='Blues', opacity=opacity_slider.value, layer_name="Masks", zoom_to_layer=False)
-                    output.clear_output()
-                    segment_button.value = False
-                    sam.prediction_fp = filename
+
+                        if hasattr(sam, "prediction_fp") and os.path.exists(
+                            sam.prediction_fp
+                        ):
+                            os.remove(sam.prediction_fp)
+
+                        # Skip the image layer if localtileserver is not available
+                        try:
+                            m.add_raster(
+                                filename,
+                                nodata=0,
+                                cmap="Blues",
+                                opacity=opacity_slider.value,
+                                layer_name="Masks",
+                                zoom_to_layer=False,
+                            )
+                        except:
+                            pass
+                        output.clear_output()
+                        segment_button.value = False
+                        sam.prediction_fp = filename
+                    except Exception as e:
+                        segment_button.value = False
+                        print(e)
+
+    segment_button.observe(segment_button_click, "value")
+
+    def filechooser_callback(chooser):
+        with output:
+            if chooser.selected is not None:
+                try:
+                    filename = chooser.selected
+                    shutil.copy(sam.prediction_fp, filename)
+                    vector = filename.replace(".tif", ".gpkg")
+                    raster_to_gpkg(filename, vector)
+
+                    fg_points = [
+                        [marker.location[1], marker.location[0]]
+                        for marker in m.fg_markers
+                    ]
+                    bg_points = [
+                        [marker.location[1], marker.location[0]]
+                        for marker in m.bg_markers
+                    ]
+
+                    coords_to_geojson(
+                        fg_points, filename.replace(".tif", "_fg_markers.geojson")
+                    )
+                    coords_to_geojson(
+                        bg_points, filename.replace(".tif", "_bg_markers.geojson")
+                    )
+
                 except Exception as e:
                     print(e)
 
-    segment_button.observe(segment_button_click, "value")
+                if hasattr(m, "save_control") and m.save_control in m.controls:
+                    m.remove_control(m.save_control)
+                    delattr(m, "save_control")
+                save_button.value = False
+
+    def save_button_click(change):
+        if change["new"]:
+            with output:
+                sandbox_path = os.environ.get("SANDBOX_PATH")
+                filechooser = FileChooser(
+                    path=os.getcwd(),
+                    filename="masks.tif",
+                    sandbox_path=sandbox_path,
+                    layout=widgets.Layout(width="454px"),
+                )
+                filechooser.use_dir_icons = True
+                filechooser.filter_pattern = ["*.tif"]
+                filechooser.register_callback(filechooser_callback)
+                save_control = ipyleaflet.WidgetControl(
+                    widget=filechooser, position="topright"
+                )
+                m.add_control(save_control)
+                m.save_control = save_control
+        else:
+            if hasattr(m, "save_control") and m.save_control in m.controls:
+                m.remove_control(m.save_control)
+                delattr(m, "save_control")
+
+    save_button.observe(save_button_click, "value")
 
     def reset_button_click(change):
         if change["new"]:
             segment_button.value = False
             reset_button.value = False
             opacity_slider.value = 0.5
             output.clear_output()
-            m.remove_layer(m.find_layer("Masks"))
-            m.clear_drawings()
-            os.remove(sam.prediction_fp)
+            try:
+                m.remove_layer(m.find_layer("Masks"))
+                m.clear_drawings()
+                if hasattr(m, "fg_markers"):
+                    m.user_rois = None
+                    m.fg_markers = []
+                    m.bg_markers = []
+                    m.fg_layer.clear_layers()
+                    m.bg_layer.clear_layers()
+                    fg_count.value = 0
+                    bg_count.value = 0
+                os.remove(sam.prediction_fp)
+            except:
+                pass
 
     reset_button.observe(reset_button_click, "value")
 
     toolbar_control = ipyleaflet.WidgetControl(
         widget=toolbar_widget, position="topright"
     )
     m.add_control(toolbar_control)
@@ -1629,8 +2063,45 @@
         str: A random string
     """
     import random
     import string
 
     # random.seed(1001)
     letters = string.ascii_lowercase
-    return "".join(random.choice(letters) for i in range(string_length))
+    return "".join(random.choice(letters) for i in range(string_length))
+
+
+def coords_to_geojson(coords, output=None):
+    """Convert a list of coordinates (lon, lat) to a GeoJSON string or file.
+
+    Args:
+        coords (list): A list of coordinates (lon, lat).
+        output (str, optional): The output file path. Defaults to None.
+
+    Returns:
+        dict: A GeoJSON dictionary.
+    """
+
+    import json
+
+    if len(coords) == 0:
+        return
+    # Create a GeoJSON FeatureCollection object
+    feature_collection = {"type": "FeatureCollection", "features": []}
+
+    # Iterate through the coordinates list and create a GeoJSON Feature object for each coordinate
+    for coord in coords:
+        feature = {
+            "type": "Feature",
+            "geometry": {"type": "Point", "coordinates": coord},
+            "properties": {},
+        }
+        feature_collection["features"].append(feature)
+
+    # Convert the FeatureCollection object to a JSON string
+    geojson_str = json.dumps(feature_collection)
+
+    if output is not None:
+        with open(output, "w") as f:
+            f.write(geojson_str)
+    else:
+        return geojson_str
```

### Comparing `segment-geospatial-0.5.0/samgeo/samgeo.py` & `segment-geospatial-0.6.0/samgeo/samgeo.py`

 * *Files 2% similar despite different names*

```diff
@@ -499,31 +499,35 @@
                     point_labels = point_labels * len(point_coords)
                 else:
                     raise ValueError(
                         "The length of point_labels must be equal to the length of point_coords."
                     )
             point_labels = np.array(point_labels)
 
+        if isinstance(box, list) and point_crs is not None:
+            box = np.array(bbox_to_xy(self.image, box, point_crs))
+
         predictor = self.predictor
         masks, scores, logits = predictor.predict(
             point_coords, point_labels, box, mask_input, multimask_output, return_logits
         )
         self.masks = masks
         self.scores = scores
         self.logits = logits
 
         if output is not None:
             self.save_prediction(output, index, mask_multiplier, dtype, **kwargs)
 
         if return_results:
             return masks, scores, logits
 
-    def show_map(self, **kwargs):
-
-        return sam_map_gui(self, **kwargs)
+    def show_map(self, basemap="SATELLITE", repeat_mode=True, out_dir=None, **kwargs):
+        return sam_map_gui(
+            self, basemap=basemap, repeat_mode=repeat_mode, out_dir=out_dir, **kwargs
+        )
 
     def image_to_image(self, image, **kwargs):
         return image_to_image(image, self, **kwargs)
 
     def download_tms_as_tiff(self, source, pt1, pt2, zoom, dist):
         image = draw_tile(source, pt1[0], pt1[1], pt2[0], pt2[1], zoom, dist)
         return image
```

### Comparing `segment-geospatial-0.5.0/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.6.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.5.0
+Version: 0.6.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -35,15 +35,18 @@
 -   Free software: MIT license
 -   Documentation: <https://samgeo.gishub.org>
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
+-   Create foreground and background markers interactively
+-   Load existing markers from vector datasets
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
+-   Save input prompts as GeoJSON files
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
 -   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
@@ -52,22 +55,35 @@
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
 
 -   Interactive segmentation with input prompts
 
-![](https://i.imgur.com/GV7Rzxt.gif)
+![](https://i.imgur.com/2Nyg9uW.gif)
+
+-   Input prompts from existing files
+
+![](https://i.imgur.com/Cb4ZaKY.gif)
 
 ## Tutorials
 
 Video tutorials are available on my [YouTube Channel](https://youtube.com/@giswqs).
 
 [![Alt text](https://img.youtube.com/vi/YHA_-QMB8_U/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
 
+## Using SAM with Desktop GIS
+
+-   **QGIS**: Check out the [Geometric Attributes plugin for QGIS](https://github.com/BjornNyberg/Geometric-Attributes-Toolbox/wiki/User-Guide#segment-anything-model). Credit goes to [Bjorn Nyberg](https://github.com/BjornNyberg).
+-   **ArcGIS**: Check out the [Segment Anything Model (SAM) Toolbox for ArcGIS](https://www.arcgis.com/home/item.html?id=9b67b441f29f4ce6810979f5f0667ebe). Credit goes to [Esri](https://www.esri.com).
+
+## Computing Resources
+
+The Segment Anything Model is computationally intensive, and a powerful GPU is recommended to process large datasets. It is recommended to have a GPU with at least 8 GB of GPU memory. You can utilize the free GPU resources provided by Google Colab. Alternatively, you can apply for [AWS Cloud Credit for Research](https://aws.amazon.com/government-education/research-and-technical-computing/cloud-credit-for-research), which offers cloud credits to support academic research. If you are in the Greater China region, apply for the AWS Cloud Credit [here](https://aws.amazon.com/cn/events/educate_cloud/research-credits).
+
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
```

### Comparing `segment-geospatial-0.5.0/setup.py` & `segment-geospatial-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords="samgeo",
     name="segment-geospatial",
     packages=find_packages(include=["samgeo", "samgeo.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/opengeos/segment-geospatial",
-    version='0.5.0',
+    version='0.6.0',
     zip_safe=False,
 )
```

