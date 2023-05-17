# Comparing `tmp/jupyterlab_nbgallery-2.0.2.tar.gz` & `tmp/jupyterlab_nbgallery-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_nbgallery-2.0.2.tar", last modified: Tue May 16 11:51:17 2023, max compression
+gzip compressed data, was "jupyterlab_nbgallery-2.0.3.tar", last modified: Wed May 17 13:12:31 2023, max compression
```

## Comparing `jupyterlab_nbgallery-2.0.2.tar` & `jupyterlab_nbgallery-2.0.3.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.123679 jupyterlab_nbgallery-2.0.2/
--rw-r--r--   0 jovyan    (1000) users      (100)     1066 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/LICENSE
--rw-r--r--   0 jovyan    (1000) users      (100)      388 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/MANIFEST.in
--rw-r--r--   0 jovyan    (1000) users      (100)     2692 2023-05-16 11:51:17.123679 jupyterlab_nbgallery-2.0.2/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     2014 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/README.md
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.107679 jupyterlab_nbgallery-2.0.2/jupyter-config/
--rw-r--r--   0 jovyan    (1000) users      (100)       96 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/jupyter-config/jupyterlab_nbgallery.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.107679 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery/
--rw-r--r--   0 jovyan    (1000) users      (100)      596 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)       72 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery/_version.py
--rw-r--r--   0 jovyan    (1000) users      (100)     3640 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery/handlers.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.107679 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)     2692 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     4443 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/not-zip-safe
--rw-r--r--   0 jovyan    (1000) users      (100)       61 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       21 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/top_level.txt
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.107679 jupyterlab_nbgallery-2.0.2/labextension/autodownload/
--rw-r--r--   0 jovyan    (1000) users      (100)     2503 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/autodownload/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/autodownload/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.107679 jupyterlab_nbgallery-2.0.2/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/
--rw-r--r--   0 jovyan    (1000) users      (100)      335 2023-05-16 11:50:36.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/autodownload.json
--rw-r--r--   0 jovyan    (1000) users      (100)     2361 2023-05-16 11:50:36.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.111679 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/
--rw-r--r--   0 jovyan    (1000) users      (100)     3438 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/542.51fb91347d8a3d9a657a.js
--rw-r--r--   0 jovyan    (1000) users      (100)     2142 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/568.8bc32e058afbf3d8a017.js
--rw-r--r--   0 jovyan    (1000) users      (100)    90038 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js
--rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js.LICENSE.txt
--rw-r--r--   0 jovyan    (1000) users      (100)     6914 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/remoteEntry.77e4acbd8dd372ff3fad.js
--rw-r--r--   0 jovyan    (1000) users      (100)      178 2023-05-16 11:50:36.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)     3692 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/third-party-licenses.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.111679 jupyterlab_nbgallery-2.0.2/labextension/environment-life/
--rw-r--r--   0 jovyan    (1000) users      (100)     2644 2023-05-16 11:50:37.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/environment-life/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/environment-life/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.111679 jupyterlab_nbgallery-2.0.2/labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/
--rw-r--r--   0 jovyan    (1000) users      (100)     2502 2023-05-16 11:50:34.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.111679 jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/
--rw-r--r--   0 jovyan    (1000) users      (100)     1162 2023-05-16 11:50:37.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/248.19732aba6894a502e197.js
--rw-r--r--   0 jovyan    (1000) users      (100)     3446 2023-05-16 11:50:37.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/542.e4d405f3b0e4f693ab53.js
--rw-r--r--   0 jovyan    (1000) users      (100)     6651 2023-05-16 11:50:37.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/remoteEntry.fe9e40141faed985c15b.js
--rw-r--r--   0 jovyan    (1000) users      (100)      182 2023-05-16 11:50:34.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)     2452 2023-05-16 11:50:37.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/third-party-licenses.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.111679 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/
--rw-r--r--   0 jovyan    (1000) users      (100)     2525 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.111679 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/
--rw-r--r--   0 jovyan    (1000) users      (100)      680 2023-05-16 11:50:35.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/environment-registration.json
--rw-r--r--   0 jovyan    (1000) users      (100)     2383 2023-05-16 11:50:35.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/
--rw-r--r--   0 jovyan    (1000) users      (100)     3460 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/542.feae6c397f33f9138fea.js
--rw-r--r--   0 jovyan    (1000) users      (100)    90062 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/638.36e464d3233849b6b07a.js
--rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/638.36e464d3233849b6b07a.js.LICENSE.txt
--rw-r--r--   0 jovyan    (1000) users      (100)     1648 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/784.201d6fbbedd26339ab72.js
--rw-r--r--   0 jovyan    (1000) users      (100)     7044 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/remoteEntry.54aae520a7b7fc99d9fd.js
--rw-r--r--   0 jovyan    (1000) users      (100)      190 2023-05-16 11:50:35.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)     3692 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/third-party-licenses.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/
--rw-r--r--   0 jovyan    (1000) users      (100)     2481 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/
--rw-r--r--   0 jovyan    (1000) users      (100)     2365 2023-05-16 11:50:36.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/
--rw-r--r--   0 jovyan    (1000) users      (100)    11664 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/56.2f2a1bce28a94a6668e1.js
--rw-r--r--   0 jovyan    (1000) users      (100)    90036 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/638.95e0186307171588df5b.js
--rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/638.95e0186307171588df5b.js.LICENSE.txt
--rw-r--r--   0 jovyan    (1000) users      (100)     7108 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/remoteEntry.fadc9f3eb62fb570716e.js
--rw-r--r--   0 jovyan    (1000) users      (100)      118 2023-05-16 11:50:36.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)     1262 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/third-party-licenses.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/
--rw-r--r--   0 jovyan    (1000) users      (100)     2418 2023-05-16 11:51:08.000000 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/
--rw-r--r--   0 jovyan    (1000) users      (100)     2302 2023-05-16 11:51:06.000000 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/static/
--rw-r--r--   0 jovyan    (1000) users      (100)     1259 2023-05-16 11:51:08.000000 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/static/568.bde16f9395a112a349ee.js
--rw-r--r--   0 jovyan    (1000) users      (100)     6305 2023-05-16 11:51:08.000000 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/static/remoteEntry.f32354aac49e7b8ba738.js
--rw-r--r--   0 jovyan    (1000) users      (100)      118 2023-05-16 11:51:06.000000 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)       20 2023-05-16 11:51:08.000000 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/static/third-party-licenses.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/
--rw-r--r--   0 jovyan    (1000) users      (100)     2434 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.119679 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/
--rw-r--r--   0 jovyan    (1000) users      (100)      345 2023-05-16 11:51:10.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/instrumentation.json
--rw-r--r--   0 jovyan    (1000) users      (100)     2318 2023-05-16 11:51:10.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.119679 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/
--rw-r--r--   0 jovyan    (1000) users      (100)     1929 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/568.274dc29b6aea1cf48d74.js
--rw-r--r--   0 jovyan    (1000) users      (100)    90044 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/638.b95125ed695cee42aae4.js
--rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/638.b95125ed695cee42aae4.js.LICENSE.txt
--rw-r--r--   0 jovyan    (1000) users      (100)     8425 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/701.d81800f5926ab62cc8b2.js
--rw-r--r--   0 jovyan    (1000) users      (100)     7555 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/remoteEntry.52d0d8f58cd3e55540ee.js
--rw-r--r--   0 jovyan    (1000) users      (100)      118 2023-05-16 11:51:10.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)     2479 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/third-party-licenses.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.119679 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/
--rw-r--r--   0 jovyan    (1000) users      (100)     2590 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.119679 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/
--rw-r--r--   0 jovyan    (1000) users      (100)     2448 2023-05-16 11:51:11.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.123679 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/
--rw-r--r--   0 jovyan    (1000) users      (100)     4026 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/542.d1718a50e23f3808ba62.js
--rw-r--r--   0 jovyan    (1000) users      (100)     4448 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/568.eab1414ad9e7f57f8e93.js
--rw-r--r--   0 jovyan    (1000) users      (100)    90044 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/638.e5080f99954048969f76.js
--rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/638.e5080f99954048969f76.js.LICENSE.txt
--rw-r--r--   0 jovyan    (1000) users      (100)     7158 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/remoteEntry.0c562dfea5f20371ffe8.js
--rw-r--r--   0 jovyan    (1000) users      (100)      181 2023-05-16 11:51:11.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)     3692 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/third-party-licenses.json
--rw-r--r--   0 jovyan    (1000) users      (100)     1135 2023-05-16 11:49:22.000000 jupyterlab_nbgallery-2.0.2/package.json
--rw-r--r--   0 jovyan    (1000) users      (100)      146 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/pyproject.toml
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-05-16 11:51:17.123679 jupyterlab_nbgallery-2.0.2/setup.cfg
--rw-r--r--   0 jovyan    (1000) users      (100)     3928 2023-05-16 11:49:22.000000 jupyterlab_nbgallery-2.0.2/setup.py
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.121980 jupyterlab_nbgallery-2.0.3/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1066 2023-05-17 13:08:48.000000 jupyterlab_nbgallery-2.0.3/LICENSE
+-rw-r--r--   0 jovyan    (1000) users      (100)      388 2023-05-17 13:08:48.000000 jupyterlab_nbgallery-2.0.3/MANIFEST.in
+-rw-r--r--   0 jovyan    (1000) users      (100)     2692 2023-05-17 13:12:31.121980 jupyterlab_nbgallery-2.0.3/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)     2014 2023-05-17 13:08:48.000000 jupyterlab_nbgallery-2.0.3/README.md
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.101980 jupyterlab_nbgallery-2.0.3/jupyter-config/
+-rw-r--r--   0 jovyan    (1000) users      (100)       96 2023-05-17 13:08:48.000000 jupyterlab_nbgallery-2.0.3/jupyter-config/jupyterlab_nbgallery.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.105980 jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery/
+-rw-r--r--   0 jovyan    (1000) users      (100)      596 2023-05-17 13:08:48.000000 jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)       72 2023-05-17 13:08:48.000000 jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery/_version.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     3640 2023-05-17 13:08:48.000000 jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery/handlers.py
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.105980 jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2692 2023-05-17 13:12:30.000000 jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)     4443 2023-05-17 13:12:30.000000 jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-05-17 13:12:30.000000 jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-05-17 13:12:30.000000 jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery.egg-info/not-zip-safe
+-rw-r--r--   0 jovyan    (1000) users      (100)       61 2023-05-17 13:12:30.000000 jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       21 2023-05-17 13:12:30.000000 jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery.egg-info/top_level.txt
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.101980 jupyterlab_nbgallery-2.0.3/labextension/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.105980 jupyterlab_nbgallery-2.0.3/labextension/autodownload/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2503 2023-05-17 13:11:50.000000 jupyterlab_nbgallery-2.0.3/labextension/autodownload/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.097980 jupyterlab_nbgallery-2.0.3/labextension/autodownload/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.097980 jupyterlab_nbgallery-2.0.3/labextension/autodownload/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.105980 jupyterlab_nbgallery-2.0.3/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/
+-rw-r--r--   0 jovyan    (1000) users      (100)      335 2023-05-17 13:11:41.000000 jupyterlab_nbgallery-2.0.3/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/autodownload.json
+-rw-r--r--   0 jovyan    (1000) users      (100)     2361 2023-05-17 13:11:41.000000 jupyterlab_nbgallery-2.0.3/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.105980 jupyterlab_nbgallery-2.0.3/labextension/autodownload/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)     3438 2023-05-17 13:11:50.000000 jupyterlab_nbgallery-2.0.3/labextension/autodownload/static/542.51fb91347d8a3d9a657a.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     2119 2023-05-17 13:11:50.000000 jupyterlab_nbgallery-2.0.3/labextension/autodownload/static/568.6448f5c1d260e1510f0b.js
+-rw-r--r--   0 jovyan    (1000) users      (100)    90038 2023-05-17 13:11:50.000000 jupyterlab_nbgallery-2.0.3/labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-17 13:11:50.000000 jupyterlab_nbgallery-2.0.3/labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js.LICENSE.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)     6916 2023-05-17 13:11:50.000000 jupyterlab_nbgallery-2.0.3/labextension/autodownload/static/remoteEntry.f0097f506f67321081da.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      178 2023-05-17 13:11:41.000000 jupyterlab_nbgallery-2.0.3/labextension/autodownload/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     3692 2023-05-17 13:11:50.000000 jupyterlab_nbgallery-2.0.3/labextension/autodownload/static/third-party-licenses.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.105980 jupyterlab_nbgallery-2.0.3/labextension/environment-life/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2644 2023-05-17 13:11:41.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-life/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.097980 jupyterlab_nbgallery-2.0.3/labextension/environment-life/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.097980 jupyterlab_nbgallery-2.0.3/labextension/environment-life/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.109980 jupyterlab_nbgallery-2.0.3/labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2502 2023-05-17 13:11:38.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.109980 jupyterlab_nbgallery-2.0.3/labextension/environment-life/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1161 2023-05-17 13:11:41.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-life/static/248.ff22e12bacd29ee749b6.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     3446 2023-05-17 13:11:41.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-life/static/542.e4d405f3b0e4f693ab53.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     6648 2023-05-17 13:11:41.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-life/static/remoteEntry.3b2f785c13bf442d8fd1.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      182 2023-05-17 13:11:38.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-life/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     2452 2023-05-17 13:11:41.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-life/static/third-party-licenses.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.109980 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2525 2023-05-17 13:11:49.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.097980 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.097980 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.109980 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/
+-rw-r--r--   0 jovyan    (1000) users      (100)      659 2023-05-17 13:11:40.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/environment-registration.json
+-rw-r--r--   0 jovyan    (1000) users      (100)     2383 2023-05-17 13:11:40.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.109980 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)     3460 2023-05-17 13:11:49.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/static/542.feae6c397f33f9138fea.js
+-rw-r--r--   0 jovyan    (1000) users      (100)    90062 2023-05-17 13:11:49.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/static/638.36e464d3233849b6b07a.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-17 13:11:49.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/static/638.36e464d3233849b6b07a.js.LICENSE.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)     1648 2023-05-17 13:11:49.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/static/784.05dd45a572b8a68b8ef0.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     7044 2023-05-17 13:11:49.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/static/remoteEntry.fad449cea8e4f679087a.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      190 2023-05-17 13:11:40.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     3692 2023-05-17 13:11:49.000000 jupyterlab_nbgallery-2.0.3/labextension/environment-registration/static/third-party-licenses.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.113980 jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2481 2023-05-17 13:11:51.000000 jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.097980 jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.097980 jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.113980 jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2365 2023-05-17 13:11:41.000000 jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.113980 jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)    11664 2023-05-17 13:11:51.000000 jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/static/56.2726b62668fa9972cd30.js
+-rw-r--r--   0 jovyan    (1000) users      (100)    90036 2023-05-17 13:11:51.000000 jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/static/638.95e0186307171588df5b.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-17 13:11:51.000000 jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/static/638.95e0186307171588df5b.js.LICENSE.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)     7107 2023-05-17 13:11:51.000000 jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/static/remoteEntry.59749b88a6eed42d676f.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      118 2023-05-17 13:11:41.000000 jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     1262 2023-05-17 13:11:51.000000 jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/static/third-party-licenses.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.113980 jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2418 2023-05-17 13:12:16.000000 jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.097980 jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.097980 jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.113980 jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2302 2023-05-17 13:12:14.000000 jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.113980 jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1259 2023-05-17 13:12:16.000000 jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/static/568.1c56cc1b2764b66bca50.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     6305 2023-05-17 13:12:16.000000 jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/static/remoteEntry.961a61df8bda40e885ae.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      118 2023-05-17 13:12:14.000000 jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)       20 2023-05-17 13:12:16.000000 jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/static/third-party-licenses.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.113980 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2434 2023-05-17 13:12:29.000000 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.101980 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.101980 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.117980 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/
+-rw-r--r--   0 jovyan    (1000) users      (100)      345 2023-05-17 13:12:23.000000 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/instrumentation.json
+-rw-r--r--   0 jovyan    (1000) users      (100)     2318 2023-05-17 13:12:23.000000 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.117980 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1930 2023-05-17 13:12:29.000000 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/static/568.b9882f522566d7c3f80b.js
+-rw-r--r--   0 jovyan    (1000) users      (100)    90044 2023-05-17 13:12:29.000000 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/static/638.b95125ed695cee42aae4.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-17 13:12:29.000000 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/static/638.b95125ed695cee42aae4.js.LICENSE.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)     8425 2023-05-17 13:12:29.000000 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/static/701.d81800f5926ab62cc8b2.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     7557 2023-05-17 13:12:29.000000 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/static/remoteEntry.e2d86efe89b107788c6a.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      118 2023-05-17 13:12:23.000000 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     2479 2023-05-17 13:12:29.000000 jupyterlab_nbgallery-2.0.3/labextension/instrumentation/static/third-party-licenses.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.117980 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2590 2023-05-17 13:12:30.000000 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.101980 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.101980 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.117980 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2448 2023-05-17 13:12:25.000000 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-17 13:12:31.121980 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)     4026 2023-05-17 13:12:30.000000 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/static/542.d1718a50e23f3808ba62.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     4449 2023-05-17 13:12:30.000000 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/static/568.d278e7473ae759d43e90.js
+-rw-r--r--   0 jovyan    (1000) users      (100)    90044 2023-05-17 13:12:30.000000 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/static/638.e5080f99954048969f76.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-17 13:12:30.000000 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/static/638.e5080f99954048969f76.js.LICENSE.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)     7159 2023-05-17 13:12:30.000000 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/static/remoteEntry.ebf7fd35624f8fdb1636.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      181 2023-05-17 13:12:25.000000 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     3692 2023-05-17 13:12:30.000000 jupyterlab_nbgallery-2.0.3/labextension/userpreferences/static/third-party-licenses.json
+-rw-r--r--   0 jovyan    (1000) users      (100)     1135 2023-05-17 13:08:48.000000 jupyterlab_nbgallery-2.0.3/package.json
+-rw-r--r--   0 jovyan    (1000) users      (100)      146 2023-05-17 13:08:48.000000 jupyterlab_nbgallery-2.0.3/pyproject.toml
+-rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-05-17 13:12:31.121980 jupyterlab_nbgallery-2.0.3/setup.cfg
+-rw-r--r--   0 jovyan    (1000) users      (100)     3928 2023-05-17 13:08:48.000000 jupyterlab_nbgallery-2.0.3/setup.py
```

### Comparing `jupyterlab_nbgallery-2.0.2/LICENSE` & `jupyterlab_nbgallery-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/PKG-INFO` & `jupyterlab_nbgallery-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nbgallery
-Version: 2.0.2
+Version: 2.0.3
 Summary: A JupyterLab Extension for NBGallery integration
 Home-page: https://github.com/nbgallery/lab-extensions
 Author: NBGallery
 License: MIT
 Keywords: Jupyter,JupyterLab
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jupyterlab_nbgallery-2.0.2/README.md` & `jupyterlab_nbgallery-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery/__init__.py` & `jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery/handlers.py` & `jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/PKG-INFO` & `jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-nbgallery
-Version: 2.0.2
+Version: 2.0.3
 Summary: A JupyterLab Extension for NBGallery integration
 Home-page: https://github.com/nbgallery/lab-extensions
 Author: NBGallery
 License: MIT
 Keywords: Jupyter,JupyterLab
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/SOURCES.txt` & `jupyterlab_nbgallery-2.0.3/jupyterlab_nbgallery.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,63 +14,63 @@
 jupyterlab_nbgallery.egg-info/not-zip-safe
 jupyterlab_nbgallery.egg-info/requires.txt
 jupyterlab_nbgallery.egg-info/top_level.txt
 labextension/autodownload/package.json
 labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/autodownload.json
 labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/package.json.orig
 labextension/autodownload/static/542.51fb91347d8a3d9a657a.js
-labextension/autodownload/static/568.8bc32e058afbf3d8a017.js
+labextension/autodownload/static/568.6448f5c1d260e1510f0b.js
 labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js
 labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js.LICENSE.txt
-labextension/autodownload/static/remoteEntry.77e4acbd8dd372ff3fad.js
+labextension/autodownload/static/remoteEntry.f0097f506f67321081da.js
 labextension/autodownload/static/style.js
 labextension/autodownload/static/third-party-licenses.json
 labextension/environment-life/package.json
 labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/package.json.orig
-labextension/environment-life/static/248.19732aba6894a502e197.js
+labextension/environment-life/static/248.ff22e12bacd29ee749b6.js
 labextension/environment-life/static/542.e4d405f3b0e4f693ab53.js
-labextension/environment-life/static/remoteEntry.fe9e40141faed985c15b.js
+labextension/environment-life/static/remoteEntry.3b2f785c13bf442d8fd1.js
 labextension/environment-life/static/style.js
 labextension/environment-life/static/third-party-licenses.json
 labextension/environment-registration/package.json
 labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/environment-registration.json
 labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/package.json.orig
 labextension/environment-registration/static/542.feae6c397f33f9138fea.js
 labextension/environment-registration/static/638.36e464d3233849b6b07a.js
 labextension/environment-registration/static/638.36e464d3233849b6b07a.js.LICENSE.txt
-labextension/environment-registration/static/784.201d6fbbedd26339ab72.js
-labextension/environment-registration/static/remoteEntry.54aae520a7b7fc99d9fd.js
+labextension/environment-registration/static/784.05dd45a572b8a68b8ef0.js
+labextension/environment-registration/static/remoteEntry.fad449cea8e4f679087a.js
 labextension/environment-registration/static/style.js
 labextension/environment-registration/static/third-party-licenses.json
 labextension/gallerymenu/package.json
 labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/package.json.orig
-labextension/gallerymenu/static/56.2f2a1bce28a94a6668e1.js
+labextension/gallerymenu/static/56.2726b62668fa9972cd30.js
 labextension/gallerymenu/static/638.95e0186307171588df5b.js
 labextension/gallerymenu/static/638.95e0186307171588df5b.js.LICENSE.txt
-labextension/gallerymenu/static/remoteEntry.fadc9f3eb62fb570716e.js
+labextension/gallerymenu/static/remoteEntry.59749b88a6eed42d676f.js
 labextension/gallerymenu/static/style.js
 labextension/gallerymenu/static/third-party-licenses.json
 labextension/inject-uuid/package.json
 labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/package.json.orig
-labextension/inject-uuid/static/568.bde16f9395a112a349ee.js
-labextension/inject-uuid/static/remoteEntry.f32354aac49e7b8ba738.js
+labextension/inject-uuid/static/568.1c56cc1b2764b66bca50.js
+labextension/inject-uuid/static/remoteEntry.961a61df8bda40e885ae.js
 labextension/inject-uuid/static/style.js
 labextension/inject-uuid/static/third-party-licenses.json
 labextension/instrumentation/package.json
 labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/instrumentation.json
 labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/package.json.orig
-labextension/instrumentation/static/568.274dc29b6aea1cf48d74.js
+labextension/instrumentation/static/568.b9882f522566d7c3f80b.js
 labextension/instrumentation/static/638.b95125ed695cee42aae4.js
 labextension/instrumentation/static/638.b95125ed695cee42aae4.js.LICENSE.txt
 labextension/instrumentation/static/701.d81800f5926ab62cc8b2.js
-labextension/instrumentation/static/remoteEntry.52d0d8f58cd3e55540ee.js
+labextension/instrumentation/static/remoteEntry.e2d86efe89b107788c6a.js
 labextension/instrumentation/static/style.js
 labextension/instrumentation/static/third-party-licenses.json
 labextension/userpreferences/package.json
 labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/package.json.orig
 labextension/userpreferences/static/542.d1718a50e23f3808ba62.js
-labextension/userpreferences/static/568.eab1414ad9e7f57f8e93.js
+labextension/userpreferences/static/568.d278e7473ae759d43e90.js
 labextension/userpreferences/static/638.e5080f99954048969f76.js
 labextension/userpreferences/static/638.e5080f99954048969f76.js.LICENSE.txt
-labextension/userpreferences/static/remoteEntry.0c562dfea5f20371ffe8.js
+labextension/userpreferences/static/remoteEntry.ebf7fd35624f8fdb1636.js
 labextension/userpreferences/static/style.js
 labextension/userpreferences/static/third-party-licenses.json
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/autodownload/package.json` & `jupyterlab_nbgallery-2.0.3/labextension/autodownload/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9716435185185185%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.f0097f506f67321081da.js'}}",*

 * * "'version'": "'1.1.1'"}*

```diff
@@ -27,15 +27,15 @@
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.77e4acbd8dd372ff3fad.js",
+            "load": "static/remoteEntry.f0097f506f67321081da.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../labextension/autodownload",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -69,9 +69,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.1.1"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/package.json.orig` & `jupyterlab_nbgallery-2.0.3/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'version'": "'1.1.1'"}*

```diff
@@ -64,9 +64,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.1.1"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/542.51fb91347d8a3d9a657a.js` & `jupyterlab_nbgallery-2.0.3/labextension/autodownload/static/542.51fb91347d8a3d9a657a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/568.8bc32e058afbf3d8a017.js` & `jupyterlab_nbgallery-2.0.3/labextension/autodownload/static/568.6448f5c1d260e1510f0b.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,127 +1,120 @@
 "use strict";
 (self.webpackChunk_jupyterlab_nbgallery_autodownload = self.webpackChunk_jupyterlab_nbgallery_autodownload || []).push([
     [568], {
-        568: (e, o, t) => {
-            t.r(o), t.d(o, {
-                default: () => l
+        568: (e, o, n) => {
+            n.r(o), n.d(o, {
+                default: () => c
             });
-            var n = t(38),
-                a = t(142),
-                r = t(569),
-                c = t.n(r);
-            const l = {
+            var t = n(629),
+                a = n(406),
+                r = n(569),
+                l = n.n(r);
+            const c = {
                 id: "@jupyterlab-nbgallery/autodownload",
                 autoStart: !0,
-                requires: [n.ISettingRegistry],
+                requires: [t.ISettingRegistry],
                 activate: async (e, o) => {
-                    let t = "",
-                        n = 0,
+                    let n = "",
+                        t = 0,
                         r = !1;
 
-                    function l() {
+                    function c() {
                         return a.PageConfig.getBaseUrl()
                     }
 
-                    function s(e, o, t) {
-                        c().ajax({
+                    function s(e, o, n) {
+                        l().ajax({
                             method: "GET",
                             headers: {
                                 Accept: "application/json"
                             },
                             url: e,
                             cache: !1,
                             xhrFields: {
                                 withCredentials: !0
                             },
                             success: function(e) {
-                                !async function(e, o, t) {
-                                    c().ajax({
-                                        url: l() + "post/" + e + "/" + encodeURIComponent(o) + ".ipynb",
+                                !async function(e, o, n) {
+                                    l().ajax({
+                                        url: c() + "post/" + e + "/" + encodeURIComponent(o) + ".ipynb",
                                         type: "POST",
                                         success: function() {},
                                         error: function(e) {
                                             console.error("Failed upload: " + o)
                                         },
                                         data: JSON.stringify({
                                             type: "notebook",
-                                            content: JSON.parse(t)
+                                            content: JSON.parse(n)
                                         })
                                     })
-                                }(o, t, e)
+                                }(o, n, e)
                             }
                         })
                     }
 
-                    function i(e, o, t) {
-                        c().ajax({
+                    function i(e, o, n) {
+                        l().ajax({
                             method: "GET",
-                            url: l() + "api/contents/" + encodeURIComponent(e),
+                            url: c() + "api/contents/" + encodeURIComponent(e),
                             cache: !1,
                             xhrFields: {
                                 withCredentials: !0
                             },
                             success: function(e) {},
-                            error: function(n) {
-                                console.info("Downloading notebooks to " + e), c().ajax({
+                            error: function(t) {
+                                console.info("Downloading notebooks to " + e), l().ajax({
                                     method: "POST",
-                                    url: l() + "post/" + encodeURIComponent(e),
+                                    url: c() + "post/" + encodeURIComponent(e),
                                     data: JSON.stringify({
                                         type: "directory"
                                     }),
                                     cache: !1,
-                                    success: function(n) {
-                                        c().ajax({
+                                    success: function(t) {
+                                        l().ajax({
                                             method: "GET",
                                             headers: {
                                                 Accept: "application/json"
                                             },
-                                            url: o + t,
+                                            url: o + n,
                                             cache: !1,
                                             xhrFields: {
                                                 withCredentials: !0
                                             },
-                                            success: function(t) {
-                                                let n;
-                                                for (n in t) {
-                                                    var a = t[n];
+                                            success: function(n) {
+                                                let t;
+                                                for (t in n) {
+                                                    var a = n[t];
                                                     s(o + "/notebooks/" + a.uuid + "/download?clickstream=false", e, a.title.replace(/\//g, "⁄"))
                                                 }
                                             }
                                         })
                                     }
                                 })
                             }
                         })
                     }
-                    Promise.all([e.restored, o.load("@jupyterlab-nbgallery/autodownload:autodownload")]).then((([, a]) => {
+                    Promise.all([e.restored, o.load("@jupyterlab-nbgallery/autodownload:autodownload"), o.load("@jupyterlab-nbgallery/environment-registration:environment-registration")]).then((([, e, o]) => {
                         try {
-                            ! function(a) {
-                                c().ajax({
+                            ! function(e, o) {
+                                n = o.get("nbgallery_url").composite, l().ajax({
                                     method: "GET",
                                     headers: {
                                         Accept: "application/json"
                                     },
-                                    url: l() + "jupyterlab_nbgallery/environment",
+                                    url: c() + "jupyterlab_nbgallery/environment",
                                     cache: !1,
                                     xhrFields: {
                                         withCredentials: !0
                                     },
-                                    success: function(c) {
-                                        try {
-                                            Promise.all([e.restored, o.load("@jupyterlab-nbgallery/environment-registration:environment-registration")]).then((([, e]) => {
-                                                t = e.get("nbgallery_url").composite
-                                            }))
-                                        } catch (e) {
-                                            t = c.NBGALLERY_URL
-                                        }
-                                        n = c.NBGALLERY_ENABLE_AUTODOWNLOAD, r = a.get("enabled").composite, console.info("Auto Downloading Notebooks"), (1 == n || r) && (i("Starred", t, "/notebooks/stars"), i("Recently Executed", t, "/notebooks/recently_executed"))
+                                    success: function(o) {
+                                        0 == n.length && (n = o.NBGALLERY_URL), t = o.NBGALLERY_ENABLE_AUTODOWNLOAD, r = e.get("enabled").composite, console.info("Auto Downloading Notebooks"), (1 == t || r && n.length > 0) && (i("Starred", n, "/notebooks/stars"), i("Recently Executed", n, "/notebooks/recently_executed"))
                                     }
                                 })
-                            }(a)
+                            }(e, o)
                         } catch (e) {
                             console.error(`Problem downloading notebooks \n ${e}`)
                         }
                     }))
                 }
             }
         }
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js` & `jupyterlab_nbgallery-2.0.3/labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/remoteEntry.77e4acbd8dd372ff3fad.js` & `jupyterlab_nbgallery-2.0.3/labextension/autodownload/static/remoteEntry.f0097f506f67321081da.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, u, d, f, s, p, c, h, b, v, g, y = {
+    var e, r, t, n, a, o, i, l, u, d, s, f, p, c, h, b, v, g, y = {
             735: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568))),
                         "./style": () => t.e(542).then((() => () => t(542)))
                     },
-                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    o = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                o = t.S[n];
-                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                a = t.S[n];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => o,
-                    init: () => a
+                    get: () => a,
+                    init: () => o
                 })
             }
         },
         m = {};
 
     function w(e) {
         var r = m[e];
@@ -44,80 +44,80 @@
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         542: "51fb91347d8a3d9a657a",
-        568: "8bc32e058afbf3d8a017",
+        568: "6448f5c1d260e1510f0b",
         638: "0ed295d9378dea7c5c7b"
     } [e] + ".js?v=" + {
         542: "51fb91347d8a3d9a657a",
-        568: "8bc32e058afbf3d8a017",
+        568: "6448f5c1d260e1510f0b",
         638: "0ed295d9378dea7c5c7b"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab-nbgallery/autodownload:", w.l = (t, n, o, a) => {
+    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab-nbgallery/autodownload:", w.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
-            if (void 0 !== o)
+            if (void 0 !== a)
                 for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
-                    var f = u[d];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                    var s = u[d];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
+                        i = s;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var s = (r, n) => {
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
+            var f = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
-                    var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
+                    var a = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         w.S = {};
         var e = {},
             r = {};
         w.I = (t, n) => {
             n || (n = []);
-            var o = r[t];
-            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
-                if (n.push(o), e[t]) return e[t];
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
+                if (n.push(a), e[t]) return e[t];
                 w.o(w.S, t) || (w.S[t] = {});
-                var a = w.S[t],
+                var o = w.S[t],
                     i = "@jupyterlab-nbgallery/autodownload",
                     l = (e, r, t, n) => {
-                        var o = a[e] = a[e] || {},
-                            l = o[r];
-                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
+                        var a = o[e] = o[e] || {},
+                            l = a[r];
+                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyterlab-nbgallery/autodownload", "1.1.0", (() => w.e(568).then((() => () => w(568))))), l("jquery", "3.6.4", (() => w.e(638).then((() => () => w(638)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyterlab-nbgallery/autodownload", "1.1.1", (() => w.e(568).then((() => () => w(568))))), l("jquery", "3.6.4", (() => w.e(638).then((() => () => w(638)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -131,152 +131,152 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var o = e[n],
-                a = (typeof o)[0];
-            if (n >= r.length) return "u" == a;
+            var a = e[n],
+                o = (typeof a)[0];
+            if (n >= r.length) return "u" == o;
             var i = r[n],
                 l = (typeof i)[0];
-            if (a != l) return "o" == a && "n" == l || "s" == l || "u" == a;
-            if ("o" != a && "u" != a && o != i) return o < i;
+            if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
+            if ("o" != o && "u" != o && a != i) return a < i;
             n++
         }
-    }, o = e => {
+    }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(l = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var i = [];
-        for (a = 1; a < e.length; a++) {
-            var l = e[a];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
+        for (o = 1; o < e.length; o++) {
+            var l = e[o];
+            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : a(l))
         }
         return u();
 
         function u() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                o = n < 0;
-            o && (n = -n - 1);
+                a = n < 0;
+            a && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var d, f, s = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !u || ("u" == s ? l > n && !o : "" == s != o);
-                if ("u" == f) {
-                    if (!u || "u" != s) return !1
+                var d, s, f = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !u || ("u" == f ? l > n && !a : "" == f != a);
+                if ("u" == s) {
+                    if (!u || "u" != f) return !1
                 } else if (u)
-                    if (s == f)
+                    if (f == s)
                         if (l <= n) {
                             if (d != e[l]) return !1
                         } else {
-                            if (o ? d > e[l] : d < e[l]) return !1;
+                            if (a ? d > e[l] : d < e[l]) return !1;
                             d != e[l] && (u = !1)
                         }
-                else if ("s" != s && "n" != s) {
-                    if (o || l <= n) return !1;
+                else if ("s" != f && "n" != f) {
+                    if (a || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || f < s != o) return !1;
+                    if (l <= n || s < f != a) return !1;
                     u = !1
-                } else "s" != s && "n" != s && (u = !1, l--)
+                } else "s" != f && "n" != f && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", d = (e, r, t, n) => {
-        var o = l(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(u(e, t, o, n)), s(e[t][o])
-    }, f = (e, r, t) => {
-        var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, s = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, o) {
-        var a = w.I(r);
-        return a && a.then ? a.then(e.bind(e, r, w.S[r], t, n, o)) : e(r, w.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), h = p(((e, r, t, n, o) => {
-        var a = r && w.o(r, t) && f(r, t, n);
-        return a ? s(a) : o()
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
+        var a = l(e, t);
+        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(u(e, t, a, n)), f(e[t][a])
+    }, s = (e, r, t) => {
+        var a = e[r];
+        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+    }, f = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, a) {
+        var o = w.I(r);
+        return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
+    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), h = p(((e, r, t, n, a) => {
+        var o = r && w.o(r, t) && s(r, t, n);
+        return o ? f(o) : a()
     })), b = {}, v = {
-        38: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
-        142: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
-        569: () => h("default", "jquery", [1, 3, 5, 0], (() => w.e(638).then((() => () => w(638)))))
+        406: () => c("default", "@jupyterlab/coreutils", [1, 6, 0, 0]),
+        569: () => h("default", "jquery", [1, 3, 5, 0], (() => w.e(638).then((() => () => w(638))))),
+        629: () => c("default", "@jupyterlab/settingregistry", [1, 4, 0, 0])
     }, g = {
-        568: [38, 142, 569]
+        568: [406, 569, 629]
     }, w.f.consumes = (e, r) => {
         w.o(g, e) && g[e].forEach((e => {
             if (w.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
                 },
                 n = r => {
                     delete b[e], w.m[e] = t => {
                         throw delete w.c[e], r
                     }
                 };
             try {
-                var o = v[e]();
-                o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
+                var a = v[e]();
+                a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             263: 0
         };
         w.f.j = (r, t) => {
             var n = w.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
-                    var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                    t.push(n[2] = o);
-                    var a = w.p + w.u(r),
+                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
+                    t.push(n[2] = a);
+                    var o = w.p + w.u(r),
                         i = new Error;
-                    w.l(a, (t => {
+                    w.l(o, (t => {
                         if (w.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var o = t && ("load" === t.type ? "missing" : t.type),
-                                a = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                            var a = t && ("load" === t.type ? "missing" : t.type),
+                                o = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, o, [a, i, l] = t,
+                var n, a, [o, i, l] = t,
                     u = 0;
-                if (a.some((r => 0 !== e[r]))) {
+                if (o.some((r => 0 !== e[r]))) {
                     for (n in i) w.o(i, n) && (w.m[n] = i[n]);
                     l && l(w)
                 }
-                for (r && r(t); u < a.length; u++) o = a[u], w.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); u < o.length; u++) a = o[u], w.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_jupyterlab_nbgallery_autodownload = self.webpackChunk_jupyterlab_nbgallery_autodownload || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), w.nc = void 0;
     var j = w(735);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlab-nbgallery/autodownload"] = j
 })();
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/third-party-licenses.json` & `jupyterlab_nbgallery-2.0.3/labextension/autodownload/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/environment-life/package.json` & `jupyterlab_nbgallery-2.0.3/labextension/environment-life/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994212962962963%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.3b2f785c13bf442d8fd1.js'}}"}*

```diff
@@ -28,15 +28,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.fe9e40141faed985c15b.js",
+            "load": "static/remoteEntry.3b2f785c13bf442d8fd1.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../labextension/environment-life",
         "schemaDir": "schema"
     },
     "keywords": [
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/package.json.orig` & `jupyterlab_nbgallery-2.0.3/labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/248.19732aba6894a502e197.js` & `jupyterlab_nbgallery-2.0.3/labextension/environment-life/static/248.ff22e12bacd29ee749b6.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunk_jupyterlab_nbgallery_environment_life = self.webpackChunk_jupyterlab_nbgallery_environment_life || []).push([
     [248], {
         248: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => l
             });
-            var r = n(832),
-                i = n(583),
-                o = n(142),
-                a = n(820);
+            var r = n(778),
+                i = n(653),
+                o = n(406),
+                a = n(67);
             const l = {
                 id: "@jupyterlab-nbgallery/environment-life",
                 autoStart: !0,
                 requires: [i.IStatusBar],
                 activate: async (e, t) => {
                     let n = "";
                     try {
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/542.e4d405f3b0e4f693ab53.js` & `jupyterlab_nbgallery-2.0.3/labextension/environment-life/static/542.e4d405f3b0e4f693ab53.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/remoteEntry.fe9e40141faed985c15b.js` & `jupyterlab_nbgallery-2.0.3/labextension/environment-life/static/remoteEntry.3b2f785c13bf442d8fd1.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -43,18 +43,18 @@
         }), r
     }, g.d = (e, r) => {
         for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + "." + {
-        248: "19732aba6894a502e197",
+        248: "ff22e12bacd29ee749b6",
         542: "e4d405f3b0e4f693ab53"
     } [e] + ".js?v=" + {
-        248: "19732aba6894a502e197",
+        248: "ff22e12bacd29ee749b6",
         542: "e4d405f3b0e4f693ab53"
     } [e], g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -205,20 +205,20 @@
     }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = l(e, t);
         return a(n, o) || "undefined" != typeof console && console.warn && console.warn(u(e, t, o, n)), s(e[t][o])
     }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
         var a = g.I(r);
         return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), p = {}, c = {
-        142: () => d("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
-        583: () => d("default", "@jupyterlab/statusbar", [1, 3, 6, 3]),
-        820: () => d("default", "@jupyterlab/services", [1, 6, 6, 3]),
-        832: () => d("default", "@lumino/widgets", [1, 1, 37, 2])
+        67: () => d("default", "@jupyterlab/services", [1, 7, 0, 0]),
+        406: () => d("default", "@jupyterlab/coreutils", [1, 6, 0, 0]),
+        653: () => d("default", "@jupyterlab/statusbar", [1, 4, 0, 0]),
+        778: () => d("default", "@lumino/widgets", [1, 2, 0, 1])
     }, h = {
-        248: [142, 583, 820, 832]
+        248: [67, 406, 653, 778]
     }, g.f.consumes = (e, r) => {
         g.o(h, e) && h[e].forEach((e => {
             if (g.o(p, e)) return r.push(p[e]);
             var t = r => {
                     p[e] = 0, g.m[e] = t => {
                         delete g.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/third-party-licenses.json` & `jupyterlab_nbgallery-2.0.3/labextension/environment-life/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/package.json` & `jupyterlab_nbgallery-2.0.3/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9652777777777778%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'1.0.6'"}*

```diff
@@ -26,19 +26,14 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.54aae520a7b7fc99d9fd.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "../labextension/environment-registration",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -70,9 +65,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "1.0.5"
+    "version": "1.0.6"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/package.json.orig` & `jupyterlab_nbgallery-2.0.3/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/package.json.orig`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8472222222222222%*

 * *Differences: {"'dependencies'": "{'ts-md5': '^1.2.9', delete: ['@jupyterlab/services']}",*

 * * "'description'": "'Track cell execution Metrics'",*

 * * "'jupyterlab'": "{'outputDir': '../labextension/instrumentation'}",*

 * * "'name'": "'@jupyterlab-nbgallery/instrumentation'",*

 * * "'version'": "'2.1.0'",*

 * * 'delete': "['style']"}*

```diff
@@ -2,19 +2,19 @@
     "author": "Team@NBG",
     "bugs": {
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
         "@jupyterlab/coreutils": ">=5.2.0",
-        "@jupyterlab/services": ">=6.6.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
-        "jquery": "^3.5.0"
+        "jquery": "^3.5.0",
+        "ts-md5": "^1.2.9"
     },
-    "description": "Register NBGallery Environment",
+    "description": "Track cell execution Metrics",
     "devDependencies": {
         "@jupyterlab/builder": ">=3.3.2",
         "@types/jquery": "^3.5.0",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
@@ -27,25 +27,25 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "extension": true,
-        "outputDir": "../labextension/environment-registration",
+        "outputDir": "../labextension/instrumentation",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
-    "name": "@jupyterlab-nbgallery/environment-registration",
+    "name": "@jupyterlab-nbgallery/instrumentation",
     "repository": {
         "type": "git",
         "url": "https://github.com/nbgallery/lab-extensions"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:all": "jlpm run build:prod",
@@ -63,11 +63,10 @@
         "install-ext": "jlpm run build",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
-    "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "1.0.5"
+    "version": "2.1.0"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/542.feae6c397f33f9138fea.js` & `jupyterlab_nbgallery-2.0.3/labextension/environment-registration/static/542.feae6c397f33f9138fea.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/638.36e464d3233849b6b07a.js` & `jupyterlab_nbgallery-2.0.3/labextension/environment-registration/static/638.36e464d3233849b6b07a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/784.201d6fbbedd26339ab72.js` & `jupyterlab_nbgallery-2.0.3/labextension/environment-registration/static/784.05dd45a572b8a68b8ef0.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 "use strict";
 (self.webpackChunk_jupyterlab_nbgallery_environment_registration = self.webpackChunk_jupyterlab_nbgallery_environment_registration || []).push([
     [784], {
         784: (e, n, t) => {
             t.r(n), t.d(n, {
                 default: () => s
             });
-            var r = t(38),
-                o = t(142),
-                a = t(820),
+            var r = t(629),
+                o = t(406),
+                a = t(67),
                 i = t(569),
                 l = t.n(i);
             const s = {
                 id: "@jupyterlab-nbgallery/environment-registration",
                 autoStart: !0,
                 requires: [r.ISettingRegistry],
                 activate: async (e, n) => {
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/remoteEntry.54aae520a7b7fc99d9fd.js` & `jupyterlab_nbgallery-2.0.3/labextension/environment-registration/static/remoteEntry.fad449cea8e4f679087a.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -45,19 +45,19 @@
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         542: "feae6c397f33f9138fea",
         638: "36e464d3233849b6b07a",
-        784: "201d6fbbedd26339ab72"
+        784: "05dd45a572b8a68b8ef0"
     } [e] + ".js?v=" + {
         542: "feae6c397f33f9138fea",
         638: "36e464d3233849b6b07a",
-        784: "201d6fbbedd26339ab72"
+        784: "05dd45a572b8a68b8ef0"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -109,15 +109,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyterlab-nbgallery/environment-registration", "1.0.5", (() => w.e(784).then((() => () => w(784))))), l("jquery", "3.6.4", (() => w.e(638).then((() => () => w(638)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyterlab-nbgallery/environment-registration", "1.0.6", (() => w.e(784).then((() => () => w(784))))), l("jquery", "3.6.4", (() => w.e(638).then((() => () => w(638)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -214,20 +214,20 @@
     }, f = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, o) {
         var a = w.I(r);
         return a && a.then ? a.then(e.bind(e, r, w.S[r], t, n, o)) : e(r, w.S[r], t, n, o)
     })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), h = p(((e, r, t, n, o) => {
         var a = r && w.o(r, t) && d(r, t, n);
         return a ? f(a) : o()
     })), v = {}, g = {
-        38: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
-        142: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        67: () => c("default", "@jupyterlab/services", [1, 7, 0, 0]),
+        406: () => c("default", "@jupyterlab/coreutils", [1, 6, 0, 0]),
         569: () => h("default", "jquery", [1, 3, 5, 0], (() => w.e(638).then((() => () => w(638))))),
-        820: () => c("default", "@jupyterlab/services", [1, 6, 6, 3])
+        629: () => c("default", "@jupyterlab/settingregistry", [1, 4, 0, 0])
     }, b = {
-        784: [38, 142, 569, 820]
+        784: [67, 406, 569, 629]
     }, w.f.consumes = (e, r) => {
         w.o(b, e) && b[e].forEach((e => {
             if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/third-party-licenses.json` & `jupyterlab_nbgallery-2.0.3/labextension/environment-registration/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/package.json` & `jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990234375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.59749b88a6eed42d676f.js'}}"}*

```diff
@@ -28,15 +28,15 @@
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.fadc9f3eb62fb570716e.js"
+            "load": "static/remoteEntry.59749b88a6eed42d676f.js"
         },
         "extension": true,
         "outputDir": "../labextension/gallerymenu",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/package.json.orig` & `jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/56.2f2a1bce28a94a6668e1.js` & `jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/static/56.2726b62668fa9972cd30.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 "use strict";
 (self.webpackChunk_jupyterlab_nbgallery_gallerymenu = self.webpackChunk_jupyterlab_nbgallery_gallerymenu || []).push([
     [56], {
         56: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => y
             });
-            var l = a(344),
-                i = a(33),
-                o = a(832),
-                n = a(123),
-                s = a(820),
-                r = a(142),
-                d = a(38),
-                h = a(271);
+            var l = a(277),
+                i = a(501),
+                o = a(778),
+                n = a(897),
+                s = a(67),
+                r = a(406),
+                d = a(629),
+                h = a(29);
             class u extends i.ReactWidget {
                 constructor() {
                     super(), this.addClass("jp-ReactWidget")
                 }
                 render() {
                     return h.createElement("div", {
                         dangerouslySetInnerHTML: {
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/638.95e0186307171588df5b.js` & `jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/static/638.95e0186307171588df5b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/remoteEntry.fadc9f3eb62fb570716e.js` & `jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/static/remoteEntry.59749b88a6eed42d676f.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -41,18 +41,18 @@
         }), r
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        56: "2f2a1bce28a94a6668e1",
+        56: "2726b62668fa9972cd30",
         638: "95e0186307171588df5b"
     } [e] + ".js?v=" + {
-        56: "2f2a1bce28a94a6668e1",
+        56: "2726b62668fa9972cd30",
         638: "95e0186307171588df5b"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -210,25 +210,25 @@
     }, d = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, a) {
         var o = w.I(r);
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
     })(((e, r, t, n) => (l(e, t), f(r, 0, t, n)))), h = p(((e, r, t, n, a) => {
         var o = r && w.o(r, t) && s(r, t, n);
         return o ? d(o) : a()
     })), v = {}, b = {
-        33: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
-        38: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
-        123: () => c("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
-        142: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
-        271: () => c("default", "react", [1, 17, 0, 1]),
-        344: () => c("default", "@jupyterlab/mainmenu", [1, 3, 6, 3]),
+        29: () => c("default", "react", [1, 18, 2, 0]),
+        67: () => c("default", "@jupyterlab/services", [1, 7, 0, 0]),
+        277: () => c("default", "@jupyterlab/mainmenu", [1, 4, 0, 0]),
+        406: () => c("default", "@jupyterlab/coreutils", [1, 6, 0, 0]),
+        501: () => c("default", "@jupyterlab/apputils", [1, 4, 0, 0]),
         569: () => h("default", "jquery", [1, 3, 5, 0], (() => w.e(638).then((() => () => w(638))))),
-        820: () => c("default", "@jupyterlab/services", [1, 6, 6, 3]),
-        832: () => c("default", "@lumino/widgets", [1, 1, 37, 2])
+        629: () => c("default", "@jupyterlab/settingregistry", [1, 4, 0, 0]),
+        778: () => c("default", "@lumino/widgets", [1, 2, 0, 1]),
+        897: () => c("default", "@jupyterlab/notebook", [1, 4, 0, 0])
     }, g = {
-        56: [33, 38, 123, 142, 271, 344, 569, 820, 832]
+        56: [29, 67, 277, 406, 501, 569, 629, 778, 897]
     }, w.f.consumes = (e, r) => {
         w.o(g, e) && g[e].forEach((e => {
             if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/third-party-licenses.json` & `jupyterlab_nbgallery-2.0.3/labextension/gallerymenu/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/package.json` & `jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990808823529411%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.961a61df8bda40e885ae.js'}}"}*

```diff
@@ -27,15 +27,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f32354aac49e7b8ba738.js"
+            "load": "static/remoteEntry.961a61df8bda40e885ae.js"
         },
         "extension": true,
         "outputDir": "../labextension/inject-uuid",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/package.json.orig` & `jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/static/568.bde16f9395a112a349ee.js` & `jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/static/568.1c56cc1b2764b66bca50.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -30,15 +30,15 @@
             }
             s.r(t), s.d(t, {
                 default: () => i
             });
             const i = {
                 id: "@jupyterlab-nbgallery/inject-uuid",
                 autoStart: !0,
-                requires: [s(123).INotebookTracker],
+                requires: [s(897).INotebookTracker],
                 activate: (e, t) => {
                     t.forEach(o), t.widgetAdded.connect(((e, t) => o(t)))
                 }
             }
         }
     }
 ]);
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/static/remoteEntry.f32354aac49e7b8ba738.js` & `jupyterlab_nbgallery-2.0.3/labextension/inject-uuid/static/remoteEntry.961a61df8bda40e885ae.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, v = {
             711: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -20,105 +20,105 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
-        b = {};
+        g = {};
 
-    function g(e) {
-        var r = b[e];
+    function b(e) {
+        var r = g[e];
         if (void 0 !== r) return r.exports;
-        var t = b[e] = {
+        var t = g[e] = {
             exports: {}
         };
-        return v[e](t, t.exports, g), t.exports
+        return v[e](t, t.exports, b), t.exports
     }
-    g.m = v, g.c = b, g.n = e => {
+    b.m = v, b.c = g, b.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return g.d(r, {
+        return b.d(r, {
             a: r
         }), r
-    }, g.d = (e, r) => {
-        for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
+    }, b.d = (e, r) => {
+        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + ".bde16f9395a112a349ee.js?v=bde16f9395a112a349ee", g.g = function() {
+    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + ".1c56cc1b2764b66bca50.js?v=1c56cc1b2764b66bca50", b.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab-nbgallery/inject-uuid:", g.l = (t, n, o, a) => {
+    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab-nbgallery/inject-uuid:", b.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
                     var f = l[s];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
                         i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, b.nc && i.setAttribute("nonce", b.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, g.r = e => {
+    }, b.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        g.S = {};
+        b.S = {};
         var e = {},
             r = {};
-        g.I = (t, n) => {
+        b.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                g.o(g.S, t) || (g.S[t] = {});
-                var a = g.S[t],
+                b.o(b.S, t) || (b.S[t] = {});
+                var a = b.S[t],
                     i = "@jupyterlab-nbgallery/inject-uuid",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => g.e(568).then((() => () => g(568))),
+                        get: () => b.e(568).then((() => () => b(568))),
                         from: i,
                         eager: !1
                     })
                 })("@jupyterlab-nbgallery/inject-uuid", "2.0.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        g.g.importScripts && (e = g.g.location + "");
-        var r = g.g.document;
+        b.g.importScripts && (e = b.g.location + "");
+        var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             t.length && (e = t[t.length - 1].src)
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), g.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -176,88 +176,88 @@
                     l = !1, u--
                 } else {
                     if (u <= n || f < d != o) return !1;
                     l = !1
                 } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, i = (e, r) => {
-        var t = g.S[e];
-        if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = b.S[e];
+        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
         return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), f(e[t][o])
     }, f = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
-        var a = g.I(r);
-        return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), p = {}, c = {
-        123: () => d("default", "@jupyterlab/notebook", [1, 3, 6, 3])
+        var a = b.I(r);
+        return a && a.then ? a.then(e.bind(e, r, b.S[r], t, n, o)) : e(r, b.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), c = {}, p = {
+        897: () => d("default", "@jupyterlab/notebook", [1, 4, 0, 0])
     }, h = {
-        568: [123]
-    }, g.f.consumes = (e, r) => {
-        g.o(h, e) && h[e].forEach((e => {
-            if (g.o(p, e)) return r.push(p[e]);
+        568: [897]
+    }, b.f.consumes = (e, r) => {
+        b.o(h, e) && h[e].forEach((e => {
+            if (b.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    p[e] = 0, g.m[e] = t => {
-                        delete g.c[e], t.exports = r()
+                    c[e] = 0, b.m[e] = t => {
+                        delete b.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete p[e], g.m[e] = t => {
-                        throw delete g.c[e], r
+                    delete c[e], b.m[e] = t => {
+                        throw delete b.c[e], r
                     }
                 };
             try {
-                var o = c[e]();
-                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
+                var o = p[e]();
+                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             582: 0
         };
-        g.f.j = (r, t) => {
-            var n = g.o(e, r) ? e[r] : void 0;
+        b.f.j = (r, t) => {
+            var n = b.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = g.p + g.u(r),
+                    var a = b.p + b.u(r),
                         i = new Error;
-                    g.l(a, (t => {
-                        if (g.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    b.l(a, (t => {
+                        if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
                     l = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) g.o(i, n) && (g.m[n] = i[n]);
-                    u && u(g)
+                    for (n in i) b.o(i, n) && (b.m[n] = i[n]);
+                    u && u(b)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], g.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], b.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupyterlab_nbgallery_inject_uuid = self.webpackChunk_jupyterlab_nbgallery_inject_uuid || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var y = g(711);
+    var y = b(711);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlab-nbgallery/inject-uuid"] = y
 })();
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/package.json` & `jupyterlab_nbgallery-2.0.3/labextension/instrumentation/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990808823529411%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e2d86efe89b107788c6a.js'}}"}*

```diff
@@ -28,15 +28,15 @@
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.52d0d8f58cd3e55540ee.js"
+            "load": "static/remoteEntry.e2d86efe89b107788c6a.js"
         },
         "extension": true,
         "outputDir": "../labextension/instrumentation",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/package.json.orig` & `jupyterlab_nbgallery-2.0.3/labextension/environment-registration/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8414351851851852%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/services': '>=6.6.0', delete: ['ts-md5']}",*

 * * "'description'": "'Register NBGallery Environment'",*

 * * "'jupyterlab'": "{'outputDir': '../labextension/environment-registration', '_build': "*

 * *                 "OrderedDict([('load', 'static/remoteEntry.fad449cea8e4f679087a.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'name'": "'@jupyterlab-nbgallery/environment-registration'",*

 * * "'style'": "'style/index.css'",*

 * * "'version'": "'1.0.6'"}*

```diff
@@ -2,19 +2,19 @@
     "author": "Team@NBG",
     "bugs": {
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
         "@jupyterlab/coreutils": ">=5.2.0",
+        "@jupyterlab/services": ">=6.6.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
-        "jquery": "^3.5.0",
-        "ts-md5": "^1.2.9"
+        "jquery": "^3.5.0"
     },
-    "description": "Track cell execution Metrics",
+    "description": "Register NBGallery Environment",
     "devDependencies": {
         "@jupyterlab/builder": ">=3.3.2",
         "@types/jquery": "^3.5.0",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
@@ -26,26 +26,31 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.fad449cea8e4f679087a.js",
+            "style": "./style"
+        },
         "extension": true,
-        "outputDir": "../labextension/instrumentation",
+        "outputDir": "../labextension/environment-registration",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
-    "name": "@jupyterlab-nbgallery/instrumentation",
+    "name": "@jupyterlab-nbgallery/environment-registration",
     "repository": {
         "type": "git",
         "url": "https://github.com/nbgallery/lab-extensions"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:all": "jlpm run build:prod",
@@ -63,10 +68,11 @@
         "install-ext": "jlpm run build",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
+    "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "2.1.0"
+    "version": "1.0.6"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/568.274dc29b6aea1cf48d74.js` & `jupyterlab_nbgallery-2.0.3/labextension/instrumentation/static/568.b9882f522566d7c3f80b.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunk_jupyterlab_nbgallery_instrumentation = self.webpackChunk_jupyterlab_nbgallery_instrumentation || []).push([
     [568], {
         568: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => d
             });
-            var l = n(38),
-                o = n(142),
-                i = n(123),
-                a = n(191),
+            var l = n(629),
+                o = n(406),
+                i = n(897),
+                a = n(225),
                 r = n(24),
                 s = n(569),
                 c = n.n(s);
             let u = null;
             const d = {
                 id: "@juptyerlab-nbgallery/instrumentation",
                 autoStart: !0,
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/638.b95125ed695cee42aae4.js` & `jupyterlab_nbgallery-2.0.3/labextension/instrumentation/static/638.b95125ed695cee42aae4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/701.d81800f5926ab62cc8b2.js` & `jupyterlab_nbgallery-2.0.3/labextension/instrumentation/static/701.d81800f5926ab62cc8b2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/remoteEntry.52d0d8f58cd3e55540ee.js` & `jupyterlab_nbgallery-2.0.3/labextension/instrumentation/static/remoteEntry.e2d86efe89b107788c6a.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, b, v, y, g, m, w, j, S = {
+    var e, r, t, n, o, a, i, u, l, s, d, f, p, c, h, b, v, y, g, m, w, j, S = {
             250: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -41,19 +41,19 @@
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        568: "274dc29b6aea1cf48d74",
+        568: "b9882f522566d7c3f80b",
         638: "b95125ed695cee42aae4",
         701: "d81800f5926ab62cc8b2"
     } [e] + ".js?v=" + {
-        568: "274dc29b6aea1cf48d74",
+        568: "b9882f522566d7c3f80b",
         638: "b95125ed695cee42aae4",
         701: "d81800f5926ab62cc8b2"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -61,31 +61,31 @@
         }
     }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab-nbgallery/instrumentation:", E.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                    var d = l[s];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        i = d;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+            var f = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -164,78 +164,78 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
-                if ("u" == f) {
-                    if (!l || "u" != d) return !1
+                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
+                if ("u" == d) {
+                    if (!l || "u" != f) return !1
                 } else if (l)
-                    if (d == f)
+                    if (f == d)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
                             if (o ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < d != o) return !1;
+                    if (u <= n || d < f != o) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", d = (e, r, t, n) => {
         var o = l(e, t);
         return a(n, o) || "undefined" != typeof console && console.warn && console.warn(s(e, t, o, n)), h(e[t][o])
-    }, d = (e, r, t) => {
+    }, f = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, c = (e, r, t, n) => {
+    }, p = (e, r, t, n) => {
         var a = e[t];
         return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
-    }, p = (e, r, t, n) => {
-        "undefined" != typeof console && console.warn && console.warn(c(e, r, t, n))
+    }, c = (e, r, t, n) => {
+        "undefined" != typeof console && console.warn && console.warn(p(e, r, t, n))
     }, h = e => (e.loaded = 1, e.get()), v = (b = e => function(r, t, n, o) {
         var a = E.I(r);
         return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), h(d(r, t, n) || p(r, e, t, n) || u(r, t))))), y = b(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), g = b(((e, r, t, n, o) => {
-        var a = r && E.o(r, t) && d(r, t, n);
+    })(((e, r, t, n) => (i(e, t), h(f(r, t, n) || c(r, e, t, n) || u(r, t))))), y = b(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), g = b(((e, r, t, n, o) => {
+        var a = r && E.o(r, t) && f(r, t, n);
         return a ? h(a) : o()
     })), m = {}, w = {
         24: () => g("default", "ts-md5", [1, 1, 2, 9], (() => E.e(701).then((() => () => E(701))))),
-        38: () => y("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
-        123: () => y("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
-        142: () => y("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
-        191: () => v("default", "@jupyterlab/cells", [1, 3, 6, 3]),
-        569: () => g("default", "jquery", [1, 3, 5, 0], (() => E.e(638).then((() => () => E(638)))))
+        225: () => v("default", "@jupyterlab/cells", [1, 4, 0, 0]),
+        406: () => y("default", "@jupyterlab/coreutils", [1, 6, 0, 0]),
+        569: () => g("default", "jquery", [1, 3, 5, 0], (() => E.e(638).then((() => () => E(638))))),
+        629: () => y("default", "@jupyterlab/settingregistry", [1, 4, 0, 0]),
+        897: () => y("default", "@jupyterlab/notebook", [1, 4, 0, 0])
     }, j = {
-        568: [24, 38, 123, 142, 191, 569]
+        568: [24, 225, 406, 569, 629, 897]
     }, E.f.consumes = (e, r) => {
         E.o(j, e) && j[e].forEach((e => {
             if (E.o(m, e)) return r.push(m[e]);
             var t = r => {
                     m[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/third-party-licenses.json` & `jupyterlab_nbgallery-2.0.3/labextension/instrumentation/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/package.json` & `jupyterlab_nbgallery-2.0.3/labextension/userpreferences/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994212962962963%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ebf7fd35624f8fdb1636.js'}}"}*

```diff
@@ -28,15 +28,15 @@
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.0c562dfea5f20371ffe8.js",
+            "load": "static/remoteEntry.ebf7fd35624f8fdb1636.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../labextension/userpreferences",
         "schemaDir": "schema"
     },
     "keywords": [
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/package.json.orig` & `jupyterlab_nbgallery-2.0.3/labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/542.d1718a50e23f3808ba62.js` & `jupyterlab_nbgallery-2.0.3/labextension/userpreferences/static/542.d1718a50e23f3808ba62.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/568.eab1414ad9e7f57f8e93.js` & `jupyterlab_nbgallery-2.0.3/labextension/userpreferences/static/568.d278e7473ae759d43e90.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 "use strict";
 (self.webpackChunk_jupyterlab_nbgallery_userpreferences = self.webpackChunk_jupyterlab_nbgallery_userpreferences || []).push([
     [568], {
         568: (e, r, t) => {
             t.r(r), t.d(r, {
                 default: () => h
             });
-            var a = t(344),
-                s = t(33),
-                n = t(832),
-                l = t(820),
-                i = t(38),
-                o = t(142),
+            var a = t(277),
+                s = t(501),
+                n = t(778),
+                l = t(67),
+                i = t(629),
+                o = t(406),
                 c = t(569),
                 u = t.n(c);
             const d = {
                 id: "@jupyterlab-nbgallery/userpreferences",
                 autoStart: !0,
                 requires: [a.IMainMenu, i.ISettingRegistry],
                 activate: function(e, r, t) {
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/638.e5080f99954048969f76.js` & `jupyterlab_nbgallery-2.0.3/labextension/userpreferences/static/638.e5080f99954048969f76.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/remoteEntry.0c562dfea5f20371ffe8.js` & `jupyterlab_nbgallery-2.0.3/labextension/userpreferences/static/remoteEntry.ebf7fd35624f8fdb1636.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, f, p, c, d, h, v, b, g, y = {
+    var e, r, t, n, a, o, i, u, l, s, f, p, d, c, h, v, b, g, y = {
             130: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568))),
                         "./style": () => t.e(542).then((() => () => t(542)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -44,19 +44,19 @@
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         542: "d1718a50e23f3808ba62",
-        568: "eab1414ad9e7f57f8e93",
+        568: "d278e7473ae759d43e90",
         638: "e5080f99954048969f76"
     } [e] + ".js?v=" + {
         542: "d1718a50e23f3808ba62",
-        568: "eab1414ad9e7f57f8e93",
+        568: "d278e7473ae759d43e90",
         638: "e5080f99954048969f76"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -71,19 +71,19 @@
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
                         i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var p = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+                    i.onerror = i.onload = null, clearTimeout(d);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(p.bind(null, void 0, {
+                d = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -187,50 +187,50 @@
                     l = !1, u--
                 } else {
                     if (u <= n || f < p != a) return !1;
                     l = !1
                 } else "s" != p && "n" != p && (l = !1, u--)
             }
         }
-        var c = [],
-            d = c.pop.bind(c);
+        var d = [],
+            c = d.pop.bind(d);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? o(h, r) : !d())
+            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
-        return !!d()
+        return !!c()
     }, i = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
         var a = u(e, t);
         return o(n, a) || "undefined" != typeof console && console.warn && console.warn(l(e, t, a, n)), p(e[t][a])
     }, f = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, p = e => (e.loaded = 1, e.get()), d = (c = e => function(r, t, n, a) {
+    }, p = e => (e.loaded = 1, e.get()), c = (d = e => function(r, t, n, a) {
         var o = w.I(r);
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), h = c(((e, r, t, n, a) => {
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), h = d(((e, r, t, n, a) => {
         var o = r && w.o(r, t) && f(r, t, n);
         return o ? p(o) : a()
     })), v = {}, b = {
-        33: () => d("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
-        38: () => d("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
-        142: () => d("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
-        344: () => d("default", "@jupyterlab/mainmenu", [1, 3, 6, 3]),
+        67: () => c("default", "@jupyterlab/services", [1, 7, 0, 0]),
+        277: () => c("default", "@jupyterlab/mainmenu", [1, 4, 0, 0]),
+        406: () => c("default", "@jupyterlab/coreutils", [1, 6, 0, 0]),
+        501: () => c("default", "@jupyterlab/apputils", [1, 4, 0, 0]),
         569: () => h("default", "jquery", [1, 3, 5, 0], (() => w.e(638).then((() => () => w(638))))),
-        820: () => d("default", "@jupyterlab/services", [1, 6, 6, 3]),
-        832: () => d("default", "@lumino/widgets", [1, 1, 37, 2])
+        629: () => c("default", "@jupyterlab/settingregistry", [1, 4, 0, 0]),
+        778: () => c("default", "@lumino/widgets", [1, 2, 0, 1])
     }, g = {
-        568: [33, 38, 142, 344, 569, 820, 832]
+        568: [67, 277, 406, 501, 569, 629, 778]
     }, w.f.consumes = (e, r) => {
         w.o(g, e) && g[e].forEach((e => {
             if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/third-party-licenses.json` & `jupyterlab_nbgallery-2.0.3/labextension/userpreferences/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/package.json` & `jupyterlab_nbgallery-2.0.3/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.2/setup.py` & `jupyterlab_nbgallery-2.0.3/setup.py`

 * *Files identical despite different names*

