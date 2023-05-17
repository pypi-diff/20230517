# Comparing `tmp/BTKSorgu-1.0.5.tar.gz` & `tmp/BTKSorgu-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.0.5.tar", last modified: Wed May 17 16:01:42 2023, max compression
+gzip compressed data, was "BTKSorgu-1.0.6.tar", last modified: Wed May 17 18:51:25 2023, max compression
```

## Comparing `BTKSorgu-1.0.5.tar` & `BTKSorgu-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:42.352206 BTKSorgu-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:42.352206 BTKSorgu-1.0.5/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/BTKSorgu/konsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/BTKSorgu/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:42.352206 BTKSorgu-1.0.5/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-17 16:01:42.000000 BTKSorgu-1.0.5/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 16:01:42.000000 BTKSorgu-1.0.5/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:01:42.000000 BTKSorgu-1.0.5/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 16:01:42.000000 BTKSorgu-1.0.5/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 16:01:42.000000 BTKSorgu-1.0.5/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 16:01:42.000000 BTKSorgu-1.0.5/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-17 16:01:42.352206 BTKSorgu-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:42.352206 BTKSorgu-1.0.5/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 16:01:42.352206 BTKSorgu-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-17 16:01:20.000000 BTKSorgu-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:51:25.797626 BTKSorgu-1.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:51:25.797626 BTKSorgu-1.0.6/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:51:25.797626 BTKSorgu-1.0.6/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-17 18:51:25.000000 BTKSorgu-1.0.6/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 18:51:25.000000 BTKSorgu-1.0.6/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:51:25.000000 BTKSorgu-1.0.6/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 18:51:25.000000 BTKSorgu-1.0.6/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 18:51:25.000000 BTKSorgu-1.0.6/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 18:51:25.000000 BTKSorgu-1.0.6/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-17 18:51:25.797626 BTKSorgu-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:51:25.797626 BTKSorgu-1.0.6/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:51:25.797626 BTKSorgu-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-17 18:50:59.000000 BTKSorgu-1.0.6/setup.py
```

### Comparing `BTKSorgu-1.0.5/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.0.6/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.5/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.0.6/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.5/BTKSorgu/arayuz.py` & `BTKSorgu-1.0.6/BTKSorgu/arayuz.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.5/BTKSorgu/konsol.py` & `BTKSorgu-1.0.6/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.5/BTKSorgu/logo.png` & `BTKSorgu-1.0.6/BTKSorgu/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.5/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,59 @@
-Metadata-Version: 2.1
-Name: BTKSorgu
-Version: 1.0.5
-Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
-Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
-Author: keyiflerolsun
-Author-email: keyiflerolsun@gmail.com
-License: GPLv3+
-Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 🔍 BTKSorgu
 
 ![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)
 ![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
 ![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white)
 ![License](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)
 
-![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)
+[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
 
 [![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
 
+[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+[![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
 ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
+### <img width="14" src="./.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
 ```
 
+### <img width="14" src="./.github/icons/flatpak.svg"> FlatHub (UI)
+
+```bash
+# Yüklemek
+flatpak install flathub org.kekikakademi.ntvHaber
+
+# Çalıştırmak
+flatpak run org.kekikakademi.ntvHaber
+```
+
 ## 📝 Kullanım
 
+### <img width="14" src="./.github/icons/python.svg"> Lib
+
 ```python
 from BTKSorgu import BTKSorgu
 from time     import time
 
 basla = time()
 print(BTKSorgu("redtube.com"))
     # » redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
@@ -62,20 +63,31 @@
     # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
 bitir = time()
 
 print(bitir-basla)
     # » 8.352766513824463
 ```
 
+### <img width="14" src="./.github/icons/iterm2.svg"> CLI
+
 ```bash
 BTKSorgu keyiflerolsun.dev
 
 # > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
 ```
 
+### <img width="14" src="./.github/icons/freedesktop.svg"> UI
+
+```bash
+BTKSorguGUI
+
+# veya
+flatpak run org.kekikakademi.ntvHaber
+```
+
 ## 🔖 Program Akış Şeması
 
 1. *Oturum Başlat,*
 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
 3. *Dönen kaynak kodundan doğrulama resmini indir,*
 4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
 5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
@@ -88,14 +100,15 @@
 > Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751412-selenium-vs-requests.html)**
 
 ## 📝 Proje İlerlemesi
 
 - ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
 - ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
 - ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
+- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
 
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
```

#### html2text {}

```diff
@@ -1,67 +1,73 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.5 Summary: Hedef websitesinin
-BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
-keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
-keyiflerolsun@gmail.com License: GPLv3+ Keywords:
-BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
-Production/Stable Classifier: License :: OSI Approved :: GNU General Public
-License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE # ð BTKSorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
+# ð BTKSorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
 keyiflerolsun/BTKSorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme](https://
 hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
 keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/
 âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/
 pyversions/BTKSorgu?logo=python&logoColor=white) ![License](https://
 img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white) ![Status](https://
-img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white) !
-[PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white) ![PyPI
-- Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/
-BTKSorgu?logo=pypi&logoColor=white) [![PyPI YÃ¼kle](https://github.com/
-keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://
-github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml) *Hedef
-websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* ![BTKSorgu](https://
-raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png) [!
-[ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](https://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install BTKSorgu #
-GÃ¼ncellemek pip install -U BTKSorgu ``` ## ð KullanÄ±m ```python from
-BTKSorgu import BTKSorgu from time import time basla = time() print(BTKSorgu
-("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105
-sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime
-engellenmiÅtir. print(BTKSorgu("kekikakademi.org")) # Â» Bilgi Teknolojileri
-ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar bulunamadÄ±. print
-(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-
-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime
-engellenmiÅtir. bitir = time() print(bitir-basla) # Â» 8.352766513824463 ```
-```bash BTKSorgu keyiflerolsun.dev # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu
-tarafÄ±ndan uygulanan bir karar bulunamadÄ±. ``` ## ð Program AkÄ±Å
-ÅemasÄ± 1. *Oturum BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://
-internet2.btk.gov.tr/) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri
-ye,* 3. *DÃ¶nen kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama
-resmini OCR ile harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini
-okuduÄun doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ±
-ayrÄ±ÅtÄ±rÄ±p edip geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak
-kodlu olarak paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu
-**gereksiz kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
+img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white) [!
+[PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)]
+(https://pypi.org/project/BTKSorgu) [![PyPI - Downloads](https://
+img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/
+project/BTKSorgu) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
+BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu) [![PyPI
+YÃ¼kle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/
+KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/
+workflows/KekikFlow.yml) [![FlatHub](https://img.shields.io/flathub/v/
+org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
+tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - Downloads](https://
+img.shields.io/flathub/downloads/
+org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
+tr/apps/org.KekikAkademi.BTKSorgu) *Hedef websitesinin BTK TarafÄ±ndan EriÅim
+Engeli Sorgusu..* ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
+BTKSorgu/main/Shared/SS.png) [![ForTheBadge made-with-python](https://
+ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ###
+[./.github/icons/pypi.svg] PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip
+install BTKSorgu # GÃ¼ncellemek pip install -U BTKSorgu ``` ### [./.github/
+icons/flatpak.svg] FlatHub (UI) ```bash # YÃ¼klemek flatpak install flathub
+org.kekikakademi.ntvHaber # ÃalÄ±ÅtÄ±rmak flatpak run
+org.kekikakademi.ntvHaber ``` ## ð KullanÄ±m ### [./.github/icons/
+python.svg] Lib ```python from BTKSorgu import BTKSorgu from time import time
+basla = time() print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008
+tarihli ve 410.01.02.2008-028105 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim
+BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime engellenmiÅtir. print(BTKSorgu
+("kekikakademi.org")) # Â» Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan
+uygulanan bir karar bulunamadÄ±. print(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/
+02/2008 tarihli ve 410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim
+BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-
+basla) # Â» 8.352766513824463 ``` ### [./.github/icons/iterm2.svg] CLI ```bash
+BTKSorgu keyiflerolsun.dev # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu
+tarafÄ±ndan uygulanan bir karar bulunamadÄ±. ``` ### [./.github/icons/
+freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
+org.kekikakademi.ntvHaber ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
+BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
+) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
+kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
+harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
+doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
+geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
+paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu **gereksiz
+kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
 etmektirâ¦* > TarayÄ±cÄ± Otomasyonu : *[Selenium IDE](https://
 www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://
 www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *
 [BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 > KarÅÄ±laÅtÄ±rmasÄ± : **[Selenium VS Requests](https://www.r10.net/off-
 topic/2751412-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
 [@raifpy](https://github.com/raifpy)** *tarafÄ±ndan kodlanmÄ±Å projenin hantal
 bir bileÅeni itinayla `dÄ±zz ð`'lanmÄ±ÅtÄ±r..* - â **Selenium**
 *baÄÄ±mlÄ±lÄ±ÄÄ±ndan dolayÄ± hantal Ã§alÄ±Åan kod yapÄ±sÄ± tamamen
 ayÄ±klanÄ±p bÃ¼tÃ¼n iÅ* `requests`*'e yaptÄ±rÄ±lÄ±p ciddi miktarda kaynak ve
 zaman tasarrufu ettirilmiÅtir..* - â *Kolay eriÅilebilir olmasÄ± ve ilham
-yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* ## ð Telif HakkÄ±
-ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
-keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
-(https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na
-gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
-isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
-(https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https:/
-/KekikAkademi.org/Kahve)** ## > **[@KekikAkademi](https://t.me/KekikAkademi)**
-*iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
+*ile basit bir arayÃ¼z tasarlanmÄ±ÅtÄ±r ve eÄitim amacÄ±yla Depolara
+yÃ¼klenmiÅtir..* ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
+[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
+PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
+BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
+â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
+mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
+ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `BTKSorgu-1.0.5/LICENSE` & `BTKSorgu-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.5/PKG-INFO` & `BTKSorgu-1.0.6/BTKSorgu.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.0.5
+Version: 1.0.6
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,39 +20,56 @@
 ![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
 ![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white)
 ![License](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)
 
-![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)
+[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
 
 [![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
 
+[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+[![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
 ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
+### <img width="14" src="./.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
 ```
 
+### <img width="14" src="./.github/icons/flatpak.svg"> FlatHub (UI)
+
+```bash
+# Yüklemek
+flatpak install flathub org.kekikakademi.ntvHaber
+
+# Çalıştırmak
+flatpak run org.kekikakademi.ntvHaber
+```
+
 ## 📝 Kullanım
 
+### <img width="14" src="./.github/icons/python.svg"> Lib
+
 ```python
 from BTKSorgu import BTKSorgu
 from time     import time
 
 basla = time()
 print(BTKSorgu("redtube.com"))
     # » redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
@@ -62,20 +79,31 @@
     # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
 bitir = time()
 
 print(bitir-basla)
     # » 8.352766513824463
 ```
 
+### <img width="14" src="./.github/icons/iterm2.svg"> CLI
+
 ```bash
 BTKSorgu keyiflerolsun.dev
 
 # > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
 ```
 
+### <img width="14" src="./.github/icons/freedesktop.svg"> UI
+
+```bash
+BTKSorguGUI
+
+# veya
+flatpak run org.kekikakademi.ntvHaber
+```
+
 ## 🔖 Program Akış Şeması
 
 1. *Oturum Başlat,*
 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
 3. *Dönen kaynak kodundan doğrulama resmini indir,*
 4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
 5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
@@ -88,14 +116,15 @@
 > Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751412-selenium-vs-requests.html)**
 
 ## 📝 Proje İlerlemesi
 
 - ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
 - ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
 - ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
+- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
 
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
```

#### html2text {}

```diff
@@ -1,67 +1,81 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.5 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.6 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # ð BTKSorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
 keyiflerolsun/BTKSorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme](https://
 hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
 keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/
 âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/
 pyversions/BTKSorgu?logo=python&logoColor=white) ![License](https://
 img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white) ![Status](https://
-img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white) !
-[PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white) ![PyPI
-- Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/
-BTKSorgu?logo=pypi&logoColor=white) [![PyPI YÃ¼kle](https://github.com/
-keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://
-github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml) *Hedef
-websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* ![BTKSorgu](https://
-raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png) [!
-[ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](https://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install BTKSorgu #
-GÃ¼ncellemek pip install -U BTKSorgu ``` ## ð KullanÄ±m ```python from
-BTKSorgu import BTKSorgu from time import time basla = time() print(BTKSorgu
-("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105
-sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime
-engellenmiÅtir. print(BTKSorgu("kekikakademi.org")) # Â» Bilgi Teknolojileri
-ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar bulunamadÄ±. print
-(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-
-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime
-engellenmiÅtir. bitir = time() print(bitir-basla) # Â» 8.352766513824463 ```
-```bash BTKSorgu keyiflerolsun.dev # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu
-tarafÄ±ndan uygulanan bir karar bulunamadÄ±. ``` ## ð Program AkÄ±Å
-ÅemasÄ± 1. *Oturum BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://
-internet2.btk.gov.tr/) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri
-ye,* 3. *DÃ¶nen kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama
-resmini OCR ile harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini
-okuduÄun doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ±
-ayrÄ±ÅtÄ±rÄ±p edip geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak
-kodlu olarak paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu
-**gereksiz kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
+img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white) [!
+[PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)]
+(https://pypi.org/project/BTKSorgu) [![PyPI - Downloads](https://
+img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/
+project/BTKSorgu) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
+BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu) [![PyPI
+YÃ¼kle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/
+KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/
+workflows/KekikFlow.yml) [![FlatHub](https://img.shields.io/flathub/v/
+org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
+tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - Downloads](https://
+img.shields.io/flathub/downloads/
+org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
+tr/apps/org.KekikAkademi.BTKSorgu) *Hedef websitesinin BTK TarafÄ±ndan EriÅim
+Engeli Sorgusu..* ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
+BTKSorgu/main/Shared/SS.png) [![ForTheBadge made-with-python](https://
+ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ###
+[./.github/icons/pypi.svg] PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip
+install BTKSorgu # GÃ¼ncellemek pip install -U BTKSorgu ``` ### [./.github/
+icons/flatpak.svg] FlatHub (UI) ```bash # YÃ¼klemek flatpak install flathub
+org.kekikakademi.ntvHaber # ÃalÄ±ÅtÄ±rmak flatpak run
+org.kekikakademi.ntvHaber ``` ## ð KullanÄ±m ### [./.github/icons/
+python.svg] Lib ```python from BTKSorgu import BTKSorgu from time import time
+basla = time() print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008
+tarihli ve 410.01.02.2008-028105 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim
+BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime engellenmiÅtir. print(BTKSorgu
+("kekikakademi.org")) # Â» Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan
+uygulanan bir karar bulunamadÄ±. print(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/
+02/2008 tarihli ve 410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim
+BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-
+basla) # Â» 8.352766513824463 ``` ### [./.github/icons/iterm2.svg] CLI ```bash
+BTKSorgu keyiflerolsun.dev # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu
+tarafÄ±ndan uygulanan bir karar bulunamadÄ±. ``` ### [./.github/icons/
+freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
+org.kekikakademi.ntvHaber ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
+BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
+) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
+kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
+harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
+doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
+geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
+paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu **gereksiz
+kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
 etmektirâ¦* > TarayÄ±cÄ± Otomasyonu : *[Selenium IDE](https://
 www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://
 www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *
 [BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 > KarÅÄ±laÅtÄ±rmasÄ± : **[Selenium VS Requests](https://www.r10.net/off-
 topic/2751412-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
 [@raifpy](https://github.com/raifpy)** *tarafÄ±ndan kodlanmÄ±Å projenin hantal
 bir bileÅeni itinayla `dÄ±zz ð`'lanmÄ±ÅtÄ±r..* - â **Selenium**
 *baÄÄ±mlÄ±lÄ±ÄÄ±ndan dolayÄ± hantal Ã§alÄ±Åan kod yapÄ±sÄ± tamamen
 ayÄ±klanÄ±p bÃ¼tÃ¼n iÅ* `requests`*'e yaptÄ±rÄ±lÄ±p ciddi miktarda kaynak ve
 zaman tasarrufu ettirilmiÅtir..* - â *Kolay eriÅilebilir olmasÄ± ve ilham
-yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* ## ð Telif HakkÄ±
-ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
-keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
-(https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na
-gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
-isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
-(https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https:/
-/KekikAkademi.org/Kahve)** ## > **[@KekikAkademi](https://t.me/KekikAkademi)**
-*iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
+*ile basit bir arayÃ¼z tasarlanmÄ±ÅtÄ±r ve eÄitim amacÄ±yla Depolara
+yÃ¼klenmiÅtir..* ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
+[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
+PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
+BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
+â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
+mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
+ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `BTKSorgu-1.0.5/README.md` & `BTKSorgu-1.0.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,75 @@
+Metadata-Version: 2.1
+Name: BTKSorgu
+Version: 1.0.6
+Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
+Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
+Author: keyiflerolsun
+Author-email: keyiflerolsun@gmail.com
+License: GPLv3+
+Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 🔍 BTKSorgu
 
 ![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)
 ![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
 ![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white)
 ![License](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)
 
-![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)
+[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
 
 [![PyPI Yükle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml)
 
+[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+[![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
 ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
+### <img width="14" src="./.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
 ```
 
+### <img width="14" src="./.github/icons/flatpak.svg"> FlatHub (UI)
+
+```bash
+# Yüklemek
+flatpak install flathub org.kekikakademi.ntvHaber
+
+# Çalıştırmak
+flatpak run org.kekikakademi.ntvHaber
+```
+
 ## 📝 Kullanım
 
+### <img width="14" src="./.github/icons/python.svg"> Lib
+
 ```python
 from BTKSorgu import BTKSorgu
 from time     import time
 
 basla = time()
 print(BTKSorgu("redtube.com"))
     # » redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
@@ -46,20 +79,31 @@
     # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
 bitir = time()
 
 print(bitir-basla)
     # » 8.352766513824463
 ```
 
+### <img width="14" src="./.github/icons/iterm2.svg"> CLI
+
 ```bash
 BTKSorgu keyiflerolsun.dev
 
 # > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
 ```
 
+### <img width="14" src="./.github/icons/freedesktop.svg"> UI
+
+```bash
+BTKSorguGUI
+
+# veya
+flatpak run org.kekikakademi.ntvHaber
+```
+
 ## 🔖 Program Akış Şeması
 
 1. *Oturum Başlat,*
 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
 3. *Dönen kaynak kodundan doğrulama resmini indir,*
 4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
 5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
@@ -72,14 +116,15 @@
 > Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751412-selenium-vs-requests.html)**
 
 ## 📝 Proje İlerlemesi
 
 - ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
 - ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
 - ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
+- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
 
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
```

#### html2text {}

```diff
@@ -1,59 +1,81 @@
-# ð BTKSorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.0.6 Summary: Hedef websitesinin
+BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
+keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
+keyiflerolsun@gmail.com License: GPLv3+ Keywords:
+BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
+Production/Stable Classifier: License :: OSI Approved :: GNU General Public
+License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
+LICENSE # ð BTKSorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
 keyiflerolsun/BTKSorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme](https://
 hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
 keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/
 âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/
 pyversions/BTKSorgu?logo=python&logoColor=white) ![License](https://
 img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white) ![Status](https://
-img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white) !
-[PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white) ![PyPI
-- Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/
-BTKSorgu?logo=pypi&logoColor=white) [![PyPI YÃ¼kle](https://github.com/
-keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://
-github.com/keyiflerolsun/BTKSorgu/actions/workflows/KekikFlow.yml) *Hedef
-websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* ![BTKSorgu](https://
-raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png) [!
-[ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](https://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install BTKSorgu #
-GÃ¼ncellemek pip install -U BTKSorgu ``` ## ð KullanÄ±m ```python from
-BTKSorgu import BTKSorgu from time import time basla = time() print(BTKSorgu
-("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105
-sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime
-engellenmiÅtir. print(BTKSorgu("kekikakademi.org")) # Â» Bilgi Teknolojileri
-ve Ä°letiÅim Kurumu tarafÄ±ndan uygulanan bir karar bulunamadÄ±. print
-(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-
-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime
-engellenmiÅtir. bitir = time() print(bitir-basla) # Â» 8.352766513824463 ```
-```bash BTKSorgu keyiflerolsun.dev # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu
-tarafÄ±ndan uygulanan bir karar bulunamadÄ±. ``` ## ð Program AkÄ±Å
-ÅemasÄ± 1. *Oturum BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://
-internet2.btk.gov.tr/) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri
-ye,* 3. *DÃ¶nen kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama
-resmini OCR ile harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini
-okuduÄun doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ±
-ayrÄ±ÅtÄ±rÄ±p edip geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak
-kodlu olarak paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu
-**gereksiz kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
+img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white) [!
+[PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)]
+(https://pypi.org/project/BTKSorgu) [![PyPI - Downloads](https://
+img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/
+project/BTKSorgu) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
+BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu) [![PyPI
+YÃ¼kle](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/
+KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/
+workflows/KekikFlow.yml) [![FlatHub](https://img.shields.io/flathub/v/
+org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
+tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - Downloads](https://
+img.shields.io/flathub/downloads/
+org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
+tr/apps/org.KekikAkademi.BTKSorgu) *Hedef websitesinin BTK TarafÄ±ndan EriÅim
+Engeli Sorgusu..* ![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
+BTKSorgu/main/Shared/SS.png) [![ForTheBadge made-with-python](https://
+ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ###
+[./.github/icons/pypi.svg] PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip
+install BTKSorgu # GÃ¼ncellemek pip install -U BTKSorgu ``` ### [./.github/
+icons/flatpak.svg] FlatHub (UI) ```bash # YÃ¼klemek flatpak install flathub
+org.kekikakademi.ntvHaber # ÃalÄ±ÅtÄ±rmak flatpak run
+org.kekikakademi.ntvHaber ``` ## ð KullanÄ±m ### [./.github/icons/
+python.svg] Lib ```python from BTKSorgu import BTKSorgu from time import time
+basla = time() print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008
+tarihli ve 410.01.02.2008-028105 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim
+BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime engellenmiÅtir. print(BTKSorgu
+("kekikakademi.org")) # Â» Bilgi Teknolojileri ve Ä°letiÅim Kurumu tarafÄ±ndan
+uygulanan bir karar bulunamadÄ±. print(BTKSorgu("xnxx.com")) # Â» xnxx.com, 23/
+02/2008 tarihli ve 410.01.02.2008-054003 sayÄ±lÄ± TelekomÃ¼nikasyon Ä°letiÅim
+BaÅkanlÄ±ÄÄ± kararÄ±yla eriÅime engellenmiÅtir. bitir = time() print(bitir-
+basla) # Â» 8.352766513824463 ``` ### [./.github/icons/iterm2.svg] CLI ```bash
+BTKSorgu keyiflerolsun.dev # > Bilgi Teknolojileri ve Ä°letiÅim Kurumu
+tarafÄ±ndan uygulanan bir karar bulunamadÄ±. ``` ### [./.github/icons/
+freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
+org.kekikakademi.ntvHaber ``` ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
+BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
+) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
+kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
+harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
+doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
+geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
+paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu **gereksiz
+kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
 etmektirâ¦* > TarayÄ±cÄ± Otomasyonu : *[Selenium IDE](https://
 www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://
 www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *
 [BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 > KarÅÄ±laÅtÄ±rmasÄ± : **[Selenium VS Requests](https://www.r10.net/off-
 topic/2751412-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
 [@raifpy](https://github.com/raifpy)** *tarafÄ±ndan kodlanmÄ±Å projenin hantal
 bir bileÅeni itinayla `dÄ±zz ð`'lanmÄ±ÅtÄ±r..* - â **Selenium**
 *baÄÄ±mlÄ±lÄ±ÄÄ±ndan dolayÄ± hantal Ã§alÄ±Åan kod yapÄ±sÄ± tamamen
 ayÄ±klanÄ±p bÃ¼tÃ¼n iÅ* `requests`*'e yaptÄ±rÄ±lÄ±p ciddi miktarda kaynak ve
 zaman tasarrufu ettirilmiÅtir..* - â *Kolay eriÅilebilir olmasÄ± ve ilham
-yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* ## ð Telif HakkÄ±
-ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
-keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
-(https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na
-gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
-isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
-(https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https:/
-/KekikAkademi.org/Kahve)** ## > **[@KekikAkademi](https://t.me/KekikAkademi)**
-*iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
+*ile basit bir arayÃ¼z tasarlanmÄ±ÅtÄ±r ve eÄitim amacÄ±yla Depolara
+yÃ¼klenmiÅtir..* ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
+[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
+PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
+BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
+â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
+mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
+ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `BTKSorgu-1.0.5/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.0.6/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 16% similar despite different names*

#### Comparing `BTKSorgu-1.0.5/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.0.6/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -25,14 +25,19 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
+    <release version="1.0.6" date="2023-5-17">
+      <description>
+        <p>Readme Düzenlendi..</p>
+      </description>
+    </release>
     <release version="1.0.5" date="2023-5-17">
       <description>
         <p>Proje Başlangıcı</p>
       </description>
     </release>
   </releases>
   <content_rating type="oars-1.1"/>
```

### Comparing `BTKSorgu-1.0.5/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.0.6/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.0.5/setup.py` & `BTKSorgu-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.0.5",
+    version      = "1.0.6",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

