# Comparing `tmp/NewsArticlesScraper-0.2.3.tar.gz` & `tmp/NewsArticlesScraper-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewsArticlesScraper-0.2.3.tar", last modified: Mon May  8 19:41:37 2023, max compression
+gzip compressed data, was "NewsArticlesScraper-0.2.4.tar", last modified: Wed May 17 14:47:23 2023, max compression
```

## Comparing `NewsArticlesScraper-0.2.3.tar` & `NewsArticlesScraper-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 19:41:37.781732 NewsArticlesScraper-0.2.3/
-drwxrwxrwx   0        0        0        0 2023-05-08 19:41:37.762231 NewsArticlesScraper-0.2.3/NewsArticlesScraper/
--rw-rw-rw-   0        0        0    13964 2023-05-08 18:46:27.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper/Scrapers.py
--rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper/__init__.py
--rw-rw-rw-   0        0        0     1074 2023-04-23 16:12:20.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper/test.py
-drwxrwxrwx   0        0        0        0 2023-05-08 19:41:37.780231 NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/
--rw-rw-rw-   0        0        0      648 2023-05-08 19:41:37.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-08 19:41:37.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 19:41:37.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-05-08 19:41:37.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-08 19:41:37.000000 NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      648 2023-05-08 19:41:37.781232 NewsArticlesScraper-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 19:41:37.782233 NewsArticlesScraper-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      996 2023-05-08 19:40:59.000000 NewsArticlesScraper-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:47:23.141795 NewsArticlesScraper-0.2.4/
+drwxrwxrwx   0        0        0        0 2023-05-17 14:47:23.119791 NewsArticlesScraper-0.2.4/NewsArticlesScraper/
+-rw-rw-rw-   0        0        0    14552 2023-05-17 14:41:40.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper/Scrapers.py
+-rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper/__init__.py
+-rw-rw-rw-   0        0        0     1074 2023-04-23 16:12:20.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper/test.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:47:23.139293 NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/
+-rw-rw-rw-   0        0        0      648 2023-05-17 14:47:23.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-17 14:47:23.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 14:47:23.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-17 14:47:23.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-17 14:47:23.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      648 2023-05-17 14:47:23.140795 NewsArticlesScraper-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 14:47:23.141795 NewsArticlesScraper-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-05-17 14:47:13.000000 NewsArticlesScraper-0.2.4/setup.py
```

### Comparing `NewsArticlesScraper-0.2.3/NewsArticlesScraper/Scrapers.py` & `NewsArticlesScraper-0.2.4/NewsArticlesScraper/Scrapers.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,19 @@
             'scrapy_user_agents.middlewares.RandomUserAgentMiddleware': 400,
         },
         'RANDOM_UA_TYPE': "random",
         'RETRY_ENABLED': True,
         'RETRY_TIMES': 5,
     }
 
-    def __init__(self, from_time: datetime.datetime, until_time: datetime.datetime, user_agent=None, **kwargs):
-        self.url_stream = "https://api.queryly.com/cnbc/json.aspx?queryly_key=31a35d40a9a64ab3&query=cnbc&endindex={" \
-                          "}&batchsize=100&timezoneoffset=-60&sort=date"
+    def __init__(self, from_time: datetime.datetime, until_time: datetime.datetime, user_agent=None,
+                 query: str = "cnbc", **kwargs):
+        self.url_stream = "https://api.queryly.com/cnbc/json.aspx?queryly_key=31a35d40a9a64ab3&query=" + \
+                          query + "&endindex={" \
+                                  "}&batchsize=100&timezoneoffset=-60&sort=date"
         self.from_time = from_time
         self.until_time = until_time
         self.start_page = None
         self.end_page = None
         if user_agent is not None:
             self.custom_settings["USER_AGENT"] = user_agent
         super().__init__(**kwargs)
@@ -146,24 +148,26 @@
             'scrapy_user_agents.middlewares.RandomUserAgentMiddleware': 400,
         },
         'RANDOM_UA_TYPE': "random",
         'RETRY_ENABLED': True,
         'RETRY_TIMES': 5,
     }
 
-    def __init__(self, from_time: datetime.datetime, until_time: datetime.datetime, api_key, user_agent=None, **kwargs):
+    def __init__(self, from_time: datetime.datetime, until_time: datetime.datetime, api_key, user_agent=None,
+                 subsections_to_include: list = None, **kwargs):
         self.api_key = api_key
         self.from_time = from_time
         self.until_time = until_time
         if (datetime.datetime.now(pytz.timezone("GMT")) - self.until_time).total_seconds() <= 86400:
             self.recent = True
         else:
             self.recent = False
         if user_agent is not None:
             self.custom_settings["USER_AGENT"] = user_agent
+        self.subsections_to_include = subsections_to_include
         super().__init__(**kwargs)
 
     def start_requests(self):
         url_api_historic = "https://api.nytimes.com/svc/archive/v1/{}/{}.json?api-key=" + self.api_key
         year_min = int(self.from_time.strftime('%Y'))
         year_max = int(self.until_time.strftime('%Y'))
         month_max = int(self.until_time.strftime('%m'))
@@ -184,14 +188,20 @@
         data = response.json()
         api_point = response.meta["api_point"]
         if api_point == "historic":
             articles = data["response"]["docs"]
         else:
             articles = data["results"]
         for article in articles:
+            if api_point == "historic" and self.subsections_to_include is not None:
+                if article["subsection_name"] not in self.subsections_to_include:
+                    continue
+            if api_point == "recent" and self.subsections_to_include is not None:
+                if article["section"] not in self.subsections_to_include:
+                    continue
             if api_point == "historic":
                 pub_date = article["pub_date"]
             else:
                 pub_date = article["published_date"]
             pub_date = ciso8601.parse_datetime(pub_date)
             if pub_date < self.from_time:
                 break
```

### Comparing `NewsArticlesScraper-0.2.3/NewsArticlesScraper/test.py` & `NewsArticlesScraper-0.2.4/NewsArticlesScraper/test.py`

 * *Files identical despite different names*

### Comparing `NewsArticlesScraper-0.2.3/NewsArticlesScraper.egg-info/PKG-INFO` & `NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.3
+Version: 0.2.4
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.3/PKG-INFO` & `NewsArticlesScraper-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.3
+Version: 0.2.4
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.3/setup.py` & `NewsArticlesScraper-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.3'
+VERSION = '0.2.4'
 DESCRIPTION = 'Scraping news articles'
 LONG_DESCRIPTION = 'A package that allows you to scrape news articles from various news sites via scrapy.'
 
 # Setting up
 setup(
     name="NewsArticlesScraper",
     version=VERSION,
```

