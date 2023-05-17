# Comparing `tmp/polygon_api_client-1.8.5.tar.gz` & `tmp/polygon_api_client-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygon_api_client-1.8.5.tar", max compression
+gzip compressed data, was "polygon_api_client-1.8.6.tar", max compression
```

## Comparing `polygon_api_client-1.8.5.tar` & `polygon_api_client-1.8.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1074 2023-04-04 15:21:27.408352 polygon_api_client-1.8.5/LICENSE
--rw-r--r--   0        0        0      148 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/__init__.py
--rw-r--r--   0        0        0      256 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/exceptions.py
--rw-r--r--   0        0        0      329 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/logging.py
--rw-r--r--   0        0        0      561 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/modelclass.py
--rw-r--r--   0        0        0     1713 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/__init__.py
--rw-r--r--   0        0        0     8840 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/aggs.py
--rw-r--r--   0        0        0     6705 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/base.py
--rw-r--r--   0        0        0    12601 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/indicators.py
--rw-r--r--   0        0        0      356 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/__init__.py
--rw-r--r--   0        0        0     3408 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/aggs.py
--rw-r--r--   0        0        0     1530 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/common.py
--rw-r--r--   0        0        0     2755 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/conditions.py
--rw-r--r--   0        0        0     1784 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/contracts.py
--rw-r--r--   0        0        0      645 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/dividends.py
--rw-r--r--   0        0        0      569 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/exchanges.py
--rw-r--r--   0        0        0    10103 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/financials.py
--rw-r--r--   0        0        0     2399 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/indicators.py
--rw-r--r--   0        0        0     2499 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/markets.py
--rw-r--r--   0        0        0     3434 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/quotes.py
--rw-r--r--   0        0        0     3687 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/request.py
--rw-r--r--   0        0        0     8754 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/snapshot.py
--rw-r--r--   0        0        0      446 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/splits.py
--rw-r--r--   0        0        0     2269 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/summaries.py
--rw-r--r--   0        0        0     6892 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/tickers.py
--rw-r--r--   0        0        0     2051 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/models/trades.py
--rw-r--r--   0        0        0     5129 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/quotes.py
--rw-r--r--   0        0        0    23790 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/reference.py
--rw-r--r--   0        0        0     7816 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/snapshot.py
--rw-r--r--   0        0        0     1201 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/summaries.py
--rw-r--r--   0        0        0     4127 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/trades.py
--rw-r--r--   0        0        0     3799 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/rest/vX.py
--rw-r--r--   0        0        0     9678 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/websocket/__init__.py
--rw-r--r--   0        0        0     1524 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/websocket/models/__init__.py
--rw-r--r--   0        0        0      719 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/websocket/models/common.py
--rw-r--r--   0        0        0     9790 2023-04-04 15:21:27.412352 polygon_api_client-1.8.5/polygon/websocket/models/models.py
--rw-r--r--   0        0        0     1005 2023-04-04 15:21:49.542537 polygon_api_client-1.8.5/pyproject.toml
--rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 polygon_api_client-1.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-17 15:05:24.035156 polygon_api_client-1.8.6/LICENSE
+-rw-r--r--   0        0        0      148 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/exceptions.py
+-rw-r--r--   0        0        0      329 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/logging.py
+-rw-r--r--   0        0        0      561 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/modelclass.py
+-rw-r--r--   0        0        0     1713 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/__init__.py
+-rw-r--r--   0        0        0     8840 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/aggs.py
+-rw-r--r--   0        0        0     6705 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/base.py
+-rw-r--r--   0        0        0    12601 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/indicators.py
+-rw-r--r--   0        0        0      356 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/__init__.py
+-rw-r--r--   0        0        0     3408 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/aggs.py
+-rw-r--r--   0        0        0     1530 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/common.py
+-rw-r--r--   0        0        0     2755 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/conditions.py
+-rw-r--r--   0        0        0     1784 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/contracts.py
+-rw-r--r--   0        0        0      645 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/dividends.py
+-rw-r--r--   0        0        0      569 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/exchanges.py
+-rw-r--r--   0        0        0    10103 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/financials.py
+-rw-r--r--   0        0        0     2399 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/indicators.py
+-rw-r--r--   0        0        0     2499 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/markets.py
+-rw-r--r--   0        0        0     3434 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/quotes.py
+-rw-r--r--   0        0        0     3687 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/request.py
+-rw-r--r--   0        0        0     8754 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/snapshot.py
+-rw-r--r--   0        0        0      446 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/splits.py
+-rw-r--r--   0        0        0     2269 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/summaries.py
+-rw-r--r--   0        0        0     6892 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/tickers.py
+-rw-r--r--   0        0        0     2051 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/trades.py
+-rw-r--r--   0        0        0     5129 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/quotes.py
+-rw-r--r--   0        0        0    23756 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/reference.py
+-rw-r--r--   0        0        0     7816 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/snapshot.py
+-rw-r--r--   0        0        0     1201 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/summaries.py
+-rw-r--r--   0        0        0     4127 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/trades.py
+-rw-r--r--   0        0        0     3799 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/vX.py
+-rw-r--r--   0        0        0     9678 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/websocket/__init__.py
+-rw-r--r--   0        0        0     1612 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/websocket/models/__init__.py
+-rw-r--r--   0        0        0      719 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/websocket/models/common.py
+-rw-r--r--   0        0        0     9844 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/websocket/models/models.py
+-rw-r--r--   0        0        0     1005 2023-05-17 15:05:49.435358 polygon_api_client-1.8.6/pyproject.toml
+-rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 polygon_api_client-1.8.6/PKG-INFO
```

### Comparing `polygon_api_client-1.8.5/LICENSE` & `polygon_api_client-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/modelclass.py` & `polygon_api_client-1.8.6/polygon/modelclass.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/__init__.py` & `polygon_api_client-1.8.6/polygon/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/aggs.py` & `polygon_api_client-1.8.6/polygon/rest/aggs.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/base.py` & `polygon_api_client-1.8.6/polygon/rest/base.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/indicators.py` & `polygon_api_client-1.8.6/polygon/rest/indicators.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/aggs.py` & `polygon_api_client-1.8.6/polygon/rest/models/aggs.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/common.py` & `polygon_api_client-1.8.6/polygon/rest/models/common.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/conditions.py` & `polygon_api_client-1.8.6/polygon/rest/models/conditions.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/contracts.py` & `polygon_api_client-1.8.6/polygon/rest/models/contracts.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/dividends.py` & `polygon_api_client-1.8.6/polygon/rest/models/dividends.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/exchanges.py` & `polygon_api_client-1.8.6/polygon/rest/models/exchanges.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/financials.py` & `polygon_api_client-1.8.6/polygon/rest/models/financials.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/indicators.py` & `polygon_api_client-1.8.6/polygon/rest/models/indicators.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/markets.py` & `polygon_api_client-1.8.6/polygon/rest/models/markets.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/quotes.py` & `polygon_api_client-1.8.6/polygon/rest/models/quotes.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/request.py` & `polygon_api_client-1.8.6/polygon/rest/models/request.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/snapshot.py` & `polygon_api_client-1.8.6/polygon/rest/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/summaries.py` & `polygon_api_client-1.8.6/polygon/rest/models/summaries.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/tickers.py` & `polygon_api_client-1.8.6/polygon/rest/models/tickers.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/models/trades.py` & `polygon_api_client-1.8.6/polygon/rest/models/trades.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/quotes.py` & `polygon_api_client-1.8.6/polygon/rest/quotes.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/reference.py` & `polygon_api_client-1.8.6/polygon/rest/reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,24 +86,24 @@
         sort: Optional[Union[str, Sort]] = "ticker",
         order: Optional[Union[str, Order]] = "asc",
         params: Optional[Dict[str, Any]] = None,
         raw: bool = False,
         options: Optional[RequestOptionBuilder] = None,
     ) -> Union[Iterator[Ticker], HTTPResponse]:
         """
-        Query all ticker symbols which are supported by Polygon.io. This API currently includes Stocks/Equities, Crypto, and Forex.
+        Query all ticker symbols which are supported by Polygon.io. This API currently includes Stocks/Equities, Indices, Forex, and Crypto.
 
         :param ticker: Specify a ticker symbol. Defaults to empty string which queries all tickers.
         :param ticker_lt: Ticker less than.
         :param ticker_lte: Ticker less than or equal to.
         :param ticker_gt: Ticker greater than.
         :param ticker_gte: Ticker greater than or equal to.
         :param type: Specify the type of the tickers. Find the types that we support via our Ticker Types API. Defaults to empty string which queries all types.
         :param market: Filter by market type. By default all markets are included.
-        :param exchange: Specify the primary exchange of the asset in the ISO code format. Find more information about the ISO codes at the ISO org website. Defaults to empty string which queries all exchanges.
+        :param exchange: Specify the assets primary exchange Market Identifier Code (MIC) according to ISO 10383. Defaults to empty string which queries all exchanges.
         :param cusip: Specify the CUSIP code of the asset you want to search for. Find more information about CUSIP codes at their website. Defaults to empty string which queries all CUSIPs.
         :param cik: Specify the CIK of the asset you want to search for. Find more information about CIK codes at their website. Defaults to empty string which queries all CIKs.
         :param date: Specify a point in time to retrieve tickers available on that date. Defaults to the most recent available date.
         :param search: Search for terms within the ticker and/or company name.
         :param active: Specify if the tickers returned should be actively traded on the queried date. Default is true.
         :param limit: Limit the size of the response per-page, default is 100 and max is 1000.
         :param sort: The field to sort the results on. Default is ticker. If the search query parameter is present, sort is ignored and results are ordered by relevance.
```

### Comparing `polygon_api_client-1.8.5/polygon/rest/snapshot.py` & `polygon_api_client-1.8.6/polygon/rest/snapshot.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/summaries.py` & `polygon_api_client-1.8.6/polygon/rest/summaries.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/trades.py` & `polygon_api_client-1.8.6/polygon/rest/trades.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/rest/vX.py` & `polygon_api_client-1.8.6/polygon/rest/vX.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/websocket/__init__.py` & `polygon_api_client-1.8.6/polygon/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/websocket/models/__init__.py` & `polygon_api_client-1.8.6/polygon/websocket/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         return CryptoQuote.from_dict(data)
     elif event_type == EventType.Imbalances.value:
         return Imbalance.from_dict(data)
     elif event_type == EventType.LimitUpLimitDown.value:
         return LimitUpLimitDown.from_dict(data)
     elif event_type == EventType.CryptoL2.value:
         return Level2Book.from_dict(data)
+    elif event_type == EventType.Value.value:
+        return IndexValue.from_dict(data)
     return None
 
 
 def parse(msg: List[Dict[str, Any]], logger: logging.Logger) -> List[WebSocketMessage]:
     res = []
     for m in msg:
         parsed = parse_single(m)
```

### Comparing `polygon_api_client-1.8.5/polygon/websocket/models/common.py` & `polygon_api_client-1.8.6/polygon/websocket/models/common.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.5/polygon/websocket/models/models.py` & `polygon_api_client-1.8.6/polygon/websocket/models/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,18 +313,20 @@
     event_type: Optional[Union[str, EventType]] = None
     value: Optional[float] = None
     ticker: Optional[str] = None
     timestamp: Optional[str] = None
 
     @staticmethod
     def from_dict(d):
-        d.get("ev", None),
-        d.get("val", None),
-        d.get("T", None),
-        d.get("t", None)
+        return IndexValue(
+            d.get("ev", None),
+            d.get("val", None),
+            d.get("T", None),
+            d.get("t", None),
+        )
 
 
 WebSocketMessage = NewType(
     "WebSocketMessage",
     List[
         Union[
             EquityAgg,
```

### Comparing `polygon_api_client-1.8.5/pyproject.toml` & `polygon_api_client-1.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polygon-api-client"
-version = "v1.8.5"
+version = "v1.8.6"
 description = "Official Polygon.io REST and Websocket client."
 authors = ["polygon.io"]
 license = "MIT"
 homepage = "https://polygon.io"
 repository = "https://github.com/polygon-io/client-python"
 documentation = "https://polygon.io/docs"
 keywords = [
```

### Comparing `polygon_api_client-1.8.5/PKG-INFO` & `polygon_api_client-1.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polygon-api-client
-Version: 1.8.5
+Version: 1.8.6
 Summary: Official Polygon.io REST and Websocket client.
 Home-page: https://polygon.io
 License: MIT
 Keywords: polygon,free,rest,stock,market,data,api,polygon.io,websocket,client
 Author: polygon.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

