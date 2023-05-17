# Comparing `tmp/cloudspot-erp-api-1.0.0.tar.gz` & `tmp/cloudspot-erp-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudspot-erp-api-1.0.0.tar", last modified: Tue Mar 14 12:38:21 2023, max compression
+gzip compressed data, was "cloudspot-erp-api-1.1.0.tar", last modified: Wed May 17 06:19:20 2023, max compression
```

## Comparing `cloudspot-erp-api-1.0.0.tar` & `cloudspot-erp-api-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 12:38:21.502827 cloudspot-erp-api-1.0.0/
--rw-rw-rw-   0        0        0    35821 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6599 2023-03-14 12:38:21.503851 cloudspot-erp-api-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5853 2023-03-14 12:36:45.000000 cloudspot-erp-api-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-14 12:38:21.458428 cloudspot-erp-api-1.0.0/cloudspot/
--rw-rw-rw-   0        0        0        0 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/__init__.py
--rw-rw-rw-   0        0        0     3787 2023-03-14 12:36:45.000000 cloudspot-erp-api-1.0.0/cloudspot/api.py
--rw-rw-rw-   0        0        0       83 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/authhandler.py
--rw-rw-rw-   0        0        0       99 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/config.py
-drwxrwxrwx   0        0        0        0 2023-03-14 12:38:21.461452 cloudspot-erp-api-1.0.0/cloudspot/constants/
--rw-rw-rw-   0        0        0      189 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/constants/errors.py
--rw-rw-rw-   0        0        0      463 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/constants/responses.py
-drwxrwxrwx   0        0        0        0 2023-03-14 12:38:21.471462 cloudspot-erp-api-1.0.0/cloudspot/endpoints/
--rw-rw-rw-   0        0        0        0 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/endpoints/__init__.py
--rw-rw-rw-   0        0        0      813 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/endpoints/artikels.py
--rw-rw-rw-   0        0        0     1786 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/endpoints/auth.py
--rw-rw-rw-   0        0        0      120 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/endpoints/base.py
--rw-rw-rw-   0        0        0      885 2022-12-28 13:40:05.000000 cloudspot-erp-api-1.0.0/cloudspot/endpoints/categorieen.py
--rw-rw-rw-   0        0        0      489 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/endpoints/klanten.py
-drwxrwxrwx   0        0        0        0 2023-03-14 12:38:21.478827 cloudspot-erp-api-1.0.0/cloudspot/models/
--rw-rw-rw-   0        0        0        0 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/models/__init__.py
--rw-rw-rw-   0        0        0     4235 2023-01-02 12:38:36.000000 cloudspot-erp-api-1.0.0/cloudspot/models/artikels.py
--rw-rw-rw-   0        0        0     1286 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/models/auth.py
--rw-rw-rw-   0        0        0     2987 2022-11-02 09:24:52.000000 cloudspot-erp-api-1.0.0/cloudspot/models/base.py
--rw-rw-rw-   0        0        0      144 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/models/errors.py
--rw-rw-rw-   0        0        0     1294 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.0.0/cloudspot/models/klanten.py
-drwxrwxrwx   0        0        0        0 2023-03-14 12:38:21.501861 cloudspot-erp-api-1.0.0/cloudspot_erp_api.egg-info/
--rw-rw-rw-   0        0        0     6599 2023-03-14 12:38:21.000000 cloudspot-erp-api-1.0.0/cloudspot_erp_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      752 2023-03-14 12:38:21.000000 cloudspot-erp-api-1.0.0/cloudspot_erp_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 12:38:21.000000 cloudspot-erp-api-1.0.0/cloudspot_erp_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-03-14 12:38:21.000000 cloudspot-erp-api-1.0.0/cloudspot_erp_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-14 12:38:21.000000 cloudspot-erp-api-1.0.0/cloudspot_erp_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-14 12:38:21.508828 cloudspot-erp-api-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-03-14 12:36:45.000000 cloudspot-erp-api-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:19:20.783081 cloudspot-erp-api-1.1.0/
+-rw-rw-rw-   0        0        0    35821 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6599 2023-05-17 06:19:20.783081 cloudspot-erp-api-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5853 2023-03-14 12:36:45.000000 cloudspot-erp-api-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 06:19:20.739080 cloudspot-erp-api-1.1.0/cloudspot/
+-rw-rw-rw-   0        0        0        0 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/__init__.py
+-rw-rw-rw-   0        0        0     3787 2023-03-14 12:36:45.000000 cloudspot-erp-api-1.1.0/cloudspot/api.py
+-rw-rw-rw-   0        0        0       83 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/authhandler.py
+-rw-rw-rw-   0        0        0       99 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/config.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:19:20.743081 cloudspot-erp-api-1.1.0/cloudspot/constants/
+-rw-rw-rw-   0        0        0      189 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/constants/errors.py
+-rw-rw-rw-   0        0        0      463 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/constants/responses.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:19:20.749080 cloudspot-erp-api-1.1.0/cloudspot/endpoints/
+-rw-rw-rw-   0        0        0        0 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/endpoints/__init__.py
+-rw-rw-rw-   0        0        0      813 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/endpoints/artikels.py
+-rw-rw-rw-   0        0        0     1786 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/endpoints/auth.py
+-rw-rw-rw-   0        0        0      120 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/endpoints/base.py
+-rw-rw-rw-   0        0        0      885 2022-12-28 13:40:05.000000 cloudspot-erp-api-1.1.0/cloudspot/endpoints/categorieen.py
+-rw-rw-rw-   0        0        0      489 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/endpoints/klanten.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:19:20.756079 cloudspot-erp-api-1.1.0/cloudspot/models/
+-rw-rw-rw-   0        0        0        0 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/models/__init__.py
+-rw-rw-rw-   0        0        0     4337 2023-05-17 06:18:31.000000 cloudspot-erp-api-1.1.0/cloudspot/models/artikels.py
+-rw-rw-rw-   0        0        0     1286 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/models/auth.py
+-rw-rw-rw-   0        0        0     2987 2022-11-02 09:24:52.000000 cloudspot-erp-api-1.1.0/cloudspot/models/base.py
+-rw-rw-rw-   0        0        0      144 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/models/errors.py
+-rw-rw-rw-   0        0        0     1294 2022-11-02 09:20:29.000000 cloudspot-erp-api-1.1.0/cloudspot/models/klanten.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:19:20.781078 cloudspot-erp-api-1.1.0/cloudspot_erp_api.egg-info/
+-rw-rw-rw-   0        0        0     6599 2023-05-17 06:19:20.000000 cloudspot-erp-api-1.1.0/cloudspot_erp_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      752 2023-05-17 06:19:20.000000 cloudspot-erp-api-1.1.0/cloudspot_erp_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 06:19:20.000000 cloudspot-erp-api-1.1.0/cloudspot_erp_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-17 06:19:20.000000 cloudspot-erp-api-1.1.0/cloudspot_erp_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-17 06:19:20.000000 cloudspot-erp-api-1.1.0/cloudspot_erp_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-17 06:19:20.785079 cloudspot-erp-api-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2023-05-17 06:18:31.000000 cloudspot-erp-api-1.1.0/setup.py
```

### Comparing `cloudspot-erp-api-1.0.0/LICENSE.txt` & `cloudspot-erp-api-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cloudspot-erp-api-1.0.0/PKG-INFO` & `cloudspot-erp-api-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cloudspot-erp-api
-Version: 1.0.0
+Version: 1.1.0
 Summary: Wrapper for the Cloudspot ERP API endpoints
 Home-page: https://github.com/Ecosy-EU/inktool-wrapper
-Download-URL: https://github.com/Ecosy-EU/cloudspot-api/archive/refs/tags/1.0.0.tar.gz
+Download-URL: https://github.com/Ecosy-EU/cloudspot-api/archive/refs/tags/1.1.0.tar.gz
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
 Keywords: cloudspot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `cloudspot-erp-api-1.0.0/README.md` & `cloudspot-erp-api-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudspot-erp-api-1.0.0/cloudspot/api.py` & `cloudspot-erp-api-1.1.0/cloudspot/api.py`

 * *Files identical despite different names*

### Comparing `cloudspot-erp-api-1.0.0/cloudspot/endpoints/artikels.py` & `cloudspot-erp-api-1.1.0/cloudspot/endpoints/artikels.py`

 * *Files identical despite different names*

### Comparing `cloudspot-erp-api-1.0.0/cloudspot/endpoints/auth.py` & `cloudspot-erp-api-1.1.0/cloudspot/endpoints/auth.py`

 * *Files identical despite different names*

### Comparing `cloudspot-erp-api-1.0.0/cloudspot/endpoints/categorieen.py` & `cloudspot-erp-api-1.1.0/cloudspot/endpoints/categorieen.py`

 * *Files identical despite different names*

### Comparing `cloudspot-erp-api-1.0.0/cloudspot/models/artikels.py` & `cloudspot-erp-api-1.1.0/cloudspot/models/artikels.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,15 +101,16 @@
         BTW=None,
         status=None,
         fotos=None,
         prijscategorieen=None,
         EAN=None,
         samenstellingen=None,
         ruwe_grondstoffen=None,
-        gebruiksaanwijzingen=None
+        gebruiksaanwijzingen=None,
+        meer_info=None,
     ):
 
         super().__init__()
 
         self.id = id
         self.naam = naam
         self.beschrijving = beschrijving
@@ -132,12 +133,13 @@
         self.BTW = BTW
         self.status = status
         self.fotos = fotos if fotos else ArtikelFotos()
         self.prijscategorieen = prijscategorieen if prijscategorieen else Prijscategorieen()
         self.samenstellingen = samenstellingen if samenstellingen else ExtraInformatieList()
         self.ruwe_grondstoffen = ruwe_grondstoffen if ruwe_grondstoffen else ExtraInformatieList()
         self.gebruiksaanwijzingen = gebruiksaanwijzingen if gebruiksaanwijzingen else ExtraInformatieList()
+        self.meer_info = meer_info if meer_info else ExtraInformatieList()
         self.EAN = EAN if EAN else []
         
 class Artikels(ObjectListModel):
     def __init__(self):
         super().__init__(list=[], listObject=Artikel)
```

### Comparing `cloudspot-erp-api-1.0.0/cloudspot/models/auth.py` & `cloudspot-erp-api-1.1.0/cloudspot/models/auth.py`

 * *Files identical despite different names*

### Comparing `cloudspot-erp-api-1.0.0/cloudspot/models/base.py` & `cloudspot-erp-api-1.1.0/cloudspot/models/base.py`

 * *Files identical despite different names*

### Comparing `cloudspot-erp-api-1.0.0/cloudspot/models/klanten.py` & `cloudspot-erp-api-1.1.0/cloudspot/models/klanten.py`

 * *Files identical despite different names*

### Comparing `cloudspot-erp-api-1.0.0/cloudspot_erp_api.egg-info/PKG-INFO` & `cloudspot-erp-api-1.1.0/cloudspot_erp_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cloudspot-erp-api
-Version: 1.0.0
+Version: 1.1.0
 Summary: Wrapper for the Cloudspot ERP API endpoints
 Home-page: https://github.com/Ecosy-EU/inktool-wrapper
-Download-URL: https://github.com/Ecosy-EU/cloudspot-api/archive/refs/tags/1.0.0.tar.gz
+Download-URL: https://github.com/Ecosy-EU/cloudspot-api/archive/refs/tags/1.1.0.tar.gz
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
 Keywords: cloudspot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `cloudspot-erp-api-1.0.0/cloudspot_erp_api.egg-info/SOURCES.txt` & `cloudspot-erp-api-1.1.0/cloudspot_erp_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudspot-erp-api-1.0.0/setup.py` & `cloudspot-erp-api-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'cloudspot-erp-api',         
   packages=['cloudspot', 'cloudspot.models', 'cloudspot.constants', 'cloudspot.endpoints'],
-  version = '1.0.0',
+  version = '1.1.0',
   license='GPL-3.0-or-later',
   description = 'Wrapper for the Cloudspot ERP API endpoints',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Alexander Schillemans',
   author_email = 'alexander.schillemans@lhs.global',
   url = 'https://github.com/Ecosy-EU/inktool-wrapper',
-  download_url = 'https://github.com/Ecosy-EU/cloudspot-api/archive/refs/tags/1.0.0.tar.gz',
+  download_url = 'https://github.com/Ecosy-EU/cloudspot-api/archive/refs/tags/1.1.0.tar.gz',
   keywords = ['cloudspot'],
   install_requires=[
           'requests',
           'python-dateutil',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

