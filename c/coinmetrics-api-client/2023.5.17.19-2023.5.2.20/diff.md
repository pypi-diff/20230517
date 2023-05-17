# Comparing `tmp/coinmetrics_api_client-2023.5.17.19.tar.gz` & `tmp/coinmetrics_api_client-2023.5.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinmetrics_api_client-2023.5.17.19.tar", max compression
+gzip compressed data, was "coinmetrics_api_client-2023.5.2.20.tar", max compression
```

## Comparing `coinmetrics_api_client-2023.5.17.19.tar` & `coinmetrics_api_client-2023.5.2.20.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1088 2023-05-02 14:59:47.712855 coinmetrics_api_client-2023.5.17.19/LICENSE
--rw-r--r--   0        0        0    20460 2023-05-02 14:59:47.712855 coinmetrics_api_client-2023.5.17.19/README.md
--rw-r--r--   0        0        0       29 2023-05-17 19:27:26.860140 coinmetrics_api_client-2023.5.17.19/coinmetrics/__init__.py
--rw-r--r--   0        0        0    20751 2023-05-17 19:27:26.860140 coinmetrics_api_client-2023.5.17.19/coinmetrics/_catalogs.py
--rw-r--r--   0        0        0     9947 2023-05-02 14:59:47.712855 coinmetrics_api_client-2023.5.17.19/coinmetrics/_data_collection.py
--rw-r--r--   0        0        0     2328 2023-05-02 14:59:47.712855 coinmetrics_api_client-2023.5.17.19/coinmetrics/_exceptions.py
--rw-r--r--   0        0        0     1181 2023-05-02 14:59:47.712855 coinmetrics_api_client-2023.5.17.19/coinmetrics/_models.py
--rw-r--r--   0        0        0      699 2023-05-02 14:59:47.712855 coinmetrics_api_client-2023.5.17.19/coinmetrics/_typing.py
--rw-r--r--   0        0        0     3951 2023-05-02 14:59:47.712855 coinmetrics_api_client-2023.5.17.19/coinmetrics/_utils.py
--rw-r--r--   0        0        0   233224 2023-05-02 22:06:59.728994 coinmetrics_api_client-2023.5.17.19/coinmetrics/api_client.py
--rw-r--r--   0        0        0        0 2023-05-17 19:35:27.249227 coinmetrics_api_client-2023.5.17.19/coinmetrics/build.py
--rw-r--r--   0        0        0      148 2023-05-02 14:59:47.712855 coinmetrics_api_client-2023.5.17.19/coinmetrics/constants.py
--rw-r--r--   0        0        0    20520 2023-05-02 14:59:47.712855 coinmetrics_api_client-2023.5.17.19/coinmetrics/data_exporter.py
--rw-r--r--   0        0        0     8669 2023-05-02 14:59:47.712855 coinmetrics_api_client-2023.5.17.19/coinmetrics/typer_cli.py
--rw-r--r--   0        0        0     1237 2023-05-17 19:27:26.860140 coinmetrics_api_client-2023.5.17.19/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 19:35:27.253227 coinmetrics_api_client-2023.5.17.19/test/__init__.py
--rw-r--r--   0        0        0     1640 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_asset_pair_candles.csv
--rw-r--r--   0        0        0      412 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_asset_pairs.csv
--rw-r--r--   0        0        0     2097 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_assets_markets.csv
--rw-r--r--   0        0        0      605 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_assets_metrics.csv
--rw-r--r--   0        0        0      436 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_exchange_assets.csv
--rw-r--r--   0        0        0     3595 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_exchanges_markets.csv
--rw-r--r--   0        0        0      822 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_exchanges_metrics.csv
--rw-r--r--   0        0        0      556 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_indexes.csv
--rw-r--r--   0        0        0      223 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_institutions.csv
--rw-r--r--   0        0        0      178 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_market_orderbooks.csv
--rw-r--r--   0        0        0      254 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_market_quotes.csv
--rw-r--r--   0        0        0      297 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_market_trades.csv
--rw-r--r--   0        0        0      579 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_markets.csv
--rw-r--r--   0        0        0     2557 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/data/catalog_metrics.csv
--rw-r--r--   0        0        0    28915 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/test_api_client.py
--rw-r--r--   0        0        0    10311 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/test_api_methods.py
--rw-r--r--   0        0        0     2910 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/test_as_list.py
--rw-r--r--   0        0        0     1788 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/test_blockchain_methods.py
--rw-r--r--   0        0        0     2273 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/test_custom_exceptions.py
--rw-r--r--   0        0        0    13462 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/test_data_exporter.py
--rw-r--r--   0        0        0     1015 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/test_debugging.py
--rw-r--r--   0        0        0     2142 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/test_models.py
--rw-r--r--   0        0        0     1193 2023-05-02 22:06:59.728994 coinmetrics_api_client-2023.5.17.19/test/test_rate_limits.py
--rw-r--r--   0        0        0    14167 2023-05-02 14:59:47.732855 coinmetrics_api_client-2023.5.17.19/test/test_to_dataframe.py
--rw-r--r--   0        0        0     5829 2023-05-02 22:06:59.728994 coinmetrics_api_client-2023.5.17.19/test/test_websocket_methods.py
--rw-r--r--   0        0        0    21649 1970-01-01 00:00:00.000000 coinmetrics_api_client-2023.5.17.19/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/LICENSE
+-rw-r--r--   0        0        0    20460 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/README.md
+-rw-r--r--   0        0        0       28 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/coinmetrics/__init__.py
+-rw-r--r--   0        0        0    21093 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_catalogs.py
+-rw-r--r--   0        0        0     9947 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_data_collection.py
+-rw-r--r--   0        0        0     2328 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_exceptions.py
+-rw-r--r--   0        0        0     1181 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_models.py
+-rw-r--r--   0        0        0      699 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_typing.py
+-rw-r--r--   0        0        0     3951 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_utils.py
+-rw-r--r--   0        0        0   233224 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/coinmetrics/api_client.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:44:04.348483 coinmetrics_api_client-2023.5.2.20/coinmetrics/build.py
+-rw-r--r--   0        0        0      148 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/constants.py
+-rw-r--r--   0        0        0    20520 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/data_exporter.py
+-rw-r--r--   0        0        0     8669 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/typer_cli.py
+-rw-r--r--   0        0        0     1236 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 20:44:04.352483 coinmetrics_api_client-2023.5.2.20/test/__init__.py
+-rw-r--r--   0        0        0     1640 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_asset_pair_candles.csv
+-rw-r--r--   0        0        0      412 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_asset_pairs.csv
+-rw-r--r--   0        0        0     2097 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_assets_markets.csv
+-rw-r--r--   0        0        0      605 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_assets_metrics.csv
+-rw-r--r--   0        0        0      436 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchange_assets.csv
+-rw-r--r--   0        0        0     3595 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchanges_markets.csv
+-rw-r--r--   0        0        0      822 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchanges_metrics.csv
+-rw-r--r--   0        0        0      556 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_indexes.csv
+-rw-r--r--   0        0        0      223 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_institutions.csv
+-rw-r--r--   0        0        0      178 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_market_orderbooks.csv
+-rw-r--r--   0        0        0      254 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_market_quotes.csv
+-rw-r--r--   0        0        0      297 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_market_trades.csv
+-rw-r--r--   0        0        0      579 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_markets.csv
+-rw-r--r--   0        0        0     2557 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_metrics.csv
+-rw-r--r--   0        0        0    28915 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_api_client.py
+-rw-r--r--   0        0        0    10311 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_api_methods.py
+-rw-r--r--   0        0        0     2910 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_as_list.py
+-rw-r--r--   0        0        0     1788 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_blockchain_methods.py
+-rw-r--r--   0        0        0     2273 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_custom_exceptions.py
+-rw-r--r--   0        0        0    13462 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_data_exporter.py
+-rw-r--r--   0        0        0     1015 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_debugging.py
+-rw-r--r--   0        0        0     2142 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_models.py
+-rw-r--r--   0        0        0     1193 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/test/test_rate_limits.py
+-rw-r--r--   0        0        0    14167 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_to_dataframe.py
+-rw-r--r--   0        0        0     5829 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/test/test_websocket_methods.py
+-rw-r--r--   0        0        0    21648 1970-01-01 00:00:00.000000 coinmetrics_api_client-2023.5.2.20/PKG-INFO
```

### Comparing `coinmetrics_api_client-2023.5.17.19/LICENSE` & `coinmetrics_api_client-2023.5.2.20/LICENSE`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/README.md` & `coinmetrics_api_client-2023.5.2.20/README.md`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/coinmetrics/_catalogs.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/_catalogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -399,19 +399,25 @@
     """
     Transforms catalog data in list form into a dataframe
     :return: Catalog Data
     """
 
     def to_dataframe(self) -> DataFrameType:
         df_markets = pd.DataFrame(self)
-        metadata = ["trades", "funding_rates", "openinterest", "liquidations"]
+        df_markets = df_markets.join(
+            df_markets["trades"].apply(pd.Series).drop(0, axis=1, errors="ignore"),
+            rsuffix="_trades",
+        )
+        metadata = ["funding_rates", "openinterest", "liquidations"]
         for col in metadata:
             if col in df_markets.columns:
-                for time_col in ["min_time", "max_time"]:
-                    df_markets[f'{time_col}_{col}'] = df_markets[col].apply(lambda item: None if isinstance(item, float) else item.get(time_col, None))
+                df_markets = df_markets.join(
+                    df_markets[col].apply(pd.Series).drop(0, axis=1, errors="ignore"),
+                    rsuffix=f"_{col}",
+                )
 
         df_markets = df_markets.drop(
             ["trades", "funding_rates", "openinterest", "liquidations"],
             axis=1,
             errors="ignore",
         )
         return convert_catalog_dtypes(df_markets)
@@ -521,23 +527,37 @@
     """
     Transforms catalog data in list form into a dataframe
     :return: Catalog Data
     """
 
     def to_dataframe(self) -> DataFrameType:
         df_catalog_market_metrics = pd.DataFrame(self)
-        df_catalog_market_metrics = df_catalog_market_metrics.explode("metrics")
-        df_metrics = pd.json_normalize(df_catalog_market_metrics['metrics'])
-        df_catalog_market_metrics = df_catalog_market_metrics.join(df_metrics)
-        df_catalog_market_metrics = df_catalog_market_metrics.explode("frequencies")
-        df_frequencies = pd.json_normalize(df_catalog_market_metrics['frequencies'])
-        df_catalog_market_metrics = df_catalog_market_metrics.join(df_frequencies)
-        df_catalog_market_metrics = df_catalog_market_metrics.drop(["metrics", "frequencies"], axis=1)
-        df_catalog_market_metrics = df_catalog_market_metrics.reset_index(drop=True)
-
+        df_catalog_market_metrics = (
+            df_catalog_market_metrics.explode("metrics")
+            .assign(metric=lambda df: _expand_df(key="metric", iterable=df.metrics))
+            .assign(
+                frequencies=lambda df: _expand_df(
+                    key="frequencies", iterable=df.metrics
+                )
+            )
+            .explode("frequencies")
+            .assign(
+                frequency=lambda df: _expand_df(
+                    key="frequency", iterable=df.frequencies
+                )
+            )
+            .assign(
+                min_time=lambda df: _expand_df(key="min_time", iterable=df.frequencies)
+            )
+            .assign(
+                max_time=lambda df: _expand_df(key="max_time", iterable=df.frequencies)
+            )
+            .reset_index(drop=True)
+            .drop(["metrics", "frequencies"], axis=1)
+        )
         return convert_catalog_dtypes(df_catalog_market_metrics)
 
 
 class CatalogMarketCandlesData(List[Any]):
     """
     Transforms catalog data in list form into a dataframe
     :return: Catalog Data
```

### Comparing `coinmetrics_api_client-2023.5.17.19/coinmetrics/_data_collection.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/_data_collection.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/coinmetrics/_exceptions.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/_exceptions.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/coinmetrics/_models.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/_models.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/coinmetrics/_typing.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/_typing.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/coinmetrics/_utils.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/_utils.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/coinmetrics/api_client.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/api_client.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/coinmetrics/data_exporter.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/data_exporter.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/coinmetrics/typer_cli.py` & `coinmetrics_api_client-2023.5.2.20/coinmetrics/typer_cli.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/pyproject.toml` & `coinmetrics_api_client-2023.5.2.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coinmetrics-api-client"
-version = "2023.5.17.19"
+version = "2023.5.2.20"
 description = "Python client for Coin Metrics API v4."
 authors = ["Coin Metrics <info@coinmetrics.io>", "Oleksandr Buchkovskyi <oleksandr@coinmetrics.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://coinmetrics.github.io/api-client-python/site/index.html"
 repository = "https://github.com/coinmetrics/api-client-python"
 packages = [{include = "coinmetrics"}]
```

### Comparing `coinmetrics_api_client-2023.5.17.19/test/data/catalog_asset_pair_candles.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_asset_pair_candles.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/data/catalog_assets_markets.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_assets_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/data/catalog_assets_metrics.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_assets_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/data/catalog_exchanges_markets.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchanges_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/data/catalog_exchanges_metrics.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchanges_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/data/catalog_indexes.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_indexes.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/data/catalog_markets.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/data/catalog_metrics.csv` & `coinmetrics_api_client-2023.5.2.20/test/data/catalog_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/test_api_client.py` & `coinmetrics_api_client-2023.5.2.20/test/test_api_client.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/test_api_methods.py` & `coinmetrics_api_client-2023.5.2.20/test/test_api_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/test_as_list.py` & `coinmetrics_api_client-2023.5.2.20/test/test_as_list.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/test_blockchain_methods.py` & `coinmetrics_api_client-2023.5.2.20/test/test_blockchain_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/test_custom_exceptions.py` & `coinmetrics_api_client-2023.5.2.20/test/test_custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/test_data_exporter.py` & `coinmetrics_api_client-2023.5.2.20/test/test_data_exporter.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/test_debugging.py` & `coinmetrics_api_client-2023.5.2.20/test/test_debugging.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/test_models.py` & `coinmetrics_api_client-2023.5.2.20/test/test_models.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/test_rate_limits.py` & `coinmetrics_api_client-2023.5.2.20/test/test_rate_limits.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/test_to_dataframe.py` & `coinmetrics_api_client-2023.5.2.20/test/test_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/test/test_websocket_methods.py` & `coinmetrics_api_client-2023.5.2.20/test/test_websocket_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.17.19/PKG-INFO` & `coinmetrics_api_client-2023.5.2.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinmetrics-api-client
-Version: 2023.5.17.19
+Version: 2023.5.2.20
 Summary: Python client for Coin Metrics API v4.
 Home-page: https://coinmetrics.github.io/api-client-python/site/index.html
 License: MIT
 Keywords: coin metrics,coin,metrics,crypto,bitcoin,network-data,market-data,api,handy
 Author: Coin Metrics
 Author-email: info@coinmetrics.io
 Requires-Python: >=3.7.1,<4.0.0
```

