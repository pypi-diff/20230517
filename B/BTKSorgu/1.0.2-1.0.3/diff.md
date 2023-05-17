# Comparing `tmp/BTKSorgu-1.0.2.tar.gz` & `tmp/BTKSorgu-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.0.2.tar", last modified: Wed May 17 14:20:17 2023, max compression
+gzip compressed data, was "BTKSorgu-1.0.3.tar", last modified: Wed May 17 14:21:58 2023, max compression
```

## Comparing `BTKSorgu-1.0.2.tar` & `BTKSorgu-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:17.455681 BTKSorgu-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:17.455681 BTKSorgu-1.0.2/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/BTKSorgu/konsol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:17.455681 BTKSorgu-1.0.2/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-17 14:20:17.000000 BTKSorgu-1.0.2/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 14:20:17.000000 BTKSorgu-1.0.2/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:20:17.000000 BTKSorgu-1.0.2/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 14:20:17.000000 BTKSorgu-1.0.2/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-17 14:20:17.000000 BTKSorgu-1.0.2/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 14:20:17.000000 BTKSorgu-1.0.2/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-17 14:20:17.455681 BTKSorgu-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:17.455681 BTKSorgu-1.0.2/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:20:17.455681 BTKSorgu-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-17 14:19:56.000000 BTKSorgu-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:21:58.974464 BTKSorgu-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:21:58.974464 BTKSorgu-1.0.3/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/BTKSorgu/konsol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:21:58.974464 BTKSorgu-1.0.3/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-17 14:21:58.000000 BTKSorgu-1.0.3/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 14:21:58.000000 BTKSorgu-1.0.3/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:21:58.000000 BTKSorgu-1.0.3/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 14:21:58.000000 BTKSorgu-1.0.3/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-17 14:21:58.000000 BTKSorgu-1.0.3/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 14:21:58.000000 BTKSorgu-1.0.3/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-17 14:21:58.974464 BTKSorgu-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:21:58.974464 BTKSorgu-1.0.3/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:21:58.974464 BTKSorgu-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-17 14:21:33.000000 BTKSorgu-1.0.3/setup.py
```

### Comparing `BTKSorgu-1.0.2/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.0.3/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.2/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.0.3/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.2/BTKSorgu/arayuz.py` & `BTKSorgu-1.0.3/BTKSorgu/arayuz.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.2/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.0.3/BTKSorgu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.2
+Version: 1.0.3
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)
 
 [![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
-![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/Shared/SS.png)
+![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.2 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.3 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -17,17 +17,17 @@
 [PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white) ![PyPI
 - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 BTKSorgu?logo=pypi&logoColor=white) [![PyPI YÃ¼kle](https://github.com/
 keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://
 github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml) *Hedef
 websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* ![BTKSorgu](https://
-raw.githubusercontent.com/keyiflerolsun/BTKSorgu/Shared/SS.png) [![ForTheBadge
-made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
-(https://www.python.org/) [![ForTheBadge built-with-love](https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png) [!
+[ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-
+python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](https://
 ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
 keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install BTKSorgu #
 GÃ¼ncellemek pip install -U BTKSorgu ``` ## ð KullanÄ±m ```python from
 BTKSorgu import BTKSorgu from time import time basla = time() print(BTKSorgu
 ("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105
 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime
 engellenmiÅtir. print(BTKSorgu("kekikakademi.org")) # Â» Bilgi Teknolojileri
```

### Comparing `BTKSorgu-1.0.2/LICENSE` & `BTKSorgu-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.2/PKG-INFO` & `BTKSorgu-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.2
+Version: 1.0.3
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)
 
 [![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
-![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/Shared/SS.png)
+![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.2 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.3 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -17,17 +17,17 @@
 [PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white) ![PyPI
 - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 BTKSorgu?logo=pypi&logoColor=white) [![PyPI YÃ¼kle](https://github.com/
 keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://
 github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml) *Hedef
 websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* ![BTKSorgu](https://
-raw.githubusercontent.com/keyiflerolsun/BTKSorgu/Shared/SS.png) [![ForTheBadge
-made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
-(https://www.python.org/) [![ForTheBadge built-with-love](https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png) [!
+[ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-
+python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](https://
 ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
 keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install BTKSorgu #
 GÃ¼ncellemek pip install -U BTKSorgu ``` ## ð KullanÄ±m ```python from
 BTKSorgu import BTKSorgu from time import time basla = time() print(BTKSorgu
 ("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105
 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime
 engellenmiÅtir. print(BTKSorgu("kekikakademi.org")) # Â» Bilgi Teknolojileri
```

### Comparing `BTKSorgu-1.0.2/README.md` & `BTKSorgu-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)
 
 [![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
-![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/Shared/SS.png)
+![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 [PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white) ![PyPI
 - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 BTKSorgu?logo=pypi&logoColor=white) [![PyPI YÃ¼kle](https://github.com/
 keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://
 github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml) *Hedef
 websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* ![BTKSorgu](https://
-raw.githubusercontent.com/keyiflerolsun/BTKSorgu/Shared/SS.png) [![ForTheBadge
-made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
-(https://www.python.org/) [![ForTheBadge built-with-love](https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png) [!
+[ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-
+python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](https://
 ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
 keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install BTKSorgu #
 GÃ¼ncellemek pip install -U BTKSorgu ``` ## ð KullanÄ±m ```python from
 BTKSorgu import BTKSorgu from time import time basla = time() print(BTKSorgu
 ("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105
 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime
 engellenmiÅtir. print(BTKSorgu("kekikakademi.org")) # Â» Bilgi Teknolojileri
```

### Comparing `BTKSorgu-1.0.2/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.0.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 2% similar despite different names*

#### Comparing `BTKSorgu-1.0.2/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.0.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -18,22 +18,22 @@
   </description>
   <description xml:lang="tr_TR">
     <p>Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..</p>
     <p>https://t.me/KekikAkademi için hazırlanmıştır..</p>
   </description>
   <screenshots>
     <screenshot type="default">
-      <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/Shared/SS.png</image>
+      <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.0.2" date="2023-5-17">
+    <release version="1.0.3" date="2023-5-17">
       <description>
         <p>Proje Başlangıcı</p>
       </description>
     </release>
   </releases>
   <content_rating type="oars-1.1"/>
 </component>
```

### Comparing `BTKSorgu-1.0.2/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.0.3/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.2/setup.py` & `BTKSorgu-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.0.2",
+    version      = "1.0.3",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

