# Comparing `tmp/cochleogram-0.2.4.tar.gz` & `tmp/cochleogram-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochleogram-0.2.4.tar", last modified: Tue May  9 20:47:45 2023, max compression
+gzip compressed data, was "cochleogram-0.2.5.tar", last modified: Wed May 17 00:08:06 2023, max compression
```

## Comparing `cochleogram-0.2.4.tar` & `cochleogram-0.2.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:45.228226 cochleogram-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:45.224225 cochleogram-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:45.224225 cochleogram-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-09 20:47:35.000000 cochleogram-0.2.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-09 20:47:35.000000 cochleogram-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-09 20:47:45.228226 cochleogram-0.2.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:45.224225 cochleogram-0.2.4/cochleogram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/gui.enaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:45.228226 cochleogram-0.2.4/cochleogram/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/cells.png
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/exclude.png
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/main-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/make_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/spiral.png
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/icons/tile.png
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    26608 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/presenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-05-09 20:47:35.000000 cochleogram-0.2.4/cochleogram/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:47:45.228226 cochleogram-0.2.4/cochleogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 20:47:45.000000 cochleogram-0.2.4/cochleogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-09 20:47:35.000000 cochleogram-0.2.4/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-09 20:47:35.000000 cochleogram-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-09 20:47:35.000000 cochleogram-0.2.4/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 20:47:45.228226 cochleogram-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:08:06.342863 cochleogram-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:08:06.338863 cochleogram-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:08:06.338863 cochleogram-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-17 00:07:56.000000 cochleogram-0.2.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-17 00:07:56.000000 cochleogram-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-17 00:08:06.342863 cochleogram-0.2.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:08:06.338863 cochleogram-0.2.5/cochleogram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/gui.enaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:08:06.342863 cochleogram-0.2.5/cochleogram/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/cells.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/exclude.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/main-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/make_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/spiral.png
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/icons/tile.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21136 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26608 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-05-17 00:07:56.000000 cochleogram-0.2.5/cochleogram/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:08:06.338863 cochleogram-0.2.5/cochleogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 00:08:06.000000 cochleogram-0.2.5/cochleogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-17 00:07:56.000000 cochleogram-0.2.5/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-17 00:07:56.000000 cochleogram-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-17 00:07:56.000000 cochleogram-0.2.5/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 00:08:06.342863 cochleogram-0.2.5/setup.cfg
```

### Comparing `cochleogram-0.2.4/.github/workflows/publish-to-pypi.yml` & `cochleogram-0.2.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/.gitignore` & `cochleogram-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/PKG-INFO` & `cochleogram-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.2.4
+Version: 0.2.5
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.2.4/cochleogram/gui.enaml` & `cochleogram-0.2.5/cochleogram/gui.enaml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/cochleogram/icons/cells.png` & `cochleogram-0.2.5/cochleogram/icons/cells.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/cochleogram/icons/exclude.png` & `cochleogram-0.2.5/cochleogram/icons/exclude.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/cochleogram/icons/main-icon.png` & `cochleogram-0.2.5/cochleogram/icons/main-icon.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/cochleogram/icons/make_icons.py` & `cochleogram-0.2.5/cochleogram/icons/make_icons.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/cochleogram/icons/spiral.png` & `cochleogram-0.2.5/cochleogram/icons/spiral.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/cochleogram/icons/tile.png` & `cochleogram-0.2.5/cochleogram/icons/tile.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/cochleogram/instructions.html` & `cochleogram-0.2.5/cochleogram/instructions.html`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/cochleogram/main.py` & `cochleogram-0.2.5/cochleogram/main.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/cochleogram/model.py` & `cochleogram-0.2.5/cochleogram/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,15 +514,15 @@
         tile = self.merge_tiles()
         x, y = self.spirals[cell_type].interpolate(resolution=0.0001)
         i = tile.map(x, y, channel, width=width)
         xn, yn = util.find_nuclei(x, y, i, spacing=spacing)
 
         # Map to centroid
         xni, yni = tile.to_indices(xn, yn)
-        image = tile.get_image(channel=channel).max(axis=-1)
+        image = tile.get_image(channel).max(axis=-1)
         x_radius = tile.to_indices_delta(width, 'x')
         y_radius = tile.to_indices_delta(width, 'y')
         log.info('Searching for centroid within %ix%i pixels of spiral', x_radius,
                  y_radius)
         xnic, ynic = util.find_centroid(xni, yni, image, x_radius, y_radius, 4)
         xnc, ync = tile.to_coords(xnic, ynic)
         log.info('Shifted points up to %.0f x %.0f microns',
```

### Comparing `cochleogram-0.2.4/cochleogram/plot.py` & `cochleogram-0.2.5/cochleogram/plot.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/cochleogram/presenter.py` & `cochleogram-0.2.5/cochleogram/presenter.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/cochleogram/readers.py` & `cochleogram-0.2.5/cochleogram/readers.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/cochleogram/util.py` & `cochleogram-0.2.5/cochleogram/util.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/cochleogram.egg-info/PKG-INFO` & `cochleogram-0.2.5/cochleogram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.2.4
+Version: 0.2.5
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.2.4/cochleogram.egg-info/SOURCES.txt` & `cochleogram-0.2.5/cochleogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/pyproject.toml` & `cochleogram-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.4/readme.rst` & `cochleogram-0.2.5/readme.rst`

 * *Files identical despite different names*

