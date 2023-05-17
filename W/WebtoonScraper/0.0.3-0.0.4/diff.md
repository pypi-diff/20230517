# Comparing `tmp/WebtoonScraper-0.0.3.tar.gz` & `tmp/WebtoonScraper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebtoonScraper-0.0.3.tar", last modified: Wed May 17 13:58:55 2023, max compression
+gzip compressed data, was "WebtoonScraper-0.0.4.tar", last modified: Wed May 17 14:01:30 2023, max compression
```

## Comparing `WebtoonScraper-0.0.3.tar` & `WebtoonScraper-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 13:58:55.988933 WebtoonScraper-0.0.3/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       56 2023-05-17 13:57:54.000000 WebtoonScraper-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2134 2023-05-17 13:58:55.988933 WebtoonScraper-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-05-15 00:37:37.000000 WebtoonScraper-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 13:58:55.977383 WebtoonScraper-0.0.3/WebtoonScraper/
--rw-rw-rw-   0        0        0      139 2023-05-17 13:57:09.000000 WebtoonScraper-0.0.3/WebtoonScraper/__init__.py
--rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.0.3/WebtoonScraper/foldermanagement.py
--rw-rw-rw-   0        0        0      682 2023-05-17 13:42:15.000000 WebtoonScraper-0.0.3/WebtoonScraper/getsoup.py
--rw-rw-rw-   0        0        0    11320 2023-05-17 13:41:09.000000 WebtoonScraper-0.0.3/WebtoonScraper/scraper.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:58:55.984978 WebtoonScraper-0.0.3/WebtoonScraper.egg-info/
--rw-rw-rw-   0        0        0     2134 2023-05-17 13:58:55.000000 WebtoonScraper-0.0.3/WebtoonScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-05-17 13:58:55.000000 WebtoonScraper-0.0.3/WebtoonScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 13:58:55.000000 WebtoonScraper-0.0.3/WebtoonScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 13:47:53.000000 WebtoonScraper-0.0.3/WebtoonScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-05-17 13:58:55.000000 WebtoonScraper-0.0.3/WebtoonScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-17 13:58:55.000000 WebtoonScraper-0.0.3/WebtoonScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    52914 2023-05-15 00:27:14.000000 WebtoonScraper-0.0.3/example1.png
--rw-rw-rw-   0        0        0       42 2023-05-17 13:58:55.989944 WebtoonScraper-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1326 2023-05-17 13:58:03.000000 WebtoonScraper-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:58:55.987427 WebtoonScraper-0.0.3/tests/
--rw-rw-rw-   0        0        0        0 2023-05-17 09:28:57.000000 WebtoonScraper-0.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0      128 2023-05-16 14:18:05.000000 WebtoonScraper-0.0.3/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:01:30.630475 WebtoonScraper-0.0.4/
+-rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-05-17 13:57:54.000000 WebtoonScraper-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2134 2023-05-17 14:01:30.630475 WebtoonScraper-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2023-05-15 00:37:37.000000 WebtoonScraper-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 14:01:30.611734 WebtoonScraper-0.0.4/WebtoonScraper/
+-rw-rw-rw-   0        0        0      167 2023-05-17 14:00:27.000000 WebtoonScraper-0.0.4/WebtoonScraper/__init__.py
+-rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.0.4/WebtoonScraper/foldermanagement.py
+-rw-rw-rw-   0        0        0      682 2023-05-17 13:42:15.000000 WebtoonScraper-0.0.4/WebtoonScraper/getsoup.py
+-rw-rw-rw-   0        0        0    11320 2023-05-17 13:41:09.000000 WebtoonScraper-0.0.4/WebtoonScraper/scraper.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:01:30.626742 WebtoonScraper-0.0.4/WebtoonScraper.egg-info/
+-rw-rw-rw-   0        0        0     2134 2023-05-17 14:01:30.000000 WebtoonScraper-0.0.4/WebtoonScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-05-17 14:01:30.000000 WebtoonScraper-0.0.4/WebtoonScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 14:01:30.000000 WebtoonScraper-0.0.4/WebtoonScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 13:47:53.000000 WebtoonScraper-0.0.4/WebtoonScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-05-17 14:01:30.000000 WebtoonScraper-0.0.4/WebtoonScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-17 14:01:30.000000 WebtoonScraper-0.0.4/WebtoonScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    52914 2023-05-15 00:27:14.000000 WebtoonScraper-0.0.4/example1.png
+-rw-rw-rw-   0        0        0       42 2023-05-17 14:01:30.630475 WebtoonScraper-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2023-05-17 14:01:26.000000 WebtoonScraper-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:01:30.629016 WebtoonScraper-0.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-17 09:28:57.000000 WebtoonScraper-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      128 2023-05-16 14:18:05.000000 WebtoonScraper-0.0.4/tests/tests.py
```

### Comparing `WebtoonScraper-0.0.3/LICENSE` & `WebtoonScraper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.3/PKG-INFO` & `WebtoonScraper-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 0.0.3
+Version: 0.0.4
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Never Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `WebtoonScraper-0.0.3/README.md` & `WebtoonScraper-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.3/WebtoonScraper/foldermanagement.py` & `WebtoonScraper-0.0.4/WebtoonScraper/foldermanagement.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.3/WebtoonScraper/getsoup.py` & `WebtoonScraper-0.0.4/WebtoonScraper/getsoup.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.3/WebtoonScraper/scraper.py` & `WebtoonScraper-0.0.4/WebtoonScraper/scraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.3/WebtoonScraper.egg-info/PKG-INFO` & `WebtoonScraper-0.0.4/WebtoonScraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 0.0.3
+Version: 0.0.4
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Never Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `WebtoonScraper-0.0.3/example1.png` & `WebtoonScraper-0.0.4/example1.png`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.3/setup.py` & `WebtoonScraper-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # long_description = (this_directory / "README.md").read_text()
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='WebtoonScraper',
-    version='0.0.3',
+    version='0.0.4',
     description='Scraping webtoons and some utils for it',
     author='ilotoki0804',
     author_email='ilotoki0804@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/ilotoki0804/WebtoonScraper',
```

