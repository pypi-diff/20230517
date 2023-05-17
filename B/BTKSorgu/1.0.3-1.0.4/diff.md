# Comparing `tmp/BTKSorgu-1.0.3.tar.gz` & `tmp/BTKSorgu-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.0.3.tar", last modified: Wed May 17 14:21:58 2023, max compression
+gzip compressed data, was "BTKSorgu-1.0.4.tar", last modified: Wed May 17 15:11:17 2023, max compression
```

## Comparing `BTKSorgu-1.0.3.tar` & `BTKSorgu-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:21:58.974464 BTKSorgu-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:21:58.974464 BTKSorgu-1.0.3/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/BTKSorgu/konsol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:21:58.974464 BTKSorgu-1.0.3/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-17 14:21:58.000000 BTKSorgu-1.0.3/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 14:21:58.000000 BTKSorgu-1.0.3/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:21:58.000000 BTKSorgu-1.0.3/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 14:21:58.000000 BTKSorgu-1.0.3/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-17 14:21:58.000000 BTKSorgu-1.0.3/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 14:21:58.000000 BTKSorgu-1.0.3/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-17 14:21:58.974464 BTKSorgu-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:21:58.974464 BTKSorgu-1.0.3/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:21:58.974464 BTKSorgu-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:11:17.321549 BTKSorgu-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:11:17.321549 BTKSorgu-1.0.4/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/BTKSorgu/konsol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:11:17.321549 BTKSorgu-1.0.4/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-17 15:11:17.000000 BTKSorgu-1.0.4/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 15:11:17.000000 BTKSorgu-1.0.4/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:11:17.000000 BTKSorgu-1.0.4/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 15:11:17.000000 BTKSorgu-1.0.4/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 15:11:17.000000 BTKSorgu-1.0.4/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 15:11:17.000000 BTKSorgu-1.0.4/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-17 15:11:17.321549 BTKSorgu-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:11:17.321549 BTKSorgu-1.0.4/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:11:17.321549 BTKSorgu-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-17 15:10:55.000000 BTKSorgu-1.0.4/setup.py
```

### Comparing `BTKSorgu-1.0.3/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.0.4/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.3/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.0.4/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.3/BTKSorgu/arayuz.py` & `BTKSorgu-1.0.4/BTKSorgu/arayuz.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.3/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.0.4/BTKSorgu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.3
+Version: 1.0.4
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
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.3 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.4 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.0.3/LICENSE` & `BTKSorgu-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.3/PKG-INFO` & `BTKSorgu-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.3
+Version: 1.0.4
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
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.3 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.4 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.0.3/README.md` & `BTKSorgu-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.0.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 1% similar despite different names*

#### Comparing `BTKSorgu-1.0.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.0.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -25,15 +25,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.0.3" date="2023-5-17">
+    <release version="1.0.4" date="2023-5-17">
       <description>
         <p>Proje Başlangıcı</p>
       </description>
     </release>
   </releases>
   <content_rating type="oars-1.1"/>
 </component>
```

### Comparing `BTKSorgu-1.0.3/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.0.4/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.3/setup.py` & `BTKSorgu-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.0.3",
+    version      = "1.0.4",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -23,15 +23,15 @@
 
     # ? Paket Bilgileri
     packages         = ["BTKSorgu"],
     python_requires  = ">=3.10",
     install_requires = [
         "setuptools",
         "wheel",
-        "Kekik",
+        "rich",
         "requests",
         "parsel",
         "cssselect",
         "regex",
         "Pillow",
         "pytesseract",
         "sv_ttk"
```

