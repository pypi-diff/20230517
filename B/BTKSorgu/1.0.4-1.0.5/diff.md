# Comparing `tmp/BTKSorgu-1.0.4.tar.gz` & `tmp/BTKSorgu-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.0.4.tar", last modified: Wed May 17 15:11:17 2023, max compression
+gzip compressed data, was "BTKSorgu-1.0.5.tar", last modified: Wed May 17 16:01:42 2023, max compression
```

## Comparing `BTKSorgu-1.0.4.tar` & `BTKSorgu-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:11:17.321549 BTKSorgu-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:11:17.321549 BTKSorgu-1.0.4/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/BTKSorgu/konsol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:11:17.321549 BTKSorgu-1.0.4/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-17 15:11:17.000000 BTKSorgu-1.0.4/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 15:11:17.000000 BTKSorgu-1.0.4/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:11:17.000000 BTKSorgu-1.0.4/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 15:11:17.000000 BTKSorgu-1.0.4/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 15:11:17.000000 BTKSorgu-1.0.4/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 15:11:17.000000 BTKSorgu-1.0.4/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-17 15:11:17.321549 BTKSorgu-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:11:17.321549 BTKSorgu-1.0.4/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:11:17.321549 BTKSorgu-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:42.352206 BTKSorgu-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:42.352206 BTKSorgu-1.0.5/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:42.352206 BTKSorgu-1.0.5/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-17 16:01:42.000000 BTKSorgu-1.0.5/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 16:01:42.000000 BTKSorgu-1.0.5/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:01:42.000000 BTKSorgu-1.0.5/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 16:01:42.000000 BTKSorgu-1.0.5/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 16:01:42.000000 BTKSorgu-1.0.5/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 16:01:42.000000 BTKSorgu-1.0.5/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-17 16:01:42.352206 BTKSorgu-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:42.352206 BTKSorgu-1.0.5/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 16:01:42.352206 BTKSorgu-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/setup.py
```

### Comparing `BTKSorgu-1.0.4/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.0.5/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.4/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.0.5/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.4/BTKSorgu/arayuz.py` & `BTKSorgu-1.0.5/BTKSorgu/arayuz.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
 from contextlib import suppress
 from BTKSorgu   import KekikGUI
 from tkinter    import ttk
 from BTKSorgu   import BTKSorgu
 
+import os
+
+ust_dizin_ver = lambda _path, n: os.sep.join(_path.split(os.sep)[:-n])
+
+def dosya_ver(dosya_yolu:str, ust_dizin:int):
+    return os.path.join(ust_dizin_ver(__file__, ust_dizin), dosya_yolu)
+
 kekik = KekikGUI(
     pencere_adi = "BTK Sorgu",
-    logo_yolu   = "logo.png",
+    logo_yolu   = dosya_ver("logo.png", 1),
     satir_sutun = 1,
     ortala      = False,
     cikis_onay  = False,
     p_genislik  = 400,
     p_yukseklik = 250
 )
```

### Comparing `BTKSorgu-1.0.4/BTKSorgu/konsol.py` & `BTKSorgu-1.0.5/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.4/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.0.5/BTKSorgu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.4
+Version: 1.0.5
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.4 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.5 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.0.4/LICENSE` & `BTKSorgu-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.4/PKG-INFO` & `BTKSorgu-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.4
+Version: 1.0.5
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.4 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.5 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.0.4/README.md` & `BTKSorgu-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.0.5/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 1% similar despite different names*

#### Comparing `BTKSorgu-1.0.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.0.5/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -25,15 +25,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.0.4" date="2023-5-17">
+    <release version="1.0.5" date="2023-5-17">
       <description>
         <p>Proje Başlangıcı</p>
       </description>
     </release>
   </releases>
   <content_rating type="oars-1.1"/>
 </component>
```

### Comparing `BTKSorgu-1.0.4/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.0.5/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.4/setup.py` & `BTKSorgu-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.0.4",
+    version      = "1.0.5",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -23,14 +23,15 @@
 
     # ? Paket Bilgileri
     packages         = ["BTKSorgu"],
     python_requires  = ">=3.10",
     install_requires = [
         "setuptools",
         "wheel",
+        "install_freedesktop",
         "rich",
         "requests",
         "parsel",
         "cssselect",
         "regex",
         "Pillow",
         "pytesseract",
```

