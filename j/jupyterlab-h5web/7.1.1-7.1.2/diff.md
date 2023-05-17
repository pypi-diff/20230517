# Comparing `tmp/jupyterlab_h5web-7.1.1.tar.gz` & `tmp/jupyterlab_h5web-7.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/jupyterlab-h5web/jupyterlab-h5web/dist/.tmp-85lrh3j6/jupyterlab_h5web-7.1.1.tar", last modified: Thu Apr 20 12:16:39 2023, max compression
+gzip compressed data, was "/home/runner/work/jupyterlab-h5web/jupyterlab-h5web/dist/.tmp-gsxpl0_y/jupyterlab_h5web-7.1.2.tar", last modified: Wed May 17 12:17:14 2023, max compression
```

## Comparing `jupyterlab_h5web-7.1.1.tar` & `jupyterlab_h5web-7.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyter-config/nb-config/jupyterlab_h5web.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyter-config/server-config/jupyterlab_h5web.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)  1208336 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/317.7320f9f9a065f27d09c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    39615 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/549.8a4bd7ffba6e2772bada.js
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/remoteEntry.ec65a8378b6cbb458b20.js
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 12:13:07.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    80860 2023-04-20 12:13:30.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:12:54.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/H5webApp.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/browser.ts
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/fileType.ts
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/icons.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/mimeplugin.tsx
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/svg.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/src/widget.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:16:39.000000 jupyterlab_h5web-7.1.1/style/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/style/h5web-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/style/hdf5-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-20 12:11:25.000000 jupyterlab_h5web-7.1.1/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)   296546 2023-04-20 12:12:21.000000 jupyterlab_h5web-7.1.1/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/jupyter-config/nb-config/jupyterlab_h5web.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/jupyter-config/server-config/jupyterlab_h5web.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-17 12:14:27.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  1208336 2023-05-17 12:14:27.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-17 12:14:27.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-05-17 12:14:27.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/317.7320f9f9a065f27d09c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39615 2023-05-17 12:14:27.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/549.8a4bd7ffba6e2772bada.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-05-17 12:14:27.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/remoteEntry.c9dd363b0bcc04cc1365.js
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 12:14:08.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80860 2023-05-17 12:14:27.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:13:56.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/jupyterlab_h5web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/src/H5webApp.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/src/browser.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/src/fileType.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/src/icons.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/src/mimeplugin.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/src/svg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/src/widget.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:17:14.000000 jupyterlab_h5web-7.1.2/style/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/style/h5web-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/style/hdf5-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-17 12:12:29.000000 jupyterlab_h5web-7.1.2/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)   296546 2023-05-17 12:13:27.000000 jupyterlab_h5web-7.1.2/yarn.lock
```

### Comparing `jupyterlab_h5web-7.1.1/LICENSE.md` & `jupyterlab_h5web-7.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/MANIFEST.in` & `jupyterlab_h5web-7.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/PKG-INFO` & `jupyterlab_h5web-7.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_h5web
-Version: 7.1.1
+Version: 7.1.2
 Summary: A JupyterLab extension to explore and visualize HDF5 file contents.
 Home-page: https://github.com/silx-kit/jupyterlab-h5web
 Author: European Synchrotron Radiation Facility
 Author-email: h5web@esrf.fr
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_h5web-7.1.1/README.md` & `jupyterlab_h5web-7.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/jupyterlab_h5web/__init__.py` & `jupyterlab_h5web-7.1.2/jupyterlab_h5web/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/jupyterlab_h5web/_version.py` & `jupyterlab_h5web-7.1.2/jupyterlab_h5web/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/jupyterlab_h5web/handlers.py` & `jupyterlab_h5web-7.1.2/jupyterlab_h5web/handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,32 @@
+import h5py
 from tornado.web import authenticated, MissingArgumentError
 from jupyter_server.base.handlers import APIHandler
 from jupyter_server.utils import url_path_join
 from pathlib import Path
 
 from h5grove.encoders import encode
 from h5grove.content import (
     get_content_from_file,
     get_list_of_paths,
     EntityContent,
     ResolvedEntityContent,
     DatasetContent,
 )
+from h5grove.utils import parse_bool_arg
 
 from .utils import as_absolute_path, create_error
 
 
+H5PY_HAS_FILE_LOCKING_ARG = h5py.version.hdf5_version_tuple >= (1, 12, 1) or (
+    h5py.version.hdf5_version_tuple[:2] == (1, 10)
+    and h5py.version.hdf5_version_tuple[2] >= 7
+)
+
+
 class BaseHandler(APIHandler):
     def initialize(self, base_dir: Path) -> None:
         self.base_dir = base_dir
 
 
 class ContentHandler(BaseHandler):
     @authenticated
@@ -29,15 +37,15 @@
         path = self.get_query_argument("path", None)
         format_arg = self.get_query_argument("format", None)
 
         with get_content_from_file(
             as_absolute_path(self.base_dir, Path(file_path)),
             path,
             create_error,
-            h5py_options={"locking": False},
+            h5py_options={"locking": False} if H5PY_HAS_FILE_LOCKING_ARG else {},
         ) as content:
             payload = self.parse_content(content)
 
         response = encode(payload, format_arg)
 
         for key, value in response.headers.items():
             self.set_header(key, value)
@@ -59,17 +67,20 @@
         return content.attributes()
 
 
 class DataHandler(ContentHandler):
     def parse_content(self, content):
         selection = self.get_query_argument("selection", None)
         dtype = self.get_query_argument("dtype", None)
+        flatten = parse_bool_arg(
+            self.get_query_argument("flatten", None), fallback=False
+        )
 
         assert isinstance(content, DatasetContent)
-        return content.data(selection, dtype=dtype)
+        return content.data(selection, flatten, dtype)
 
 
 class MetadataHandler(ContentHandler):
     def parse_content(self, content):
         return content.metadata()
```

### Comparing `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/package.json` & `jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9731359649122806%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.c9dd363b0bcc04cc1365.js'}}",*

 * * "'version'": "'7.1.2'"}*

```diff
@@ -45,15 +45,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/silx-kit/jupyterlab-h5web",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ec65a8378b6cbb458b20.js",
+            "load": "static/remoteEntry.c9dd363b0bcc04cc1365.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_h5web"
                 },
@@ -99,9 +99,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "7.1.1"
+    "version": "7.1.2"
 }
```

### Comparing `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js` & `jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js.LICENSE.txt` & `jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/317.7320f9f9a065f27d09c7.js` & `jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/317.7320f9f9a065f27d09c7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/549.8a4bd7ffba6e2772bada.js` & `jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/549.8a4bd7ffba6e2772bada.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/remoteEntry.ec65a8378b6cbb458b20.js` & `jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/remoteEntry.c9dd363b0bcc04cc1365.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -112,15 +112,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@h5web/app", "7.1.0", (() => Promise.all([E.e(295), E.e(832)]).then((() => () => E(6295))))), l("jupyterlab-h5web", "7.1.1", (() => Promise.all([E.e(832), E.e(317)]).then((() => () => E(317)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@h5web/app", "7.1.0", (() => Promise.all([E.e(295), E.e(832)]).then((() => () => E(6295))))), l("jupyterlab-h5web", "7.1.2", (() => Promise.all([E.e(832), E.e(317)]).then((() => () => E(317)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_h5web-7.1.1/jupyterlab_h5web/labextension/static/third-party-licenses.json` & `jupyterlab_h5web-7.1.2/jupyterlab_h5web/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/jupyterlab_h5web/widget.py` & `jupyterlab_h5web-7.1.2/jupyterlab_h5web/widget.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/PKG-INFO` & `jupyterlab_h5web-7.1.2/jupyterlab_h5web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-h5web
-Version: 7.1.1
+Version: 7.1.2
 Summary: A JupyterLab extension to explore and visualize HDF5 file contents.
 Home-page: https://github.com/silx-kit/jupyterlab-h5web
 Author: European Synchrotron Radiation Facility
 Author-email: h5web@esrf.fr
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_h5web-7.1.1/jupyterlab_h5web.egg-info/SOURCES.txt` & `jupyterlab_h5web-7.1.2/jupyterlab_h5web.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 jupyterlab_h5web.egg-info/requires.txt
 jupyterlab_h5web.egg-info/top_level.txt
 jupyterlab_h5web/labextension/package.json
 jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js
 jupyterlab_h5web/labextension/static/295.1c78f11e9ce3f6be3d93.js.LICENSE.txt
 jupyterlab_h5web/labextension/static/317.7320f9f9a065f27d09c7.js
 jupyterlab_h5web/labextension/static/549.8a4bd7ffba6e2772bada.js
-jupyterlab_h5web/labextension/static/remoteEntry.ec65a8378b6cbb458b20.js
+jupyterlab_h5web/labextension/static/remoteEntry.c9dd363b0bcc04cc1365.js
 jupyterlab_h5web/labextension/static/style.js
 jupyterlab_h5web/labextension/static/third-party-licenses.json
 src/H5webApp.tsx
 src/browser.ts
 src/fileType.ts
 src/icons.ts
 src/index.ts
```

### Comparing `jupyterlab_h5web-7.1.1/package.json` & `jupyterlab_h5web-7.1.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'version'": "'7.1.2'"}*

```diff
@@ -94,9 +94,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "7.1.1"
+    "version": "7.1.2"
 }
```

### Comparing `jupyterlab_h5web-7.1.1/pyproject.toml` & `jupyterlab_h5web-7.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/setup.py` & `jupyterlab_h5web-7.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/src/H5webApp.tsx` & `jupyterlab_h5web-7.1.2/src/H5webApp.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/src/browser.ts` & `jupyterlab_h5web-7.1.2/src/browser.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/src/fileType.ts` & `jupyterlab_h5web-7.1.2/src/fileType.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/src/index.ts` & `jupyterlab_h5web-7.1.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/src/mimeplugin.tsx` & `jupyterlab_h5web-7.1.2/src/mimeplugin.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/src/widget.tsx` & `jupyterlab_h5web-7.1.2/src/widget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/style/h5web-icon.svg` & `jupyterlab_h5web-7.1.2/style/h5web-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/style/hdf5-icon.svg` & `jupyterlab_h5web-7.1.2/style/hdf5-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/style/index.css` & `jupyterlab_h5web-7.1.2/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/tsconfig.json` & `jupyterlab_h5web-7.1.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_h5web-7.1.1/yarn.lock` & `jupyterlab_h5web-7.1.2/yarn.lock`

 * *Files identical despite different names*

