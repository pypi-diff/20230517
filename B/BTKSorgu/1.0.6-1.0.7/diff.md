# Comparing `tmp/BTKSorgu-1.0.6.tar.gz` & `tmp/BTKSorgu-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.0.6.tar", last modified: Wed May 17 18:51:25 2023, max compression
+gzip compressed data, was "BTKSorgu-1.0.7.tar", last modified: Wed May 17 18:54:58 2023, max compression
```

## Comparing `BTKSorgu-1.0.6.tar` & `BTKSorgu-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:51:25.797626 BTKSorgu-1.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:51:25.797626 BTKSorgu-1.0.6/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/BTKSorgu/konsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/BTKSorgu/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:51:25.797626 BTKSorgu-1.0.6/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-17 18:51:25.000000 BTKSorgu-1.0.6/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 18:51:25.000000 BTKSorgu-1.0.6/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:51:25.000000 BTKSorgu-1.0.6/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 18:51:25.000000 BTKSorgu-1.0.6/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 18:51:25.000000 BTKSorgu-1.0.6/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 18:51:25.000000 BTKSorgu-1.0.6/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-17 18:51:25.797626 BTKSorgu-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:51:25.797626 BTKSorgu-1.0.6/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:51:25.797626 BTKSorgu-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:54:58.522625 BTKSorgu-1.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:54:58.518625 BTKSorgu-1.0.7/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 18:54:39.000000 BTKSorgu-1.0.7/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 18:54:39.000000 BTKSorgu-1.0.7/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 18:54:39.000000 BTKSorgu-1.0.7/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-17 18:54:39.000000 BTKSorgu-1.0.7/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 18:54:39.000000 BTKSorgu-1.0.7/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-17 18:54:39.000000 BTKSorgu-1.0.7/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:54:58.518625 BTKSorgu-1.0.7/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-17 18:54:58.000000 BTKSorgu-1.0.7/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 18:54:58.000000 BTKSorgu-1.0.7/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:54:58.000000 BTKSorgu-1.0.7/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 18:54:58.000000 BTKSorgu-1.0.7/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 18:54:58.000000 BTKSorgu-1.0.7/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 18:54:58.000000 BTKSorgu-1.0.7/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 18:54:39.000000 BTKSorgu-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 18:54:39.000000 BTKSorgu-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-17 18:54:58.522625 BTKSorgu-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-05-17 18:54:39.000000 BTKSorgu-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:54:58.522625 BTKSorgu-1.0.7/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-17 18:54:39.000000 BTKSorgu-1.0.7/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 18:54:39.000000 BTKSorgu-1.0.7/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 18:54:39.000000 BTKSorgu-1.0.7/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:54:58.522625 BTKSorgu-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-17 18:54:39.000000 BTKSorgu-1.0.7/setup.py
```

### Comparing `BTKSorgu-1.0.6/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.0.7/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.6/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.0.7/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.6/BTKSorgu/arayuz.py` & `BTKSorgu-1.0.7/BTKSorgu/arayuz.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.6/BTKSorgu/konsol.py` & `BTKSorgu-1.0.7/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.6/BTKSorgu/logo.png` & `BTKSorgu-1.0.7/BTKSorgu/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.6/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.0.7/BTKSorgu.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.6
+Version: 1.0.7
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,44 +31,44 @@
 [![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
 
 [![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 [![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
-![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png)
+![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
-### <img width="14" src="./.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
 
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
 ```
 
-### <img width="14" src="./.github/icons/flatpak.svg"> FlatHub (UI)
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"> FlatHub (UI)
 
 ```bash
 # Yüklemek
 flatpak install flathub org.kekikakademi.ntvHaber
 
 # Çalıştırmak
 flatpak run org.kekikakademi.ntvHaber
 ```
 
 ## 📝 Kullanım
 
-### <img width="14" src="./.github/icons/python.svg"> Lib
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Lib
 
 ```python
 from BTKSorgu import BTKSorgu
 from time     import time
 
 basla = time()
 print(BTKSorgu("redtube.com"))
@@ -79,23 +79,23 @@
     # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
 bitir = time()
 
 print(bitir-basla)
     # » 8.352766513824463
 ```
 
-### <img width="14" src="./.github/icons/iterm2.svg"> CLI
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"> CLI
 
 ```bash
 BTKSorgu keyiflerolsun.dev
 
 # > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
 ```
 
-### <img width="14" src="./.github/icons/freedesktop.svg"> UI
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"> UI
 
 ```bash
 BTKSorguGUI
 
 # veya
 flatpak run org.kekikakademi.ntvHaber
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.6 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.7 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -24,35 +24,38 @@
 workflows/KekikFlow.yml) [![FlatHub](https://img.shields.io/flathub/v/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - Downloads](https://
 img.shields.io/flathub/downloads/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.KekikAkademi.BTKSorgu) *Hedef websitesinin BTK TarafÄ±ndan EriÅim
 Engeli Sorgusu..* ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
-BTKSorgu/main/Shared/SS.png) [![ForTheBadge made-with-python](https://
+BTKSorgu/main/.github/icons/SS.png) [![ForTheBadge made-with-python](https://
 ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ###
-[./.github/icons/pypi.svg] PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip
-install BTKSorgu # GÃ¼ncellemek pip install -U BTKSorgu ``` ### [./.github/
-icons/flatpak.svg] FlatHub (UI) ```bash # YÃ¼klemek flatpak install flathub
-org.kekikakademi.ntvHaber # ÃalÄ±ÅtÄ±rmak flatpak run
-org.kekikakademi.ntvHaber ``` ## ð KullanÄ±m ### [./.github/icons/
-python.svg] Lib ```python from BTKSorgu import BTKSorgu from time import time
-basla = time() print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008
-tarihli ve 410.01.02.2008-028105 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim
-BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime engellenmiÅtir. print(BTKSorgu
-("kekikakademi.org")) # Â» Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan
-uygulanan bir karar bulunamadÄ±. print(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/
-02/2008 tarihli ve 410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim
-BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-
-basla) # Â» 8.352766513824463 ``` ### [./.github/icons/iterm2.svg] CLI ```bash
-BTKSorgu keyiflerolsun.dev # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu
-tarafÄ±ndan uygulanan bir karar bulunamadÄ±. ``` ### [./.github/icons/
-freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https:/
+/raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
+PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
+pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
+keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg] FlatHub (UI) ```bash #
+YÃ¼klemek flatpak install flathub org.kekikakademi.ntvHaber # ÃalÄ±ÅtÄ±rmak
+flatpak run org.kekikakademi.ntvHaber ``` ## ð KullanÄ±m ### [https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg]
+Lib ```python from BTKSorgu import BTKSorgu from time import time basla = time
+() print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve
+410.01.02.2008-028105 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
+kararÄ±yla eriÅime engellenmiÅtir. print(BTKSorgu("kekikakademi.org")) # Â»
+Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
+bulunamadÄ±. print(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/02/2008 tarihli ve
+410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
+kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-basla) # Â»
+8.352766513824463 ``` ### [https://raw.githubusercontent.com/keyiflerolsun/
+BTKSorgu/main/.github/icons/iterm2.svg] CLI ```bash BTKSorgu keyiflerolsun.dev
+# > Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
+bulunamadÄ±. ``` ### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/
+main/.github/icons/freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
 org.kekikakademi.ntvHaber ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
 BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
 ) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
 kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
 harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
 doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
 geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
```

### Comparing `BTKSorgu-1.0.6/LICENSE` & `BTKSorgu-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.6/PKG-INFO` & `BTKSorgu-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.6
+Version: 1.0.7
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,44 +31,44 @@
 [![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
 
 [![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 [![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
-![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png)
+![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
-### <img width="14" src="./.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
 
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
 ```
 
-### <img width="14" src="./.github/icons/flatpak.svg"> FlatHub (UI)
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"> FlatHub (UI)
 
 ```bash
 # Yüklemek
 flatpak install flathub org.kekikakademi.ntvHaber
 
 # Çalıştırmak
 flatpak run org.kekikakademi.ntvHaber
 ```
 
 ## 📝 Kullanım
 
-### <img width="14" src="./.github/icons/python.svg"> Lib
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Lib
 
 ```python
 from BTKSorgu import BTKSorgu
 from time     import time
 
 basla = time()
 print(BTKSorgu("redtube.com"))
@@ -79,23 +79,23 @@
     # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
 bitir = time()
 
 print(bitir-basla)
     # » 8.352766513824463
 ```
 
-### <img width="14" src="./.github/icons/iterm2.svg"> CLI
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"> CLI
 
 ```bash
 BTKSorgu keyiflerolsun.dev
 
 # > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
 ```
 
-### <img width="14" src="./.github/icons/freedesktop.svg"> UI
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"> UI
 
 ```bash
 BTKSorguGUI
 
 # veya
 flatpak run org.kekikakademi.ntvHaber
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.6 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.7 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -24,35 +24,38 @@
 workflows/KekikFlow.yml) [![FlatHub](https://img.shields.io/flathub/v/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - Downloads](https://
 img.shields.io/flathub/downloads/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.KekikAkademi.BTKSorgu) *Hedef websitesinin BTK TarafÄ±ndan EriÅim
 Engeli Sorgusu..* ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
-BTKSorgu/main/Shared/SS.png) [![ForTheBadge made-with-python](https://
+BTKSorgu/main/.github/icons/SS.png) [![ForTheBadge made-with-python](https://
 ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ###
-[./.github/icons/pypi.svg] PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip
-install BTKSorgu # GÃ¼ncellemek pip install -U BTKSorgu ``` ### [./.github/
-icons/flatpak.svg] FlatHub (UI) ```bash # YÃ¼klemek flatpak install flathub
-org.kekikakademi.ntvHaber # ÃalÄ±ÅtÄ±rmak flatpak run
-org.kekikakademi.ntvHaber ``` ## ð KullanÄ±m ### [./.github/icons/
-python.svg] Lib ```python from BTKSorgu import BTKSorgu from time import time
-basla = time() print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008
-tarihli ve 410.01.02.2008-028105 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim
-BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime engellenmiÅtir. print(BTKSorgu
-("kekikakademi.org")) # Â» Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan
-uygulanan bir karar bulunamadÄ±. print(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/
-02/2008 tarihli ve 410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim
-BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-
-basla) # Â» 8.352766513824463 ``` ### [./.github/icons/iterm2.svg] CLI ```bash
-BTKSorgu keyiflerolsun.dev # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu
-tarafÄ±ndan uygulanan bir karar bulunamadÄ±. ``` ### [./.github/icons/
-freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https:/
+/raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
+PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
+pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
+keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg] FlatHub (UI) ```bash #
+YÃ¼klemek flatpak install flathub org.kekikakademi.ntvHaber # ÃalÄ±ÅtÄ±rmak
+flatpak run org.kekikakademi.ntvHaber ``` ## ð KullanÄ±m ### [https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg]
+Lib ```python from BTKSorgu import BTKSorgu from time import time basla = time
+() print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve
+410.01.02.2008-028105 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
+kararÄ±yla eriÅime engellenmiÅtir. print(BTKSorgu("kekikakademi.org")) # Â»
+Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
+bulunamadÄ±. print(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/02/2008 tarihli ve
+410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
+kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-basla) # Â»
+8.352766513824463 ``` ### [https://raw.githubusercontent.com/keyiflerolsun/
+BTKSorgu/main/.github/icons/iterm2.svg] CLI ```bash BTKSorgu keyiflerolsun.dev
+# > Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
+bulunamadÄ±. ``` ### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/
+main/.github/icons/freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
 org.kekikakademi.ntvHaber ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
 BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
 ) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
 kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
 harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
 doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
 geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
```

### Comparing `BTKSorgu-1.0.6/README.md` & `BTKSorgu-1.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -15,44 +15,44 @@
 [![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
 
 [![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 [![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
-![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png)
+![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
-### <img width="14" src="./.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
 
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
 ```
 
-### <img width="14" src="./.github/icons/flatpak.svg"> FlatHub (UI)
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"> FlatHub (UI)
 
 ```bash
 # Yüklemek
 flatpak install flathub org.kekikakademi.ntvHaber
 
 # Çalıştırmak
 flatpak run org.kekikakademi.ntvHaber
 ```
 
 ## 📝 Kullanım
 
-### <img width="14" src="./.github/icons/python.svg"> Lib
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"> Lib
 
 ```python
 from BTKSorgu import BTKSorgu
 from time     import time
 
 basla = time()
 print(BTKSorgu("redtube.com"))
@@ -63,23 +63,23 @@
     # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
 bitir = time()
 
 print(bitir-basla)
     # » 8.352766513824463
 ```
 
-### <img width="14" src="./.github/icons/iterm2.svg"> CLI
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"> CLI
 
 ```bash
 BTKSorgu keyiflerolsun.dev
 
 # > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
 ```
 
-### <img width="14" src="./.github/icons/freedesktop.svg"> UI
+### <img width="14" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"> UI
 
 ```bash
 BTKSorguGUI
 
 # veya
 flatpak run org.kekikakademi.ntvHaber
 ```
```

#### html2text {}

```diff
@@ -16,35 +16,38 @@
 workflows/KekikFlow.yml) [![FlatHub](https://img.shields.io/flathub/v/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - Downloads](https://
 img.shields.io/flathub/downloads/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
 tr/apps/org.KekikAkademi.BTKSorgu) *Hedef websitesinin BTK TarafÄ±ndan EriÅim
 Engeli Sorgusu..* ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
-BTKSorgu/main/Shared/SS.png) [![ForTheBadge made-with-python](https://
+BTKSorgu/main/.github/icons/SS.png) [![ForTheBadge made-with-python](https://
 ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ###
-[./.github/icons/pypi.svg] PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip
-install BTKSorgu # GÃ¼ncellemek pip install -U BTKSorgu ``` ### [./.github/
-icons/flatpak.svg] FlatHub (UI) ```bash # YÃ¼klemek flatpak install flathub
-org.kekikakademi.ntvHaber # ÃalÄ±ÅtÄ±rmak flatpak run
-org.kekikakademi.ntvHaber ``` ## ð KullanÄ±m ### [./.github/icons/
-python.svg] Lib ```python from BTKSorgu import BTKSorgu from time import time
-basla = time() print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008
-tarihli ve 410.01.02.2008-028105 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim
-BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime engellenmiÅtir. print(BTKSorgu
-("kekikakademi.org")) # Â» Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan
-uygulanan bir karar bulunamadÄ±. print(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/
-02/2008 tarihli ve 410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim
-BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-
-basla) # Â» 8.352766513824463 ``` ### [./.github/icons/iterm2.svg] CLI ```bash
-BTKSorgu keyiflerolsun.dev # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu
-tarafÄ±ndan uygulanan bir karar bulunamadÄ±. ``` ### [./.github/icons/
-freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https:/
+/raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
+PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
+pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
+keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg] FlatHub (UI) ```bash #
+YÃ¼klemek flatpak install flathub org.kekikakademi.ntvHaber # ÃalÄ±ÅtÄ±rmak
+flatpak run org.kekikakademi.ntvHaber ``` ## ð KullanÄ±m ### [https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg]
+Lib ```python from BTKSorgu import BTKSorgu from time import time basla = time
+() print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve
+410.01.02.2008-028105 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
+kararÄ±yla eriÅime engellenmiÅtir. print(BTKSorgu("kekikakademi.org")) # Â»
+Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
+bulunamadÄ±. print(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/02/2008 tarihli ve
+410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ±
+kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-basla) # Â»
+8.352766513824463 ``` ### [https://raw.githubusercontent.com/keyiflerolsun/
+BTKSorgu/main/.github/icons/iterm2.svg] CLI ```bash BTKSorgu keyiflerolsun.dev
+# > Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar
+bulunamadÄ±. ``` ### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/
+main/.github/icons/freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
 org.kekikakademi.ntvHaber ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
 BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
 ) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
 kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
 harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
 doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
 geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
```

### Comparing `BTKSorgu-1.0.6/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.0.7/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 5% similar despite different names*

#### Comparing `BTKSorgu-1.0.6/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.0.7/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -18,22 +18,22 @@
   </description>
   <description xml:lang="tr_TR">
     <p>Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..</p>
     <p>https://t.me/KekikAkademi için hazırlanmıştır..</p>
   </description>
   <screenshots>
     <screenshot type="default">
-      <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png</image>
+      <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.0.6" date="2023-5-17">
+    <release version="1.0.7" date="2023-5-17">
       <description>
         <p>Readme Düzenlendi..</p>
       </description>
     </release>
     <release version="1.0.5" date="2023-5-17">
       <description>
         <p>Proje Başlangıcı</p>
```

### Comparing `BTKSorgu-1.0.6/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.0.7/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.6/setup.py` & `BTKSorgu-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.0.6",
+    version      = "1.0.7",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

