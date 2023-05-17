# Comparing `tmp/BTKSorgu-1.0.1.tar.gz` & `tmp/BTKSorgu-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.0.1.tar", last modified: Wed May 10 18:28:02 2023, max compression
+gzip compressed data, was "BTKSorgu-1.0.2.tar", last modified: Wed May 17 14:20:17 2023, max compression
```

## Comparing `BTKSorgu-1.0.1.tar` & `BTKSorgu-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:28:02.436343 BTKSorgu-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:28:02.436343 BTKSorgu-1.0.1/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-10 18:27:40.000000 BTKSorgu-1.0.1/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-10 18:27:40.000000 BTKSorgu-1.0.1/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-10 18:27:40.000000 BTKSorgu-1.0.1/BTKSorgu/konsol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:28:02.436343 BTKSorgu-1.0.1/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-10 18:28:02.000000 BTKSorgu-1.0.1/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-10 18:28:02.000000 BTKSorgu-1.0.1/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:28:02.000000 BTKSorgu-1.0.1/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 18:28:02.000000 BTKSorgu-1.0.1/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 18:28:02.000000 BTKSorgu-1.0.1/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 18:28:02.000000 BTKSorgu-1.0.1/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 18:27:40.000000 BTKSorgu-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-10 18:28:02.436343 BTKSorgu-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-10 18:27:40.000000 BTKSorgu-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:28:02.436343 BTKSorgu-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-10 18:27:40.000000 BTKSorgu-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:17.455681 BTKSorgu-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:17.455681 BTKSorgu-1.0.2/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/BTKSorgu/konsol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:17.455681 BTKSorgu-1.0.2/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-17 14:20:17.000000 BTKSorgu-1.0.2/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 14:20:17.000000 BTKSorgu-1.0.2/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:20:17.000000 BTKSorgu-1.0.2/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 14:20:17.000000 BTKSorgu-1.0.2/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-17 14:20:17.000000 BTKSorgu-1.0.2/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 14:20:17.000000 BTKSorgu-1.0.2/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-17 14:20:17.455681 BTKSorgu-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:17.455681 BTKSorgu-1.0.2/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:20:17.455681 BTKSorgu-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/setup.py
```

### Comparing `BTKSorgu-1.0.1/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.0.2/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.1/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.0.2/BTKSorgu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.1
+Version: 1.0.2
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,14 +28,16 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)
 
 [![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
+![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/Shared/SS.png)
+
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
 # Yüklemek
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.1 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.2 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -16,16 +16,17 @@
 img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white) !
 [PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white) ![PyPI
 - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 BTKSorgu?logo=pypi&logoColor=white) [![PyPI YÃ¼kle](https://github.com/
 keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://
 github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml) *Hedef
-websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* [![ForTheBadge made-
-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
+websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* ![BTKSorgu](https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/Shared/SS.png) [![ForTheBadge
+made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
 (https://www.python.org/) [![ForTheBadge built-with-love](https://
 ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
 keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install BTKSorgu #
 GÃ¼ncellemek pip install -U BTKSorgu ``` ## ð KullanÄ±m ```python from
 BTKSorgu import BTKSorgu from time import time basla = time() print(BTKSorgu
 ("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105
 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime
```

### Comparing `BTKSorgu-1.0.1/LICENSE` & `BTKSorgu-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.1/PKG-INFO` & `BTKSorgu-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.1
+Version: 1.0.2
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,14 +28,16 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)
 
 [![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
+![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/Shared/SS.png)
+
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
 # Yüklemek
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.1 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.2 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -16,16 +16,17 @@
 img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white) !
 [PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white) ![PyPI
 - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 BTKSorgu?logo=pypi&logoColor=white) [![PyPI YÃ¼kle](https://github.com/
 keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://
 github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml) *Hedef
-websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* [![ForTheBadge made-
-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
+websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* ![BTKSorgu](https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/Shared/SS.png) [![ForTheBadge
+made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
 (https://www.python.org/) [![ForTheBadge built-with-love](https://
 ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
 keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install BTKSorgu #
 GÃ¼ncellemek pip install -U BTKSorgu ``` ## ð KullanÄ±m ```python from
 BTKSorgu import BTKSorgu from time import time basla = time() print(BTKSorgu
 ("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105
 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime
```

### Comparing `BTKSorgu-1.0.1/README.md` & `BTKSorgu-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)
 
 [![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
+![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/Shared/SS.png)
+
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
 # Yüklemek
```

#### html2text {}

```diff
@@ -8,16 +8,17 @@
 img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white) !
 [PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white) ![PyPI
 - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 BTKSorgu?logo=pypi&logoColor=white) [![PyPI YÃ¼kle](https://github.com/
 keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://
 github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml) *Hedef
-websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* [![ForTheBadge made-
-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
+websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* ![BTKSorgu](https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/Shared/SS.png) [![ForTheBadge
+made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
 (https://www.python.org/) [![ForTheBadge built-with-love](https://
 ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
 keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install BTKSorgu #
 GÃ¼ncellemek pip install -U BTKSorgu ``` ## ð KullanÄ±m ```python from
 BTKSorgu import BTKSorgu from time import time basla = time() print(BTKSorgu
 ("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105
 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime
```

### Comparing `BTKSorgu-1.0.1/setup.py` & `BTKSorgu-1.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.0.1",
+    version      = "1.0.2",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -26,24 +26,35 @@
     python_requires  = ">=3.10",
     install_requires = [
         "setuptools",
         "wheel",
         "Kekik",
         "requests",
         "parsel",
+        "cssselect",
         "regex",
         "Pillow",
-        "pytesseract"
+        "pytesseract",
+        "sv_ttk"
     ],
 
     # ? Konsoldan Çalıştırılabilir
     entry_points = {
         "console_scripts": [
-            "BTKSorgu = BTKSorgu.konsol:basla",
+            "BTKSorgu    = BTKSorgu.konsol:basla",
+            "BTKSorguGUI = BTKSorgu.arayuz:basla"
         ]
     },
 
+    # ? Masaüstü Paketi
+    setup_requires = ["install_freedesktop"],
+    data_files     = [
+        ("share/applications",                ["Shared/org.KekikAkademi.BTKSorgu.desktop"]),
+        ("share/appdata",                     ["Shared/org.KekikAkademi.BTKSorgu.appdata.xml"]),
+        ("share/icons/hicolor/scalable/apps", ["Shared/org.KekikAkademi.BTKSorgu.svg"])
+    ],
+
     # ? PyPI Bilgileri
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True
 )
```

