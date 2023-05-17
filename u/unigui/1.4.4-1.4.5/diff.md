# Comparing `tmp/unigui-1.4.4.tar.gz` & `tmp/unigui-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.4.4.tar", last modified: Thu May 11 15:37:46 2023, max compression
+gzip compressed data, was "dist/unigui-1.4.5.tar", last modified: Wed May 17 15:18:47 2023, max compression
```

## Comparing `unigui-1.4.4.tar` & `unigui-1.4.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui/
--rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.4/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     7831 2023-05-11 09:43:13.000000 unigui-1.4.4/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.4/unigui/userset.py
--rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.4/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.4/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.4/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/css/603.d94da9c0.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/css/vendor.49a52e8f.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)   847622 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/js/vendor.c0de6c67.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/js/193.b4cc3ffe.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/js/430.4be6e8a8.js
--rw-rw-r--   0 george    (1000) george    (1000)    40010 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/js/603.baf52338.js
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/js/app.a12bb431.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-11 15:24:52.000000 unigui-1.4.4/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.4/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      585 2023-05-11 15:37:06.000000 unigui-1.4.4/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19428 2023-05-11 15:37:46.000000 unigui-1.4.4/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-11 15:37:46.000000 unigui-1.4.4/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    19138 2023-05-08 23:39:42.000000 unigui-1.4.4/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.4/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19428 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.4/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1223 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-11 15:37:46.000000 unigui-1.4.4/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-17 15:18:47.000000 unigui-1.4.5/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-17 15:18:47.000000 unigui-1.4.5/unigui/
+-rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.5/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7900 2023-05-16 12:54:09.000000 unigui-1.4.5/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.5/unigui/userset.py
+-rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.5/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.5/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.5/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-17 15:18:47.000000 unigui-1.4.5/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-17 15:18:47.000000 unigui-1.4.5/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/css/22.f5c7cbc7.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/css/vendor.49a52e8f.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-17 15:18:47.000000 unigui-1.4.5/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-17 15:18:47.000000 unigui-1.4.5/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-17 15:18:47.000000 unigui-1.4.5/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5862 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/js/app.c8cc6f16.js
+-rw-rw-r--   0 george    (1000) george    (1000)    42532 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/js/22.b5025a55.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/js/vendor.3e8714c2.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-17 14:48:00.000000 unigui-1.4.5/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.5/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      585 2023-05-17 15:18:39.000000 unigui-1.4.5/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19455 2023-05-17 15:18:47.000000 unigui-1.4.5/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-17 15:18:47.000000 unigui-1.4.5/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    19165 2023-05-17 15:17:52.000000 unigui-1.4.5/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.5/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-17 15:18:47.000000 unigui-1.4.5/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-05-17 15:18:47.000000 unigui-1.4.5/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-17 15:18:47.000000 unigui-1.4.5/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19455 2023-05-17 15:18:47.000000 unigui-1.4.5/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.5/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1221 2023-05-17 15:18:47.000000 unigui-1.4.5/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-17 15:18:47.000000 unigui-1.4.5/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.4.4/unigui/manager.py` & `unigui-1.4.5/unigui/manager.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/guielements.py` & `unigui-1.4.5/unigui/guielements.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,16 @@
                 del t.rows[value]  
             t.value = None    
 
 class Table(Gui):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)             
         self.check('rows', 'headers','value')
+        if not hasattr(self,'type'):
+            self.type = 'table'
         if not hasattr(self,'edit') or self.edit:
             if not hasattr(self,'modify'):
                 self.modify = accept_cell_value 
             if not hasattr(self,'delete'):
                 self.delete = standart_table_delete 
         if not hasattr(self,'rows'):
             self.rows = []
```

### Comparing `unigui-1.4.4/unigui/server.py` & `unigui-1.4.5/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/utils.py` & `unigui-1.4.5/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/favicon.ico` & `unigui-1.4.5/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/css/603.d94da9c0.css` & `unigui-1.4.5/unigui/web/css/22.f5c7cbc7.css`

 * *Files 16% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-9805fac6]{display:flex;justify-content:center}.custom-caption[data-v-9805fac6]{padding:5px!important}.web-camera-container[data-v-9805fac6]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-9805fac6]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-9805fac6]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-9805fac6]{opacity:1}.web-camera-container .camera-shoot[data-v-9805fac6]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-9805fac6]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-9805fac6]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-9805fac6]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-9805fac6]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-9805fac6]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-9805fac6]{animation:preload-9805fac6 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-9805fac6]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-9805fac6]:nth-child(3){animation-delay:.4s}@keyframes preload-9805fac6{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-9805fac6]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-6d149d62]{display:flex;justify-content:center}.custom-caption[data-v-6d149d62]{padding:5px!important}.web-camera-container[data-v-6d149d62]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-6d149d62]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-6d149d62]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-6d149d62]{opacity:1}.web-camera-container .camera-shoot[data-v-6d149d62]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-6d149d62]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-6d149d62]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-6d149d62]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-6d149d62]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-6d149d62]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-6d149d62]{animation:preload-6d149d62 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-6d149d62]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-6d149d62]:nth-child(3){animation-delay:.4s}@keyframes preload-6d149d62{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-6d149d62]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
```

### Comparing `unigui-1.4.4/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.4.5/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/icons/favicon-96x96.png` & `unigui-1.4.5/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/icons/favicon-16x16.png` & `unigui-1.4.5/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/icons/favicon-32x32.png` & `unigui-1.4.5/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/icons/favicon-128x128.png` & `unigui-1.4.5/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.4.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.4.5/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.4.5/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.4.5/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.4.5/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.4.5/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.4.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.4.5/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/js/193.b4cc3ffe.js` & `unigui-1.4.5/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/js/430.4be6e8a8.js` & `unigui-1.4.5/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/unigui/web/js/603.baf52338.js` & `unigui-1.4.5/unigui/web/js/22.b5025a55.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [603], {
-        7603: (e, t, a) => {
+    [22], {
+        22: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => Qt
+                default: () => Gt
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
                 class: "q-pa-lg"
             }, null, -1);
 
@@ -16,16 +16,16 @@
                     c = (0, l.up)("q-tab"),
                     h = (0, l.up)("q-tabs"),
                     u = (0, l.up)("q-toolbar"),
                     p = (0, l.up)("q-header"),
                     g = (0, l.up)("zone"),
                     m = (0, l.up)("q-page"),
                     f = (0, l.up)("q-page-container"),
-                    w = (0, l.up)("q-layout");
-                return (0, l.wg)(), (0, l.j4)(w, {
+                    y = (0, l.up)("q-layout");
+                return (0, l.wg)(), (0, l.j4)(y, {
                     view: "lHh Lpr lFf"
                 }, {
                     default: (0, l.w5)((() => [(0, l.Wm)(p, {
                         elevated: ""
                     }, {
                         default: (0, l.w5)((() => [(0, l.Wm)(u, null, {
                             default: (0, l.w5)((() => [(0, l.Wm)(r, {
@@ -97,146 +97,145 @@
                         })])),
                         _: 1
                     })])),
                     _: 1
                 }, 8, ["onClick"])
             }
             var d, r = a(698),
-                c = a(8603),
-                h = a.n(c);
-            let u = null,
-                p = {},
-                g = !0;
-            const m = 136,
-                f = 400,
-                w = `height: ${m}px; width: ${f}px`;
+                c = a(8603);
+            let h = null,
+                u = {},
+                p = !0;
+            const g = 136,
+                m = 400,
+                f = `height: ${g}px; width: ${m}px`;
 
             function y(e) {
-                let t = e.minheight ? e.minheight : m,
-                    a = e.minwidth ? e.minwidth : f;
+                let t = e.minheight ? e.minheight : g,
+                    a = e.minwidth ? e.minwidth : m;
                 return `height: ${t}px; width: ${a}px`
             }
-            const b = {},
-                k = {},
-                v = ["error", "progress", "warning", "info"];
+            const w = {},
+                b = {},
+                k = ["error", "progress", "warning", "info"];
 
-            function C(e) {
+            function v(e) {
                 d = new WebSocket("ws://localhost:8000/ws"), d.onopen = () => e.statusConnect = !0, d.onmessage = t => {
-                    g && console.log("socket message", t.data), e.processMessage(JSON.parse(t.data))
+                    p && console.log("socket message", t.data), e.processMessage(JSON.parse(t.data))
                 }, d.onerror = t => e.error(t), d.onclose = t => {
-                    t.wasClean ? e.info("Connection closed and was clean.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, g && console.info("close code : " + t.code + " reason: " + t.reason)
-                }, u = e
+                    t.wasClean ? e.info("Connection closed and was clean.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, p && console.info("close code : " + t.code + " reason: " + t.reason)
+                }, h = e
             }
 
-            function q(e) {
+            function C(e) {
                 console.log("sended", e), d.send(JSON.stringify(e))
             }
-            let _, j = 0;
+            let q, S = 0;
 
-            function S(e) {
+            function j(e) {
                 for (var t in e) e.hasOwnProperty(t) && delete e[t]
             }
 
             function A(e, t, a, l = "?") {
-                let s = ++j,
+                let s = ++S,
                     i = [e.pdata.name, e.data.name, l, t, s];
-                q(i), p[s] = a
+                C(i), u[s] = a
             }
 
-            function Z() {
-                S(b), S(k)
+            function z() {
+                j(w), j(b)
             }
 
-            function M(e, t) {
+            function Z(e, t) {
                 Object.assign(e.data, t), e.updated = t.value, e.value = t.value
             }
 
-            function $(e) {
+            function M(e) {
                 if (e.multi)
                     for (let [t, a] of e.update.entries())
                         if (a.length > 1) {
                             a.reverse();
                             let l = a.join("@"),
-                                s = k[l];
-                            M(s, e.data[t])
+                                s = b[l];
+                            Z(s, e.data[t])
                         } else {
-                            let l = b[a[0]];
+                            let l = w[a[0]];
                             Object.assign(l.data, e.data[t])
                         }
                 else {
                     let t, a = e.update;
                     if (a.length > 1) {
                         a.reverse();
                         let e = a.join("@");
-                        t = k[e]
-                    } else t = b[a[0]];
-                    M(t, e.data), 1 == a.length && h().delay(W, 200, t)
+                        t = b[e]
+                    } else t = w[a[0]];
+                    Z(t, e.data), 1 == a.length && (0, c.delay)(Q, 200, t)
                 }
             }
 
-            function z(e) {
-                typeof e.answer == String ? u.showError() : p[e.id](e.answer), delete p[e.id]
+            function $(e) {
+                typeof e.answer == String ? h.showError() : u[e.id](e.answer), delete u[e.id]
             }
 
             function D(e) {
                 let t = [];
                 for (let l of e) l instanceof Array ? t.push(l) : t.push([l]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
-            function O() {
-                for (let [e, t] of Object.entries(k)) t.expanding && (t.styleSize = y(t.data));
+            function V() {
+                for (let [e, t] of Object.entries(b)) t.expanding && (t.styleSize = y(t.data));
                 (0, l.Y3)((() => {
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
-                            W()
+                            Q()
                         }))
                     }))
                 }))
             }
-            let Q = h().debounce(O, 200);
+            let O = _.debounce(V, 200);
 
-            function W(e) {
-                Array.isArray(e) && (e = null), _ && (_.disconnect(), _ = null), g && console.log("------------------recalc design");
-                const t = V(e),
-                    a = E(e);
+            function Q(e) {
+                Array.isArray(e) && (e = null), q && (q.disconnect(), q = null), p && console.log("------------------recalc design");
+                const t = W(e),
+                    a = H(e);
                 for (let [l, s] of Object.entries(t)) {
-                    let e = k[l];
+                    let e = b[l];
                     const [t, i] = a[l];
                     let o, n = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
-                        r = b[d];
+                        r = w[d];
                     for (let a of r.data.childs)
                         if (Array.isArray(a)) {
                             if (a.find((t => t.name == e.data.name))) {
                                 let e = a[a.length - 1],
                                     t = `${e.name}@${d}`;
-                                o = k[t];
+                                o = b[t];
                                 break
                             }
                         } else if (a.name == e.data.name) {
                         o = e;
                         break
                     }
                     let c = r.data.width ? r.data.width - n.clientWidth - t : r.$el.getBoundingClientRect().right - (o ? o.geom().right : e.geom().right);
                     c /= i;
                     let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : n.clientHeight;
                     e.styleSize = `height: ${h+s}px; width: ${n.clientWidth+c+t}px;`
                 }
             }
 
-            function V(e) {
-                const t = u.screen.blocks;
+            function W(e) {
+                const t = h.screen.blocks;
                 let a = window.innerHeight;
                 a -= 2;
                 let l = {},
                     s = new Map,
                     i = {};
-                for (let [d, r] of Object.entries(b)) i[r.name] = r.$el.getBoundingClientRect().height;
+                for (let [d, r] of Object.entries(w)) i[r.name] = r.$el.getBoundingClientRect().height;
                 let o = [];
                 for (let d of t) {
                     const e = [];
                     let t = d instanceof Array,
                         n = t ? D(d) : [
                             [d]
                         ];
@@ -246,15 +245,15 @@
                         o.push([e, a])
                     }
                     o.sort(((e, t) => e[0] > t[0] ? -1 : e[0] == t[0] ? 0 : 1));
                     for (let l of o) {
                         let t = l[1];
                         (0, r.hu)(Array.isArray(t));
                         const i = [];
-                        for (let [e, a] of Object.entries(k))
+                        for (let [e, a] of Object.entries(b))
                             if (a.expanding_height) {
                                 let [l, o] = e.split("@");
                                 if (t.find((e => e.name == o))) {
                                     let e = !0;
                                     const t = a.geom();
                                     for (let [l, o] of i.entries()) {
                                         let n = o.geom();
@@ -287,17 +286,17 @@
                 }
                 let n = Array.from(s.entries());
                 n.sort(((e, t) => e[0] in l || e[1] in l ? -1 : 1));
                 for (let [d, r] of n) r in l ? l[d] = l[r] : l[r] = l[d];
                 return l
             }
 
-            function E(e) {
+            function H(e) {
                 e = null;
-                const t = e ? [e] : u.screen.blocks;
+                const t = e ? [e] : h.screen.blocks;
                 let a = window.innerWidth - 30,
                     l = [],
                     s = {};
                 for (let n of t)
                     if (0 == l.length)
                         if (Array.isArray(n))
                             for (let e of n) l.push(Array.isArray(e) ? e : [e]);
@@ -314,20 +313,20 @@
                     l = e
                 }
                 l.sort(((e, t) => e.length > t.length ? -1 : e.length == t.length ? 0 : 1));
                 const i = [];
                 let o = new Map;
                 for (let n of l) {
                     let e = Array.isArray(n) ? n[n.length - 1] : n,
-                        t = b[e.name].$el.getBoundingClientRect().right;
+                        t = w[e.name].$el.getBoundingClientRect().right;
                     e = Array.isArray(n) ? n[0] : n;
-                    let l = b[e.name].$el.getBoundingClientRect().left,
+                    let l = w[e.name].$el.getBoundingClientRect().left,
                         s = a - t + l - 10;
                     const d = [];
-                    for (let [a, i] of Object.entries(k))
+                    for (let [a, i] of Object.entries(b))
                         if (i.expanding_width) {
                             let e = a.split("@")[1];
                             if (n.find((t => t.name == e))) {
                                 let e = !0,
                                     t = i.geom().left;
                                 for (let [a, l] of d.entries())
                                     if (l !== i && l.geom().left == t) {
@@ -354,75 +353,75 @@
                             s[a.fullname] = [Math.floor(n / e), t[l]]
                         }
                     }
                 }
                 for (let [n, d] of o.entries()) d in s ? s[n] = s[d] : s[d] = s[n];
                 return s
             }
-            const H = (0, l.aZ)({
+            const E = (0, l.aZ)({
                 name: "menubar",
                 methods: {
                     send() {
-                        q(["root", this.name])
+                        C(["root", this.name])
                     }
                 },
                 props: {
                     name: {
                         type: String,
                         required: !0
                     },
                     icon: {
                         type: String,
                         default: ""
                     }
                 }
             });
-            var U = a(4260),
-                K = a(3414),
+            var N = a(4260),
+                U = a(3414),
                 P = a(2035),
-                T = a(4554),
-                N = a(2350),
-                I = a(7518),
-                R = a.n(I);
-            const L = (0, U.Z)(H, [
+                F = a(4554),
+                K = a(2350),
+                T = a(7518),
+                I = a.n(T);
+            const R = (0, N.Z)(E, [
                     ["render", n]
                 ]),
-                B = L;
-            R()(H, "components", {
-                QItem: K.Z,
+                B = R;
+            I()(E, "components", {
+                QItem: U.Z,
                 QItemSection: P.Z,
-                QIcon: T.Z,
-                QItemLabel: N.Z
+                QIcon: F.Z,
+                QItemLabel: K.Z
             });
-            const F = {
+            const L = {
                     key: 0,
                     class: "row q-col-gutter-sm q-py-sm"
                 },
                 Y = {
-                    class: "q-col-gutter-sm q-py-sm"
+                    class: "q-col-gutter-sm"
                 },
                 X = {
                     key: 0,
-                    class: "column q-col-gutter-sm q-py-sm"
+                    class: "column q-col-gutter-sm"
                 };
 
-            function J(e, t, a, s, i, o) {
+            function G(e, t, a, s, i, o) {
                 const n = (0, l.up)("zone", !0),
                     d = (0, l.up)("block");
-                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", F, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", Y, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", X, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(n, {
+                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", L, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", Y, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", X, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(n, {
                     data: e
                 }, null, 8, ["data"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e
                 }, null, 8, ["data"]))])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e.data
                 }, null, 8, ["data"]))
             }
-            const G = {
+            const J = {
                     class: "row"
                 },
                 ee = {
                     key: 2,
                     class: "q-ma-sm",
                     style: {
                         "font-size": "18px"
@@ -443,15 +442,15 @@
                 const d = (0, l.up)("element"),
                     r = (0, l.up)("q-icon"),
                     c = (0, l.up)("q-scroll-area"),
                     h = (0, l.up)("q-card");
                 return (0, l.wg)(), (0, l.j4)(h, {
                     class: "my-card q-ma-xs"
                 }, {
-                    default: (0, l.w5)((() => [(0, l._)("div", G, [e.data.logo ? ((0, l.wg)(), (0, l.j4)(d, {
+                    default: (0, l.w5)((() => [(0, l._)("div", J, [e.data.logo ? ((0, l.wg)(), (0, l.j4)(d, {
                         key: 0,
                         data: e.data.logo,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])) : e.data.icon ? ((0, l.wg)(), (0, l.j4)(r, {
                         key: 1,
                         size: "sm",
                         name: e.data.icon
@@ -496,19 +495,19 @@
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"]))], 8, le)))), 256))])),
                     _: 1
                 })
             }
             var oe = a(8880);
-            const ne = e => ((0, l.dD)("data-v-9805fac6"), e = e(), (0, l.Cn)(), e),
+            const ne = e => ((0, l.dD)("data-v-6d149d62"), e = e(), (0, l.Cn)(), e),
                 de = ["width", "height"],
                 re = ["src"],
                 ce = {
-                    key: 15,
+                    key: 16,
                     class: "web-camera-container"
                 },
                 he = {
                     class: "camera-button"
                 },
                 ue = {
                     key: 0
@@ -519,16 +518,16 @@
                 ge = {
                     class: "camera-loading"
                 },
                 me = ne((() => (0, l._)("ul", {
                     class: "loader-circle"
                 }, [(0, l._)("li"), (0, l._)("li"), (0, l._)("li")], -1))),
                 fe = [me],
-                we = ["height"],
                 ye = ["height"],
+                we = ["height"],
                 be = {
                     key: 1,
                     class: "camera-shoot"
                 },
                 ke = ne((() => (0, l._)("img", {
                     src: "https://img.icons8.com/material-outlined/50/000000/camera--v2.png"
                 }, null, -1))),
@@ -543,21 +542,22 @@
                     r = (0, l.up)("q-img"),
                     c = (0, l.up)("q-badge"),
                     h = (0, l.up)("q-select"),
                     u = (0, l.up)("q-checkbox"),
                     p = (0, l.up)("q-toggle"),
                     g = (0, l.up)("q-btn-toggle"),
                     m = (0, l.up)("utable"),
-                    f = (0, l.up)("q-input"),
+                    f = (0, l.up)("linechart"),
+                    y = (0, l.up)("q-input"),
                     w = (0, l.up)("q-tree"),
-                    y = (0, l.up)("q-scroll-area"),
-                    b = (0, l.up)("q-separator"),
-                    k = (0, l.up)("q-uploader"),
-                    v = (0, l.up)("cgraph"),
-                    x = (0, l.up)("q-btn");
+                    b = (0, l.up)("q-scroll-area"),
+                    k = (0, l.up)("q-separator"),
+                    v = (0, l.up)("q-uploader"),
+                    x = (0, l.up)("cgraph"),
+                    C = (0, l.up)("q-btn");
                 return "image" == e.type ? ((0, l.wg)(), (0, l.j4)(r, {
                     key: 0,
                     src: e.data.name,
                     "spinner-color": "blue",
                     onClick: (0, oe.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
                     style: (0, s.j5)(e.elemSize)
@@ -634,42 +634,47 @@
                     })) : (0, l.kq)("", !0)])),
                     _: 1
                 }, 8, ["modelValue", "options"])) : "table" == e.type ? ((0, l.wg)(), (0, l.j4)(m, {
                     key: 5,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.styleSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "edit" == e.type ? ((0, l.wg)(), (0, l.j4)(f, {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "linechart" == e.type ? ((0, l.wg)(), (0, l.j4)(f, {
                     key: 6,
+                    data: e.data,
+                    pdata: e.pdata,
+                    styleSize: e.styleSize
+                }, null, 8, ["data", "pdata", "styleSize"])) : "edit" == e.type ? ((0, l.wg)(), (0, l.j4)(y, {
+                    key: 7,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[5] || (t[5] = t => e.value = t),
                     label: e.name,
                     ref: "inputRef",
                     autogrow: e.data.autogrow,
                     dense: "",
                     onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"]),
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "autoedit" == e.type ? ((0, l.wg)(), (0, l.j4)(h, {
-                    key: 7,
+                    key: 8,
                     dense: "",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[6] || (t[6] = t => e.value = t),
                     "use-input": "",
                     "hide-selected": "",
                     borderless: "",
                     outlined: "",
                     "hide-bottom-space": "",
                     "fill-input": "",
                     "input-debounce": "0",
                     options: e.options,
                     onFilter: e.complete,
                     label: e.name,
                     onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"])
-                }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, l.wg)(), (0, l.j4)(y, {
-                    key: 8,
+                }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, l.wg)(), (0, l.j4)(b, {
+                    key: 9,
                     style: (0, s.j5)(e.styleSize),
                     "thumb-style": e.thumbStyle,
                     "bar-style": e.barStyle
                 }, {
                     default: (0, l.w5)((() => [(0, l.Wm)(w, {
                         nodes: e.treeNodes,
                         selected: e.value,
@@ -678,56 +683,56 @@
                         "onUpdate:expanded": t[8] || (t[8] = t => e.expandedKeys = t),
                         "node-key": "label",
                         "default-expand-all": "",
                         "selected-color": "blue-10"
                     }, null, 8, ["nodes", "selected", "expanded"])])),
                     _: 1
                 }, 8, ["style", "thumb-style", "bar-style"])) : "docviewer" == e.type ? (0, l.wy)(((0, l.wg)(), (0, l.iD)("textarea", {
-                    key: 9,
+                    key: 10,
                     class: "textarea",
                     "onUpdate:modelValue": t[9] || (t[9] = t => e.value = t),
                     filled: "",
                     type: "textarea",
                     style: (0, s.j5)(e.elemSize)
                 }, null, 4)), [
                     [oe.nr, e.value]
-                ]) : "line" == e.type ? ((0, l.wg)(), (0, l.j4)(b, {
-                    key: 10,
+                ]) : "line" == e.type ? ((0, l.wg)(), (0, l.j4)(k, {
+                    key: 11,
                     color: "green"
                 })) : "video" == e.type ? ((0, l.wg)(), (0, l.iD)("video", {
                     width: e.data.width,
                     height: e.data.height,
                     key: e.data.src,
                     controls: ""
                 }, [(0, l._)("source", {
                     src: e.data.src,
                     type: "video/mp4"
-                }, null, 8, re)], 8, de)) : "gallery" == e.type ? ((0, l.wg)(), (0, l.j4)(k, {
-                    key: 12,
+                }, null, 8, re)], 8, de)) : "gallery" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
+                    key: 13,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: "http://localhost:8000",
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
                     style: (0, s.j5)(e.elemSize),
                     ref: "uploaderRef",
                     flat: ""
-                }, null, 8, ["label", "onUploaded", "onAdded", "style"])) : "gimages" == e.type ? ((0, l.wg)(), (0, l.j4)(k, {
-                    key: 13,
+                }, null, 8, ["label", "onUploaded", "onAdded", "style"])) : "gimages" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
+                    key: 14,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: "http://localhost:8000",
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
                     ref: "uploaderRef",
                     flat: ""
-                }, null, 8, ["label", "onUploaded", "onAdded"])) : "graph" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
-                    key: 14,
+                }, null, 8, ["label", "onUploaded", "onAdded"])) : "graph" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
+                    key: 15,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.elemSize
                 }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", ce, [(0, l._)("div", he, [(0, l._)("button", {
                     class: (0, s.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
@@ -746,66 +751,66 @@
                         flash: e.isShotPhoto
                     }])
                 }, null, 2), (0, l.wy)((0, l._)("video", {
                     ref: "camera",
                     width: 450,
                     height: 337.5,
                     autoplay: ""
-                }, null, 8, we), [
+                }, null, 8, ye), [
                     [oe.F8, !e.isPhotoTaken]
                 ]), (0, l.wy)((0, l._)("canvas", {
                     id: "photoTaken",
                     ref: "canvas",
                     width: 450,
                     height: 337.5
-                }, null, 8, ye), [
+                }, null, 8, we), [
                     [oe.F8, e.isPhotoTaken]
                 ])], 2)), [
                     [oe.F8, !e.isLoading]
                 ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", be, [(0, l._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, ve)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", xe, [(0, l.Wm)(x, {
+                }, ve)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", xe, [(0, l.Wm)(C, {
                     onClick: e.downloadImage,
                     label: "Send"
-                }, null, 8, ["onClick"])])) : (0, l.kq)("", !0)])) : "" != e.showname ? ((0, l.wg)(), (0, l.j4)(x, {
-                    key: 16,
+                }, null, 8, ["onClick"])])) : (0, l.kq)("", !0)])) : "" != e.showname ? ((0, l.wg)(), (0, l.j4)(C, {
+                    key: 17,
                     "no-caps": "",
                     label: e.name,
                     icon: e.data.icon,
                     onClick: e.sendValue
-                }, null, 8, ["label", "icon", "onClick"])) : ((0, l.wg)(), (0, l.j4)(x, {
-                    key: 17,
+                }, null, 8, ["label", "icon", "onClick"])) : ((0, l.wg)(), (0, l.j4)(C, {
+                    key: 18,
                     "no-caps": "",
                     dense: "",
                     icon: e.data.icon,
                     onClick: e.sendValue
                 }, null, 8, ["icon", "onClick"]))
             }
             const qe = {
                     key: 0
                 },
                 _e = {
                     class: "row"
                 },
-                je = ["onClick"];
+                Se = ["onClick"];
 
-            function Se(e, t, a, i, o, n) {
+            function je(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-input"),
                     c = (0, l.up)("q-tooltip"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-th"),
                     p = (0, l.up)("q-tr"),
                     g = (0, l.up)("q-checkbox"),
                     m = (0, l.up)("q-select"),
                     f = (0, l.up)("q-td"),
-                    w = (0, l.up)("q-table");
-                return (0, l.wg)(), (0, l.j4)(w, {
+                    y = (0, l.up)("q-table");
+                return (0, l.wg)(), (0, l.j4)(y, {
                     class: "my-sticky-virtscroll-table",
                     "virtual-scroll": "",
                     dense: "",
                     style: (0, s.j5)(e.styleSize),
                     flat: "",
                     filter: e.search,
                     ref: "table",
@@ -983,28 +988,28 @@
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, e.change],
                                 dense: "",
                                 onKeydown: e.keyInput,
                                 autofocus: ""
                             }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, l.wg)(), (0, l.iD)("div", {
                                 key: 3,
                                 onClick: a => e.select(t.row.iiid, i)
-                            }, (0, s.zw)(t.row[a.name]), 9, je))])),
+                            }, (0, s.zw)(t.row[a.name]), 9, Se))])),
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
                 }, 8, ["style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
             var Ae = a(1959);
 
-            function Ze(e, t) {
+            function ze(e, t) {
                 return e.length === t.length && e.every(((e, a) => e.iiid == t[a].iiid))
             }
-            const Me = (0, l.aZ)({
+            const Ze = (0, l.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
                     } = (0, Ae.BK)(e);
                     let s = (0, l.Fl)((() => {
@@ -1028,22 +1033,22 @@
                             return a
                         },
                         o = i(),
                         n = (0, Ae.iH)(o),
                         d = (0, Ae.iH)(o),
                         r = (0, Ae.iH)(!Array.isArray(t.value.value)),
                         c = (e, l) => {
-                            q([a.value.name, t.value.name, e, l])
+                            C([a.value.name, t.value.name, e, l])
                         },
                         h = (0, l.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
                         u = (0, l.Fl)((() => t.value.value));
                     return (0, l.YP)(s, ((e, t) => {
                         d.value = i(), n.value = d.value
                     })), (0, l.YP)(t, ((e, a) => {
-                        g && console.log("data update", a.name), d.value = i(), n.value = d.value, r.value = !Array.isArray(t.value.value)
+                        p && console.log("data update", a.name), d.value = i(), n.value = d.value, r.value = !Array.isArray(t.value.value)
                     })), {
                         rows: s,
                         value: h,
                         selected: d,
                         singleMode: r,
                         sendMessage: c,
                         datavalue: u,
@@ -1056,35 +1061,35 @@
                         editMode: !1,
                         options: [],
                         cedit: null
                     }
                 },
                 methods: {
                     select(e, t) {
-                        this.editMode && (this.cedit = t, g && console.log("selected", e, this.cedit))
+                        this.editMode && (this.cedit = t, p && console.log("selected", e, this.cedit))
                     },
                     change_switcher(e, t, a) {
                         if (console.log(e, t, a, e[t]), this.editMode) {
                             this.cedit = a;
                             const l = e.iiid;
                             let s = this.data.rows;
                             s[l][a] = e[t], this.sendMessage("#", [e[t],
                                 [l, a]
                             ])
                         }
                     },
                     change(e) {
-                        if (g && console.log("changed", this.data.headers[this.cedit], e), this.editMode && this.selected.length) {
+                        if (p && console.log("changed", this.data.headers[this.cedit], e), this.editMode && this.selected.length) {
                             const t = this.selected[0].iiid;
                             let a = this.rows;
                             a[t][this.data.headers[this.cedit]] = e, this.sendMessage("#", [e, [t, this.cedit]])
                         }
                     },
                     keyInput(e) {
-                        if ("Control" != e.key) switch (g && console.log("keypress", e), e.key) {
+                        if ("Control" != e.key) switch (p && console.log("keypress", e), e.key) {
                             case "Enter":
                                 "update" in this.data && this.sendMessage("->", [this.rows[this.redit][this.data.headers[this.cedit]],
                                     [this.redit, this.cedit]
                                 ]);
                                 break;
                             case "Escape":
                                 this.switchEdit();
@@ -1131,16 +1136,16 @@
                         }))))
                     },
                     append() {
                         let e = this.data.rows,
                             t = e.length,
                             a = this;
                         A(this, [t, this.search], (function(l) {
-                            if (!Array.isArray(l)) return u.error(l);
-                            g && console.log("added row", l), a.search = "", e.push(l), setTimeout((() => {
+                            if (!Array.isArray(l)) return h.error(l);
+                            p && console.log("added row", l), a.search = "", e.push(l), setTimeout((() => {
                                 let e = a.rows;
                                 a.select(e[t], 0), a.showSelected()
                             }), 100)
                         }), "+")
                     },
                     showSelected() {
                         let e = this.$refs.table;
@@ -1148,36 +1153,39 @@
                             let t = e.computedRows.findIndex((e => e.iiid === this.selected[0].iiid));
                             e.scrollTo(t)
                         }
                     },
                     deselectAll() {
                         this.selected = [], this.sendMessage("=", this.value)
                     },
-                    chart() {},
+                    chart() {
+                        let e = this.data;
+                        e.type = "linechart"
+                    },
                     switchMode() {
                         this.singleMode = !this.singleMode, this.singleMode && this.selected.length > 1 && this.selected.splice(1)
                     },
                     switchEdit() {
                         this.editMode = !this.editMode, this.sendMessage("!", this.editMode), this.editMode && !this.singleMode && this.switchMode()
                     },
                     delSelected() {
-                        if (!this.selected.length) return void u.error("Rows are not selected!");
+                        if (!this.selected.length) return void h.error("Rows are not selected!");
                         this.sendMessage("-", this.value);
                         let e = this.data.rows;
                         if (this.singleMode) e.splice(this.selected[0].iiid, 1);
                         else {
                             this.selected.length > 1 && this.selected.sort(((e, t) => t.iiid - e.iiid));
                             for (let t of this.selected) e.splice(t.iiid, 1)
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
-                        Ze(this.updated, this.selected) || (this.sendMessage("=", this.value), this.updated = this.selected), this.data.show && this.showSelected()
+                        ze(this.updated, this.selected) || (this.sendMessage("=", this.value), this.updated = this.selected), this.data.show && this.showSelected()
                     }
                 },
                 computed: {
                     redit() {
                         return console.log("redit", this.editMode && this.selected.length ? this.selected[0].iiid : null), this.editMode && this.selected.length ? this.selected[0].iiid : null
                     },
                     editable() {
@@ -1198,52 +1206,52 @@
                 },
                 props: {
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
-            var $e = a(9267),
-                ze = a(4842),
+            var Me = a(9267),
+                $e = a(4842),
                 De = a(2165),
-                Oe = a(8870),
-                Qe = a(8186),
-                We = a(2414),
-                Ve = a(3884),
-                Ee = a(5735),
-                He = a(7208);
-            const Ue = (0, U.Z)(Me, [
-                    ["render", Se]
+                Ve = a(8870),
+                Oe = a(8186),
+                Qe = a(2414),
+                We = a(3884),
+                He = a(5735),
+                Ee = a(7208);
+            const Ne = (0, N.Z)(Ze, [
+                    ["render", je]
                 ]),
-                Ke = Ue;
-            R()(Me, "components", {
-                QTable: $e.Z,
-                QInput: ze.Z,
-                QIcon: T.Z,
+                Ue = Ne;
+            I()(Ze, "components", {
+                QTable: Me.Z,
+                QInput: $e.Z,
+                QIcon: F.Z,
                 QBtn: De.Z,
-                QTooltip: Oe.Z,
-                QTr: Qe.Z,
-                QTh: We.Z,
-                QTd: Ve.Z,
-                QCheckbox: Ee.Z,
-                QSelect: He.Z
+                QTooltip: Ve.Z,
+                QTr: Oe.Z,
+                QTh: Qe.Z,
+                QTd: We.Z,
+                QCheckbox: He.Z,
+                QSelect: Ee.Z
             });
             const Pe = ["nodes", "edges"];
 
-            function Te(e, t, a, i, o, n) {
+            function Fe(e, t, a, i, o, n) {
                 return (0, l.wg)(), (0, l.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, s.j5)(e.styleSize),
                     ref: "cy"
                 }, null, 12, Pe)
             }
-            var Ne = a(2393),
-                Ie = a.n(Ne);
-            const Re = Ie().stylesheet().selector("node").css({
+            var Ke = a(2393),
+                Te = a.n(Ke);
+            const Ie = Te().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
                     "border-color": "#ff5555"
                 }).selector("node[label]").css({
                     label: "data(label)",
@@ -1262,45 +1270,45 @@
                 }).selector("edge[label]").css({
                     label: "data(label)",
                     "text-rotation": "autorotate",
                     "text-margin-x": "-8px",
                     "text-margin-y": "-8px",
                     color: "gray"
                 }),
-                Le = {
+                Re = {
                     animate: !0,
                     randomize: !0
                 };
 
             function Be(e, t) {
                 if (e.length != t.length) return !0;
                 for (let a = 0; a < e.length; a++)
                     if (e[a].id != t[a].id) return !0;
                 return !1
             }
-            const Fe = (0, l.aZ)({
+            const Le = (0, l.aZ)({
                     name: "cgraph",
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
                         return {
                             cy: null,
-                            style: Re,
-                            layoutOptions: Le,
+                            style: Ie,
+                            layoutOptions: Re,
                             selectedNodes: [],
                             selectedEdges: [],
                             oldNodes: [],
                             oldEdges: []
                         }
                     },
                     mounted() {
-                        let e = Ie()({
+                        let e = Te()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1348,15 +1356,15 @@
                         },
                         value() {
                             return this.data.value
                         }
                     },
                     methods: {
                         sendMessage(e, t) {
-                            q([this.pdata["name"], this.data["name"], e, t])
+                            C([this.pdata["name"], this.data["name"], e, t])
                         },
                         showClusterNode(e) {
                             const t = e.data("cluster"),
                                 a = this.cy.nodes(`[cluster='${t}']`),
                                 l = this.cy.nodes(`#${t}`);
                             l.data("isClusterNode", !0), l.animate({
                                 position: {
@@ -1440,49 +1448,185 @@
                             this.cy.style(e)
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
-                Ye = (0, U.Z)(Fe, [
-                    ["render", Te]
+                Ye = (0, N.Z)(Le, [
+                    ["render", Fe]
                 ]),
                 Xe = Ye;
 
-            function Je(e) {
+            function Ge(e, t, a, i, o, n) {
+                const d = (0, l.up)("v-chart");
+                return (0, l.wg)(), (0, l.j4)(d, {
+                    ref: "chart",
+                    option: o.options,
+                    style: (0, s.j5)(a.styleSize),
+                    autoresize: !0,
+                    onClick: n.clicked
+                }, null, 8, ["option", "style", "onClick"])
+            }
+            var Je = a(5512),
+                et = a(4447),
+                tt = a(1006),
+                at = a(3526),
+                lt = a(763),
+                st = a(546),
+                it = a(6902),
+                ot = a(2826),
+                nt = a(5256),
+                dt = a(3825),
+                rt = a(8825);
+            (0, lt.D)([et.N, tt.N, at.N]), (0, lt.D)([st.N, it.N, ot.N, nt.N, dt.N]);
+            let ct = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"],
+                ht = {
+                    responsive: !0,
+                    maintainAspectRatio: !1,
+                    legend: {
+                        data: [],
+                        bottom: 10
+                    },
+                    tooltip: {
+                        trigger: "axis",
+                        position: function(e) {
+                            return [e[0], "10%"]
+                        }
+                    },
+                    title: {
+                        left: "center",
+                        text: ""
+                    },
+                    toolbox: {
+                        feature: {
+                            dataZoom: {
+                                yAxisIndex: "none"
+                            }
+                        }
+                    },
+                    xAxis: {
+                        type: "category",
+                        boundaryGap: !1,
+                        data: null
+                    },
+                    yAxis: {
+                        type: "value",
+                        boundaryGap: [0, "100%"]
+                    },
+                    dataZoom: [{
+                        type: "inside",
+                        start: 0,
+                        end: 10
+                    }, {
+                        start: 0,
+                        end: 10
+                    }],
+                    series: []
+                };
+            const ut = {
+                    name: "linechart",
+                    components: {
+                        VChart: Je.ZP
+                    },
+                    props: {
+                        data: Object,
+                        pdata: Object,
+                        styleSize: String
+                    },
+                    data() {
+                        const e = (0, rt.Z)();
+                        return {
+                            $q: e,
+                            model: !1,
+                            options: null
+                        }
+                    },
+                    methods: {
+                        clicked(e) {
+                            var t = [e.offsetX, e.offsetY],
+                                a = myChart.convertFromPixel("grid", t),
+                                l = myChart.getModel().get("xAxis")[0].data[a[0]];
+                            console.log(l)
+                        },
+                        calcSeries() {
+                            this.options.toolbox.feature.mySwitcher = {
+                                show: !0,
+                                title: "Switch view to the table",
+                                icon: "image:M0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2zm15 2h-4v3h4V4zm0 4h-4v3h4V8zm0 4h-4v3h3a1 1 0 0 0 1-1v-2zm-5 3v-3H6v3h4zm-5 0v-3H1v2a1 1 0 0 0 1 1h3zm-4-4h4V8H1v3zm0-4h4V4H1v3zm5-3v3h4V4H6zm4 4H6v3h4V8z",
+                                onclick: () => {
+                                    let e = this.data;
+                                    e.type = "table"
+                                }
+                            };
+                            let e = this.data.view,
+                                t = this.data.headers;
+                            "_" != this.data.name[0] && (this.options.title.text = this.data.name);
+                            let a = e.split("-"),
+                                l = a[1].split(",");
+                            l.unshift(a[0]);
+                            let s = [];
+                            for (let o = 0; o < l.length; o++) l[o] = "i" == l[o] ? -1 : parseInt(l[o]), s.push([]), o && (this.options.series.push({
+                                name: t[l[o]],
+                                type: "line",
+                                symbol: "none",
+                                sampling: "lttb",
+                                itemStyle: {
+                                    color: ct[o]
+                                },
+                                data: s[o]
+                            }), this.options.legend.data.push(t[l[o]]));
+                            this.options.xAxis.data = s[0];
+                            let i = this.data.rows;
+                            for (let o = 0; o < i.length; o++)
+                                for (let e = 0; e < l.length; e++) s[e].push(-1 == l[e] ? o : i[o][l[e]]);
+                            this.$refs.chart.setOption(this.options)
+                        }
+                    },
+                    mounted() {
+                        this.options = (0, c.cloneDeep)(ht), this.calcSeries(), this.$refs.chart.chart.on("click", this.clicked)
+                    },
+                    watch: {}
+                },
+                pt = (0, N.Z)(ut, [
+                    ["render", Ge]
+                ]),
+                gt = pt;
+
+            function mt(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", "http://localhost:8000", !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const Ge = (0, l.aZ)({
+            const ft = (0, l.aZ)({
                 name: "element",
                 components: {
-                    utable: Ke,
-                    cgraph: Xe
+                    utable: Ue,
+                    cgraph: Xe,
+                    linechart: gt
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
                     },
                     sendMessage(e, t) {
-                        q([this.pdata["name"], this.data["name"], e, t])
+                        C([this.pdata["name"], this.data["name"], e, t])
                     },
                     pressedEnter() {
                         "update" in this.data && this.sendMessage("->", this.value)
                     },
                     updateDom(e) {
                         let t = e.files.length;
-                        t && (this.sendMessage("=", e.files[t - 1].name), Q())
+                        t && (this.sendMessage("=", e.files[t - 1].name), O())
                     },
                     sendValue() {
                         this.sendMessage("=", this.value)
                     },
                     switchValue() {
                         this.value = !this.value
                     },
@@ -1491,15 +1635,15 @@
                     },
                     complete(e, t, a) {
                         this.value = e, A(this, e, (e => t((() => {
                             this.options = e
                         }))))
                     },
                     lens() {
-                        u.lens(this.data)
+                        h.lens(this.data)
                     },
                     toggleCamera() {
                         this.isCameraOpen ? (this.isCameraOpen = !1, this.isPhotoTaken = !1, this.isShotPhoto = !1, this.stopCameraStream()) : (this.isCameraOpen = !0, this.createCameraElement())
                     },
                     createCameraElement() {
                         this.isLoading = !0;
                         const e = window.constraints = {
@@ -1527,35 +1671,35 @@
                             }), e)
                         }
                         this.isPhotoTaken = !this.isPhotoTaken;
                         const e = this.$refs.canvas.getContext("2d");
                         e.drawImage(this.$refs.camera, 0, 0, 450, 337.5)
                     },
                     downloadImage() {
-                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(Je, "image/jpeg")
+                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(mt, "image/jpeg")
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         e || (e = this.$el.previousElementSibling, e = "clientHeight" in e ? e : e.nextElementSibling);
                         let t = this.type;
-                        const a = "docviewer" == t || "graph" == t ? e : e.querySelector("table" == t ? ".scroll" : ".q-tree"),
+                        const a = "docviewer" == t || "graph" == t || "linechart" == t ? e : e.querySelector("table" == t ? ".scroll" : ".q-tree"),
                             l = e.getBoundingClientRect();
                         return {
                             el: e,
                             inner: a,
                             left: l.left,
                             right: l.right,
                             top: l.top,
                             scrollHeight: a.scrollHeight,
                             scrollWidth: a.scrollWidth
                         }
                     }
                 },
                 mounted() {
-                    k[this.fullname] = this, g && console.log("mounted", this.fullname)
+                    b[this.fullname] = this, p && console.log("mounted", this.fullname)
                 },
                 data() {
                     return {
                         value: this.data.value,
                         styleSize: y(this.data),
                         options: [],
                         expandedKeys: [],
@@ -1600,15 +1744,15 @@
                         return this.data.label ? this.data.label : "_" != this.data.name[0] ? this.data.name : ""
                     },
                     text() {
                         return this.data.text
                     },
                     expanding() {
                         let e = this.type;
-                        return "tree" == e || "table" == e || "list" == e || "docviewer" == e || "graph" == e
+                        return "tree" == e || "table" == e || "list" == e || "docviewer" == e || "graph" == e || "linechart" == e
                     },
                     expanding_width() {
                         return !this.data.width && this.expanding
                     },
                     expanding_height() {
                         return !this.data.height && this.expanding
                     },
@@ -1656,64 +1800,64 @@
                     pdata: {
                         type: Object,
                         required: !0
                     }
                 },
                 watch: {
                     value(e, t) {
-                        "tree" == this.type && this.data.options[e] == t && this.expandedKeys.indexOf(t) < 0 && this.expandedKeys.push(t), e !== this.updated && (g && console.log("value changed", e, t), this.sendValue(), this.updated = e)
+                        "tree" == this.type && this.data.options[e] == t && this.expandedKeys.indexOf(t) < 0 && this.expandedKeys.push(t), e !== this.updated && (p && console.log("value changed", e, t), this.sendValue(), this.updated = e)
                     },
                     selection(e) {
-                        g && console.log("selection changed", e, this.$refs.inputRef), Array.isArray(e) || (e = [0, 0]);
+                        p && console.log("selection changed", e, this.$refs.inputRef), Array.isArray(e) || (e = [0, 0]);
                         let t = this.$refs.inputRef.$el;
                         t.focus();
                         let a = t.getElementsByTagName("textarea");
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
-                        g && console.log("data update", this.fullname, t.name), this.expanding && (this.styleSize || (this.styleSize = y(this.data), console.log(`${this.name} size changed`))), this.value = this.data.value, this.updated = this.value, k[this.fullname] = this
+                        p && console.log("data update", this.fullname, t.name), this.expanding && (this.styleSize || (this.styleSize = y(this.data), console.log(`${this.name} size changed`))), this.value = this.data.value, this.updated = this.value, b[this.fullname] = this
                     }
                 }
             });
-            var et = a(4027),
-                tt = a(9721),
-                at = a(8886),
-                lt = a(8761),
-                st = a(1232),
-                it = a(5551),
-                ot = a(5869),
-                nt = a(1745);
-            const dt = (0, U.Z)(Ge, [
+            var yt = a(4027),
+                wt = a(9721),
+                bt = a(8886),
+                kt = a(8761),
+                vt = a(1232),
+                xt = a(5551),
+                Ct = a(5869),
+                qt = a(1745);
+            const _t = (0, N.Z)(ft, [
                     ["render", Ce],
-                    ["__scopeId", "data-v-9805fac6"]
+                    ["__scopeId", "data-v-6d149d62"]
                 ]),
-                rt = dt;
-            R()(Ge, "components", {
-                QImg: et.Z,
-                QIcon: T.Z,
-                QSelect: He.Z,
-                QBadge: tt.Z,
-                QCheckbox: Ee.Z,
-                QToggle: at.Z,
-                QBtnToggle: lt.Z,
-                QInput: ze.Z,
-                QScrollArea: st.Z,
-                QTree: it.Z,
-                QSeparator: ot.Z,
-                QUploader: nt.Z,
+                St = _t;
+            I()(ft, "components", {
+                QImg: yt.Z,
+                QIcon: F.Z,
+                QSelect: Ee.Z,
+                QBadge: wt.Z,
+                QCheckbox: He.Z,
+                QToggle: bt.Z,
+                QBtnToggle: kt.Z,
+                QInput: $e.Z,
+                QScrollArea: vt.Z,
+                QTree: xt.Z,
+                QSeparator: Ct.Z,
+                QUploader: qt.Z,
                 QBtn: De.Z
             });
-            const ct = (0, l.aZ)({
+            const jt = (0, l.aZ)({
                 name: "block",
                 components: {
-                    element: rt
+                    element: St
                 },
                 data() {
                     return {
-                        styleSize: w,
+                        styleSize: f,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
                             opacity: .75
                         },
@@ -1724,15 +1868,15 @@
                             width: "8px",
                             opacity: .2
                         }
                     }
                 },
                 methods: {
                     log() {
-                        console.log(Object.keys(b).length, this.name, this.$el.getBoundingClientRect())
+                        console.log(Object.keys(w).length, this.name, this.$el.getBoundingClientRect())
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         const t = e.querySelector(".q-scrollarea"),
                             a = e.getBoundingClientRect();
                         return {
                             el: e,
@@ -1742,15 +1886,15 @@
                             top: a.top,
                             scrollHeight: window.innerHeight,
                             scrollWidth: window.innerWidth
                         }
                     }
                 },
                 mounted() {
-                    b[this.name] = this, this.expanding && (k[this.fullname] = this)
+                    w[this.name] = this, this.expanding && (b[this.fullname] = this)
                 },
                 computed: {
                     name() {
                         return this.data.name
                     },
                     fullname() {
                         return `_scroll@${this.name}`
@@ -1772,55 +1916,55 @@
                     data: {
                         type: Object,
                         required: !0
                     }
                 },
                 watch: {
                     data(e) {
-                        g && console.log("data update", this.name), this.styleSize = w, b[this.name] = this, this.expanding && (k[this.fullname] = this)
+                        p && console.log("data update", this.name), this.styleSize = f, w[this.name] = this, this.expanding && (b[this.fullname] = this)
                     }
                 }
             });
-            var ht = a(151);
-            const ut = (0, U.Z)(ct, [
+            var At = a(151);
+            const zt = (0, N.Z)(jt, [
                     ["render", ie]
                 ]),
-                pt = ut;
-            R()(ct, "components", {
-                QCard: ht.Z,
-                QIcon: T.Z,
-                QScrollArea: st.Z
+                Zt = zt;
+            I()(jt, "components", {
+                QCard: At.Z,
+                QIcon: F.Z,
+                QScrollArea: vt.Z
             });
-            const gt = (0, l.aZ)({
+            const Mt = (0, l.aZ)({
                     name: "zone",
                     components: {
-                        block: pt
+                        block: Zt
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
                         (0, l.Y3)((() => {
                             requestAnimationFrame((() => {
                                 requestAnimationFrame((() => {
-                                    W()
+                                    Q()
                                 }))
                             }))
                         }))
                     }
                 }),
-                mt = (0, U.Z)(gt, [
-                    ["render", J]
+                $t = (0, N.Z)(Mt, [
+                    ["render", G]
                 ]),
-                ft = mt,
-                wt = {
+                Dt = $t,
+                Vt = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function yt(e, t, a, i, o, n) {
+            function Ot(e, t, a, i, o, n) {
                 const d = (0, l.up)("block"),
                     r = (0, l.up)("q-item-label"),
                     c = (0, l.up)("q-space"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-card"),
                     p = (0, l.up)("q-dialog");
                 return (0, l.wg)(), (0, l.j4)(p, {
@@ -1836,40 +1980,40 @@
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, l.kq)("", !0), (0, l.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, l._)("div", wt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
+                        }), (0, l._)("div", Vt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => n.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide"])
             }
-            const bt = {
+            const Qt = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: pt
+                    block: Zt
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
-                        this.data.internal || q([this.data["name"], e]), this.hide()
+                        this.data.internal || C([this.data["name"], e]), this.hide()
                     },
                     hide() {
                         this.$refs.dialog.hide()
                     },
                     onDialogHide() {
                         this.$emit("hide")
                     },
@@ -1877,30 +2021,30 @@
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var kt = a(5926),
-                vt = a(2025);
-            const xt = (0, U.Z)(bt, [
-                    ["render", yt]
+            var Wt = a(5926),
+                Ht = a(2025);
+            const Et = (0, N.Z)(Qt, [
+                    ["render", Ot]
                 ]),
-                Ct = xt;
-            R()(bt, "components", {
-                QDialog: kt.Z,
-                QCard: ht.Z,
-                QItemLabel: N.Z,
-                QSpace: vt.Z,
+                Nt = Et;
+            I()(Qt, "components", {
+                QDialog: Wt.Z,
+                QCard: At.Z,
+                QItemLabel: K.Z,
+                QSpace: Ht.Z,
                 QBtn: De.Z
             });
-            var qt = !0;
-            let _t = null;
-            const jt = (0, l.aZ)({
+            var Ut = !0;
+            let Pt = null;
+            const Ft = (0, l.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         menu: [],
                         tab: "",
                         localServer: !0,
@@ -1908,39 +2052,39 @@
                         screen: {
                             blocks: []
                         }
                     }
                 },
                 components: {
                     menubar: B,
-                    zone: ft
+                    zone: Dt
                 },
                 created() {
-                    C(this)
+                    v(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
                 methods: {
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
-                        q(["root", e])
+                        C(["root", e])
                     },
                     onResize(e) {
-                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), Q()
+                        p && console.log("window has been resized", window.innerHeight, window.innerWidth), O()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: Ct
+                                component: Nt
                             },
                             {
                                 height: a,
                                 ...l
                             } = e;
                         l.width = 750;
                         let s = {
@@ -1958,82 +2102,82 @@
                         let a = t,
                             l = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == _t ? (l = {
+                        "progress" == t ? null == Pt ? (l = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, _t = this.$q.notify(l)) : null == e ? (_t(), _t = null) : (l = {
+                        }, Pt = this.$q.notify(l)) : null == e ? (Pt(), Pt = null) : (l = {
                             caption: e
-                        }, _t(l)) : ("error" == t && l.type, this.$q.notify(l))
+                        }, Pt(l)) : ("error" == t && l.type, this.$q.notify(l))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if (qt) qt = !1, this.menu = e[0].map((e => ({
+                        if (Ut) Ut = !1, this.menu = e[0].map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
-                        }))), this.screen = e[1], this.tab = this.screen.name, g && console.log("init loading..");
-                        else if ("screen" == e.type) Z(), this.screen = e;
+                        }))), this.screen = e[1], this.tab = this.screen.name, p && console.log("init loading..");
+                        else if ("screen" == e.type) z(), this.screen = e;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = Ct, t.componentProps = {
+                            t.component = Nt, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
-                        } else if (e.hasOwnProperty("answer")) z(e);
+                        } else if (e.hasOwnProperty("answer")) $(e);
                         else {
-                            e.update && $(e);
+                            e.update && M(e);
                             let t = !1;
-                            for (let a of v) a in e && (this.notify(e[a], a), t = !0);
+                            for (let a of k) a in e && (this.notify(e[a], a), t = !0);
                             t || e.update || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        _t && !e.progress && this.notify(null, "progress")
+                        Pt && !e.progress && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize)
                 }
             });
-            var St = a(9214),
-                At = a(3812),
-                Zt = a(9570),
-                Mt = a(7547),
-                $t = a(3269),
-                zt = a(2652),
-                Dt = a(4379);
-            const Ot = (0, U.Z)(jt, [
+            var Kt = a(9214),
+                Tt = a(3812),
+                It = a(9570),
+                Rt = a(7547),
+                Bt = a(3269),
+                Lt = a(2652),
+                Yt = a(4379);
+            const Xt = (0, N.Z)(Ft, [
                     ["render", o]
                 ]),
-                Qt = Ot;
-            R()(jt, "components", {
-                QLayout: St.Z,
-                QHeader: At.Z,
-                QToolbar: Zt.Z,
+                Gt = Xt;
+            I()(Ft, "components", {
+                QLayout: Kt.Z,
+                QHeader: Tt.Z,
+                QToolbar: It.Z,
                 QBtn: De.Z,
-                QItemLabel: N.Z,
-                QTabs: Mt.Z,
-                QTab: $t.Z,
-                QPageContainer: zt.Z,
-                QPage: Dt.Z
+                QItemLabel: K.Z,
+                QTabs: Rt.Z,
+                QTab: Bt.Z,
+                QPageContainer: Lt.Z,
+                QPage: Yt.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.4.4/unigui/web/js/app.a12bb431.js` & `unigui-1.4.5/unigui/web/js/app.c8cc6f16.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(603)]).then(r.bind(r, 7603)),
+                        component: () => Promise.all([r.e(736), r.e(22)]).then(r.bind(r, 22)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -44,30 +44,30 @@
                                     top: 0
                                 }),
                                 routes: v,
                                 history: e("")
                             });
                         return t
                     }));
-                async function b(e, t) {
+                async function g(e, t) {
                     const r = "function" === typeof m ? await m({}) : m,
                         n = e(d);
                     return n.use(o.Z, t), {
                         app: n,
                         router: r
                     }
                 }
-                var g = r(6417),
+                var b = r(6417),
                     y = r(5597);
                 const w = {
                         config: {
                             notify: {}
                         },
                         plugins: {
-                            Notify: g.Z,
+                            Notify: b.Z,
                             Dialog: y.Z
                         }
                     },
                     O = "";
                 async function k({
                     app: e,
                     router: t
@@ -94,15 +94,15 @@
                             urlPath: i,
                             publicPath: O
                         })
                     } catch (l) {
                         return l && l.url ? void a(l.url) : void console.error("[Quasar] boot error:", l)
                     }!0 !== n && (e.use(t), e.mount("#q-app"))
                 }
-                b(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
+                g(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
                     const r = t.map((e => e.default)).filter((e => "function" === typeof e));
                     k(e, r)
                 }))))
             },
             2390: (e, t, r) => {
                 r.r(t), r.d(t, {
                     default: () => o
@@ -158,25 +158,25 @@
                 get: t[n]
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
-            193: "b4cc3ffe",
-            430: "4be6e8a8",
-            603: "baf52338"
+            22: "b5025a55",
+            193: "283445be",
+            430: "591e9a73"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
+            22: "f5c7cbc7",
             143: "31d6cfe0",
-            603: "d94da9c0",
             736: "49a52e8f"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                603: 1
+                22: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.4.4/unigui/web/index.html` & `unigui-1.4.5/unigui/web/index.html`

 * *Files 9% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.c0de6c67.js></script><script defer src=js/app.a12bb431.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.c8cc6f16.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.4.4/LICENSE` & `unigui-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.4.4/setup.py` & `unigui-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.4.4',      
+      version='1.4.5',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal app browser',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.4.4/PKG-INFO` & `unigui-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.4
+Version: 1.4.5
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 Provide a programming technology that does not require front-end programming, for a server written in any language, for displaying on any device, in any resolution, without any tuning. 
 
 ### Installing ###
 ```
 pip install unigui
 ```
 
-### How does work inside ###
+### How it works inside ###
 The exchange protocol for the solution is JSON as the most universally accessible, comprehensible, readable, and popular format compatible with all programming languages.  The server sends JSON data to Unigui which has built-in tools (autodesigner) and automatically builds a standart Google Material Design GUI for user data. No markup, drawing instructions and the other dull job are required. Just the simplest description what you want. From the constructed Unigui screen the server receives a JSON message flow which fully describes what the user did. The message format is ["Block", "Elem", "type of action", value], where "Block"and "Elem"are the names of the block and its element, "value" is the JSON value of the action/event that has happened. The server can either accept the change or roll it back by sending an info window about an inconsistency. The server can open a dialog box, send popup Warning, Error,.. or an entirely new screen. Unigui instantly and automatically displays actual server state. 
 
 ### Programming ###
 Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that.
 Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
 
 ### High level - Screen ###
@@ -63,15 +63,15 @@
 #app name, port for initial connection and upload_dir folder are optional
 unigui.start('Test app') 
 ```
 Unigui builds the interactive app for the code above.
 Connect a browser to localhast:8000 which are by default and will see:
 server port and ip config is in config.py file in the working directory
 
-![alt text](https://github.com/Claus1/unigui/blob/main/tests/screen1.png?raw=true)
+![image](https://github.com/Claus1/unigui/assets/1247062/5afcf4ac-b388-4237-98ff-3a92e802d44a)
 
 ### Handling events ###
 All handlers are functions which have a signature
 ```
 def handler_x(gui_object, value_x)
 ```
 where gui_object is a Python object the user interacted with and value for the event.
@@ -155,15 +155,15 @@
 #### Layout of blocks. #### 
 If the blocks are simply listed Unigui draws them from left to right or from top to bottom depending on the orientation setting. If a different layout is needed, it can be set according to the following rule: if the vertical area must contain more than one block, then the enumeration in the array will arrange the elements vertically one after another. If such an element enumeration is an array of blocks, then they will be drawn horizontally in the corresponding area.
 
 #### Example ####
 blocks = [ [b1,b2], [b3, [b4, b5]]]
 #[b1,b2] - the first vertical area, [b3, [b4, b5]] - the second one.
 
-![alt text](https://github.com/Claus1/unigui/blob/main/tests/multiscreen.png?raw=true)
+![image](https://github.com/Claus1/unigui/assets/1247062/75d0f64c-d457-43c6-a909-0c97f4b4ab0f)
 
 ### Basic gui elements ###
 Normally they have type property which says unigui what data it contains and optionally how to draw the element. 
 #### If the element name starts from _ , unigui will hide its name on the screen. ####
 if we need to paint an icon in an element, add 'icon': 'any MD icon name' to the element constructor.
 
 #### Most constructor parameters are optional for Gui elements except the first one which is the element name. ####
@@ -312,15 +312,15 @@
     if error_found:
         return Error('Can not accept the value!')
     accept_rowvalue(table_, tabval)
 ```
 
 ### Chart ###
 Chart is a table with additional Table constructor parameter 'view' which explaines unigui how to draw a chart. The format is '{x index}-{y index1},{y index2}[,..]'. '0-1,2,3' means that x axis values will be taken from 0 column, and y values from 1,2,3 columns of row data.
-'i-3,5' means that x axis values will be equal the row indexes in rows, and y values from 3,5 columns of rows data. If a table constructor got view = '..' parameter then unigui displays a chart icon at the table header, pushing it switches table mode to the chart mode. If a table constructor got type = 'view' in addition to view parameter the table will be displayed as chart on start. In the chart mode pushing the icon button on the top right switches back to table row mode.
+'i-3,5' means that x axis values will be equal the row indexes in rows, and y values from 3,5 columns of rows data. If a table constructor got view = '..' parameter then unigui displays a chart icon at the table header, pushing it switches table mode to the chart mode. If a table constructor got type = 'linechart' in addition to view parameter the table will be displayed as a chart on start. In the chart mode pushing the icon button on the top right switches back to table view mode.
 
 ### Graph ###
 Graph supports an interactive graph with optional draw methods.
 ```
 graph = Graph('X graph', graph_value, graph_selection, 
     nodes = [
      { 'id' : 'node1', 'label': "Node 1" },
```

### Comparing `unigui-1.4.4/README.md` & `unigui-1.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Provide a programming technology that does not require front-end programming, for a server written in any language, for displaying on any device, in any resolution, without any tuning. 
 
 ### Installing ###
 ```
 pip install unigui
 ```
 
-### How does work inside ###
+### How it works inside ###
 The exchange protocol for the solution is JSON as the most universally accessible, comprehensible, readable, and popular format compatible with all programming languages.  The server sends JSON data to Unigui which has built-in tools (autodesigner) and automatically builds a standart Google Material Design GUI for user data. No markup, drawing instructions and the other dull job are required. Just the simplest description what you want. From the constructed Unigui screen the server receives a JSON message flow which fully describes what the user did. The message format is ["Block", "Elem", "type of action", value], where "Block"and "Elem"are the names of the block and its element, "value" is the JSON value of the action/event that has happened. The server can either accept the change or roll it back by sending an info window about an inconsistency. The server can open a dialog box, send popup Warning, Error,.. or an entirely new screen. Unigui instantly and automatically displays actual server state. 
 
 ### Programming ###
 Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that.
 Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
 
 ### High level - Screen ###
@@ -51,15 +51,15 @@
 #app name, port for initial connection and upload_dir folder are optional
 unigui.start('Test app') 
 ```
 Unigui builds the interactive app for the code above.
 Connect a browser to localhast:8000 which are by default and will see:
 server port and ip config is in config.py file in the working directory
 
-![alt text](https://github.com/Claus1/unigui/blob/main/tests/screen1.png?raw=true)
+![image](https://github.com/Claus1/unigui/assets/1247062/5afcf4ac-b388-4237-98ff-3a92e802d44a)
 
 ### Handling events ###
 All handlers are functions which have a signature
 ```
 def handler_x(gui_object, value_x)
 ```
 where gui_object is a Python object the user interacted with and value for the event.
@@ -143,15 +143,15 @@
 #### Layout of blocks. #### 
 If the blocks are simply listed Unigui draws them from left to right or from top to bottom depending on the orientation setting. If a different layout is needed, it can be set according to the following rule: if the vertical area must contain more than one block, then the enumeration in the array will arrange the elements vertically one after another. If such an element enumeration is an array of blocks, then they will be drawn horizontally in the corresponding area.
 
 #### Example ####
 blocks = [ [b1,b2], [b3, [b4, b5]]]
 #[b1,b2] - the first vertical area, [b3, [b4, b5]] - the second one.
 
-![alt text](https://github.com/Claus1/unigui/blob/main/tests/multiscreen.png?raw=true)
+![image](https://github.com/Claus1/unigui/assets/1247062/75d0f64c-d457-43c6-a909-0c97f4b4ab0f)
 
 ### Basic gui elements ###
 Normally they have type property which says unigui what data it contains and optionally how to draw the element. 
 #### If the element name starts from _ , unigui will hide its name on the screen. ####
 if we need to paint an icon in an element, add 'icon': 'any MD icon name' to the element constructor.
 
 #### Most constructor parameters are optional for Gui elements except the first one which is the element name. ####
@@ -300,15 +300,15 @@
     if error_found:
         return Error('Can not accept the value!')
     accept_rowvalue(table_, tabval)
 ```
 
 ### Chart ###
 Chart is a table with additional Table constructor parameter 'view' which explaines unigui how to draw a chart. The format is '{x index}-{y index1},{y index2}[,..]'. '0-1,2,3' means that x axis values will be taken from 0 column, and y values from 1,2,3 columns of row data.
-'i-3,5' means that x axis values will be equal the row indexes in rows, and y values from 3,5 columns of rows data. If a table constructor got view = '..' parameter then unigui displays a chart icon at the table header, pushing it switches table mode to the chart mode. If a table constructor got type = 'view' in addition to view parameter the table will be displayed as chart on start. In the chart mode pushing the icon button on the top right switches back to table row mode.
+'i-3,5' means that x axis values will be equal the row indexes in rows, and y values from 3,5 columns of rows data. If a table constructor got view = '..' parameter then unigui displays a chart icon at the table header, pushing it switches table mode to the chart mode. If a table constructor got type = 'linechart' in addition to view parameter the table will be displayed as a chart on start. In the chart mode pushing the icon button on the top right switches back to table view mode.
 
 ### Graph ###
 Graph supports an interactive graph with optional draw methods.
 ```
 graph = Graph('X graph', graph_value, graph_selection, 
     nodes = [
      { 'id' : 'node1', 'label': "Node 1" },
```

### Comparing `unigui-1.4.4/unigui.egg-info/PKG-INFO` & `unigui-1.4.5/unigui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.4
+Version: 1.4.5
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 Provide a programming technology that does not require front-end programming, for a server written in any language, for displaying on any device, in any resolution, without any tuning. 
 
 ### Installing ###
 ```
 pip install unigui
 ```
 
-### How does work inside ###
+### How it works inside ###
 The exchange protocol for the solution is JSON as the most universally accessible, comprehensible, readable, and popular format compatible with all programming languages.  The server sends JSON data to Unigui which has built-in tools (autodesigner) and automatically builds a standart Google Material Design GUI for user data. No markup, drawing instructions and the other dull job are required. Just the simplest description what you want. From the constructed Unigui screen the server receives a JSON message flow which fully describes what the user did. The message format is ["Block", "Elem", "type of action", value], where "Block"and "Elem"are the names of the block and its element, "value" is the JSON value of the action/event that has happened. The server can either accept the change or roll it back by sending an info window about an inconsistency. The server can open a dialog box, send popup Warning, Error,.. or an entirely new screen. Unigui instantly and automatically displays actual server state. 
 
 ### Programming ###
 Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that.
 Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
 
 ### High level - Screen ###
@@ -63,15 +63,15 @@
 #app name, port for initial connection and upload_dir folder are optional
 unigui.start('Test app') 
 ```
 Unigui builds the interactive app for the code above.
 Connect a browser to localhast:8000 which are by default and will see:
 server port and ip config is in config.py file in the working directory
 
-![alt text](https://github.com/Claus1/unigui/blob/main/tests/screen1.png?raw=true)
+![image](https://github.com/Claus1/unigui/assets/1247062/5afcf4ac-b388-4237-98ff-3a92e802d44a)
 
 ### Handling events ###
 All handlers are functions which have a signature
 ```
 def handler_x(gui_object, value_x)
 ```
 where gui_object is a Python object the user interacted with and value for the event.
@@ -155,15 +155,15 @@
 #### Layout of blocks. #### 
 If the blocks are simply listed Unigui draws them from left to right or from top to bottom depending on the orientation setting. If a different layout is needed, it can be set according to the following rule: if the vertical area must contain more than one block, then the enumeration in the array will arrange the elements vertically one after another. If such an element enumeration is an array of blocks, then they will be drawn horizontally in the corresponding area.
 
 #### Example ####
 blocks = [ [b1,b2], [b3, [b4, b5]]]
 #[b1,b2] - the first vertical area, [b3, [b4, b5]] - the second one.
 
-![alt text](https://github.com/Claus1/unigui/blob/main/tests/multiscreen.png?raw=true)
+![image](https://github.com/Claus1/unigui/assets/1247062/75d0f64c-d457-43c6-a909-0c97f4b4ab0f)
 
 ### Basic gui elements ###
 Normally they have type property which says unigui what data it contains and optionally how to draw the element. 
 #### If the element name starts from _ , unigui will hide its name on the screen. ####
 if we need to paint an icon in an element, add 'icon': 'any MD icon name' to the element constructor.
 
 #### Most constructor parameters are optional for Gui elements except the first one which is the element name. ####
@@ -312,15 +312,15 @@
     if error_found:
         return Error('Can not accept the value!')
     accept_rowvalue(table_, tabval)
 ```
 
 ### Chart ###
 Chart is a table with additional Table constructor parameter 'view' which explaines unigui how to draw a chart. The format is '{x index}-{y index1},{y index2}[,..]'. '0-1,2,3' means that x axis values will be taken from 0 column, and y values from 1,2,3 columns of row data.
-'i-3,5' means that x axis values will be equal the row indexes in rows, and y values from 3,5 columns of rows data. If a table constructor got view = '..' parameter then unigui displays a chart icon at the table header, pushing it switches table mode to the chart mode. If a table constructor got type = 'view' in addition to view parameter the table will be displayed as chart on start. In the chart mode pushing the icon button on the top right switches back to table row mode.
+'i-3,5' means that x axis values will be equal the row indexes in rows, and y values from 3,5 columns of rows data. If a table constructor got view = '..' parameter then unigui displays a chart icon at the table header, pushing it switches table mode to the chart mode. If a table constructor got type = 'linechart' in addition to view parameter the table will be displayed as a chart on start. In the chart mode pushing the icon button on the top right switches back to table view mode.
 
 ### Graph ###
 Graph supports an interactive graph with optional draw methods.
 ```
 graph = Graph('X graph', graph_value, graph_selection, 
     nodes = [
      { 'id' : 'node1', 'label': "Node 1" },
```

### Comparing `unigui-1.4.4/unigui.egg-info/SOURCES.txt` & `unigui-1.4.5/unigui.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/603.d94da9c0.css
+unigui/web/css/22.f5c7cbc7.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
 unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
-unigui/web/js/193.b4cc3ffe.js
-unigui/web/js/430.4be6e8a8.js
-unigui/web/js/603.baf52338.js
-unigui/web/js/app.a12bb431.js
-unigui/web/js/vendor.c0de6c67.js
+unigui/web/js/193.283445be.js
+unigui/web/js/22.b5025a55.js
+unigui/web/js/430.591e9a73.js
+unigui/web/js/app.c8cc6f16.js
+unigui/web/js/vendor.3e8714c2.js
```

