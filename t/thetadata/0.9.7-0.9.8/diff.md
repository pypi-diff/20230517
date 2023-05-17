# Comparing `tmp/thetadata-0.9.7.tar.gz` & `tmp/thetadata-0.9.8.tar.gz`

## Comparing `thetadata-0.9.7.tar` & `thetadata-0.9.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.7/mkdocs.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.7/setup.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.7/.github/workflows/main.yml
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/__init__.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/connection_msgs.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/explanation.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/how-to-guides.md
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/index.md
--rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/logo.png
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/manipulate_df.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/manipulate_series.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/reference.md
--rw-r--r--   0        0        0    30099 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/tutorials.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/__init__.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/cancel_streams.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/eod.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/get_last.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/list_roots.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/open_interest_streaming.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/quote_1min.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/quote_streaming.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/quote_tick.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/trade_streaming.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/trade_streaming_full.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/stocks/__init__.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/stocks/eod.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/stocks/get_last.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/stocks/list_roots.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/stocks/quote_1min.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/stocks/quote_tick.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.7/tests/__init__.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.7/tests/test_client.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.7/tests/test_docs.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/__init__.py
--rw-r--r--   0        0        0    58685 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/client.py
--rw-r--r--   0        0        0    20277 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/enums.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/exceptions.py
--rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/parsing.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/py.typed
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/terminal.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 thetadata-0.9.7/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.7/LICENSE
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 thetadata-0.9.7/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 thetadata-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 thetadata-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.8/mkdocs.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.8/setup.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.8/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/__init__.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/connection_msgs.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/explanation.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/how-to-guides.md
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/index.md
+-rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/logo.png
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/manipulate_df.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/manipulate_series.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/reference.md
+-rw-r--r--   0        0        0    30099 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/tutorials.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/__init__.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/cancel_streams.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/eod.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/get_last.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/list_roots.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/open_interest_streaming.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/quote_1min.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/quote_streaming.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/quote_tick.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/trade_streaming.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/trade_streaming_full.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/stocks/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/stocks/eod.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/stocks/get_last.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/stocks/list_roots.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/stocks/quote_1min.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/stocks/quote_tick.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.8/tests/__init__.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.8/tests/test_client.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.8/tests/test_docs.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/__init__.py
+-rw-r--r--   0        0        0    58685 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/client.py
+-rw-r--r--   0        0        0    20348 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/enums.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/exceptions.py
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/parsing.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/py.typed
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/terminal.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 thetadata-0.9.8/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.8/LICENSE
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 thetadata-0.9.8/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 thetadata-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 thetadata-0.9.8/PKG-INFO
```

### Comparing `thetadata-0.9.7/mkdocs.yml` & `thetadata-0.9.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/.github/workflows/main.yml` & `thetadata-0.9.8/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/.github/workflows/python-publish.yml` & `thetadata-0.9.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/connection_msgs.py` & `thetadata-0.9.8/docs/connection_msgs.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/explanation.md` & `thetadata-0.9.8/docs/explanation.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/how-to-guides.md` & `thetadata-0.9.8/docs/how-to-guides.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/index.md` & `thetadata-0.9.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/logo.png` & `thetadata-0.9.8/docs/logo.png`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/manipulate_series.py` & `thetadata-0.9.8/docs/manipulate_series.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/tutorials.md` & `thetadata-0.9.8/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/options/cancel_streams.py` & `thetadata-0.9.8/docs/options/cancel_streams.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/options/eod.py` & `thetadata-0.9.8/docs/options/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/options/get_last.py` & `thetadata-0.9.8/docs/options/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/options/open_interest_streaming.py` & `thetadata-0.9.8/docs/options/open_interest_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/options/quote_1min.py` & `thetadata-0.9.8/docs/options/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/options/quote_streaming.py` & `thetadata-0.9.8/docs/options/quote_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/options/quote_tick.py` & `thetadata-0.9.8/docs/options/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/options/trade_streaming.py` & `thetadata-0.9.8/docs/options/trade_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/options/trade_streaming_full.py` & `thetadata-0.9.8/docs/options/trade_streaming_full.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/stocks/eod.py` & `thetadata-0.9.8/docs/stocks/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/stocks/get_last.py` & `thetadata-0.9.8/docs/stocks/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/stocks/quote_1min.py` & `thetadata-0.9.8/docs/stocks/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/docs/stocks/quote_tick.py` & `thetadata-0.9.8/docs/stocks/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/tests/test_client.py` & `thetadata-0.9.8/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/tests/test_docs.py` & `thetadata-0.9.8/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/thetadata/client.py` & `thetadata-0.9.8/thetadata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     TickBody,
     ListBody,
     parse_list_REST, parse_flexible_REST, parse_hist_REST, parse_hist_REST_stream, parse_hist_REST_stream_ijson,
 )
 from .terminal import check_download, launch_terminal
 
 _NOT_CONNECTED_MSG = "You must establish a connection first."
-_VERSION = '0.9.7'
+_VERSION = '0.9.8'
 URL_BASE = "http://127.0.0.1:25510/"
 
 
 def _format_strike(strike: float) -> int:
     """Round USD to the nearest tenth of a cent, acceptable by the terminal."""
     return round(strike * 1000)
```

### Comparing `thetadata-0.9.7/thetadata/enums.py` & `thetadata-0.9.8/thetadata/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,14 +307,16 @@
     EOD_TRADE_GREEKS = 209
 
     # PRO
     TRADE_GREEKS = 301
     GREEKS_SECOND_ORDER = 302
     GREEKS_THIRD_ORDER = 303
     ALT_CALCS = 304
+    TRADE_GREEKS_SECOND_ORDER = 305
+    TRADE_GREEKS_THIRD_ORDER = 306
 
 
 @enum.unique
 class StockReqType(enum.Enum):
     """Stock request type codes."""
 
     # FREE
```

### Comparing `thetadata-0.9.7/thetadata/exceptions.py` & `thetadata-0.9.8/thetadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/thetadata/parsing.py` & `thetadata-0.9.8/thetadata/parsing.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/thetadata/terminal.py` & `thetadata-0.9.8/thetadata/terminal.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/LICENSE` & `thetadata-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.7/README.md` & `thetadata-0.9.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Thetadata Python API
 
 The [Thetadata](https://thetadata.net) Python API provides low latency US equities & options data that may be used for
 market research or algorithmic trading applications.
 
-Please see this repository's [documentation](https://thetadata-api.github.io/thetadata-python) for more details.
+Please see this repository's [documentation](https://thetadata-api.github.io/thetadata-python) and [GitHub](https://github.com/ThetaData-API/thetadata-python) for more details.
 
 ## Installation
 
 Java 11 or higher is required. If you are on Windows, Java 19 will automatically be installed for you. Python 10 or higher is **highly** recommended.
 
 `pip install thetadata`
```

### Comparing `thetadata-0.9.7/pyproject.toml` & `thetadata-0.9.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thetadata"
-version = "0.9.7"
+version = "0.9.8"
 authors = [
   { name="Bailey Danseglio", email="bailey@thetadata.net" },
   { name="Adler Weber", email="redacted@thetadata.net" },
 ]
 description = "Python API for Thetadata"
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `thetadata-0.9.7/PKG-INFO` & `thetadata-0.9.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thetadata
-Version: 0.9.7
+Version: 0.9.8
 Summary: Python API for Thetadata
 Project-URL: Homepage, https://thetadata.net
 Project-URL: Source, https://thetadata-api.github.io/thetadata-python/reference/
 Project-URL: Bug Tracker, https://github.com/ThetaData-API/thetadata-python/issues
 Project-URL: Documentation, https://thetadata-api.github.io/thetadata-python/
 Author-email: Bailey Danseglio <bailey@thetadata.net>, Adler Weber <redacted@thetadata.net>
 License: MIT License
@@ -50,15 +50,15 @@
 Description-Content-Type: text/markdown
 
 # Thetadata Python API
 
 The [Thetadata](https://thetadata.net) Python API provides low latency US equities & options data that may be used for
 market research or algorithmic trading applications.
 
-Please see this repository's [documentation](https://thetadata-api.github.io/thetadata-python) for more details.
+Please see this repository's [documentation](https://thetadata-api.github.io/thetadata-python) and [GitHub](https://github.com/ThetaData-API/thetadata-python) for more details.
 
 ## Installation
 
 Java 11 or higher is required. If you are on Windows, Java 19 will automatically be installed for you. Python 10 or higher is **highly** recommended.
 
 `pip install thetadata`
```

