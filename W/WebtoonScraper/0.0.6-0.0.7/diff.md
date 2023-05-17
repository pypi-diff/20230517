# Comparing `tmp/WebtoonScraper-0.0.6.tar.gz` & `tmp/WebtoonScraper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebtoonScraper-0.0.6.tar", last modified: Wed May 17 14:11:47 2023, max compression
+gzip compressed data, was "WebtoonScraper-0.0.7.tar", last modified: Wed May 17 14:16:54 2023, max compression
```

## Comparing `WebtoonScraper-0.0.6.tar` & `WebtoonScraper-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 14:11:47.685099 WebtoonScraper-0.0.6/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       56 2023-05-17 13:57:54.000000 WebtoonScraper-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2134 2023-05-17 14:11:47.685099 WebtoonScraper-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-05-15 00:37:37.000000 WebtoonScraper-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 14:11:47.663260 WebtoonScraper-0.0.6/WebtoonScraper/
--rw-rw-rw-   0        0        0      167 2023-05-17 14:07:13.000000 WebtoonScraper-0.0.6/WebtoonScraper/__init__.py
--rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.0.6/WebtoonScraper/foldermanagement.py
--rw-rw-rw-   0        0        0      682 2023-05-17 13:42:15.000000 WebtoonScraper-0.0.6/WebtoonScraper/getsoup.py
--rw-rw-rw-   0        0        0    11320 2023-05-17 13:41:09.000000 WebtoonScraper-0.0.6/WebtoonScraper/scraper.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:11:47.682333 WebtoonScraper-0.0.6/WebtoonScraper.egg-info/
--rw-rw-rw-   0        0        0     2134 2023-05-17 14:11:47.000000 WebtoonScraper-0.0.6/WebtoonScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-05-17 14:11:47.000000 WebtoonScraper-0.0.6/WebtoonScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 14:11:47.000000 WebtoonScraper-0.0.6/WebtoonScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 13:47:53.000000 WebtoonScraper-0.0.6/WebtoonScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-05-17 14:11:47.000000 WebtoonScraper-0.0.6/WebtoonScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-17 14:11:47.000000 WebtoonScraper-0.0.6/WebtoonScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    52914 2023-05-15 00:27:14.000000 WebtoonScraper-0.0.6/example1.png
--rw-rw-rw-   0        0        0       42 2023-05-17 14:11:47.685099 WebtoonScraper-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1326 2023-05-17 14:11:45.000000 WebtoonScraper-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:11:47.684087 WebtoonScraper-0.0.6/tests/
--rw-rw-rw-   0        0        0        0 2023-05-17 09:28:57.000000 WebtoonScraper-0.0.6/tests/__init__.py
--rw-rw-rw-   0        0        0      128 2023-05-16 14:18:05.000000 WebtoonScraper-0.0.6/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:16:54.895525 WebtoonScraper-0.0.7/
+-rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-05-17 13:57:54.000000 WebtoonScraper-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2134 2023-05-17 14:16:54.895525 WebtoonScraper-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2023-05-15 00:37:37.000000 WebtoonScraper-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 14:16:54.876461 WebtoonScraper-0.0.7/WebtoonScraper/
+-rw-rw-rw-   0        0        0      165 2023-05-17 14:15:41.000000 WebtoonScraper-0.0.7/WebtoonScraper/__init__.py
+-rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.0.7/WebtoonScraper/foldermanagement.py
+-rw-rw-rw-   0        0        0      682 2023-05-17 13:42:15.000000 WebtoonScraper-0.0.7/WebtoonScraper/getsoup.py
+-rw-rw-rw-   0        0        0    11309 2023-05-17 14:16:32.000000 WebtoonScraper-0.0.7/WebtoonScraper/scraper.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:16:54.892513 WebtoonScraper-0.0.7/WebtoonScraper.egg-info/
+-rw-rw-rw-   0        0        0     2134 2023-05-17 14:16:54.000000 WebtoonScraper-0.0.7/WebtoonScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-05-17 14:16:54.000000 WebtoonScraper-0.0.7/WebtoonScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 14:16:54.000000 WebtoonScraper-0.0.7/WebtoonScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-0.0.7/WebtoonScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-05-17 14:16:54.000000 WebtoonScraper-0.0.7/WebtoonScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-17 14:16:54.000000 WebtoonScraper-0.0.7/WebtoonScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    52914 2023-05-15 00:27:14.000000 WebtoonScraper-0.0.7/example1.png
+-rw-rw-rw-   0        0        0       42 2023-05-17 14:16:54.895525 WebtoonScraper-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2023-05-17 14:16:52.000000 WebtoonScraper-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:16:54.894526 WebtoonScraper-0.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-17 09:28:57.000000 WebtoonScraper-0.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      128 2023-05-16 14:18:05.000000 WebtoonScraper-0.0.7/tests/tests.py
```

### Comparing `WebtoonScraper-0.0.6/LICENSE` & `WebtoonScraper-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.6/PKG-INFO` & `WebtoonScraper-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 0.0.6
+Version: 0.0.7
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Never Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `WebtoonScraper-0.0.6/README.md` & `WebtoonScraper-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.6/WebtoonScraper/foldermanagement.py` & `WebtoonScraper-0.0.7/WebtoonScraper/foldermanagement.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.6/WebtoonScraper/getsoup.py` & `WebtoonScraper-0.0.7/WebtoonScraper/getsoup.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.6/WebtoonScraper/scraper.py` & `WebtoonScraper-0.0.7/WebtoonScraper/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # 네이버 웹툰 fetching(공식, 비동기적)
 import requests
 from bs4 import BeautifulSoup as bs
 import re
 import os
-import pickle
 import re
 import asyncio
 import functools
-import getsoup as getsoup
+import WebtoonScraper.getsoup
 from tqdm import tqdm
 import shutil
 
 class NaverWebtoonScraper:
     def __init__(self):
         # for aviod 403 error / user agent or Chrome
         self.user_agent = {'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36'}
```

### Comparing `WebtoonScraper-0.0.6/WebtoonScraper.egg-info/PKG-INFO` & `WebtoonScraper-0.0.7/WebtoonScraper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 0.0.6
+Version: 0.0.7
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Never Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `WebtoonScraper-0.0.6/example1.png` & `WebtoonScraper-0.0.7/example1.png`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.6/setup.py` & `WebtoonScraper-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # long_description = (this_directory / "README.md").read_text()
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='WebtoonScraper',
-    version='0.0.6',
+    version='0.0.7',
     description='Scraping webtoons and some utils for it',
     author='ilotoki0804',
     author_email='ilotoki0804@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/ilotoki0804/WebtoonScraper',
```

