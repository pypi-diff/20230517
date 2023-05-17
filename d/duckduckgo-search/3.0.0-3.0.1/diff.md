# Comparing `tmp/duckduckgo_search-3.0.0.tar.gz` & `tmp/duckduckgo_search-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.0.0.tar", last modified: Wed May 17 16:41:45 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.0.1.tar", last modified: Wed May 17 17:10:40 2023, max compression
```

## Comparing `duckduckgo_search-3.0.0.tar` & `duckduckgo_search-3.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:41:45.091647 duckduckgo_search-3.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-17 16:41:27.000000 duckduckgo_search-3.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-05-17 16:41:45.091647 duckduckgo_search-3.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    13485 2023-05-17 16:41:27.000000 duckduckgo_search-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:41:45.091647 duckduckgo_search-3.0.0/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-17 16:41:27.000000 duckduckgo_search-3.0.0/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-17 16:41:27.000000 duckduckgo_search-3.0.0/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-17 16:41:27.000000 duckduckgo_search-3.0.0/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-17 16:41:27.000000 duckduckgo_search-3.0.0/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    23623 2023-05-17 16:41:27.000000 duckduckgo_search-3.0.0/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-17 16:41:27.000000 duckduckgo_search-3.0.0/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:41:45.091647 duckduckgo_search-3.0.0/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-05-17 16:41:45.000000 duckduckgo_search-3.0.0/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-17 16:41:45.000000 duckduckgo_search-3.0.0/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:41:45.000000 duckduckgo_search-3.0.0/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 16:41:45.000000 duckduckgo_search-3.0.0/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 16:41:45.000000 duckduckgo_search-3.0.0/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 16:41:45.000000 duckduckgo_search-3.0.0/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-17 16:41:27.000000 duckduckgo_search-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 16:41:45.091647 duckduckgo_search-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:41:45.091647 duckduckgo_search-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-17 16:41:27.000000 duckduckgo_search-3.0.0/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:10:40.512138 duckduckgo_search-3.0.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-17 17:10:20.000000 duckduckgo_search-3.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-05-17 17:10:40.508138 duckduckgo_search-3.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13485 2023-05-17 17:10:20.000000 duckduckgo_search-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:10:40.508138 duckduckgo_search-3.0.1/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-17 17:10:20.000000 duckduckgo_search-3.0.1/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-17 17:10:20.000000 duckduckgo_search-3.0.1/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-17 17:10:20.000000 duckduckgo_search-3.0.1/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-17 17:10:20.000000 duckduckgo_search-3.0.1/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23626 2023-05-17 17:10:20.000000 duckduckgo_search-3.0.1/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-17 17:10:20.000000 duckduckgo_search-3.0.1/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:10:40.508138 duckduckgo_search-3.0.1/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-05-17 17:10:40.000000 duckduckgo_search-3.0.1/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-17 17:10:40.000000 duckduckgo_search-3.0.1/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:10:40.000000 duckduckgo_search-3.0.1/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 17:10:40.000000 duckduckgo_search-3.0.1/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 17:10:40.000000 duckduckgo_search-3.0.1/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 17:10:40.000000 duckduckgo_search-3.0.1/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-17 17:10:20.000000 duckduckgo_search-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:10:40.512138 duckduckgo_search-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:10:40.508138 duckduckgo_search-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-17 17:10:20.000000 duckduckgo_search-3.0.1/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.0.0/LICENSE.md` & `duckduckgo_search-3.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.0.0/PKG-INFO` & `duckduckgo_search-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 3.0.0
+Version: 3.0.1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-3.0.0/README.md` & `duckduckgo_search-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.0.0/duckduckgo_search/__init__.py` & `duckduckgo_search-3.0.1/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.0.0/duckduckgo_search/cli.py` & `duckduckgo_search-3.0.1/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.0.0/duckduckgo_search/compat.py` & `duckduckgo_search-3.0.1/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.0.0/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.0.1/duckduckgo_search/duckduckgo_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 )
                 if self._is_500_in_url(resp.url):
                     logger.debug(f"_get_url() 500 in url={resp.url}. Sleep 5 s.")
                     sleep(5)
                 resp.raise_for_status()
                 return resp
             except Exception as ex:
-                logger.debug(f"_get_url() {url=} {type(ex).__name__}")
+                logger.debug(f"_get_url() url={url} {type(ex).__name__}")
             sleep(0.25)
 
     def _resp_to_json(self, resp):
         try:
             return resp.json()
         except Exception as ex:
             logger.debug(f"_resp_to_json() {type(ex).__name__} url={resp.url}")
```

### Comparing `duckduckgo_search-3.0.0/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.0.1/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 3.0.0
+Version: 3.0.1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-3.0.0/pyproject.toml` & `duckduckgo_search-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.0.0/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.0.1/tests/test_duckduckgo_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 
 
 def test_videos():
     results_gen = DDGS().videos("cat")
     counter = 0
     for i, x in enumerate(results_gen):
         counter += 1
-        if i >= 75:
+        if i >= 40:
             break
-    assert counter >= 75
+    assert counter >= 40
 
 
 def test_news():
     results_gen = DDGS().news("cat")
     counter = 0
     for i, x in enumerate(results_gen):
         counter += 1
```

