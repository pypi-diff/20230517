# Comparing `tmp/newspaper_scraper-0.2.0.tar.gz` & `tmp/newspaper_scraper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newspaper_scraper-0.2.0.tar", last modified: Fri Apr 28 18:00:45 2023, max compression
+gzip compressed data, was "newspaper_scraper-0.2.1.tar", last modified: Wed May 17 02:51:38 2023, max compression
```

## Comparing `newspaper_scraper-0.2.0.tar` & `newspaper_scraper-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-28 18:00:45.219705 newspaper_scraper-0.2.0/
--rw-r--r--   0 lukas      (501) staff       (20)     1069 2023-04-13 03:30:30.000000 newspaper_scraper-0.2.0/LICENSE
--rw-r--r--   0 lukas      (501) staff       (20)     5697 2023-04-28 18:00:45.219799 newspaper_scraper-0.2.0/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)     3824 2023-04-28 17:51:35.000000 newspaper_scraper-0.2.0/README.md
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-28 18:00:45.215572 newspaper_scraper-0.2.0/newspaper_scraper/
--rw-r--r--   0 lukas      (501) staff       (20)      414 2023-04-28 17:52:31.000000 newspaper_scraper-0.2.0/newspaper_scraper/__init__.py
--rw-r--r--   0 lukas      (501) staff       (20)      296 2023-04-11 02:03:26.000000 newspaper_scraper-0.2.0/newspaper_scraper/constants.py
--rw-r--r--   0 lukas      (501) staff       (20)     9516 2023-04-28 14:58:08.000000 newspaper_scraper-0.2.0/newspaper_scraper/database.py
--rw-r--r--   0 lukas      (501) staff       (20)    20975 2023-04-28 14:48:37.000000 newspaper_scraper-0.2.0/newspaper_scraper/scraper.py
--rw-r--r--   0 lukas      (501) staff       (20)     1359 2023-04-08 00:32:47.000000 newspaper_scraper-0.2.0/newspaper_scraper/settings.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-28 18:00:45.218326 newspaper_scraper-0.2.0/newspaper_scraper/sites/
--rw-r--r--   0 lukas      (501) staff       (20)        0 2023-03-02 19:40:23.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/__init__.py
--rw-r--r--   0 lukas      (501) staff       (20)     5578 2023-04-28 02:09:25.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/bild.py
--rw-r--r--   0 lukas      (501) staff       (20)     5660 2023-04-28 16:56:27.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/handelsblatt.py
--rw-r--r--   0 lukas      (501) staff       (20)     6875 2023-04-28 02:09:25.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/spiegel.py
--rw-r--r--   0 lukas      (501) staff       (20)     6949 2023-04-28 13:46:32.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/sz.py
--rw-r--r--   0 lukas      (501) staff       (20)     6098 2023-04-28 02:09:25.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/welt.py
--rw-r--r--   0 lukas      (501) staff       (20)     6238 2023-04-28 15:03:43.000000 newspaper_scraper-0.2.0/newspaper_scraper/sites/zeit.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-28 18:00:45.219337 newspaper_scraper-0.2.0/newspaper_scraper/utils/
--rw-r--r--   0 lukas      (501) staff       (20)        0 2023-03-02 19:40:25.000000 newspaper_scraper-0.2.0/newspaper_scraper/utils/__init__.py
--rw-r--r--   0 lukas      (501) staff       (20)     1423 2023-04-07 19:51:55.000000 newspaper_scraper-0.2.0/newspaper_scraper/utils/logger.py
--rw-r--r--   0 lukas      (501) staff       (20)     3534 2023-04-11 02:04:40.000000 newspaper_scraper-0.2.0/newspaper_scraper/utils/utils.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-28 18:00:45.216400 newspaper_scraper-0.2.0/newspaper_scraper.egg-info/
--rw-r--r--   0 lukas      (501) staff       (20)     5697 2023-04-28 18:00:45.000000 newspaper_scraper-0.2.0/newspaper_scraper.egg-info/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)      736 2023-04-28 18:00:45.000000 newspaper_scraper-0.2.0/newspaper_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 lukas      (501) staff       (20)        1 2023-04-28 18:00:45.000000 newspaper_scraper-0.2.0/newspaper_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 lukas      (501) staff       (20)       64 2023-04-28 18:00:45.000000 newspaper_scraper-0.2.0/newspaper_scraper.egg-info/requires.txt
--rw-r--r--   0 lukas      (501) staff       (20)       18 2023-04-28 18:00:45.000000 newspaper_scraper-0.2.0/newspaper_scraper.egg-info/top_level.txt
--rw-r--r--   0 lukas      (501) staff       (20)      924 2023-04-28 17:52:31.000000 newspaper_scraper-0.2.0/pyproject.toml
--rw-r--r--   0 lukas      (501) staff       (20)      101 2023-04-28 18:00:45.220045 newspaper_scraper-0.2.0/setup.cfg
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-05-17 02:51:38.410372 newspaper_scraper-0.2.1/
+-rw-r--r--   0 lukas      (501) staff       (20)     1069 2023-04-13 03:30:30.000000 newspaper_scraper-0.2.1/LICENSE
+-rw-r--r--   0 lukas      (501) staff       (20)     6327 2023-05-17 02:51:38.410443 newspaper_scraper-0.2.1/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)     4454 2023-05-17 02:38:57.000000 newspaper_scraper-0.2.1/README.md
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-05-17 02:51:38.406418 newspaper_scraper-0.2.1/newspaper_scraper/
+-rw-r--r--   0 lukas      (501) staff       (20)      568 2023-05-17 02:43:48.000000 newspaper_scraper-0.2.1/newspaper_scraper/__init__.py
+-rw-r--r--   0 lukas      (501) staff       (20)      296 2023-04-11 02:03:26.000000 newspaper_scraper-0.2.1/newspaper_scraper/constants.py
+-rw-r--r--   0 lukas      (501) staff       (20)     9516 2023-04-28 14:58:08.000000 newspaper_scraper-0.2.1/newspaper_scraper/database.py
+-rw-r--r--   0 lukas      (501) staff       (20)    22733 2023-05-04 16:38:58.000000 newspaper_scraper-0.2.1/newspaper_scraper/scraper.py
+-rw-r--r--   0 lukas      (501) staff       (20)     1848 2023-05-01 16:36:46.000000 newspaper_scraper-0.2.1/newspaper_scraper/settings.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-05-17 02:51:38.409511 newspaper_scraper-0.2.1/newspaper_scraper/sites/
+-rw-r--r--   0 lukas      (501) staff       (20)        0 2023-03-02 19:40:23.000000 newspaper_scraper-0.2.1/newspaper_scraper/sites/__init__.py
+-rw-r--r--   0 lukas      (501) staff       (20)     5296 2023-05-03 02:12:50.000000 newspaper_scraper-0.2.1/newspaper_scraper/sites/bild.py
+-rw-r--r--   0 lukas      (501) staff       (20)     7332 2023-05-02 14:44:07.000000 newspaper_scraper-0.2.1/newspaper_scraper/sites/handelsblatt.py
+-rw-r--r--   0 lukas      (501) staff       (20)     6256 2023-05-02 14:44:07.000000 newspaper_scraper-0.2.1/newspaper_scraper/sites/spiegel.py
+-rw-r--r--   0 lukas      (501) staff       (20)     7447 2023-05-16 19:43:24.000000 newspaper_scraper-0.2.1/newspaper_scraper/sites/sueddeutsche.py
+-rw-r--r--   0 lukas      (501) staff       (20)     5842 2023-05-02 14:39:34.000000 newspaper_scraper-0.2.1/newspaper_scraper/sites/tagesspiegel.py
+-rw-r--r--   0 lukas      (501) staff       (20)     5975 2023-05-02 14:44:07.000000 newspaper_scraper-0.2.1/newspaper_scraper/sites/welt.py
+-rw-r--r--   0 lukas      (501) staff       (20)     6080 2023-05-02 14:42:39.000000 newspaper_scraper-0.2.1/newspaper_scraper/sites/zeit.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-05-17 02:51:38.410103 newspaper_scraper-0.2.1/newspaper_scraper/utils/
+-rw-r--r--   0 lukas      (501) staff       (20)        0 2023-03-02 19:40:25.000000 newspaper_scraper-0.2.1/newspaper_scraper/utils/__init__.py
+-rw-r--r--   0 lukas      (501) staff       (20)     2595 2023-05-01 16:30:40.000000 newspaper_scraper-0.2.1/newspaper_scraper/utils/logger.py
+-rw-r--r--   0 lukas      (501) staff       (20)     3534 2023-04-11 02:04:40.000000 newspaper_scraper-0.2.1/newspaper_scraper/utils/utils.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-05-17 02:51:38.407297 newspaper_scraper-0.2.1/newspaper_scraper.egg-info/
+-rw-r--r--   0 lukas      (501) staff       (20)     6327 2023-05-17 02:51:38.000000 newspaper_scraper-0.2.1/newspaper_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)      786 2023-05-17 02:51:38.000000 newspaper_scraper-0.2.1/newspaper_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas      (501) staff       (20)        1 2023-05-17 02:51:38.000000 newspaper_scraper-0.2.1/newspaper_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas      (501) staff       (20)       64 2023-05-17 02:51:38.000000 newspaper_scraper-0.2.1/newspaper_scraper.egg-info/requires.txt
+-rw-r--r--   0 lukas      (501) staff       (20)       18 2023-05-17 02:51:38.000000 newspaper_scraper-0.2.1/newspaper_scraper.egg-info/top_level.txt
+-rw-r--r--   0 lukas      (501) staff       (20)      924 2023-05-17 02:43:59.000000 newspaper_scraper-0.2.1/pyproject.toml
+-rw-r--r--   0 lukas      (501) staff       (20)      101 2023-05-17 02:51:38.410675 newspaper_scraper-0.2.1/setup.cfg
```

### Comparing `newspaper_scraper-0.2.0/LICENSE` & `newspaper_scraper-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `newspaper_scraper-0.2.0/PKG-INFO` & `newspaper_scraper-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newspaper_scraper
-Version: 0.2.0
+Version: 0.2.1
 Summary: The all-in-one Python package for seamless newspaper article indexing, scraping, and processing – supports public and premium content!
 Author-email: Lukas Trippe <lkstrp@pm.me>
 License: MIT License
         
         Copyright (c) 2023 Lukas Trippe
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,21 +44,23 @@
 1. Indexing: Index articles from a newspaper website using the [beautifulsoup](https://beautiful-soup-4.readthedocs.io/en/latest/) package for public articles and [selenium](https://selenium-python.readthedocs.io/) for paywall content.  
 2. Extraction: Extract article content using the [goose3](https://github.com/goose3/goose3) package.  
 3. Processing: Process articles for nlp features using the [spaCy](https://spacy.io/) package.  
   
 The indexing functionality is based on a dedicated file for each newspaper. A few newspapers are already supported, but it is easy to add new ones.  
   
 ### Supported Newspapers  
-| Logo | Newspaper | Country | Time span | Number of articles |  
-| ----------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------- | ------- | --------- | --------------- |  
-| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Der_Spiegel_2022_logo.svg/640px-Der_Spiegel_2022_logo.svg.png" height="70"> | [Der Spiegel](https://www.spiegel.de/) | Germany | Since 2000 | tbd |  
-| <img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/Die_Welt_Logo_2015.png" height="70"> | [Die Welt](https://www.welt.de/) | Germany | Since 2000 | tbd  
-| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/Logo_BILD.svg/1920px-Logo_BILD.svg.png" height="70"> | [Bild](https://www.bild.de/) | Germany | Since 2006 | tbd |  
-| <img src="https://upload.wikimedia.org/wikipedia/commons/6/60/Die_Zeit-Logo-Bremen.svg" height="70"> | [Die Zeit](https://www.zeit.de/) | Germany | Since 1946 | tbd |   
-| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/ff/Handelsblatt_201x_logo.svg/2880px-Handelsblatt_201x_logo.svg.png" height="70"> | [Handelsblatt](https://www.handelsblatt.com/) | Germany | Since 2003 | tbd |  
+| Logo | Newspaper                                        | Country | Time span  | Number of articles |  
+| ----------------------------------------------------------------------------------------------------------------------------------------------- |--------------------------------------------------| ------- |------------| --------------- |  
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Der_Spiegel_2022_logo.svg/640px-Der_Spiegel_2022_logo.svg.png" height="70"> | [Der Spiegel](https://www.spiegel.de/)           | Germany | Since 2000 | tbd |  
+| <img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/Die_Welt_Logo_2015.png" height="70"> | [Die Welt](https://www.welt.de/)                 | Germany | Since 2000 | tbd  
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/Logo_BILD.svg/1920px-Logo_BILD.svg.png" height="70"> | [Bild](https://www.bild.de/)                     | Germany | Since 2006 | tbd |  
+| <img src="https://upload.wikimedia.org/wikipedia/commons/6/60/Die_Zeit-Logo-Bremen.svg" height="70"> | [Die Zeit](https://www.zeit.de/)                 | Germany | Since 1946 | tbd |   
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/ff/Handelsblatt_201x_logo.svg/2880px-Handelsblatt_201x_logo.svg.png" height="70"> | [Handelsblatt](https://www.handelsblatt.com/)    | Germany | Since 2003 | tbd | 
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1d/Tagesspiegel_%282022-11-29%29.svg/2880px-Tagesspiegel_%282022-11-29%29.svg.png" height="70"> | [Der Tagesspiegel](https://www.tagesspiegel.de/) | Germany | Since 2000 | tbd |
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/42/S%C3%BCddeutsche_Zeitung_Logo.svg/2880px-S%C3%BCddeutsche_Zeitung_Logo.svg.png" height="70"> | [Süddeutsche Zeitung](https://www.sueddeutsche.de/)    | Germany | Since 2001 | tbd |
 
 ## Setup  
 It is recommended to install the package in an dedicated Python environment.  
 To install the package via pip, run the following command:  
   
 ```bash  
 pip install newspaper-scraper
@@ -70,21 +72,21 @@
 pip install newspaper-scraper[nlp]
 ```  
   
 ## Usage  
 To index, extract and process all public and premium articles from [Der Spiegel](https://www.spiegel.de/), published in August 2021, run the following code:  
   
 ```python  
-import newspaper_scraper as ns  
+import newspaper_scraper as nps  
 from credentials import username, password  
   
-with ns.Spiegel(db_file='articles.db') as news:
-news.index_articles_by_date_range('2021-08-01', '2021-08-31')  
-news.scrape_public_articles()
-news.scrape_premium_articles(username=username, password=password)  
-news.nlp()
+with nps.Spiegel(db_file='articles.db') as news:
+    news.index_articles_by_date_range('2021-08-01', '2021-08-31')  
+    news.scrape_public_articles()
+    news.scrape_premium_articles(username=username, password=password)  
+    news.nlp()
 ```  
   
 This will create a sqlite database file called `articles.db` in the current working directory. The database contains the following tables:  
 - `tblArticlesIndexed`: Contains all indexed articles with their scraping/ processing status and whether they are public or premium content.  
 - `tblArticlesScraped`: Contains metadata for all parsed articles, provided by goose3.  
 - `tblArticlesProcessed`: Contains nlp features of the cleaned article text, provided by spaCy.
```

### Comparing `newspaper_scraper-0.2.0/README.md` & `newspaper_scraper-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 1. Indexing: Index articles from a newspaper website using the [beautifulsoup](https://beautiful-soup-4.readthedocs.io/en/latest/) package for public articles and [selenium](https://selenium-python.readthedocs.io/) for paywall content.  
 2. Extraction: Extract article content using the [goose3](https://github.com/goose3/goose3) package.  
 3. Processing: Process articles for nlp features using the [spaCy](https://spacy.io/) package.  
   
 The indexing functionality is based on a dedicated file for each newspaper. A few newspapers are already supported, but it is easy to add new ones.  
   
 ### Supported Newspapers  
-| Logo | Newspaper | Country | Time span | Number of articles |  
-| ----------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------- | ------- | --------- | --------------- |  
-| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Der_Spiegel_2022_logo.svg/640px-Der_Spiegel_2022_logo.svg.png" height="70"> | [Der Spiegel](https://www.spiegel.de/) | Germany | Since 2000 | tbd |  
-| <img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/Die_Welt_Logo_2015.png" height="70"> | [Die Welt](https://www.welt.de/) | Germany | Since 2000 | tbd  
-| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/Logo_BILD.svg/1920px-Logo_BILD.svg.png" height="70"> | [Bild](https://www.bild.de/) | Germany | Since 2006 | tbd |  
-| <img src="https://upload.wikimedia.org/wikipedia/commons/6/60/Die_Zeit-Logo-Bremen.svg" height="70"> | [Die Zeit](https://www.zeit.de/) | Germany | Since 1946 | tbd |   
-| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/ff/Handelsblatt_201x_logo.svg/2880px-Handelsblatt_201x_logo.svg.png" height="70"> | [Handelsblatt](https://www.handelsblatt.com/) | Germany | Since 2003 | tbd |  
+| Logo | Newspaper                                        | Country | Time span  | Number of articles |  
+| ----------------------------------------------------------------------------------------------------------------------------------------------- |--------------------------------------------------| ------- |------------| --------------- |  
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Der_Spiegel_2022_logo.svg/640px-Der_Spiegel_2022_logo.svg.png" height="70"> | [Der Spiegel](https://www.spiegel.de/)           | Germany | Since 2000 | tbd |  
+| <img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/Die_Welt_Logo_2015.png" height="70"> | [Die Welt](https://www.welt.de/)                 | Germany | Since 2000 | tbd  
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/Logo_BILD.svg/1920px-Logo_BILD.svg.png" height="70"> | [Bild](https://www.bild.de/)                     | Germany | Since 2006 | tbd |  
+| <img src="https://upload.wikimedia.org/wikipedia/commons/6/60/Die_Zeit-Logo-Bremen.svg" height="70"> | [Die Zeit](https://www.zeit.de/)                 | Germany | Since 1946 | tbd |   
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/ff/Handelsblatt_201x_logo.svg/2880px-Handelsblatt_201x_logo.svg.png" height="70"> | [Handelsblatt](https://www.handelsblatt.com/)    | Germany | Since 2003 | tbd | 
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1d/Tagesspiegel_%282022-11-29%29.svg/2880px-Tagesspiegel_%282022-11-29%29.svg.png" height="70"> | [Der Tagesspiegel](https://www.tagesspiegel.de/) | Germany | Since 2000 | tbd |
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/42/S%C3%BCddeutsche_Zeitung_Logo.svg/2880px-S%C3%BCddeutsche_Zeitung_Logo.svg.png" height="70"> | [Süddeutsche Zeitung](https://www.sueddeutsche.de/)    | Germany | Since 2001 | tbd |
 
 ## Setup  
 It is recommended to install the package in an dedicated Python environment.  
 To install the package via pip, run the following command:  
   
 ```bash  
 pip install newspaper-scraper
@@ -33,21 +35,21 @@
 pip install newspaper-scraper[nlp]
 ```  
   
 ## Usage  
 To index, extract and process all public and premium articles from [Der Spiegel](https://www.spiegel.de/), published in August 2021, run the following code:  
   
 ```python  
-import newspaper_scraper as ns  
+import newspaper_scraper as nps  
 from credentials import username, password  
   
-with ns.Spiegel(db_file='articles.db') as news:
-news.index_articles_by_date_range('2021-08-01', '2021-08-31')  
-news.scrape_public_articles()
-news.scrape_premium_articles(username=username, password=password)  
-news.nlp()
+with nps.Spiegel(db_file='articles.db') as news:
+    news.index_articles_by_date_range('2021-08-01', '2021-08-31')  
+    news.scrape_public_articles()
+    news.scrape_premium_articles(username=username, password=password)  
+    news.nlp()
 ```  
   
 This will create a sqlite database file called `articles.db` in the current working directory. The database contains the following tables:  
 - `tblArticlesIndexed`: Contains all indexed articles with their scraping/ processing status and whether they are public or premium content.  
 - `tblArticlesScraped`: Contains metadata for all parsed articles, provided by goose3.  
 - `tblArticlesProcessed`: Contains nlp features of the cleaned article text, provided by spaCy.
```

### Comparing `newspaper_scraper-0.2.0/newspaper_scraper/database.py` & `newspaper_scraper-0.2.1/newspaper_scraper/database.py`

 * *Files identical despite different names*

### Comparing `newspaper_scraper-0.2.0/newspaper_scraper/scraper.py` & `newspaper_scraper-0.2.1/newspaper_scraper/scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module contains the NewspaperManager class which is used to scrape articles from a newspaper website. It is only
 used as a base class for the actual scrapers.
 """
 
 import re
 import datetime as dt
+import requests
 
 import numpy as np
 import pandas as pd
 from goose3 import Goose
 from tqdm.auto import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 
@@ -20,14 +21,15 @@
 from .utils.logger import log
 from .settings import settings
 from .constants import NLP_ATTRIBUTES
 from .utils.utils import flatten_dict
 from .utils.utils import get_selenium_webdriver
 from .utils.utils import retry_on_exception
 from .database import Database
+from selenium.common.exceptions import WebDriverException
 
 
 class NewspaperManager:
     """
     The NewspaperManager class is used to scrape articles from a newspaper website. It is only used as a base class for
     the actual scrapers and can not be instantiated directly. Each newspaper scraper needs to inherit from this class
     and implement the _get_published_articles, _soup_get_html, and _selenium_login methods.
@@ -87,25 +89,49 @@
         self._db.connect()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._db.close()
 
     @staticmethod
+    def _request(url, get_full_response=False):
+
+        # Get the HTML of the article
+        try:
+            response = requests.get(url)
+        except requests.exceptions.ConnectionError:
+            log.warning(f'Connection error while requesting {url}.')
+            return None
+
+        # Check if the response is valid
+        if response.status_code == 200:
+            if get_full_response:
+                return response
+            else:
+                return response.text
+        elif response.status_code == 404:
+            return None
+        else:
+            log.warning(f"{response.status_code} error scraping {response.url}.")
+            return None
+
+    @staticmethod
     def _parse_article(html, url):
         """
         Parses the HTML of an article with goose3 and returns a DataFrame with the parsed infos.
 
         Args:
             html (str or bytes): The HTML of the article.
             url (str): The URL of the article.
 
         Returns:
             pd.DataFrame: A DataFrame with the parsed infos.
         """
+        if not html:
+            return pd.DataFrame()
         g = Goose()
         article = g.extract(raw_html=html)
 
         # Get all parsed infos
         parsed_infos = article.infos
         parsed_infos = flatten_dict(parsed_infos)
         # Change all keys to CamelCase
@@ -120,34 +146,35 @@
         # Rename CleanedText to Text
         parsed_infos = parsed_infos.rename({'CleanedText': 'Text'}, axis=1)
         parsed_infos.index.name = 'URL'
 
         return parsed_infos
 
     @retry_on_exception
-    def index_articles_by_date_range(self, date_from, date_to, skip_existing=True):
+    def index_articles_by_date_range(self, date_from, date_to, freq='D', skip_existing=True):
         """
         Indexes all articles published between date_from and date_to for a given newspaper. Indexing means that the
         articles are added to the database and their URLs are stored. The actual scraping of the articles is done
         separately with the scrape_public_articles and scrape_premium_articles methods.
 
         Args:
             date_from (dt.datetime or str): The first day to scrape articles from.
             date_to (dt.datetime or str): The last day to scrape articles from.
+            freq (str, optional): The frequency of the date range. Defaults to 'D'.
             skip_existing (bool, optional): If True, days that are already indexed are skipped. Defaults to True.
         """
         date_from = pd.to_datetime(date_from)
         date_to = pd.to_datetime(date_to)
 
         already_indexed = self._db.df_indexed[(self._db.df_indexed.NewspaperID == self.newspaper_id)]
 
         # Convert already_indexed.PubDateIndexPage to set of dates for faster lookup
         indexed_dates = {index_day.date() for index_day in already_indexed.PubDateIndexPage}
         # Create pd.date_range and convert it to a numpy array of dates for faster lookup
-        date_range = pd.date_range(date_from, date_to)
+        date_range = pd.date_range(date_from, date_to, freq=freq)
         date_range_dates = np.array([day.date() for day in date_range])
 
         if skip_existing:
             date_range = date_range[~np.in1d(date_range_dates, list(indexed_dates))]
         else:
             date_range = date_range.tolist()
 
@@ -161,46 +188,51 @@
         counter = 0
         with logging_redirect_tqdm(loggers=[log]):
             for day in tqdm(date_range):
                 counter += 1
 
                 urls, pub_dates = self._get_articles_by_date(day)
 
+                # Remove query strings from urls
+                urls = [url.split('?')[0] for url in urls]
+
+                assert len(urls) == len(set(urls)), \
+                    f'Found {len(urls) - len(set(urls))} duplicates in urls. Please remove them in the newspaper' \
+                    f'specific _get_articles_by_date method.'
+                assert len(urls) == len(pub_dates), \
+                    'Number of urls and pub_dates does not match.'
                 assert all([isinstance(pub_date, dt.datetime) for pub_date in pub_dates]), \
                     f'Not all pub_dates are datetime objects.'
                 assert all([pub_date.tzinfo is not None for pub_date in pub_dates]), \
                     f'Not all pub_dates contain timezone info.'
 
                 # Convert pub_dates to UTC
                 pub_dates = [pub_date.astimezone(dt.timezone.utc) for pub_date in pub_dates]
                 # Remove timezone info from pub_dates
                 pub_dates = [pub_date.replace(tzinfo=None) for pub_date in pub_dates]
 
-                # Remove query strings from urls
-                urls = [url.split('?')[0] for url in urls]
-
                 urls = pd.DataFrame({'NewspaperID': self.newspaper_id,
                                      'PubDateIndexPage': pub_dates,
                                      'DateIndexed': dt.datetime.now(),
                                      'Public': None,
                                      'Scraped': False,
                                      'Processed': False},
                                     index=urls)
                 # Mark if urls are new
                 urls['new'] = ~urls.index.isin(self._db.df_indexed.index).astype(bool)
 
                 # Add new urls to articles table
                 self._db.df_indexed = pd.concat([self._db.df_indexed, urls[urls['new']].drop('new', axis=1)])
-                log.info(f'{counter}/{len(date_range)}: Indexed {urls.new.sum()}/{len(urls)} articles '
+                log.info(f'{counter}/{len(date_range):>3}: Indexed {urls.new.sum()}/{len(urls):>3} articles '
                          f'for {day.strftime("%d.%m.%Y")} (n={len(self._db.df_indexed):,}).')
 
                 self._db.save_data('df_indexed', mode='replace')
 
     @retry_on_exception
-    def index_articles_by_edition(self, edition_from: str, edition_to: str, editions_per_year=55, skip_existing=True):
+    def index_articles_by_editions(self, edition_from: str, edition_to: str, editions_per_year=55, skip_existing=True):
         """
         Index all articles published in between two editions for a given newspaper. Indexing means that the
         articles are added to the database and their URLs are stored. The actual scraping of the articles is done
         separately with the scrape_public_articles and scrape_premium_articles methods.
 
         Args:
             edition_from (str): The first edition to scrape articles from. The format must be 'YYYY-EDITION'
@@ -257,27 +289,31 @@
                 edition = int(edition.split('-')[1])
 
                 urls = self._get_articles_by_edition(year, edition)
 
                 # Remove query strings from urls
                 urls = [url.split('?')[0] for url in urls]
 
+                assert len(urls) == len(set(urls)), \
+                    f'Found {len(urls) - len(set(urls))} duplicates in urls. Please remove them in the newspaper' \
+                    f'specific _get_articles_by_edition method.'
+
                 urls = pd.DataFrame({'NewspaperID': self.newspaper_id,
                                      'Edition': f'{year}-{edition}',
                                      'DateIndexed': dt.datetime.now(),
                                      'Public': None,
                                      'Scraped': False,
                                      'Processed': False},
                                     index=urls)
                 # Mark if urls are new
                 urls['new'] = ~urls.index.isin(self._db.df_indexed.index).astype(bool)
 
                 # Add new urls to articles table
                 self._db.df_indexed = pd.concat([self._db.df_indexed, urls[urls['new']].drop('new', axis=1)])
-                log.info(f'{counter}/{len(edition_range)}: Indexed {urls.new.sum()}/{len(urls)} articles '
+                log.info(f'{counter}/{len(edition_range)}: Indexed {urls.new.sum()}/{len(urls):>3} articles '
                          f'for {year}-{edition} (n={len(self._db.df_indexed):,}).')
 
                 self._db.save_data('df_indexed', mode='replace')
 
     @retry_on_exception
     def scrape_public_articles(self):
         """
@@ -446,15 +482,22 @@
         raise NotImplemented
 
     def _selenium_get_html(self, url):
         """
         Function to get the html of a private article. Uses selenium to get the html. Can be optionally overwritten by
         the child if a different method is needed.
         """
-        self.selenium_driver.get(url)
-        return self.selenium_driver.page_source
+        try:
+            self.selenium_driver.get(url)
+            return self.selenium_driver.page_source
+        except WebDriverException as e:
+            if "ERR_NAME_NOT_RESOLVED" in str(e):
+                print(f"URL is not valid: {url}")
+                return None
+            else:
+                raise e
 
     def _selenium_login(self, username: str, password: str):
         """
         Exists only as a placeholder. Needs to be implemented by the child class for each newspaper.
         """
         raise NotImplemented
```

### Comparing `newspaper_scraper-0.2.0/newspaper_scraper/settings.py` & `newspaper_scraper-0.2.1/newspaper_scraper/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,26 +6,39 @@
 class _Settings:
     """
     This class contains the package-wide settings. It should not be instantiated and only used via the settings
     variable (see below).
     """
 
     _log_file = 'logs.log'
+    _log_level = 'DEBUG'
     retry_on_exception = True
     save_interval = 60
     selenium_driver = None
 
     _description = {
         'log_file': 'Path to the log file. If None, no log file is created.',
+        'log_level': 'Log level. Possible values: DEBUG, INFO, WARNING, ERROR, CRITICAL.',
         'retry_on_exception': 'If True, retry on exception.',
         'save_interval': 'Interval in seconds to save the database. Smaller values will slow down the process.',
+        'selenium_driver': 'Selenium driver object. Pass a driver object to use it if the provided one does not work.'
     }
 
     # noinspection PyMissingOrEmptyDocstring
     @property
+    def log_level(self):
+        return self._log_level
+
+    @log_level.setter
+    def log_level(self, value):
+        self._log_level = value
+        logger.change_log_level(logger.log, value)
+
+    # noinspection PyMissingOrEmptyDocstring
+    @property
     def log_file(self):
         return self._log_file
 
     @log_file.setter
     def log_file(self, value):
         self._log_file = value
         logger.change_log_file_path(logger.log, value)
```

### Comparing `newspaper_scraper-0.2.0/newspaper_scraper/sites/bild.py` & `newspaper_scraper-0.2.1/newspaper_scraper/sites/bild.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 The class inherits from the NewspaperManager class and needs an implementation of the abstract methods.
 With a similar implementation, it is possible to scrape articles from other news websites.
 """
 import re
 import datetime as dt
 import time
 
-import requests
 from bs4 import BeautifulSoup
 import pandas as pd
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as ec
 from selenium.common.exceptions import ElementNotInteractableException
 
@@ -19,15 +18,15 @@
 from ..scraper import NewspaperManager
 
 
 class DeBild(NewspaperManager):
     """
     This class inherits from the NewspaperManager class and implements the newspaper specific methods.
     These methods are:
-        - _get_published_articles: Index articles published on a given day and return the urls and publication dates.
+        - _get_articles_by_date: Index articles published on a given day and return the urls and publication dates.
         - _soup_get_html: Determine if an article is premium content and scrape the html if it is not. Uses
             beautifulsoup.
         - _selenium_login: Login to the newspaper website to allow scraping of premium content after the login. Uses
             selenium.
     """
 
     def __init__(self, db_file: str = 'articles.db'):
@@ -37,73 +36,66 @@
         """
         Index articles published on a given day and return the urls and publication dates.
 
         Args:
             day (dt.date): Date of the articles to index.
 
         Returns:
-            urls ([str]): List of urls of the articles published on the given day.
-            pub_dates ([dt.datetime]): List of publication dates of the articles published on the given day.
-              Needs timezone information.
+            [str]: List of urls of the articles published on the given day.
+            [dt.datetime]: List of publication dates of the articles published on the given day. Needs timezone
+                information.
         """
-        URL = f'https://www.bild.de/themen/uebersicht/archiv/archiv-82532020.bild.html?archiveDate=' \
+        url = f'https://www.bild.de/themen/uebersicht/archiv/archiv-82532020.bild.html?archiveDate=' \
               f'{day.strftime("%Y-%m-%d")}'
-        soup = BeautifulSoup(requests.get(URL).content, "html.parser")
+
+        html = self._request(url)
+        if html is None:
+            return []
+        soup = BeautifulSoup(html, "html.parser")
+
+        # Get list of article elements
         articles = soup \
             .find("section", {"class": "stage-feed stage-feed--archive"}) \
             .find('ul', {'class': 'stage-feed__viewport'}) \
             .find_all('li')
-
-        # Get articles urls
+        # Get article urls
         urls = ['https://www.bild.de' + article.find('a')['href'] for article in articles]
-
         # Get articles publication dates
         pub_dates = [pd.to_datetime(article.find('time')['datetime']) for article in articles]
 
-        assert len(urls) == len(pub_dates), 'Number of urls and pub_dates does not match.'
-
         return urls, pub_dates
 
     def _soup_get_html(self, url: str):
         """
         For a single article, determine if it is premium content and scrape the html if it is not.
 
         Args:
             url (str): Url of the article to scrape.
 
         Returns:
-            html (str): Html of the article. If the article is premium content, None is returned.
-            is_premium (bool): True if the article is premium content, False otherwise.
+            str: Html of the article. If the article is premium content, None is returned.
+            bool: True if the article is premium content, False otherwise.
         """
-        try:
-            html = requests.get(url).content
-            premium = re.search(r'https://www.bild.de/bild-plus/', url)
-
-        except AttributeError:
-            log.warning(f'Error scraping {url}.')
+        html = self._request(url)
+        if html is None:
             return None, False
+        premium = re.search(r'https://www.bild.de/bild-plus/', url)
 
         return html, not bool(premium)
 
     def _selenium_login(self, username: str, password: str):
         """
-        Using selenium, login to the newspaper website to allow scraping of premium content after the login. Does three
-        things:
-            1. Go to main page and accept cookies.
-            2. Login.
-            3. Check if login was successful.
-
+        Using selenium, login to the newspaper website to allow scraping of premium content after the login.
         Args:
             username (str): Username to login to the newspaper website.
             password (str): Password to login to the newspaper website.
 
         Returns:
             bool: True if login was successful, False otherwise.
         """
-
         # Go to main page and accept cookies
         self.selenium_driver.get('https://www.bild.de/')
         privacy_frame = WebDriverWait(self.selenium_driver, 10).until(
             ec.presence_of_element_located((By.XPATH, '//iframe[@title="SP Consent Message"]'))
         )
         self.selenium_driver.switch_to.frame(privacy_frame)
         WebDriverWait(self.selenium_driver, 10).until(
```

### Comparing `newspaper_scraper-0.2.0/newspaper_scraper/sites/handelsblatt.py` & `newspaper_scraper-0.2.1/newspaper_scraper/sites/welt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """
-This module contains the class to scrape articles from the "Handelsblatt" newspaper (https://www.handelsblatt.com/).
+This module contains the class to scrape articles from the "Welt" newspaper (https://www.welt.de/).
 The class inherits from the NewspaperManager class and needs an implementation of the abstract methods.
 With a similar implementation, it is possible to scrape articles from other news websites.
 """
+import re
 import datetime as dt
 
 import requests
 from bs4 import BeautifulSoup
+import pandas as pd
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as ec
-from selenium.common.exceptions import TimeoutException
+from selenium.common.exceptions import NoSuchElementException
 
 from ..utils.logger import log
 from ..scraper import NewspaperManager
 
 
-class DeHandelsblatt(NewspaperManager):
+class DeWelt(NewspaperManager):
     """
     This class inherits from the NewspaperManager class and implements the newspaper specific methods.
     These methods are:
-        - _get_published_articles: Index articles published on a given day and return the urls and publication dates.
+        - _get_articles_by_date: Index articles published on a given day and return the urls and publication dates.
         - _soup_get_html: Determine if an article is premium content and scrape the html if it is not. Uses
             beautifulsoup.
         - _selenium_login: Login to the newspaper website to allow scraping of premium content after the login. Uses
             selenium.
     """
 
     def __init__(self, db_file: str = 'articles.db'):
@@ -34,90 +36,97 @@
         """
         Index articles published on a given day and return the urls and publication dates.
 
         Args:
             day (dt.date): Date of the articles to index.
 
         Returns:
-            urls ([str]): List of urls of the articles published on the given day.
-            pub_dates ([dt.datetime]): List of publication dates of the articles published on the given day.
-              Needs timezone information.
-        """
-        URL = f'https://www.handelsblatt.com/archiv/{day.strftime("%Y/%-m/%-d")}'
-
-        soup = BeautifulSoup(requests.get(URL).content, "html.parser")
-        _articles = soup.find_all("a", {"class": "vhb-teaser-link"})
-        urls = ['https://www.handelsblatt.com' + article['href'] for article in _articles]
-
-        # Also add paginated articles
-        pages_exist = soup.find("div", {"class": "vhb-teaser-pagination"})
-        if pages_exist:
-            page_urls = pages_exist.find("div", {"class": "vhb-tp-list"}).find_all('a')
-            page_urls = ['https://www.handelsblatt.com' + page_url['href'] for page_url in page_urls]
-
-            for page_url in page_urls:
-                soup = BeautifulSoup(requests.get(page_url).content, "html.parser")
-                _articles = soup.find_all("a", {"class": "vhb-teaser-link"})
-                [urls.append('https://www.handelsblatt.com' + article['href']) for article in _articles]
-
-        # Create list of publication dates, since the website does not provide them
-        pub_dates = [dt.datetime.combine(day, dt.datetime.min.time(), tzinfo=dt.timezone.utc)] * len(urls)
-
-        assert len(urls) == len(pub_dates), 'Number of urls and pub_dates does not match.'
+            [str]: List of urls of the articles published on the given day.
+            [dt.datetime]: List of publication dates of the articles published on the given day. Needs timezone
+                information.
+        """
+        url = f'https://www.welt.de/schlagzeilen/nachrichten-vom-{day.strftime("%-d-%-m-%Y")}.html'
+
+        html = self._request(url)
+        if html is None:
+            return []
+        soup = BeautifulSoup(html, "html.parser")
+
+        # Get list of article elements
+        articles = soup \
+            .find("div", {"class": "c-tabs__panel-content"}) \
+            .find_all("article", {"class": "c-teaser c-teaser--archive"})
+        # Get articles urls
+        urls = ['https://www.welt.de' + article.find('h4').find('a')['href'] for article in articles]
+        # Get articles publication dates
+        time_regex = re.compile(r'\d{2}\.\d{2}\.\d{4}\s\|\s\d{2}:\d{2}')
+        pub_dates = [pd.to_datetime(f'{article.find(string=time_regex)}', format='%d.%m.%Y | %H:%M')
+                     for article in articles]
+        # Add timezone Europe/Berlin to pub_dates
+        pub_dates = [pub_date.tz_localize('UTC') for pub_date in pub_dates]
 
         return urls, pub_dates
 
     def _soup_get_html(self, url: str):
         """
         For a single article, determine if it is premium content and scrape the html if it is not.
 
         Args:
             url (str): Url of the article to scrape.
 
         Returns:
-            html (str): Html of the article. If the article is premium content, None is returned.
-            is_premium (bool): True if the article is premium content, False otherwise.
+            str: Html of the article. If the article is premium content, None is returned.
+            bool: True if the article is premium content, False otherwise.
         """
-        # Handelsblatt uses a login paywall via javascript. Therefore, selenium is needed to login. The following
-        # return indicates that the article is premium content and they are all scraped self.scrape_premium_articles.
-        return None, False
+        html = self._request(url)
+        if not html:
+            return None, False
+        soup = BeautifulSoup(html, "html.parser")
+        try:
+            premium_icon = soup.find("header", {"class": "c-content-container"}). \
+                find('a', {"class": "o-dreifaltigkeit__premium-badge"})
+            return html, not bool(premium_icon)
+        except AttributeError:
+            log.warning(f'Could not identify if article is premium: {url}.')
+            return None, False
 
     def _selenium_login(self, username: str, password: str):
         """
-        Using selenium, login to the newspaper website to allow scraping of premium content after the login. Does three
-        things:
-            1. Login
-            2. Accept cookies
-            3. Check if login was successful
-
+        Using selenium, login to the newspaper website to allow scraping of premium content after the login.
         Args:
             username (str): Username to login to the newspaper website.
             password (str): Password to login to the newspaper website.
 
         Returns:
             bool: True if login was successful, False otherwise.
         """
-
         # Login
-        self.selenium_driver.get('https://id.handelsblatt.com/login')
-        self.selenium_driver.find_element(By.XPATH, '//input[@type="email"]').send_keys(username)
-        self.selenium_driver.find_element(By.XPATH, '//input[@type="password"]').send_keys(password)
-        self.selenium_driver.find_element(By.XPATH, '//button[@type="submit"]').click()
-        self.selenium_driver.get('https://www.handelsblatt.com/ ')
+        self.selenium_driver.get('https://lo.la.welt.de/login')
+        WebDriverWait(self.selenium_driver, 10).until(
+            ec.presence_of_element_located((By.NAME, 'username')))
+        self.selenium_driver.find_element(By.NAME, 'username').send_keys(username)
+        self.selenium_driver.find_element(By.NAME, 'password').send_keys(password)
+        self.selenium_driver.find_element(By.CSS_SELECTOR, 'button[type="submit"]').click()
 
-        # Accept cookies
+        # Go to main page and accept cookies
+        self.selenium_driver.get('https://www.welt.de/')
         privacy_frame = WebDriverWait(self.selenium_driver, 10).until(
-            ec.presence_of_element_located((By.XPATH, '//iframe[@title="Iframe title"]')))
+            ec.presence_of_element_located((By.XPATH, '//iframe[@title="SP Consent Message"]'))
+        )
         self.selenium_driver.switch_to.frame(privacy_frame)
-        cookie_accept_button = WebDriverWait(self.selenium_driver, 10).until(
-            ec.element_to_be_clickable((By.XPATH, "//button[contains(text(), 'ZUSTIMMEN')]")))
-        cookie_accept_button.click()
+        WebDriverWait(self.selenium_driver, 10).until(
+            ec.presence_of_element_located((By.CSS_SELECTOR, 'button[title="Alle akzeptieren"]')))
+        self.selenium_driver.find_element(By.CSS_SELECTOR, 'button[title="Alle akzeptieren"]').click()
 
         # Check if login was successful
         try:
+            self.selenium_driver.get('https://www.welt.de/meinewelt/')
             WebDriverWait(self.selenium_driver, 10).until(
-                ec.presence_of_element_located((By.XPATH, f"//span[contains(text(), '{username}')]")))
-            log.info('Logged in to Handelsblatt.')
+                ec.presence_of_element_located((By.CSS_SELECTOR, 'div[data-component-name="home"]')))
+            _elem = self.selenium_driver.find_element(By.CSS_SELECTOR, 'div[data-component-name="home"]')
+            WebDriverWait(_elem, 10).until(ec.presence_of_element_located((By.CSS_SELECTOR, 'div[name="greeting"]')))
+            self.selenium_driver.get('https://www.welt.de')
+            log.info('Logged in to Welt Plus.')
             return True
-        except TimeoutException:
-            log.error('Login to Handelsblatt failed.')
+        except NoSuchElementException:
+            log.warning('Login to Welt Plus failed.')
             return False
```

### Comparing `newspaper_scraper-0.2.0/newspaper_scraper/sites/spiegel.py` & `newspaper_scraper-0.2.1/newspaper_scraper/sites/handelsblatt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,154 +1,163 @@
 """
-This module contains the class to scrape articles from the "Spiegel" newspaper (https://www.spiegel.de/).
+This module contains the class to scrape articles from the "Handelsblatt" newspaper (https://www.handelsblatt.com/).
 The class inherits from the NewspaperManager class and needs an implementation of the abstract methods.
 With a similar implementation, it is possible to scrape articles from other news websites.
 """
-
-import re
-import locale
 import datetime as dt
+import time
 
-import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as ec
-from selenium.common.exceptions import ElementNotInteractableException
 from selenium.common.exceptions import TimeoutException
 
 from ..utils.logger import log
 from ..scraper import NewspaperManager
 
 
-class DeSpiegel(NewspaperManager):
+class DeHandelsblatt(NewspaperManager):
     """
     This class inherits from the NewspaperManager class and implements the newspaper specific methods.
     These methods are:
-        - _get_published_articles: Index articles published on a given day and return the urls and publication dates.
+        - _get_articles_by_date: Index articles published on a given day and return the urls and publication dates.
         - _soup_get_html: Determine if an article is premium content and scrape the html if it is not. Uses
             beautifulsoup.
         - _selenium_login: Login to the newspaper website to allow scraping of premium content after the login. Uses
             selenium.
     """
 
     def __init__(self, db_file: str = 'articles.db'):
         super().__init__(db_file)
 
-        # Set locale to German
-        locale.setlocale(locale.LC_TIME, "de_DE")
-
     def _get_articles_by_date(self, day: dt.date):
         """
         Index articles published on a given day and return the urls and publication dates.
 
         Args:
             day (dt.date): Date of the articles to index.
 
         Returns:
-            urls ([str]): List of urls of the articles published on the given day.
-            pub_dates ([dt.datetime]): List of publication dates of the articles published on the given day.
-              Needs timezone information.
-        """
-        URL = f'https://www.spiegel.de/nachrichtenarchiv/artikel-{day.strftime("%d.%m.%Y")}.html'
-        soup = BeautifulSoup(requests.get(URL).content, "html.parser")
-        articles = soup.find("section", {"data-area": "article-teaser-list"}) \
-            .find_all("div", {"data-block-el": "articleTeaser"})
-
-        # Remove advertisement articles
-        articles = [article for article in articles if not article.find("h3")]
-
-        # Get articles urls
-        urls = [article.find('a')['href'] for article in articles]
-
-        # Get articles publication dates
-        time_regex = re.compile(r'\d{1,2}\.\s\w+,\s\d{1,2}\.\d{2}\sUhr')
-        pub_dates = []
-        for article in articles:
-            try:
-                pub_dates.append(pd.to_datetime(f'{article.find(string=time_regex)}; {day.year}',
-                                                format='%d. %B, %H.%M Uhr; %Y').tz_localize('Europe/Berlin'))
-
-            except ValueError:
-                log.warning(f'Could not parse publication date for article {article.find("a")["href"]}: '
-                            f'{article.find(string=time_regex)}.')
-                pub_dates.append(dt.datetime(day.year, day.month, day.day, tzinfo=dt.timezone.utc))
+            [str]: List of urls of the articles published on the given day.
+            [dt.datetime]: List of publication dates of the articles published on the given day. Needs timezone
+                information.
+        """
+        url = f'https://www.handelsblatt.com/archiv/{day.strftime("%Y/%-m/%-d")}'
+
+        html = self._request(url)
+        if html is None:
+            return []
+        soup = BeautifulSoup(html, "html.parser")
+
+        # Get list of article elements
+        articles = soup.find_all("a", {"class": "vhb-teaser-link"})
+        # Get article urls
+        urls = ['https://www.handelsblatt.com' + article['href'] for article in articles]
+        # Also add paginated articles
+        pages_exist = soup.find("div", {"class": "vhb-teaser-pagination"})
+        if pages_exist:
+            page_urls = pages_exist.find("div", {"class": "vhb-tp-list"}).find_all('a')
+            page_urls = ['https://www.handelsblatt.com' + page_url['href'] for page_url in page_urls]
+
+            for page_url in page_urls:
+                html = self._request(page_url)
+                soup = BeautifulSoup(html, "html.parser")
+                # Get list of article elements
+                articles = soup.find_all("a", {"class": "vhb-teaser-link"})
+                # Add article urls to list
+                [urls.append('https://www.handelsblatt.com' + article['href']) for article in articles]
+
+        # Remove duplicates
+        old_len = len(urls)
+        urls = list(set(urls))
+        if len(urls) < old_len:
+            log.warning(f"Removed {old_len - len(urls)} duplicate urls for {day.strftime('%Y-%m-%d')}.")
 
-        assert len(urls) == len(pub_dates), 'Number of urls and pub_dates does not match.'
+        # Create list of publication dates, since the website does not provide them
+        pub_dates = [dt.datetime.combine(day, dt.datetime.min.time(), tzinfo=dt.timezone.utc)] * len(urls)
 
         return urls, pub_dates
 
     def _soup_get_html(self, url: str):
         """
         For a single article, determine if it is premium content and scrape the html if it is not.
 
         Args:
             url (str): Url of the article to scrape.
 
         Returns:
-            html (str): Html of the article. If the article is premium content, None is returned.
-            is_premium (bool): True if the article is premium content, False otherwise.
+            str: Html of the article. If the article is premium content, None is returned.
+            bool: True if the article is premium content, False otherwise.
         """
-        try:
-            html = requests.get(url).content
-            soup = BeautifulSoup(html, "html.parser")
-            premium_icon = soup.find("header", {"data-area": "intro"}).find('svg', {"id": "spon-spplus-flag-l"})
-        except AttributeError:
-            log.warning(f'Error scraping {url}.')
-            return None, False
-        return html, not bool(premium_icon)
+
+        # Handelsblatt uses a login paywall via javascript, which means that selenium is needed to login. The following
+        # return indicates that the article is premium content and therefore all articles are scraped
+        # in self.scrape_premium_articles.
+        return None, False
 
     def _selenium_login(self, username: str, password: str):
         """
-        Using selenium, login to the newspaper website to allow scraping of premium content after the login. Does three
-        things:
-            1. Go to main page and accept cookies.
-            2. Login.
-            3. Check if login was successful.
-
+        Using selenium, login to the newspaper website to allow scraping of premium content after the login.
         Args:
             username (str): Username to login to the newspaper website.
             password (str): Password to login to the newspaper website.
 
         Returns:
             bool: True if login was successful, False otherwise.
         """
-        # Go to main page and accept cookies
-        self.selenium_driver.get('https://www.spiegel.de/')
+        # Accept cookies on Main Page
+        self.selenium_driver.get('https://www.handelsblatt.com/ ')
         privacy_frame = WebDriverWait(self.selenium_driver, 10).until(
-            ec.presence_of_element_located((By.XPATH, '//iframe[@title="Privacy Center"]')))
+            ec.presence_of_element_located((By.XPATH, '//iframe[@title="Iframe title"]')))
         self.selenium_driver.switch_to.frame(privacy_frame)
-        self.selenium_driver.find_element(By.XPATH, "//button[contains(text(), 'Akzeptieren und weiter')]").click()
-
-        # Login
-        self.selenium_driver.get('https://gruppenkonto.spiegel.de/anmelden.html')
-        self.selenium_driver.find_element(By.NAME, 'loginform:username').send_keys(username)
-        self.selenium_driver.find_element(By.NAME, 'loginform:submit').click()
-        self.selenium_driver.find_element(By.NAME, 'loginform:password').send_keys(password)
-        self.selenium_driver.find_element(By.NAME, 'loginform:submit').click()
+        cookie_accept_button = WebDriverWait(self.selenium_driver, 10).until(
+            ec.element_to_be_clickable((By.XPATH, "//button[contains(text(), 'ZUSTIMMEN')]")))
+        cookie_accept_button.click()
+
+        # Go to Login Page
+        login_button = WebDriverWait(self.selenium_driver, 10).until(
+            ec.element_to_be_clickable((By.XPATH, "//a[contains(text(), 'Login')]")))
+        login_button.click()
 
-        # Go to main page
-        self.selenium_driver.get('https://www.spiegel.de/')
+        # Accept cookies on Login Page, if necessary
+        try:
+            time.sleep(1)
+            privacy_frame = WebDriverWait(self.selenium_driver, 10).until(
+                ec.presence_of_element_located((By.XPATH, '//iframe[@title="Iframe title"]')))
+            self.selenium_driver.switch_to.frame(privacy_frame)
+            cookie_accept_button = WebDriverWait(self.selenium_driver, 10).until(
+                ec.element_to_be_clickable((By.XPATH, "//button[contains(text(), 'ZUSTIMMEN')]")))
+            cookie_accept_button.click()
+        except TimeoutException:
+            pass
 
-        # Accept cookies again, if needed
-        privacy_frame = WebDriverWait(self.selenium_driver, 10).until(
-            ec.presence_of_element_located((By.XPATH, '//iframe[@title="Privacy Center"]')))
-        self.selenium_driver.switch_to.frame(privacy_frame)
-        self.selenium_driver.find_element(By.XPATH, "//button[contains(text(), 'Akzeptieren und weiter')]").click()
+        # Login
+        time.sleep(1)
+        self.selenium_driver.find_element(By.XPATH, '//input[@type="email"]').send_keys(username)
+        time.sleep(1)
+        self.selenium_driver.find_element(By.XPATH, '//input[@type="password"]').send_keys(password)
+        time.sleep(1)
+        self.selenium_driver.find_element(By.XPATH, '//button[@type="submit"]').click()
 
-        # Click on Anmelden button because sometimes the login is not saved on main page
+        # Accept cookies on Login Page after login again
         try:
-            self.selenium_driver.find_element(By.XPATH, '//a[@data-sara-link="gruppenkonto"]').click()
-        except ElementNotInteractableException:
+            time.sleep(1)
+            privacy_frame = WebDriverWait(self.selenium_driver, 10).until(
+                ec.presence_of_element_located((By.XPATH, '//iframe[@title="Iframe title"]')))
+            self.selenium_driver.switch_to.frame(privacy_frame)
+            cookie_accept_button = WebDriverWait(self.selenium_driver, 10).until(
+                ec.element_to_be_clickable((By.XPATH, "//button[contains(text(), 'ZUSTIMMEN')]")))
+            cookie_accept_button.click()
+        except TimeoutException:
             pass
 
-        # Check if loggin was successful
-        self.selenium_driver.get('https://www.spiegel.de/')
+        # Check if login was successful
         try:
             WebDriverWait(self.selenium_driver, 10).until(
-                ec.presence_of_element_located((By.XPATH, '//a[@href="https://www.spiegel.de/fuermich/"]')))
-            log.info('Logged in to Spiegel Plus.')
+                ec.presence_of_element_located((By.XPATH, f"//span[contains(text(), '{username}')]")))
+            log.info('Logged in to Handelsblatt.')
             return True
         except TimeoutException:
-            log.error('Login to Spiegel Plus failed.')
+            log.error('Login to Handelsblatt failed.')
             return False
```

### Comparing `newspaper_scraper-0.2.0/newspaper_scraper/sites/sz.py` & `newspaper_scraper-0.2.1/newspaper_scraper/sites/sueddeutsche.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,155 +1,168 @@
 """
-This module contains the class to scrape articles from the "Spiegel" newspaper (https://www.spiegel.de/).
+This module contains the class to scrape articles from the "Süddeutsche Zeitung" newspaper
+(https://www.sueddeutsche.de/).
 The class inherits from the NewspaperManager class and needs an implementation of the abstract methods.
 With a similar implementation, it is possible to scrape articles from other news websites.
 """
-
-import re
-import locale
 import datetime as dt
+import time
+import re
 
-import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as ec
-from selenium.common.exceptions import ElementNotInteractableException
-from selenium.common.exceptions import NoSuchElementException
 from selenium.common.exceptions import TimeoutException
 
 from ..utils.logger import log
 from ..scraper import NewspaperManager
 
 
-class DeSueddeutscheZeitung(NewspaperManager):
+class DeSueddeutsche(NewspaperManager):
     """
     This class inherits from the NewspaperManager class and implements the newspaper specific methods.
     These methods are:
-        - _get_published_articles: Index articles published on a given day and return the urls and publication dates.
+        - _get_articles_by_date: Index articles published on a given day and return the urls and publication dates.
         - _soup_get_html: Determine if an article is premium content and scrape the html if it is not. Uses
             beautifulsoup.
         - _selenium_login: Login to the newspaper website to allow scraping of premium content after the login. Uses
             selenium.
     """
 
     def __init__(self, db_file: str = 'articles.db'):
         super().__init__(db_file)
 
-        # Set locale to German
-        locale.setlocale(locale.LC_TIME, "de_DE")
-
     def _get_articles_by_date(self, day: dt.date):
         """
-        Index articles published on a given day and return the urls and publication dates.
+        Index articles published on a given day and return the urls and publication dates. The website list articles on
+        a per day basis but per month and per category, so indexing works a bit different than for other newspapers.
+        When the day of the date is 1, the function will index all articles for the given month. Otherwise it returns an
+        empty list. Indexing included various requests since different categories have different urls. This takes
+        longer than for other newspapers.
 
         Args:
-            day (dt.date): Date of the articles to index.
+            day (dt.date): Date of the articles to index. The function only return something if the day is the first of
+                the month.
 
         Returns:
-            urls ([str]): List of urls of the articles published on the given day.
-            pub_dates ([dt.datetime]): List of publication dates of the articles published on the given day.
-              Needs timezone information.
-        """
-        URL = f'https://www.spiegel.de/nachrichtenarchiv/artikel-{day.strftime("%d.%m.%Y")}.html'
-        soup = BeautifulSoup(requests.get(URL).content, "html.parser")
-        articles = soup.find("section", {"data-area": "article-teaser-list"}) \
-            .find_all("div", {"data-block-el": "articleTeaser"})
-
-        # Remove advertisement articles
-        articles = [article for article in articles if not article.find("h3")]
-
-        # Get articles urls
-        urls = [article.find('a')['href'] for article in articles]
-
-        # Get articles publication dates
-        time_regex = re.compile(r'\d{1,2}\.\s\w+,\s\d{1,2}\.\d{2}\sUhr')
-        pub_dates = []
-        for article in articles:
-            try:
-                pub_dates.append(pd.to_datetime(f'{article.find(string=time_regex)}; {day.year}',
-                                                format='%d. %B, %H.%M Uhr; %Y').tz_localize('Europe/Berlin'))
-
-            except ValueError:
-                log.warning(f'Could not parse publication date for article {article.find("a")["href"]}: '
-                            f'{article.find(string=time_regex)}.')
-                pub_dates.append(dt.datetime(day.year, day.month, day.day, tzinfo=dt.timezone.utc))
+            [str]: List of urls of the articles published on the given day.
+            [dt.datetime]: List of publication dates of the articles published on the given day. Needs timezone
+                information.
+        """
+        if day.day != 1:
+            return [], []
+
+        # Get all categories
+        bla = self._request('https://www.sueddeutsche.de/archiv/politik/2021')
+        soup = BeautifulSoup(bla, "html.parser")
+        categories = soup.find('select', {'id': 'dep'}).find_all('option')
+        categories = [category['value'] for category in categories]
+        categories.remove('none')
+
+        # Handle categories
+        urls = []
+        for category in categories:
+            # Handle pagination
+            old_len = len(urls)
+            page = 0
+            while True:
+                page += 1
+                url = f'https://www.sueddeutsche.de/archiv/{category}/{day.strftime("%Y/%-m")}/page/{page}'
+                html = self._request(url)
+                if html is None:
+                    return []
+                soup = BeautifulSoup(html, "html.parser")
+                # Get list of article elements
+                articles = soup.find_all('div', {'class': 'entrylist__entry'})
+                if not articles:
+                    break
+
+                # Filter out dpa articles
+                articles = [article for article in articles if not (
+                        article.find("span", class_="breadcrumb-list__item")
+                        and article.find("span", class_="breadcrumb-list__item").text.strip() == "dpa")]
+
+                # Add article urls to list
+                [urls.append(article.find('a')['href']) for article in articles]
+            log.info(f'Indexed {len(urls) - old_len} articles for category {category} in {day.strftime("%Y-%m")}.')
+
+        # Remove query strings from urls (already here because this will create duplicates)
+        urls = [url.split('?')[0] for url in urls]
+
+        # Remove duplicates
+        old_len = len(urls)
+        urls = list(set(urls))
+        if len(urls) < old_len:
+            log.warning(f"Removed {old_len - len(urls)} duplicate urls for {day.strftime('%Y-%m-%d')}.")
 
-        assert len(urls) == len(pub_dates), 'Number of urls and pub_dates does not match.'
+        # Remove advertisements
+        urls = [url for url in urls if not re.search(r'advertorial.sueddeutsche.de', url)]
+
+        # Create list of publication dates, since the website does not provide them
+        pub_dates = [dt.datetime.combine(day, dt.datetime.min.time(), tzinfo=dt.timezone.utc)] * len(urls)
 
         return urls, pub_dates
 
     def _soup_get_html(self, url: str):
         """
         For a single article, determine if it is premium content and scrape the html if it is not.
 
         Args:
             url (str): Url of the article to scrape.
 
         Returns:
-            html (str): Html of the article. If the article is premium content, None is returned.
-            is_premium (bool): True if the article is premium content, False otherwise.
+            str: Html of the article. If the article is premium content, None is returned.
+            bool: True if the article is premium content, False otherwise.
         """
-        try:
-            html = requests.get(url).content
-            soup = BeautifulSoup(html, "html.parser")
-            premium_icon = soup.find("header", {"data-area": "intro"}).find('svg', {"id": "spon-spplus-flag-l"})
-        except AttributeError:
-            log.warning(f'Error scraping {url}.')
+        response = self._request(url, get_full_response=True)
+        if not response:
             return None, False
-        return html, not bool(premium_icon)
+        if response.history:
+            redirected_url = response.url
+        else:
+            redirected_url = url
+
+        premium = re.search(r'reduced=true', redirected_url)
+
+        return response.text, not bool(premium)
 
     def _selenium_login(self, username: str, password: str):
         """
-        Using selenium, login to the newspaper website to allow scraping of premium content after the login. Does three
-        things:
-            1. Go to main page and accept cookies.
-            2. Login.
-            3. Check if login was successful.
-
+        Using selenium, login to the newspaper website to allow scraping of premium content after the login.
         Args:
             username (str): Username to login to the newspaper website.
             password (str): Password to login to the newspaper website.
 
         Returns:
             bool: True if login was successful, False otherwise.
         """
-        # Go to main page and accept cookies
-        self.selenium_driver.get('https://www.spiegel.de/')
+        # Accept cookies
+        self.selenium_driver.get('https://www.sueddeutsche.de/')
         privacy_frame = WebDriverWait(self.selenium_driver, 10).until(
-            ec.presence_of_element_located((By.XPATH, '//iframe[@title="Privacy Center"]')))
+            ec.presence_of_element_located((By.XPATH, '//iframe[@title="SP Consent Message"]')))
         self.selenium_driver.switch_to.frame(privacy_frame)
-        self.selenium_driver.find_element(By.XPATH, "//button[contains(text(), 'Akzeptieren und weiter')]").click()
+        cookie_accept_button = WebDriverWait(self.selenium_driver, 10).until(
+            ec.element_to_be_clickable((By.XPATH, "//button[contains(text(), 'Ich bin einverstanden')]")))
+        cookie_accept_button.click()
 
         # Login
-        self.selenium_driver.get('https://gruppenkonto.spiegel.de/anmelden.html')
-        self.selenium_driver.find_element(By.NAME, 'loginform:username').send_keys(username)
-        self.selenium_driver.find_element(By.NAME, 'loginform:submit').click()
-        self.selenium_driver.find_element(By.NAME, 'loginform:password').send_keys(password)
-        self.selenium_driver.find_element(By.NAME, 'loginform:submit').click()
-
-        # Go to main page
-        self.selenium_driver.get('https://www.spiegel.de/')
-
-        # Accept cookies again, if needed
-        privacy_frame = WebDriverWait(self.selenium_driver, 10).until(
-            ec.presence_of_element_located((By.XPATH, '//iframe[@title="Privacy Center"]')))
-        self.selenium_driver.switch_to.frame(privacy_frame)
-        self.selenium_driver.find_element(By.XPATH, "//button[contains(text(), 'Akzeptieren und weiter')]").click()
-
-        # Click on Anmelden button because sometimes the login is not saved on main page
-        try:
-            self.selenium_driver.find_element(By.XPATH, '//a[@data-sara-link="gruppenkonto"]').click()
-        except ElementNotInteractableException:
-            pass
+        self.selenium_driver.get('https://id.sueddeutsche.de/login')
+        self.selenium_driver.find_element(By.XPATH, '//input[@name="login"]').send_keys(username)
+        self.selenium_driver.find_element(By.XPATH, '//input[@name="password"]').send_keys(password)
+        self.selenium_driver.find_element(By.XPATH, '//button[@type="submit"]').click()
+        time.sleep(10)
+
+        # Go to main page and click on login button (it is not saved)
+        self.selenium_driver.get('https://www.sueddeutsche.de/')
+        self.selenium_driver.find_element(By.XPATH, '//a[@class="custom-u47b19"]').click()
 
-        # Check if loggin was successful
-        self.selenium_driver.get('https://www.spiegel.de/')
+        # Check if login was successful
         try:
             WebDriverWait(self.selenium_driver, 10).until(
-                ec.presence_of_element_located((By.XPATH, '//a[@href="https://www.spiegel.de/fuermich/"]')))
-            log.info('Logged in to Spiegel Plus.')
+                ec.presence_of_element_located((By.XPATH, f"//a[contains(text(), 'Logout')]")))
+            log.info('Logged in to Sueddeutsche Zeitung.')
             return True
         except TimeoutException:
-            log.error('Login to Spiegel Plus failed.')
+            log.error('Login to Sueddeutsche Zeitung failed.')
             return False
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `newspaper_scraper-0.2.0/newspaper_scraper/sites/welt.py` & `newspaper_scraper-0.2.1/newspaper_scraper/sites/tagesspiegel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 """
-This module contains the class to scrape articles from the "Welt" newspaper (https://www.welt.de/).
+This module contains the class to scrape articles from the "Tagesspiegel" newspaper (https://www.tagesspiegel.de/).
 The class inherits from the NewspaperManager class and needs an implementation of the abstract methods.
 With a similar implementation, it is possible to scrape articles from other news websites.
 """
-import re
 import datetime as dt
-import time
 
 import requests
 from bs4 import BeautifulSoup
-import pandas as pd
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as ec
-from selenium.common.exceptions import NoSuchElementException
+from selenium.common.exceptions import TimeoutException
 
 from ..utils.logger import log
 from ..scraper import NewspaperManager
 
 
-class DeWelt(NewspaperManager):
+class DeTagesspiegel(NewspaperManager):
     """
     This class inherits from the NewspaperManager class and implements the newspaper specific methods.
     These methods are:
-        - _get_published_articles: Index articles published on a given day and return the urls and publication dates.
+        - _get_articles_by_date: Index articles published on a given day and return the urls and publication dates.
         - _soup_get_html: Determine if an article is premium content and scrape the html if it is not. Uses
             beautifulsoup.
         - _selenium_login: Login to the newspaper website to allow scraping of premium content after the login. Uses
             selenium.
     """
 
     def __init__(self, db_file: str = 'articles.db'):
@@ -37,99 +34,98 @@
         """
         Index articles published on a given day and return the urls and publication dates.
 
         Args:
             day (dt.date): Date of the articles to index.
 
         Returns:
-            urls ([str]): List of urls of the articles published on the given day.
-            pub_dates ([dt.datetime]): List of publication dates of the articles published on the given day.
-              Needs timezone information.
-        """
-        URL = f'https://www.welt.de/schlagzeilen/nachrichten-vom-{day.strftime("%-d-%-m-%Y")}.html'
-
-        soup = BeautifulSoup(requests.get(URL).content, "html.parser")
-        articles = soup \
-            .find("div", {"class": "c-tabs__panel-content"}) \
-            .find_all("article", {"class": "c-teaser c-teaser--archive"})
-
-        # Get articles urls
-        urls = ['https://www.welt.de' + article.find('h4').find('a')['href'] for article in articles]
-
-        # Get articles publication dates
-        time_regex = re.compile(r'\d{2}\.\d{2}\.\d{4}\s\|\s\d{2}:\d{2}')
-        pub_dates = [pd.to_datetime(f'{article.find(string=time_regex)}', format='%d.%m.%Y | %H:%M')
-                     for article in articles]
-        # Add timezone Europe/Berlin to pub_dates
-        pub_dates = [pub_date.tz_localize('UTC') for pub_date in pub_dates]
+            [str]: List of urls of the articles published on the given day.
+            [dt.datetime]: List of publication dates of the articles published on the given day. Needs timezone
+                information.
+        """
+        url = f'https://www.tagesspiegel.de/archiv/{day.strftime("%Y/%m/%d")}/'
+
+        # Handle pagination
+        urls = []
+        page = 0
+        while True:
+            page += 1
+            html = self._request(url + (f'{page}' if page > 1 else ''))
+            if not html:
+                break
+            soup = BeautifulSoup(html, "html.parser")
+            # Get list of article elements
+            articles = soup.find_all('article')
+            # Add article urls to list
+            [urls.append('https://www.tagesspiegel.de' + article.find('a')['href']) for article in articles]
+
+        # Remove duplicates
+        old_len = len(urls)
+        urls = list(set(urls))
+        if len(urls) < old_len:
+            log.warning(f"Removed {old_len - len(urls)} duplicate urls for {day.strftime('%Y-%m-%d')}.")
 
-        assert len(urls) == len(pub_dates), 'Number of urls and pub_dates does not match.'
+        # Create list of publication dates, since the website does not provide them
+        pub_dates = [dt.datetime.combine(day, dt.datetime.min.time(), tzinfo=dt.timezone.utc)] * len(urls)
 
         return urls, pub_dates
 
     def _soup_get_html(self, url: str):
         """
         For a single article, determine if it is premium content and scrape the html if it is not.
 
         Args:
             url (str): Url of the article to scrape.
 
         Returns:
-            html (str): Html of the article. If the article is premium content, None is returned.
-            is_premium (bool): True if the article is premium content, False otherwise.
+            str: Html of the article. If the article is premium content, None is returned.
+            bool: True if the article is premium content, False otherwise.
         """
+        html = self._request(url)
+        soup = BeautifulSoup(html, "html.parser")
         try:
-            html = requests.get(url).content
-            soup = BeautifulSoup(html, "html.parser")
-            premium_icon = soup.find("header", {"class": "c-content-container"}).\
-                find('a', {"class": "o-dreifaltigkeit__premium-badge"})
+            premium_icon = soup.find('div', {'class': 'Uk'}).find('svg')
+            return html, not bool(premium_icon)
         except AttributeError:
-            log.warning(f'Error scraping {url}.')
+            log.warning(f'Could not identify if article is premium: {url}.')
             return None, False
-        return html, not bool(premium_icon)
 
     def _selenium_login(self, username: str, password: str):
         """
-        Using selenium, login to the newspaper website to allow scraping of premium content after the login. Does three
-        things:
-            1. Go to main page and accept cookies.
-            2. Login.
-            3. Check if login was successful.
-
+        Using selenium, login to the newspaper website to allow scraping of premium content after the login.
         Args:
             username (str): Username to login to the newspaper website.
             password (str): Password to login to the newspaper website.
 
         Returns:
             bool: True if login was successful, False otherwise.
         """
-        # Go to main page and accept cookies
-        self.selenium_driver.get('https://www.welt.de/')
+        # Accept cookies on main page
+        self.selenium_driver.get('https://www.tagesspiegel.de/')
         privacy_frame = WebDriverWait(self.selenium_driver, 10).until(
-            ec.presence_of_element_located((By.XPATH, '//iframe[@title="SP Consent Message"]'))
-        )
+            ec.presence_of_element_located((By.XPATH, '//iframe[@title="Iframe title"]')))
         self.selenium_driver.switch_to.frame(privacy_frame)
-        WebDriverWait(self.selenium_driver, 10).until(
-            ec.presence_of_element_located((By.CSS_SELECTOR, 'button[title="Alle akzeptieren"]')))
-        self.selenium_driver.find_element(By.CSS_SELECTOR, 'button[title="Alle akzeptieren"]').click()
+        cookie_accept_button = WebDriverWait(self.selenium_driver, 10).until(
+            ec.element_to_be_clickable((By.XPATH, "//button[contains(text(), 'Alle akzeptieren')]")))
+        cookie_accept_button.click()
 
         # Login
-        self.selenium_driver.get('https://lo.la.welt.de/login')
+        self.selenium_driver.find_element(By.XPATH,
+                                          '//a[@title="Melden Sie sich mit Ihrem Tagesspiegel-Konto an"]').click()
+        privacy_frame = WebDriverWait(self.selenium_driver, 10).until(
+            ec.presence_of_element_located((By.XPATH, '//iframe[@id="modal-iframe"]')))
+        self.selenium_driver.switch_to.frame(privacy_frame)
         WebDriverWait(self.selenium_driver, 10).until(
-            ec.presence_of_element_located((By.NAME, 'username')))
-        self.selenium_driver.find_element(By.NAME, 'username').send_keys(username)
-        self.selenium_driver.find_element(By.NAME, 'password').send_keys(password)
-        self.selenium_driver.find_element(By.CSS_SELECTOR, 'button[type="submit"]').click()
+            ec.element_to_be_clickable((By.XPATH, '//input[@name="email"]')))
+        self.selenium_driver.find_element(By.XPATH, '//input[@name="email"]').send_keys(username)
+        self.selenium_driver.find_element(By.XPATH, '//input[@name="password"]').send_keys(password)
+        self.selenium_driver.find_element(By.XPATH, '//button[@type="submit"]').click()
 
         # Check if login was successful
         try:
-            self.selenium_driver.get('https://www.welt.de/meinewelt/')
             WebDriverWait(self.selenium_driver, 10).until(
-                ec.presence_of_element_located((By.CSS_SELECTOR, 'div[data-component-name="home"]')))
-            _elem = self.selenium_driver.find_element(By.CSS_SELECTOR, 'div[data-component-name="home"]')
-            WebDriverWait(_elem, 10).until(ec.presence_of_element_located((By.CSS_SELECTOR, 'div[name="greeting"]')))
-            self.selenium_driver.get('https://www.welt.de')
-            log.info('Logged in to Welt Plus.')
+                ec.presence_of_element_located((By.XPATH, "//span[contains(text(), 'Mein Konto')]")))
+            log.info('Logged in to Tagesspiegel.')
             return True
-        except NoSuchElementException:
-            log.warning('Login to Welt Plus failed.')
+        except TimeoutException:
+            log.error('Login to Tagesspiegel failed.')
             return False
```

### Comparing `newspaper_scraper-0.2.0/newspaper_scraper/sites/zeit.py` & `newspaper_scraper-0.2.1/newspaper_scraper/sites/zeit.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ..scraper import NewspaperManager
 
 
 class DeZeit(NewspaperManager):
     """
     This class inherits from the NewspaperManager class and implements the newspaper specific methods.
     These methods are:
-        - _get_articles_by_edition: Index articles published in a given edition and return the urls and publication
+        - _get_articles_by_date: Index articles published in a given edition and return the urls and publication
         - _soup_get_html: Determine if an article is premium content and scrape the html if it is not. Uses
             beautifulsoup.
         - _selenium_login: Login to the newspaper website to allow scraping of premium content after the login. Uses
             selenium.
         - _selenium_get_html: Scrape the html of an article using selenium. Uses selenium. A specific implementation is
             needed here because the website uses pagination on some articles.
     """
@@ -39,91 +39,88 @@
 
         Args:
             year (int): Year of the edition to index.
             edition (int): Edition number of the edition to index. Can be similar to a week number, but is not
                 necessarily the same.
 
         Returns:
-            urls ([str]): List of urls of the articles published on the given day.
+        [str]: List of urls of the articles published on the given day.
         """
         # Get week number of day
-        URL = f'https://www.zeit.de/{year}/{edition:02}/index'
+        url = f'https://www.zeit.de/{year}/{edition:02}/index'
 
-        soup = BeautifulSoup(requests.get(URL).content, "html.parser")
-        articles = soup.find_all("article")
+        html = self._request(url)
+        if html is None:
+            return []
+        soup = BeautifulSoup(html, "html.parser")
 
+        # Get list of article elements
+        articles = soup.find_all("article")
         # Get articles urls
         urls = [article.find('a')['href'] for article in articles]
         urls = [url for url in urls if url.startswith('https://www.zeit.de/')]
+
         # Remove duplicates
+        old_len = len(urls)
         urls = list(set(urls))
+        log.warning(f"Removed {old_len - len(urls)} duplicate urls for {year}/{edition:02}.")
 
         return urls
 
     def _soup_get_html(self, url: str):
         """
         For a single article, determine if it is premium content and scrape the html if it is not.
 
         Args:
             url (str): Url of the article to scrape.
 
         Returns:
-            html (str): Html of the article. If the article is premium content, None is returned.
-            is_premium (bool): True if the article is premium content, False otherwise.
+            str: Html of the article. If the article is premium content, None is returned.
+            bool: True if the article is premium content, False otherwise.
         """
-        response = requests.get(url)
-        if response.status_code == 200:
-            soup = BeautifulSoup(response.text, 'html.parser')
-            komplettansicht_link = soup.find("a", href=f"{url}/komplettansicht")
-            # Run again with /komplettansicht if it exists
-            if komplettansicht_link:
-                return self._soup_get_html(f"{url}/komplettansicht")
-            else:
-                try:
-                    premium = soup.find('aside', {'id': 'paywall'})
-                    return response.text, not bool(premium)
-                except AttributeError:
-                    log.warning(f'Error scraping {url}.')
-                    return None, False
-        else:
-            log.warning(f"Error fetching the URL: {response.status_code}")
-            return None, False
+        html = self._request(url)
+        soup = BeautifulSoup(html, "html.parser")
 
+        # Run again with /komplettansicht if a full page exists
+        komplettansicht_link = soup.find("a", href=f"{url}/komplettansicht")
+        if komplettansicht_link:
+            return self._soup_get_html(f"{url}/komplettansicht")
+
+        try:
+            premium_icon = soup.find('aside', {'id': 'paywall'})
+            return html, not bool(premium_icon)
+        except AttributeError:
+            log.warning(f'Could not identify if article is premium: {url}.')
+            return None, False
 
     def _selenium_login(self, username: str, password: str):
         """
-        Using selenium, login to the newspaper website to allow scraping of premium content after the login. Does three
-        things:
-            1. Login
-            2. Accept cookies
-            3. Check if login was successful
-
+        Using selenium, login to the newspaper website to allow scraping of premium content after the login.
         Args:
             username (str): Username to login to the newspaper website.
             password (str): Password to login to the newspaper website.
 
         Returns:
             bool: True if login was successful, False otherwise.
         """
-
         # Login
         self.selenium_driver.get('https://meine.zeit.de/anmelden')
         self.selenium_driver.find_element(By.XPATH, '//input[@type="email"]').send_keys(username)
         self.selenium_driver.find_element(By.XPATH, '//input[@type="password"]').send_keys(password)
         self.selenium_driver.find_element(By.XPATH, '//input[@type="submit"]').click()
 
         # Accept cookies
         privacy_frame = WebDriverWait(self.selenium_driver, 10).until(
             ec.presence_of_element_located((By.XPATH, '//iframe[@title="SP Consent Message"]')))
         self.selenium_driver.switch_to.frame(privacy_frame)
         cookie_accept_button = WebDriverWait(self.selenium_driver, 10).until(
             ec.element_to_be_clickable((By.XPATH, "//button[contains(text(), 'AKZEPTIEREN UND WEITER')]")))
         cookie_accept_button.click()
 
-        # Check if loggin was successful
+        # Check if login was successful
         try:
             WebDriverWait(self.selenium_driver, 10).until(
                 ec.presence_of_element_located((By.XPATH, '//span[@class="dashboard__title"]')))
             log.info('Logged in to Zeit Plus.')
             return True
         except TimeoutException:
             log.error('Login to Zeit Plus failed.')
```

### Comparing `newspaper_scraper-0.2.0/newspaper_scraper/utils/utils.py` & `newspaper_scraper-0.2.1/newspaper_scraper/utils/utils.py`

 * *Files identical despite different names*

### Comparing `newspaper_scraper-0.2.0/newspaper_scraper.egg-info/PKG-INFO` & `newspaper_scraper-0.2.1/newspaper_scraper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newspaper-scraper
-Version: 0.2.0
+Version: 0.2.1
 Summary: The all-in-one Python package for seamless newspaper article indexing, scraping, and processing – supports public and premium content!
 Author-email: Lukas Trippe <lkstrp@pm.me>
 License: MIT License
         
         Copyright (c) 2023 Lukas Trippe
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,21 +44,23 @@
 1. Indexing: Index articles from a newspaper website using the [beautifulsoup](https://beautiful-soup-4.readthedocs.io/en/latest/) package for public articles and [selenium](https://selenium-python.readthedocs.io/) for paywall content.  
 2. Extraction: Extract article content using the [goose3](https://github.com/goose3/goose3) package.  
 3. Processing: Process articles for nlp features using the [spaCy](https://spacy.io/) package.  
   
 The indexing functionality is based on a dedicated file for each newspaper. A few newspapers are already supported, but it is easy to add new ones.  
   
 ### Supported Newspapers  
-| Logo | Newspaper | Country | Time span | Number of articles |  
-| ----------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------- | ------- | --------- | --------------- |  
-| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Der_Spiegel_2022_logo.svg/640px-Der_Spiegel_2022_logo.svg.png" height="70"> | [Der Spiegel](https://www.spiegel.de/) | Germany | Since 2000 | tbd |  
-| <img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/Die_Welt_Logo_2015.png" height="70"> | [Die Welt](https://www.welt.de/) | Germany | Since 2000 | tbd  
-| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/Logo_BILD.svg/1920px-Logo_BILD.svg.png" height="70"> | [Bild](https://www.bild.de/) | Germany | Since 2006 | tbd |  
-| <img src="https://upload.wikimedia.org/wikipedia/commons/6/60/Die_Zeit-Logo-Bremen.svg" height="70"> | [Die Zeit](https://www.zeit.de/) | Germany | Since 1946 | tbd |   
-| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/ff/Handelsblatt_201x_logo.svg/2880px-Handelsblatt_201x_logo.svg.png" height="70"> | [Handelsblatt](https://www.handelsblatt.com/) | Germany | Since 2003 | tbd |  
+| Logo | Newspaper                                        | Country | Time span  | Number of articles |  
+| ----------------------------------------------------------------------------------------------------------------------------------------------- |--------------------------------------------------| ------- |------------| --------------- |  
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Der_Spiegel_2022_logo.svg/640px-Der_Spiegel_2022_logo.svg.png" height="70"> | [Der Spiegel](https://www.spiegel.de/)           | Germany | Since 2000 | tbd |  
+| <img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/Die_Welt_Logo_2015.png" height="70"> | [Die Welt](https://www.welt.de/)                 | Germany | Since 2000 | tbd  
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/Logo_BILD.svg/1920px-Logo_BILD.svg.png" height="70"> | [Bild](https://www.bild.de/)                     | Germany | Since 2006 | tbd |  
+| <img src="https://upload.wikimedia.org/wikipedia/commons/6/60/Die_Zeit-Logo-Bremen.svg" height="70"> | [Die Zeit](https://www.zeit.de/)                 | Germany | Since 1946 | tbd |   
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/ff/Handelsblatt_201x_logo.svg/2880px-Handelsblatt_201x_logo.svg.png" height="70"> | [Handelsblatt](https://www.handelsblatt.com/)    | Germany | Since 2003 | tbd | 
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1d/Tagesspiegel_%282022-11-29%29.svg/2880px-Tagesspiegel_%282022-11-29%29.svg.png" height="70"> | [Der Tagesspiegel](https://www.tagesspiegel.de/) | Germany | Since 2000 | tbd |
+| <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/42/S%C3%BCddeutsche_Zeitung_Logo.svg/2880px-S%C3%BCddeutsche_Zeitung_Logo.svg.png" height="70"> | [Süddeutsche Zeitung](https://www.sueddeutsche.de/)    | Germany | Since 2001 | tbd |
 
 ## Setup  
 It is recommended to install the package in an dedicated Python environment.  
 To install the package via pip, run the following command:  
   
 ```bash  
 pip install newspaper-scraper
@@ -70,21 +72,21 @@
 pip install newspaper-scraper[nlp]
 ```  
   
 ## Usage  
 To index, extract and process all public and premium articles from [Der Spiegel](https://www.spiegel.de/), published in August 2021, run the following code:  
   
 ```python  
-import newspaper_scraper as ns  
+import newspaper_scraper as nps  
 from credentials import username, password  
   
-with ns.Spiegel(db_file='articles.db') as news:
-news.index_articles_by_date_range('2021-08-01', '2021-08-31')  
-news.scrape_public_articles()
-news.scrape_premium_articles(username=username, password=password)  
-news.nlp()
+with nps.Spiegel(db_file='articles.db') as news:
+    news.index_articles_by_date_range('2021-08-01', '2021-08-31')  
+    news.scrape_public_articles()
+    news.scrape_premium_articles(username=username, password=password)  
+    news.nlp()
 ```  
   
 This will create a sqlite database file called `articles.db` in the current working directory. The database contains the following tables:  
 - `tblArticlesIndexed`: Contains all indexed articles with their scraping/ processing status and whether they are public or premium content.  
 - `tblArticlesScraped`: Contains metadata for all parsed articles, provided by goose3.  
 - `tblArticlesProcessed`: Contains nlp features of the cleaned article text, provided by spaCy.
```

### Comparing `newspaper_scraper-0.2.0/newspaper_scraper.egg-info/SOURCES.txt` & `newspaper_scraper-0.2.1/newspaper_scraper.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 newspaper_scraper.egg-info/dependency_links.txt
 newspaper_scraper.egg-info/requires.txt
 newspaper_scraper.egg-info/top_level.txt
 newspaper_scraper/sites/__init__.py
 newspaper_scraper/sites/bild.py
 newspaper_scraper/sites/handelsblatt.py
 newspaper_scraper/sites/spiegel.py
-newspaper_scraper/sites/sz.py
+newspaper_scraper/sites/sueddeutsche.py
+newspaper_scraper/sites/tagesspiegel.py
 newspaper_scraper/sites/welt.py
 newspaper_scraper/sites/zeit.py
 newspaper_scraper/utils/__init__.py
 newspaper_scraper/utils/logger.py
 newspaper_scraper/utils/utils.py
```

### Comparing `newspaper_scraper-0.2.0/pyproject.toml` & `newspaper_scraper-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "newspaper_scraper"
-version = "0.2.0"
+version = "0.2.1"
 description = "The all-in-one Python package for seamless newspaper article indexing, scraping, and processing – supports public and premium content!"
 authors = [{ name = "Lukas Trippe", email = "lkstrp@pm.me" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

