# Comparing `tmp/mktrader-0.0.5.tar.gz` & `tmp/mktrader-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mktrader-0.0.5.tar", last modified: Sat May 13 17:50:03 2023, max compression
+gzip compressed data, was "mktrader-0.0.6.tar", last modified: Wed May 17 19:17:54 2023, max compression
```

## Comparing `mktrader-0.0.5.tar` & `mktrader-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mmurphy  (433907835) 1133555842        0 2023-05-13 17:50:03.184641 mktrader-0.0.5/
--rw-r--r--   0 mmurphy  (433907835) 1133555842     1068 2023-05-11 23:09:55.000000 mktrader-0.0.5/LICENSE
--rw-r--r--   0 mmurphy  (433907835) 1133555842      699 2023-05-13 17:50:03.184512 mktrader-0.0.5/PKG-INFO
--rw-r--r--   0 mmurphy  (433907835) 1133555842      213 2023-05-11 23:10:15.000000 mktrader-0.0.5/README.md
-drwxr-xr-x   0 mmurphy  (433907835) 1133555842        0 2023-05-13 17:50:03.183627 mktrader-0.0.5/mktrader/
--rw-r--r--   0 mmurphy  (433907835) 1133555842      185 2023-05-11 23:10:15.000000 mktrader-0.0.5/mktrader/__init__.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     5507 2023-05-13 13:56:42.000000 mktrader-0.0.5/mktrader/brokers.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     4300 2023-05-12 03:52:25.000000 mktrader-0.0.5/mktrader/engines.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     6389 2023-05-13 17:46:41.000000 mktrader-0.0.5/mktrader/feeds.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     3894 2023-05-12 03:57:48.000000 mktrader-0.0.5/mktrader/helpers.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     4754 2023-05-11 23:10:15.000000 mktrader-0.0.5/mktrader/indicators.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     1244 2023-05-11 23:10:15.000000 mktrader-0.0.5/mktrader/logger.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     7590 2023-05-13 13:53:12.000000 mktrader-0.0.5/mktrader/models.py
--rw-r--r--   0 mmurphy  (433907835) 1133555842     1055 2023-05-12 03:59:20.000000 mktrader-0.0.5/mktrader/strategies.py
-drwxr-xr-x   0 mmurphy  (433907835) 1133555842        0 2023-05-13 17:50:03.184324 mktrader-0.0.5/mktrader.egg-info/
--rw-r--r--   0 mmurphy  (433907835) 1133555842      699 2023-05-13 17:50:03.000000 mktrader-0.0.5/mktrader.egg-info/PKG-INFO
--rw-r--r--   0 mmurphy  (433907835) 1133555842      368 2023-05-13 17:50:03.000000 mktrader-0.0.5/mktrader.egg-info/SOURCES.txt
--rw-r--r--   0 mmurphy  (433907835) 1133555842        1 2023-05-13 17:50:03.000000 mktrader-0.0.5/mktrader.egg-info/dependency_links.txt
--rw-r--r--   0 mmurphy  (433907835) 1133555842       26 2023-05-13 17:50:03.000000 mktrader-0.0.5/mktrader.egg-info/requires.txt
--rw-r--r--   0 mmurphy  (433907835) 1133555842        9 2023-05-13 17:50:03.000000 mktrader-0.0.5/mktrader.egg-info/top_level.txt
--rw-r--r--   0 mmurphy  (433907835) 1133555842       38 2023-05-13 17:50:03.184679 mktrader-0.0.5/setup.cfg
--rw-r--r--   0 mmurphy  (433907835) 1133555842     1017 2023-05-13 17:48:29.000000 mktrader-0.0.5/setup.py
+drwxr-xr-x   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)        0 2023-05-17 19:17:54.086475 mktrader-0.0.6/
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     1068 2023-05-16 19:25:03.000000 mktrader-0.0.6/LICENSE
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)      699 2023-05-17 19:17:54.086333 mktrader-0.0.6/PKG-INFO
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)      213 2023-05-16 19:25:03.000000 mktrader-0.0.6/README.md
+drwxr-xr-x   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)        0 2023-05-17 19:17:54.085349 mktrader-0.0.6/mktrader/
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)      185 2023-05-16 19:25:03.000000 mktrader-0.0.6/mktrader/__init__.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     5514 2023-05-17 19:15:24.000000 mktrader-0.0.6/mktrader/brokers.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     4300 2023-05-16 19:25:03.000000 mktrader-0.0.6/mktrader/engines.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     6389 2023-05-16 19:25:03.000000 mktrader-0.0.6/mktrader/feeds.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     3894 2023-05-16 19:25:03.000000 mktrader-0.0.6/mktrader/helpers.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     4754 2023-05-16 19:25:03.000000 mktrader-0.0.6/mktrader/indicators.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     1244 2023-05-16 19:25:03.000000 mktrader-0.0.6/mktrader/logger.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     7590 2023-05-16 19:25:03.000000 mktrader-0.0.6/mktrader/models.py
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     1055 2023-05-16 19:25:03.000000 mktrader-0.0.6/mktrader/strategies.py
+drwxr-xr-x   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)        0 2023-05-17 19:17:54.086129 mktrader-0.0.6/mktrader.egg-info/
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)      699 2023-05-17 19:17:54.000000 mktrader-0.0.6/mktrader.egg-info/PKG-INFO
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)      368 2023-05-17 19:17:54.000000 mktrader-0.0.6/mktrader.egg-info/SOURCES.txt
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)        1 2023-05-17 19:17:54.000000 mktrader-0.0.6/mktrader.egg-info/dependency_links.txt
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)       26 2023-05-17 19:17:54.000000 mktrader-0.0.6/mktrader.egg-info/requires.txt
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)        9 2023-05-17 19:17:54.000000 mktrader-0.0.6/mktrader.egg-info/top_level.txt
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)       38 2023-05-17 19:17:54.086513 mktrader-0.0.6/setup.cfg
+-rw-r--r--   0 mmurphy  (433907835) CHCS\Domain Users (1133555842)     1017 2023-05-17 19:16:28.000000 mktrader-0.0.6/setup.py
```

### Comparing `mktrader-0.0.5/LICENSE` & `mktrader-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mktrader-0.0.5/PKG-INFO` & `mktrader-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktrader
-Version: 0.0.5
+Version: 0.0.6
 Summary: Stock Market Trading Framework
 Home-page: https://github.com/matthewkurtis/mktrader.git
 Author: Matthew K Murphy (MatthewKurtis)
 Author-email: <mkmurphy526@gmail.com>
 Keywords: python,trading,stock,market
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `mktrader-0.0.5/mktrader/brokers.py` & `mktrader-0.0.6/mktrader/brokers.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             self.api_url = ALPACA_TRADE_API_URL_LIVE
 
         self.headers = {
             'APCA-API-KEY-ID': self.api_key,
             'APCA-API-SECRET-KEY': self.api_secret
         }
 
-    def market_is_open(self) -> bool:
+    def market_is_open(self, *args) -> bool:
         logger.debug("Checking if market is open...")
         endpoint = '/v2/clock'
         url = self.api_url + endpoint
         response = requests.get(url=url, headers=self.headers)
         json_response = response.json()
         return json_response['is_open']
```

### Comparing `mktrader-0.0.5/mktrader/engines.py` & `mktrader-0.0.6/mktrader/engines.py`

 * *Files identical despite different names*

### Comparing `mktrader-0.0.5/mktrader/feeds.py` & `mktrader-0.0.6/mktrader/feeds.py`

 * *Files identical despite different names*

### Comparing `mktrader-0.0.5/mktrader/helpers.py` & `mktrader-0.0.6/mktrader/helpers.py`

 * *Files identical despite different names*

### Comparing `mktrader-0.0.5/mktrader/indicators.py` & `mktrader-0.0.6/mktrader/indicators.py`

 * *Files identical despite different names*

### Comparing `mktrader-0.0.5/mktrader/logger.py` & `mktrader-0.0.6/mktrader/logger.py`

 * *Files identical despite different names*

### Comparing `mktrader-0.0.5/mktrader/models.py` & `mktrader-0.0.6/mktrader/models.py`

 * *Files identical despite different names*

### Comparing `mktrader-0.0.5/mktrader/strategies.py` & `mktrader-0.0.6/mktrader/strategies.py`

 * *Files identical despite different names*

### Comparing `mktrader-0.0.5/mktrader.egg-info/PKG-INFO` & `mktrader-0.0.6/mktrader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktrader
-Version: 0.0.5
+Version: 0.0.6
 Summary: Stock Market Trading Framework
 Home-page: https://github.com/matthewkurtis/mktrader.git
 Author: Matthew K Murphy (MatthewKurtis)
 Author-email: <mkmurphy526@gmail.com>
 Keywords: python,trading,stock,market
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `mktrader-0.0.5/setup.py` & `mktrader-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Stock Market Trading Framework'
 LONG_DESCRIPTION = 'A Framework for simple creation and deployment of trading strategies.'
 
 # Setting up
 setup(
     name="mktrader",
     version=VERSION,
```

