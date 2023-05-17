# Comparing `tmp/pyalgotrader-protocols-0.0.1.tar.gz` & `tmp/pyalgotrader-protocols-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalgotrader-protocols-0.0.1.tar", last modified: Wed Mar 22 02:28:59 2023, max compression
+gzip compressed data, was "pyalgotrader-protocols-0.0.2.tar", last modified: Wed May 17 01:41:42 2023, max compression
```

## Comparing `pyalgotrader-protocols-0.0.1.tar` & `pyalgotrader-protocols-0.0.2.tar`

### file list

```diff
@@ -1,69 +1,24 @@
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 02:28:59.679031 pyalgotrader-protocols-0.0.1/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      380 2023-03-22 02:28:59.679031 pyalgotrader-protocols-0.0.1/PKG-INFO
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 02:28:59.675031 pyalgotrader-protocols-0.0.1/algorithm/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 01:22:24.000000 pyalgotrader-protocols-0.0.1/algorithm/__init__.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     2429 2023-03-22 01:22:24.000000 pyalgotrader-protocols-0.0.1/algorithm/strategy.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 02:28:59.675031 pyalgotrader-protocols-0.0.1/pyalgotrader_core/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-01 07:38:47.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/__init__.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     7599 2023-03-21 04:52:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/algorithm.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1818 2023-03-20 01:09:24.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/broker_manager.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 02:28:59.675031 pyalgotrader-protocols-0.0.1/pyalgotrader_core/brokers/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-18 06:25:18.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/brokers/__init__.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     5126 2023-03-21 10:27:29.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/brokers/fyers_broker.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4455 2023-03-21 09:56:01.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/brokers/fyers_feed.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     2795 2023-03-21 09:56:01.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/brokers/order.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      132 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/brokers/order_type.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     2323 2023-03-21 09:56:01.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/brokers/position.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       77 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/brokers/position_type.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      141 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/brokers/product_type.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     3537 2023-03-21 12:57:13.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/brokers/pyalgotrader_broker.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     2185 2023-03-21 07:59:35.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/chart.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      255 2023-03-20 01:09:24.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/config.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1386 2023-03-20 01:09:24.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/core.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1579 2023-03-21 07:25:28.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/data.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     3918 2023-03-21 09:37:27.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/data_manager.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 02:28:59.675031 pyalgotrader-protocols-0.0.1/pyalgotrader_core/helpers/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/helpers/__init__.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      662 2023-03-21 09:56:01.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/helpers/generate_ranges.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      445 2023-03-22 01:25:42.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/helpers/load_strategy.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     2496 2023-03-21 07:25:28.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/index_manager.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      880 2023-03-21 07:25:28.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/indicator.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 02:28:59.675031 pyalgotrader-protocols-0.0.1/pyalgotrader_core/loggers/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/loggers/__init__.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      854 2023-03-18 13:06:54.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/loggers/orders_logger.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     2259 2023-03-21 10:27:29.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/loggers/trades_logger.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 02:28:59.675031 pyalgotrader-protocols-0.0.1/pyalgotrader_core/modes/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/modes/__init__.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      216 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/modes/backtest_mode.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      212 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/modes/live_mode.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      213 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/modes/paper_mode.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4469 2023-03-22 01:11:13.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/session.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      316 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/stoploss.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1341 2023-03-22 01:11:13.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/store.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      767 2023-03-20 01:09:25.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/symbol_list.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 02:28:59.679031 pyalgotrader-protocols-0.0.1/pyalgotrader_core/symbols/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-20 01:09:25.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/symbols/__init__.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      374 2023-03-20 01:09:25.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/symbols/equity.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      440 2023-03-20 01:09:25.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/symbols/future.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      869 2023-03-21 10:27:29.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/symbols/option.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      262 2023-03-20 01:09:25.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/symbols/symbol.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      338 2023-03-20 01:09:25.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_core/timeframes.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 02:28:59.679031 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      190 2023-03-01 07:38:47.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols/__init__.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      573 2023-03-20 01:09:25.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols/algorithm.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      434 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols/broker.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      622 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols/broker_manager.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      498 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols/chart.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      490 2023-03-01 07:38:47.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols/feed.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      191 2023-03-01 07:38:47.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols/indicator.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      491 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols/store.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      210 2023-03-01 07:38:47.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols/strategy.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      131 2023-03-18 06:25:19.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols/symbol.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 02:28:59.679031 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols.egg-info/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      380 2023-03-22 02:28:59.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols.egg-info/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     2037 2023-03-22 02:28:59.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols.egg-info/SOURCES.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-03-22 02:28:59.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols.egg-info/dependency_links.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        9 2023-03-22 02:28:59.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols.egg-info/requires.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       51 2023-03-22 02:28:59.000000 pyalgotrader-protocols-0.0.1/pyalgotrader_protocols.egg-info/top_level.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      586 2023-03-22 02:13:42.000000 pyalgotrader-protocols-0.0.1/pyproject.toml
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-03-22 02:28:59.679031 pyalgotrader-protocols-0.0.1/setup.cfg
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-17 01:41:41.995088 pyalgotrader-protocols-0.0.2/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/LICENSE
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      405 2023-05-17 01:41:41.995088 pyalgotrader-protocols-0.0.2/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/README.md
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-17 01:41:41.995088 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      190 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/__init__.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      573 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/algorithm.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      434 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/broker.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      622 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/broker_manager.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      498 2023-05-15 02:37:46.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/chart.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       37 2023-05-17 01:39:43.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/data_manager.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      490 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/feed.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      191 2023-05-15 02:37:46.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/indicator.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      491 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/store.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      210 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/strategy.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      131 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/symbol.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-17 01:41:41.995088 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols.egg-info/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      405 2023-05-17 01:41:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols.egg-info/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      638 2023-05-17 01:41:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols.egg-info/SOURCES.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-17 01:41:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols.egg-info/dependency_links.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        9 2023-05-17 01:41:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols.egg-info/requires.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-17 01:41:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols.egg-info/top_level.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-17 01:41:41.995088 pyalgotrader-protocols-0.0.2/setup.cfg
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      878 2023-05-17 01:40:10.000000 pyalgotrader-protocols-0.0.2/setup.py
```

### Comparing `pyalgotrader-protocols-0.0.1/pyalgotrader_protocols/algorithm.py` & `pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/algorithm.py`

 * *Files identical despite different names*

### Comparing `pyalgotrader-protocols-0.0.1/pyalgotrader_protocols/broker_manager.py` & `pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/broker_manager.py`

 * *Files identical despite different names*

