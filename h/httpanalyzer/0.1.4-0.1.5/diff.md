# Comparing `tmp/httpanalyzer-0.1.4.tar.gz` & `tmp/httpanalyzer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpanalyzer-0.1.4.tar", last modified: Tue Apr 11 15:32:25 2023, max compression
+gzip compressed data, was "httpanalyzer-0.1.5.tar", last modified: Wed May 17 06:54:38 2023, max compression
```

## Comparing `httpanalyzer-0.1.4.tar` & `httpanalyzer-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 15:32:25.456770 httpanalyzer-0.1.4/
--rw-rw-rw-   0        0        0     1091 2023-01-16 19:33:15.000000 httpanalyzer-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3249 2023-04-11 15:32:25.456770 httpanalyzer-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2555 2023-03-16 17:24:20.000000 httpanalyzer-0.1.4/README.md
--rw-rw-rw-   0        0        0      779 2023-04-11 15:30:31.000000 httpanalyzer-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 15:32:25.458852 httpanalyzer-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 15:32:25.425169 httpanalyzer-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 15:32:25.439031 httpanalyzer-0.1.4/src/httpanalyzer/
--rw-rw-rw-   0        0        0     3769 2023-02-16 16:21:07.000000 httpanalyzer-0.1.4/src/httpanalyzer/__init__.py
--rw-rw-rw-   0        0        0    10517 2023-04-11 15:28:27.000000 httpanalyzer-0.1.4/src/httpanalyzer/src.py
--rw-rw-rw-   0        0        0      444 2023-02-09 13:36:28.000000 httpanalyzer-0.1.4/src/httpanalyzer/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:32:25.454748 httpanalyzer-0.1.4/src/httpanalyzer.egg-info/
--rw-rw-rw-   0        0        0     3249 2023-04-11 15:32:25.000000 httpanalyzer-0.1.4/src/httpanalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-11 15:32:25.000000 httpanalyzer-0.1.4/src/httpanalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 15:32:25.000000 httpanalyzer-0.1.4/src/httpanalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 15:32:25.000000 httpanalyzer-0.1.4/src/httpanalyzer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 06:54:38.151331 httpanalyzer-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-01-16 19:33:15.000000 httpanalyzer-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     3249 2023-05-17 06:54:38.151331 httpanalyzer-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2555 2023-03-16 17:24:20.000000 httpanalyzer-0.1.5/README.md
+-rw-rw-rw-   0        0        0      779 2023-05-17 06:53:38.000000 httpanalyzer-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 06:54:38.151331 httpanalyzer-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 06:54:38.116483 httpanalyzer-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 06:54:38.134628 httpanalyzer-0.1.5/src/httpanalyzer/
+-rw-rw-rw-   0        0        0     4338 2023-04-29 10:00:22.000000 httpanalyzer-0.1.5/src/httpanalyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:54:38.146292 httpanalyzer-0.1.5/src/httpanalyzer/lists/
+-rw-rw-rw-   0        0        0        0 2023-04-29 09:34:34.000000 httpanalyzer-0.1.5/src/httpanalyzer/lists/__init__.py
+-rw-rw-rw-   0        0        0    10519 2023-04-29 09:25:06.000000 httpanalyzer-0.1.5/src/httpanalyzer/src.py
+-rw-rw-rw-   0        0        0      444 2023-04-29 09:33:58.000000 httpanalyzer-0.1.5/src/httpanalyzer/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:54:38.145238 httpanalyzer-0.1.5/src/httpanalyzer.egg-info/
+-rw-rw-rw-   0        0        0     3249 2023-05-17 06:54:38.000000 httpanalyzer-0.1.5/src/httpanalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-05-17 06:54:38.000000 httpanalyzer-0.1.5/src/httpanalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 06:54:38.000000 httpanalyzer-0.1.5/src/httpanalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-17 06:54:38.000000 httpanalyzer-0.1.5/src/httpanalyzer.egg-info/top_level.txt
```

### Comparing `httpanalyzer-0.1.4/LICENSE.txt` & `httpanalyzer-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `httpanalyzer-0.1.4/PKG-INFO` & `httpanalyzer-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpanalyzer
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library for analyzing http-requests
 Author-email: Martin Merkli <martin.merkli@protonmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/MartinMerkli/httpanalyzer
 Project-URL: repository, https://github.com/MartinMerkli/httpanalyzer
 Keywords: python,http
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: httpanalyzer Version: 0.1.4 Summary: Library for
+Metadata-Version: 2.1 Name: httpanalyzer Version: 0.1.5 Summary: Library for
 analyzing http-requests Author-email: Martin Merkli
 merkli@protonmail.com> License: MIT License Project-URL: homepage, https://
 github.com/MartinMerkli/httpanalyzer Project-URL: repository, https://
 github.com/MartinMerkli/httpanalyzer Keywords: python,http Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: System Administrators Requires-
```

### Comparing `httpanalyzer-0.1.4/README.md` & `httpanalyzer-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `httpanalyzer-0.1.4/pyproject.toml` & `httpanalyzer-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "httpanalyzer"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Martin Merkli", email="martin.merkli@protonmail.com" },
 ]
 description = "Library for analyzing http-requests"
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.6"
```

### Comparing `httpanalyzer-0.1.4/src/httpanalyzer/__init__.py` & `httpanalyzer-0.1.5/src/httpanalyzer/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+from .src import MALICIOUS_PATHS as _MALICIOUS_PATHS, BOTS_PATH as _BOTS_PATH, BOTS_AGENT as _BOTS_AGENT
+from .src import SEARCH_ENGINE_AGENT as _SEARCH_ENGINE_AGENT
+from .utils import url_decode as _url_decode
+import importlib.resources as _importlib_resources
+from . import lists as _lists
+from math import log2 as _log2
 
 
 class Request:
 
     def __init__(self, http_headers: dict, ip: str, path: str, admin_pages: list = None) -> None:
         """
         Class for analyzing http traffic from the http headers and the ip address.
@@ -23,66 +29,68 @@
 
     def bot(self) -> float:
         """
         Get a rating on the possibility that this request was made by a bot.
         :return: float between 0.0 and 1.0 (NOT linear distribution)
         """
         if self._bot_rating is None:
-            from .src import BOTS_AGENT, BOTS_PATH
             yes = 0.0
             no = 1.0
             user_agent = self._http_headers.get('User-Agent', '').lower()
-            for element in BOTS_AGENT:
+            for element in _BOTS_AGENT:
                 if element in user_agent:
                     yes += 10.0
-            if self._path in BOTS_PATH:
+            if _url_decode(self._path.lower()) in _BOTS_PATH:
                 yes += 5.0
             if self._http_headers.get('Referer', '') != '':
                 no += 2.0
+            for wordlist in []:
+                if self._path in _importlib_resources.read_text(_lists, wordlist).splitlines():
+                    yes += 0.05 * _log2(len(self._path) + 1) ** 2
             self._bot_rating = yes / (yes + no)
         return self._bot_rating
 
     def search_engine(self) -> float:
         """
         Get a rating on the possibility that this request was made by a search engine.
         :return: float between 0.0 and 1.0 (NOT linear distribution)
         """
         if self._search_rating is None:
-            from .src import SEARCH_ENGINE_AGENT, BOTS_PATH
             yes = 0.0
             no = 1.0
             user_agent = self._http_headers.get('User-Agent', '').lower()
-            for element in SEARCH_ENGINE_AGENT:
+            for element in _SEARCH_ENGINE_AGENT:
                 if element in user_agent:
                     yes += 10.0
-            if self._path in BOTS_PATH:
+            if _url_decode(self._path.lower()) in _BOTS_PATH:
                 yes += 0.2
             self._search_rating = yes / (yes + no)
         return self._search_rating
 
     def malicious(self) -> float:
         """
         Get a rating on the possibility that this request was made with malicious intends.
         :return: float between 0.0 and 1.0 (NOT linear distribution)
         """
         if self._malicious_rating is None:
-            from .src import MALICIOUS_PATHS
-            from .utils import url_decode
             yes = 0.0
             no = 1.0
-            path = url_decode(self._path.lower())
-            for element in MALICIOUS_PATHS:
+            path = _url_decode(self._path.lower())
+            for element in _MALICIOUS_PATHS:
                 excluded = False
                 for page in self._admin_pages:
                     if page in element:
                         excluded = True
                 if (element in path) and (not excluded):
                     yes += 10.0
             if self._http_headers.get('Referer', '') != '':
                 no += 2.0
+            for wordlist in []:
+                if self._path in _importlib_resources.read_text(_lists, wordlist).splitlines():
+                    yes += 0.05 * _log2(len(self._path) + 1) ** 2
             self._malicious_rating = yes / (yes + no)
         return self._malicious_rating
 
 
 class FlaskRequest(Request):
 
     def __init__(self, request, admin_pages: list = None):
```

### Comparing `httpanalyzer-0.1.4/src/httpanalyzer/src.py` & `httpanalyzer-0.1.5/src/httpanalyzer/src.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     'yandex',  # Yandex
 }
 BOTS_PATH = {
     '/robots.txt',
     '/sitemap.xml',
 }
 MALICIOUS_PATHS = {
-    '${''.class.forname(\'javax',
+    '${\'\'.class.forname(\'javax',
     '${@die(md5',
     '${jndi:ldap://$',
     '&_method=__construct&method=*&filter[]=',
     '(*),concat(0x7e,md5(1)',
     '--exec=<divd',
     '.git/config',
     '.git/head',
```

### Comparing `httpanalyzer-0.1.4/src/httpanalyzer.egg-info/PKG-INFO` & `httpanalyzer-0.1.5/src/httpanalyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpanalyzer
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library for analyzing http-requests
 Author-email: Martin Merkli <martin.merkli@protonmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/MartinMerkli/httpanalyzer
 Project-URL: repository, https://github.com/MartinMerkli/httpanalyzer
 Keywords: python,http
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: httpanalyzer Version: 0.1.4 Summary: Library for
+Metadata-Version: 2.1 Name: httpanalyzer Version: 0.1.5 Summary: Library for
 analyzing http-requests Author-email: Martin Merkli
 merkli@protonmail.com> License: MIT License Project-URL: homepage, https://
 github.com/MartinMerkli/httpanalyzer Project-URL: repository, https://
 github.com/MartinMerkli/httpanalyzer Keywords: python,http Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: System Administrators Requires-
```

