# Comparing `tmp/WebtoonScraper-0.0.1.tar.gz` & `tmp/WebtoonScraper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebtoonScraper-0.0.1.tar", last modified: Mon May 15 00:47:46 2023, max compression
+gzip compressed data, was "WebtoonScraper-0.0.2.tar", last modified: Wed May 17 13:50:52 2023, max compression
```

## Comparing `WebtoonScraper-0.0.1.tar` & `WebtoonScraper-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 00:47:46.329487 WebtoonScraper-0.0.1/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      543 2023-05-15 00:47:46.328139 WebtoonScraper-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-05-15 00:37:37.000000 WebtoonScraper-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 00:47:46.326843 WebtoonScraper-0.0.1/WebtoonScraper.egg-info/
--rw-rw-rw-   0        0        0      543 2023-05-15 00:47:46.000000 WebtoonScraper-0.0.1/WebtoonScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-15 00:47:46.000000 WebtoonScraper-0.0.1/WebtoonScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 00:47:46.000000 WebtoonScraper-0.0.1/WebtoonScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 00:47:46.000000 WebtoonScraper-0.0.1/WebtoonScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2023-05-15 00:47:46.000000 WebtoonScraper-0.0.1/WebtoonScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 00:47:46.000000 WebtoonScraper-0.0.1/WebtoonScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 00:47:46.329487 WebtoonScraper-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      783 2023-05-15 00:47:26.000000 WebtoonScraper-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:50:52.072443 WebtoonScraper-0.0.2/
+-rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-17 13:35:57.000000 WebtoonScraper-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2134 2023-05-17 13:50:52.072443 WebtoonScraper-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2023-05-15 00:37:37.000000 WebtoonScraper-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 13:50:52.061103 WebtoonScraper-0.0.2/WebtoonScraper/
+-rw-rw-rw-   0        0        0      109 2023-05-17 13:49:34.000000 WebtoonScraper-0.0.2/WebtoonScraper/__init__.py
+-rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.0.2/WebtoonScraper/foldermanagement.py
+-rw-rw-rw-   0        0        0      682 2023-05-17 13:42:15.000000 WebtoonScraper-0.0.2/WebtoonScraper/getsoup.py
+-rw-rw-rw-   0        0        0    11320 2023-05-17 13:41:09.000000 WebtoonScraper-0.0.2/WebtoonScraper/scraper.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:50:52.068804 WebtoonScraper-0.0.2/WebtoonScraper.egg-info/
+-rw-rw-rw-   0        0        0     2134 2023-05-17 13:50:51.000000 WebtoonScraper-0.0.2/WebtoonScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-05-17 13:50:51.000000 WebtoonScraper-0.0.2/WebtoonScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 13:50:51.000000 WebtoonScraper-0.0.2/WebtoonScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 13:47:53.000000 WebtoonScraper-0.0.2/WebtoonScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-05-17 13:50:51.000000 WebtoonScraper-0.0.2/WebtoonScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-17 13:50:51.000000 WebtoonScraper-0.0.2/WebtoonScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 13:50:52.072443 WebtoonScraper-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2023-05-17 13:47:51.000000 WebtoonScraper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:50:52.071281 WebtoonScraper-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-17 09:28:57.000000 WebtoonScraper-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      128 2023-05-16 14:18:05.000000 WebtoonScraper-0.0.2/tests/tests.py
```

### Comparing `WebtoonScraper-0.0.1/LICENSE` & `WebtoonScraper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.0.1/README.md` & `WebtoonScraper-0.0.2/README.md`

 * *Files identical despite different names*

